# Comparing `tmp/balepy-1.3.7.4.tar.gz` & `tmp/balepy-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balepy-1.3.7.4.tar", last modified: Sun Mar 31 09:00:24 2024, max compression
+gzip compressed data, was "balepy-1.3.8.tar", last modified: Sat Apr 20 16:16:32 2024, max compression
```

## Comparing `balepy-1.3.7.4.tar` & `balepy-1.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 onlymamad  (1000) onlymamad  (1000)        0 2024-03-31 09:00:24.702895 balepy-1.3.7.4/
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)     1073 2024-03-30 19:35:26.000000 balepy-1.3.7.4/LICENSE
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)     1672 2024-03-31 09:00:24.702895 balepy-1.3.7.4/PKG-INFO
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)      879 2024-03-30 19:35:26.000000 balepy-1.3.7.4/README.md
-drwxr-xr-x   0 onlymamad  (1000) onlymamad  (1000)        0 2024-03-31 09:00:24.699561 balepy-1.3.7.4/bale/
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)      360 2024-03-30 19:35:26.000000 balepy-1.3.7.4/bale/__init__.py
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)    13718 2024-03-30 19:35:26.000000 balepy-1.3.7.4/bale/client.py
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)       44 2024-03-30 19:35:26.000000 balepy-1.3.7.4/bale/exceptions.py
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)      562 2024-03-30 19:35:26.000000 balepy-1.3.7.4/bale/network.py
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)     7868 2024-03-30 19:35:26.000000 balepy-1.3.7.4/bale/util.py
-drwxr-xr-x   0 onlymamad  (1000) onlymamad  (1000)        0 2024-03-31 09:00:24.699561 balepy-1.3.7.4/balepy.egg-info/
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)     1672 2024-03-31 09:00:24.000000 balepy-1.3.7.4/balepy.egg-info/PKG-INFO
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)      255 2024-03-31 09:00:24.000000 balepy-1.3.7.4/balepy.egg-info/SOURCES.txt
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)        1 2024-03-31 09:00:24.000000 balepy-1.3.7.4/balepy.egg-info/dependency_links.txt
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)        9 2024-03-31 09:00:24.000000 balepy-1.3.7.4/balepy.egg-info/requires.txt
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)        5 2024-03-31 09:00:24.000000 balepy-1.3.7.4/balepy.egg-info/top_level.txt
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)       38 2024-03-31 09:00:24.702895 balepy-1.3.7.4/setup.cfg
--rw-r--r--   0 onlymamad  (1000) onlymamad  (1000)     1017 2024-03-31 08:59:35.000000 balepy-1.3.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:16:32.482368 balepy-1.3.8/
+-rw-rw-rw-   0        0        0     1093 2024-04-08 17:05:20.000000 balepy-1.3.8/LICENSE
+-rw-rw-rw-   0        0        0     1860 2024-04-20 16:16:32.482368 balepy-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1048 2024-04-19 19:21:25.000000 balepy-1.3.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 16:16:32.466742 balepy-1.3.8/bale/
+-rw-rw-rw-   0        0        0      352 2024-04-15 16:03:43.000000 balepy-1.3.8/bale/__init__.py
+-rw-rw-rw-   0        0        0    16178 2024-04-20 15:44:33.000000 balepy-1.3.8/bale/client.py
+-rw-rw-rw-   0        0        0       47 2024-04-08 17:05:20.000000 balepy-1.3.8/bale/exceptions.py
+-rw-rw-rw-   0        0        0      898 2024-04-08 17:05:20.000000 balepy-1.3.8/bale/network.py
+-rw-rw-rw-   0        0        0     8964 2024-04-15 16:31:35.000000 balepy-1.3.8/bale/util.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:16:32.482368 balepy-1.3.8/balepy.egg-info/
+-rw-rw-rw-   0        0        0     1860 2024-04-20 16:16:32.000000 balepy-1.3.8/balepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-20 16:16:32.000000 balepy-1.3.8/balepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 16:16:32.000000 balepy-1.3.8/balepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-20 16:16:32.000000 balepy-1.3.8/balepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-20 16:16:32.000000 balepy-1.3.8/balepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 16:16:32.482368 balepy-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2024-04-20 16:02:33.000000 balepy-1.3.8/setup.py
```

### Comparing `balepy-1.3.7.4/LICENSE` & `balepy-1.3.8/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Mamad Mehrabi Rad
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Mamad Mehrabi Rad
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `balepy-1.3.7.4/PKG-INFO` & `balepy-1.3.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,57 @@
-Metadata-Version: 2.1
-Name: balepy
-Version: 1.3.7.4
-Summary: balepy a Library Python for create bots API in bale application
-Home-page: https://github.com/OnlyRad/balepy
-Author: Mohammad, AmirAli
-Author-email: mohammadmehrabi175@gmail.com
-Keywords: bot,Bot,bale,robot,messangers
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: ~=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-
-# balepy
-
-<h3 align="center"> balepy a Library Python for create bot API in bale application </h3>
-
-## Install and Update:
-```bash
-pip install -U balepy
-```
-
-## For See Docs:
-- <a href="https://balepy.github.io">WebSite</a>
-- <a href="https://t.me/TheCommit">Telegram</a>
-
-## START:
-```python
-from bale import Client
-import asyncio
-
-
-__token = 'your-token-here'
-client = Client(__token, timeout=10)
-
-async def main():
-    for update in client.on_message():
-        await client.send_message(
-            chat_id=update.chat_id,
-            text='Hello __from__ *balepy*',
-            reply_to_message_id=update.message_id
-        )
-
-if __name__ == '__main__':
-    asyncio.run(main())
-```
-
-
-## Thanks To:
-### <a href="https://github.com/metect">AmirAli</a>
-
-## Social Media:
-#### <a href="https://t.me/TheCommit">TELEGRAM</a>
-#### <a href="https://rubika.ir/TheBalepy">RUBIKA</a>
+Metadata-Version: 2.1
+Name: balepy
+Version: 1.3.8
+Summary: balepy a Library Python for create bots API in bale application
+Home-page: https://github.com/OnlyRad/balepy
+Author: Mohammad, AmirAli
+Author-email: mohammadmehrabi175@gmail.com
+Keywords: bot,Bot,bale,robot,messangers
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: ~=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
+# balepy
+
+<p align=center>
+<img src="https://s8.uupload.ir/files/balethon_uvi2_esnh.png" style="width: 300px; height: 300px;" align=center alt="background">
+</p>
+<h3 align="center"> balepy a Library Python for create bot API in bale application <br> <h5 align=center> <a href="https://balepy.github.io"> Docs</a> | <a href="https://t.me/TheLinuxGP">Community</a> | <a href="https://t.me/TheCommit">Telegram Channel</a> | <a href="https://github.com/OnlyRad">Owner</a></h5></h3>
+
+
+## Install and Update:
+```bash
+pip install -U balepy
+```
+
+## START:
+```python
+from bale import Client
+from asyncio import run
+
+
+__token = 'your-token-here'
+client = Client(__token, timeout=10)
+
+async def main():
+    async for message in client.on_message():
+        await message.reply('hello __from__ **balepy**')
+
+
+if __name__ == '__main__':
+    run(main())
+```
+
+
+## Thanks To:
+### <a href="https://github.com/metect">AmirAli</a>
+
+<p>Thanks to all those who contributed directly or indirectly to the development of the module</p>
```

### Comparing `balepy-1.3.7.4/README.md` & `balepy-1.3.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-# balepy
-
-<h3 align="center"> balepy a Library Python for create bot API in bale application </h3>
-
-## Install and Update:
-```bash
-pip install -U balepy
-```
-
-## For See Docs:
-- <a href="https://balepy.github.io">WebSite</a>
-- <a href="https://t.me/TheCommit">Telegram</a>
-
-## START:
-```python
-from bale import Client
-import asyncio
-
-
-__token = 'your-token-here'
-client = Client(__token, timeout=10)
-
-async def main():
-    for update in client.on_message():
-        await client.send_message(
-            chat_id=update.chat_id,
-            text='Hello __from__ *balepy*',
-            reply_to_message_id=update.message_id
-        )
-
-if __name__ == '__main__':
-    asyncio.run(main())
-```
-
-
-## Thanks To:
-### <a href="https://github.com/metect">AmirAli</a>
-
-## Social Media:
-#### <a href="https://t.me/TheCommit">TELEGRAM</a>
-#### <a href="https://rubika.ir/TheBalepy">RUBIKA</a>
+# balepy
+
+<p align=center>
+<img src="https://s8.uupload.ir/files/balethon_uvi2_esnh.png" style="width: 300px; height: 300px;" align=center alt="background">
+</p>
+<h3 align="center"> balepy a Library Python for create bot API in bale application <br> <h5 align=center> <a href="https://balepy.github.io"> Docs</a> | <a href="https://t.me/TheLinuxGP">Community</a> | <a href="https://t.me/TheCommit">Telegram Channel</a> | <a href="https://github.com/OnlyRad">Owner</a></h5></h3>
+
+
+## Install and Update:
+```bash
+pip install -U balepy
+```
+
+## START:
+```python
+from bale import Client
+from asyncio import run
+
+
+__token = 'your-token-here'
+client = Client(__token, timeout=10)
+
+async def main():
+    async for message in client.on_message():
+        await message.reply('hello __from__ **balepy**')
+
+
+if __name__ == '__main__':
+    run(main())
+```
+
+
+## Thanks To:
+### <a href="https://github.com/metect">AmirAli</a>
+
+<p>Thanks to all those who contributed directly or indirectly to the development of the module</p>
```

### Comparing `balepy-1.3.7.4/bale/client.py` & `balepy-1.3.8/bale/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,418 +1,473 @@
-from .network import Network
-from .util import message
-from .exceptions import *
-
-import asyncio
-
-
-class Client:
-
-    def __init__(self, token: str, timeout: float = 20) -> None:
-        self.loop = asyncio.get_event_loop()
-        self.network = Network(token=token, timeout=timeout)
-
-        if not token:
-            raise TokenNotInvalid('`token` did\'t passed')
-
-    def request(self, method: str, data: dict = None, request_method: str = 'post') -> dict:
-        try:
-            return self.network.connect(method=method, data=data, request_method=request_method)
-        except Exception as err:
-            print(__file__, err, __file__)
-
-    def on_message(self):
-        '''Use this method to receive updates
-        Example:
-            from balepy import Client
-            import asyncio
-
-            client = Client('token', timeout=10)
-            def main():
-                for update in client.on_message():
-                    print(update.text)
-
-            asyncio.run(main())
-        '''
-        payload: dict = {
-            'offset': -1, 'limit': 100
-        }
-        while True:
-            update = self.request('getupdates', payload, 'post')
-            payload['offset'] = 1
-            if (update != None) and (update['ok']) and (update['result'] != []):
-                break
-
-        payload['offset'], payload['limit'] = update['result'][len(update['result'])-1]['update_id'], 1
-        while True:
-            responce = self.request('getupdates', payload, 'post')
-            if responce != None and responce['result'] != []:
-                payload['offset'] += 1
-                yield message(responce['result'][0])
-
-    async def send_message(
-            self,
-            chat_id: str | int,
-            text: str,
-            reply_markup: int = None,
-            reply_to_message_id: int = None
-    ) -> dict:
-        '''Use this method to send text messages
-        :param chat_id:
-            The ID of the group you can send messages to. requirement**
-        :param text:
-            You can only send between 1 and 4096 characters*. requirement**
-        :param reply_markup:
-            Additional features of the arm user interface. optional**
-        :param reply_to_message_id:
-            The ID of the original message, if the message is a reply. optional**
-        :return:
-            If successful, the sent message will be returned.
-        '''
-        payload: dict = {
-            'chat_id': chat_id,
-            'text': text,
-            'reply_markup': reply_markup,
-            'reply_to_message_id': reply_to_message_id
-        }
-        return self.request('sendmessage', data=payload)
-
-    async def edit_message(
-            self,
-            chat_id: str | int,
-            text: str,
-            message_id: int,
-            reply_markup: int = None
-    ) -> dict:
-        payload: dict = {
-            'chat_id': chat_id,
-            'text': text,
-            'reply_to_message_id': message_id,
-            'reply_markup': reply_markup
-        }
-        return self.request('editmessage', data=payload)
-
-
-    async def forward_message(
-            self,
-            chat_id: str | int,
-            from_chat_id: str | int,
-            message_id: int
-    ) -> dict:
-        payload: dict = {
-            'chat_id': chat_id, 'from_chat_id': from_chat_id, 'message_id': message_id
-        }
-        return self.request('forwardmessage', data=payload)
-
-
-    async def delete_message(self, chat_id: str | int, message_id: int) -> dict:
-        payload: dict = {
-            'chat_id': chat_id, 'reply_to_message_id': message_id
-        }
-        return self.request('deletemessage', data=payload)
-
-
-    async def send_contact(
-            self,
-            chat_id: str | int,
-            phone_number: int,
-            first_name: str,
-            last_name: str = None,
-            reply_to_message_id: int = None
-    ) -> dict:
-        '''This method is used to send a phone contact
-        :param chat_id:
-            The ID of the group you can send messages to. requirement**
-        :param phone_number:
-            contact number. requirement**
-        :param first_name:
-            Contact's first name. requirement**
-        :param last_name:
-            Last name of the addressee. optional**
-        :param reply_to_message_id:
-            The ID of the original message, if the message is a reply. optional**
-        :return:
-            On successful execution, the sent message is returned as output.
-        '''
-        payload: dict = {
-            'chat_id': chat_id,
-            'phone_number': phone_number,
-            'first_name': first_name,
-            'last_name': last_name,
-            'reply_to_message_id': reply_to_message_id
-        }
-        return self.request('sendcontact', data=payload)
-
-
-    async def send_photo(
-            self,
-            chat_id: str | int,
-            from_chat_id: str | int,
-            file: str | bytes,
-            caption: str = None,
-            reply_to_message_id: int = None,
-            reply_markup: int = None
-    ) -> dict:
-        payload: dict = {
-            'chat_id': chat_id,
-            'from_chat_id': from_chat_id,
-            'photo': open(file, 'rb'),
-            'caption': caption,
-            'reply_to_message_id': reply_to_message_id,
-            'reply_markup': reply_markup
-        }
-        return self.request('sendphoto', data=payload)
-
-
-    async def send_audio(
-            self,
-            chat_id: str | int,
-            file: str | bytes,
-            caption: str = None,
-            reply_to_message_id: int = None,
-            reply_markup: str = None
-    ) -> dict:
-        payload: dict = {
-            'chat_id': chat_id,
-            'audio': open(file, 'rb'),
-            'caption': caption,
-            'reply_to_message_id': reply_to_message_id,
-            'reply_markup': reply_markup
-        }
-        return self.request('sendaudio', data=payload)
-
-
-    async def send_document(
-            self,
-            chat_id: str | int,
-            file: str | bytes,
-            caption: str = None,
-            reply_to_message_id: int = None,
-            reply_markup: int = None
-    ) -> dict:
-        '''This method is used to send public files.
-        :param chat_id:
-            Conversation ID. requirement**
-        :param file:
-            Document file to be sent. The maximum file size is 50 MB. requirement**
-        :param caption:
-            Subtitle of the document, between 0 and 1024 characters. optional**
-        :param reply_to_message_id:
-            The ID of the original message, if the message is a reply. optional**
-        :param reply_markup:
-            Additional features of the arm user interface. optional**
-        :return:
-            If successful, the sent message will be returned
-        '''
-        payload: dict = {
-            'chat_id': chat_id,
-            'document': open(file, 'rb'),
-            'caption': caption,
-            'reply_to_message_id': reply_to_message_id,
-            'reply_markup': reply_markup
-        }
-        return self.request('senddocument', data=payload)
-
-
-    async def send_animation(
-            self,
-            chat_id: str | int,
-            file: str | bytes,
-            reply_to_message_id: int = None,
-            caption: str = None,
-            reply_markup: int = None
-    ) -> dict:
-        '''This method is used to send animation files (GIF video or H.264/MPEG-4 AVC without sound)'''
-        payload: dict = {
-            'chat_id': chat_id,
-            'animation': open(file, 'rb'),
-            'caption': caption,
-            'reply_to_message_id': reply_to_message_id,
-            'reply_markup': reply_markup
-        }
-        return self.request('sendanimation', data=self.form_data)
-
-
-
-    async def send_voice(
-            self,
-            chat_id: str | int,
-            file: str | bytes,
-            caption: str,
-            reply_to_message_id: int = None,
-            reply_markup: int = None
-    ) -> dict:
-        payload: dict = {
-            'chat_id': chat_id,
-            'voice': open(file, 'rb'),
-            'caption': caption,
-            'reply_to_message_id': reply_to_message_id,
-            'reply_markup': reply_markup
-        }
-        return self.request('sendvoice', data=self.form_data)
-
-
-    async def send_location(
-            self,
-            chat_id: str | int,
-            latitude: float,
-            longitude: float,
-            horizontal_accuracy: float,
-            reply_to_message_id: int = None,
-            reply_markup: int = None
-    ) -> dict:
-        '''This method is used to send a map point
-        :param chat_id:
-            Conversation ID. requirement**
-        :param latitude:
-            The latitude of the location. requirement**
-        :param longitude
-            The longitude of the location. requirement**
-        :param horizontal_accuracy
-            The radius of uncertainty for a spatial point
-            is measured in meters and is a number between 0 and 1500. optional**
-        :param reply_to_message_id:
-            The ID of the original message, if the message is a reply. optional**
-        :param reply_markup:
-            Additional features of the arm user interface. optional**
-        :return:
-            On successful execution, the sent message is returned as output.
-        '''
-        payload: dict = {
-            'chat_id': chat_id,
-            'latitude': latitude,
-            'longitude': longitude,
-            'horizontal_accuracy': horizontal_accuracy,
-            'reply_to_message_id': reply_to_message_id,
-            'reply_markup': reply_markup
-        }
-        return self.request('sendlocation', data=payload)
-
-
-    async def set_webhook(self, url: str) -> dict:
-        '''This method is used to specify an outgoing webhook URL'''
-        payload: dict = {
-            'url': url
-        }
-        return self.request('setwebhook', data=payload)
-
-
-    async def delete_webhook(self) -> dict:
-        return self.request(method='deletewebhook')
-
-
-    async def get_webhook_info(self) -> dict:
-        '''Use this method to get the current state of the webhook'''
-        return self.request(data='getwebhookinfo')
-
-
-    async def webhook_info(self, url: str) -> dict:
-        '''Displays the current state of a webhook'''
-        payload: dict = {
-            'url': url
-        }
-        return self.request('webhookinfo', data=payload)
-
-    async def get_me(self) -> dict:
-        '''get bot account information'''
-        return self.request(method='getme')
-
-
-    async def get_chat(self, chat_id: str) -> dict:
-        '''This method is used to get up-to-date information
-        about the conversation (current username for one-to-one conversations,
-        current username of a user, group or channel).
-        :param chat_id:
-            Conversation ID. requirement**
-        :return:
-            Returns a Chat object on success.
-        '''
-        payload: dict = {
-            'chat_id': chat_id
-        }
-        return self.request('getchat', data=payload)
-
-
-    async def leave_chat(self, chat_id: str) -> dict:
-        '''This method is used for the arm to leave a group, group or channel
-        :param chat_id:
-            Conversation ID. requirement**
-        :return:
-            If successful, its output is True.
-        '''
-        payload: dict = {
-            'chat_id': chat_id
-        }
-        return self.request('leavechat', data=payload)
-
-
-    async def get_updates(self, offset: int = 0, limit: int = 0) -> dict:
-        payload: dict = {
-            'offset': offset, 'limit': limit
-        }
-        return self.request('getupdates', data=payload)
-
-
-    async def get_chat_administrators(self, chat_id: str, just_get_id: bool = False) -> dict:
-        payload: dict = {
-            'chat_id': chat_id
-        }
-        responce = self.request('getchatadministrators', data=payload)
-
-        if just_get_id:
-            ids = []
-            for user in responce['result']:
-                ids.append(user['user']['id'])
-
-            return ids
-        else:
-            return responce
-
-
-    async def get_chat_members_count(self, chat_id: str) -> dict:
-        payload: dict = {
-            'chat_id': chat_id
-        }
-        return self.request('getchatmemberscount', data=payload)
-
-
-    async def get_chat_member(self, chat_id: str, user_id: str) -> dict:
-        payload: dict = {
-            'chat_id': chat_id, 'user_id': user_id
-        }
-        return self.request('getchatmember', data=payload)
-
-
-    async def set_chat_photo(self, chat_id: str | int, file = str | bytes) -> dict:
-        payload: dict = {
-            'chat_id': chat_id,
-            'photo': open(file, 'rb')
-        }
-        return self.request('setchatphoto', data=payload)
-
-
-    async def ban_chat_member(self, chat_id: str | int, user_id: str | int) ->  dict:
-        payload: dict = {
-            'chat_id': chat_id, 'user_id': user_id
-        }
-        return self.request('banchatmember', data=payload)
-
-
-    async def un_ban_chat_member(self, chat_id: str | int, user_id: str | int) -> dict:
-        payload: dict = {
-            'chat_id': chat_id, 'user_id': user_id
-        }
-        return self.request('unbanchatmember', data=payload)
-
-
-    async def get_file(self, file_id: str) -> dict:
-        '''This method is used to get the basic information
-        of a file and prepare it for download.
-        :param file_id:
-            ID of the file whose information should be received. requirement**
-        :return:
-            Returns a File object on successful execution
-        '''
-        payload: dict = {
-            'file_id': file_id
-        }
-        return self.request('getfile', data=payload)
+from .network import Network
+from .util import message
+from .exceptions import TokenNotInvalid
+
+from requests import post
+from json import loads, dump
+import asyncio
+
+
+class Client:
+
+    def __init__(self, token: str, timeout: float = 20) -> None:
+        self.loop = asyncio.get_event_loop()
+        self.network = Network(token=token, timeout=timeout)
+        self.url = f'https://tapi.bale.ai/bot{token}/'
+
+        if not token or len(token) < 50 or len(token) > 50:
+            raise TokenNotInvalid('`token` did\'t passed')
+        
+        elif len(token) == 50:
+            js = post(f"{self.url}getme").json()
+            if js["ok"] == True:
+                with open('config.json', 'w') as json_file:
+                    dump(js, json_file, indent=4)
+            else:
+                raise TokenNotInvalid('`token` did\'t passed')
+
+    async def request(self, method: str, data: dict = None, files: dict = None) -> dict:
+        try:
+            return await self.network.connect(method=method, data=data, files=files)
+        except Exception as err:
+            print(__file__, err, __file__)
+
+    async def on_message(self):
+        '''Use this method to receive updates
+        Example:
+            from bale import Client
+            import asyncio
+
+            client = Client('token', timeout=10)
+            async def main():
+                for update in client.on_message():
+                    print(update.text)
+                    await update.reply('hello __from__ **balepy**')
+
+            asyncio.run(main())
+        '''
+        payload: dict = {
+            'offset': 0, 'limit': 100
+        }
+        while True:
+            update = await self.request('getupdates', payload)
+            payload['offset'] = 1
+            if update != None and update != []:
+                break
+
+        payload['offset'], payload['limit'] = update[len(update)-1]['update_id'], 1
+        while True:
+            responce = await self.request('getupdates', payload)
+            if responce != None and responce != []:
+                payload['offset'] += 1
+                yield message(responce[0], self.network.token, self.network.timeout)
+
+
+    async def send_message(
+            self,
+            chat_id: str | int,
+            text: str,
+            reply_markup: int = None,
+            reply_to_message_id: int = None
+    ) -> dict:
+        '''Use this method to send text messages
+        :param chat_id:
+            The ID of the group you can send messages to. requirement**
+        :param text:
+            You can only send between 1 and 4096 characters*. requirement**
+        :param reply_markup:
+            Additional features of the arm user interface. optional**
+        :param reply_to_message_id:
+            The ID of the original message, if the message is a reply. optional**
+        :return:
+            If successful, the sent message will be returned.
+        '''
+        payload: dict = {
+            'chat_id': chat_id,
+            'text': text,
+            'reply_markup': reply_markup,
+            'reply_to_message_id': reply_to_message_id
+        }
+        return await self.request('sendmessage', data=payload)
+
+    # async def InlineKeyboard(
+    #         self,
+    #         chat_id: str | int,
+    #         text: str,
+    #         name_keyboard: str,
+    #         callback: str
+    # ) -> dict:
+    #     '''
+    #     Use Method for send Inline Keyboard in chat
+    #     :param chat_id:
+    #         The ID of the group you can send messages to. requirement**
+    #     :param text:
+    #         You can only send between 1 and 4096 characters*. requirement**
+    #     :param name_keyboard:
+    #         The Name for create keyboard in chat. requirement**
+    #     :param callback:
+    #         callback for get answer name_keyboard. requiremnt**
+    #     '''
+    #     payload = {
+    #         'chat_id': chat_id,
+    #         'text': text,
+    #         'reply_markup': {"inline_keyboard": [[{name_keyboard, callback}]]}
+    #     }
+    #     return await self.request('sendmessage', data=payload)
+
+
+    async def edit_message(
+            self,
+            chat_id: str | int,
+            text: str,
+            message_id: int,
+            reply_markup: int = None
+    ) -> dict:
+        payload: dict = {
+            'chat_id': chat_id,
+            'text': text,
+            'reply_to_message_id': message_id,
+            'reply_markup': reply_markup
+        }
+        return await self.request('editmessage', data=payload)
+
+
+    async def forward_message(
+            self,
+            chat_id: str | int,
+            from_chat_id: str | int,
+            message_id: int
+    ) -> dict:
+        payload: dict = {
+            'chat_id': chat_id, 'from_chat_id': from_chat_id, 'message_id': message_id
+        }
+        return await self.request('forwardmessage', data=payload)
+
+
+    async def delete_message(self, chat_id: str | int, message_id: int) -> dict:
+        payload: dict = {
+            'chat_id': chat_id, 'reply_to_message_id': message_id
+        }
+        return await self.request('deletemessage', data=payload)
+
+
+    async def send_contact(
+            self,
+            chat_id: str | int,
+            phone_number: int,
+            first_name: str,
+            last_name: str = None,
+            reply_to_message_id: int = None
+    ) -> dict:
+        '''This method is used to send a phone contact
+        :param chat_id:
+            The ID of the group you can send messages to. requirement**
+        :param phone_number:
+            contact number. requirement**
+        :param first_name:
+            Contact's first name. requirement**
+        :param last_name:
+            Last name of the addressee. optional**
+        :param reply_to_message_id:
+            The ID of the original message, if the message is a reply. optional**
+        :return:
+            On successful execution, the sent message is returned as output.
+        '''
+        payload: dict = {
+            'chat_id': chat_id,
+            'phone_number': phone_number,
+            'first_name': first_name,
+            'last_name': last_name,
+            'reply_to_message_id': reply_to_message_id
+        }
+        return await self.request('sendcontact', data=payload)
+
+
+    async def send_photo(
+            self,
+            chat_id: str | int,
+            from_chat_id: str | int,
+            file: str | bytes,
+            caption: str = None,
+            reply_to_message_id: int = None,
+            reply_markup: int = None
+    ) -> dict:
+        files: dict = {
+            'photo': open(file, 'rb')
+        }
+        payload: dict = {
+            'chat_id': chat_id,
+            'from_chat_id': from_chat_id,
+            'caption': caption,
+            'reply_to_message_id': reply_to_message_id,
+            'reply_markup': reply_markup
+        }
+        return await self.request('sendphoto', data=payload, files=files)
+
+
+    async def send_audio(
+            self,
+            chat_id: str | int,
+            file: str | bytes,
+            caption: str = None,
+            reply_to_message_id: int = None,
+            reply_markup: str = None
+    ) -> dict:
+        files: dict = {
+            'audio': open(file, 'rb')
+        }
+        payload: dict = {
+            'chat_id': chat_id,
+            'caption': caption,
+            'reply_to_message_id': reply_to_message_id,
+            'reply_markup': reply_markup
+        }
+        return await self.request('sendaudio', data=payload, files=files)
+
+
+    async def send_document(
+            self,
+            chat_id: str | int,
+            file: str | bytes,
+            caption: str = None,
+            reply_to_message_id: int = None,
+            reply_markup: int = None
+    ) -> dict:
+        '''This method is used to send public files.
+        :param chat_id:
+            Conversation ID. requirement**
+        :param file:
+            Document file to be sent. The maximum file size is 50 MB. requirement**
+        :param caption:
+            Subtitle of the document, between 0 and 1024 characters. optional**
+        :param reply_to_message_id:
+            The ID of the original message, if the message is a reply. optional**
+        :param reply_markup:
+            Additional features of the arm user interface. optional**
+        :return:
+            If successful, the sent message will be returned
+        '''
+        files: dict = {
+            'document': open(file, 'rb')
+        }
+        payload: dict = {
+            'chat_id': chat_id,
+            'caption': caption,
+            'reply_to_message_id': reply_to_message_id,
+            'reply_markup': reply_markup
+        }
+        return await self.request('senddocument', data=payload, files=files)
+
+
+    async def send_animation(
+            self,
+            chat_id: str | int,
+            file: str | bytes,
+            reply_to_message_id: int = None,
+            caption: str = None,
+            reply_markup: int = None
+    ) -> dict:
+        '''This method is used to send animation files (GIF video or H.264/MPEG-4 AVC without sound)'''
+        files: dict = {
+            'animation': open(file, 'rb')
+        }
+        payload: dict = {
+            'chat_id': chat_id,
+            'caption': caption,
+            'reply_to_message_id': reply_to_message_id,
+            'reply_markup': reply_markup
+        }
+        return await self.request('sendanimation', data=payload, files=files)
+
+
+
+    async def send_voice(
+            self,
+            chat_id: str | int,
+            file: str | bytes,
+            caption: str,
+            reply_to_message_id: int = None,
+            reply_markup: int = None
+    ) -> dict:
+        files: dict = {
+            'voice': open(file, 'rb')
+        }
+        payload: dict = {
+            'chat_id': chat_id,
+            'caption': caption,
+            'reply_to_message_id': reply_to_message_id,
+            'reply_markup': reply_markup
+        }
+        return await self.request('sendvoice', data=payload, files=files)
+
+
+    async def send_location(
+            self,
+            chat_id: str | int,
+            latitude: float,
+            longitude: float,
+            horizontal_accuracy: float,
+            reply_to_message_id: int = None,
+            reply_markup: int = None
+    ) -> dict:
+        '''This method is used to send a map point
+        :param chat_id:
+            Conversation ID. requirement**
+        :param latitude:
+            The latitude of the location. requirement**
+        :param longitude
+            The longitude of the location. requirement**
+        :param horizontal_accuracy
+            The radius of uncertainty for a spatial point
+            is measured in meters and is a number between 0 and 1500. optional**
+        :param reply_to_message_id:
+            The ID of the original message, if the message is a reply. optional**
+        :param reply_markup:
+            Additional features of the arm user interface. optional**
+        :return:
+            On successful execution, the sent message is returned as output.
+        '''
+        payload: dict = {
+            'chat_id': chat_id,
+            'latitude': latitude,
+            'longitude': longitude,
+            'horizontal_accuracy': horizontal_accuracy,
+            'reply_to_message_id': reply_to_message_id,
+            'reply_markup': reply_markup
+        }
+        return await self.request('sendlocation', data=payload)
+
+
+    async def set_webhook(self, url: str) -> dict:
+        '''This method is used to specify an outgoing webhook URL'''
+        payload: dict = {
+            'url': url
+        }
+        return self.request('setwebhook', data=payload)
+
+
+    async def delete_webhook(self) -> dict:
+        return await self.request(method='deletewebhook')
+
+
+    async def get_webhook_info(self) -> dict:
+        '''Use this method to get the current state of the webhook'''
+        return await self.request(data='getwebhookinfo')
+
+
+    async def webhook_info(self, url: str) -> dict:
+        '''Displays the current state of a webhook'''
+        payload: dict = {
+            'url': url
+        }
+        return await self.request('webhookinfo', data=payload)
+
+    async def get_me(self) -> dict:
+        '''get bot account information'''
+        return await self.request(method='getme')
+
+
+    async def get_chat(self, chat_id: str) -> dict:
+        '''This method is used to get up-to-date information
+        about the conversation (current username for one-to-one conversations,
+        current username of a user, group or channel).
+        :param chat_id:
+            Conversation ID. requirement**
+        :return:
+            Returns a Chat object on success.
+        '''
+        payload: dict = {
+            'chat_id': chat_id
+        }
+        return await self.request('getchat', data=payload)
+
+
+    async def leave_chat(self, chat_id: str) -> dict:
+        '''This method is used for the arm to leave a group, group or channel
+        :param chat_id:
+            Conversation ID. requirement**
+        :return:
+            If successful, its output is True.
+        '''
+        payload: dict = {
+            'chat_id': chat_id
+        }
+        return await self.request('leavechat', data=payload)
+
+
+    async def get_chat_invite_link(self, chat_id: str) -> str:
+        chat_data = await self.get_chat(chat_id=chat_id)
+        return chat_data['invite_link']
+
+
+    async def get_updates(self, offset: int = 0, limit: int = 0) -> dict:
+        payload: dict = {
+            'offset': offset, 'limit': limit
+        }
+        return await self.request('getupdates', data=payload)
+
+
+    async def get_chat_administrators(self, chat_id: str, just_get_id: bool = False) -> dict:
+        payload: dict = {
+            'chat_id': chat_id
+        }
+        responce = await self.request('getchatadministrators', data=payload)
+
+        if just_get_id:
+            chat_admins = list()
+            for admin in responce:
+                chat_admins.append(admin['user']['id'])
+
+            return chat_admins
+        return responce
+
+
+    async def get_chat_members_count(self, chat_id: str) -> dict:
+        payload: dict = {
+            'chat_id': chat_id
+        }
+        return await self.request('getchatmemberscount', data=payload)
+
+
+    async def get_chat_member(self, chat_id: str, user_id: str) -> dict:
+        payload: dict = {
+            'chat_id': chat_id, 'user_id': user_id
+        }
+        return await self.request('getchatmember', data=payload)
+
+
+    async def set_chat_photo(self, chat_id: str | int, file = str | bytes) -> dict:
+        files: dict = {
+            'photo': open(file, 'rb')
+        }
+        payload: dict = {
+            'chat_id': chat_id,
+        }
+        return await self.request('setchatphoto', data=payload, files=files)
+
+
+    async def ban_chat_member(self, chat_id: str | int, user_id: str | int) ->  dict:
+        payload: dict = {
+            'chat_id': chat_id, 'user_id': user_id
+        }
+        return await self.request('banchatmember', data=payload)
+
+
+    async def un_ban_chat_member(self, chat_id: str | int, user_id: str | int) -> dict:
+        payload: dict = {
+            'chat_id': chat_id, 'user_id': user_id
+        }
+        return await self.request('unbanchatmember', data=payload)
+
+
+    async def get_file(self, file_id: str) -> dict:
+        '''This method is used to get the basic information
+        of a file and prepare it for download.
+        :param file_id:
+            ID of the file whose information should be received. requirement**
+        :return:
+            Returns a File object on successful execution
+        '''
+        payload: dict = {
+            'file_id': file_id
+        }
+        return await self.request('getfile', data=payload)
```

### Comparing `balepy-1.3.7.4/bale/util.py` & `balepy-1.3.8/bale/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,300 +1,326 @@
-
-class message:
-
-    def __init__(self, data: dict):
-        self.data = data
-
-    @property
-    def message(self):
-        if 'callback_query' in self.data:
-            return self.data['callback_query']['message']
-        elif 'message' in self.data:
-            return self.data['message']
-
-    @property
-    def is_callback(self):
-        if 'callback_query' in self.data:
-            return True
-        else:
-            return False
-
-    @property
-    def update_id(self):
-        return self.data['update_id']
-
-    @property
-    def message_id(self):
-        return self.message['message_id']
-
-    @property
-    def author_id(self):
-        return self.message['from']['id']
-
-    @property
-    def callback_author_id(self):
-        if self.is_callback:
-            return self.data['callback_query']['from']['id']
-        else:
-            return None
-
-    @property
-    def is_bot(self):
-        return self.message['from']['is_bot']
-
-    @property
-    def callback_is_bot(self):
-        if self.is_callback:
-            return self.data['callback_query']['from']['is_bot']
-        else:
-            return None
-
-    @property
-    def author_first_name(self):
-        return self.message['from']['first_name']
-
-    @property
-    def callback_author_first_name(self):
-        if self.is_callback:
-            return self.data['callback_query']['from']['first_name']
-        else:
-            return None
-
-    @property
-    def author_last_name(self):
-        return self.message['from']['last_name']
-
-    @property
-    def callback_author_last_name(self):
-        if self.is_callback:
-            return self.data['callback_query']['from']['last_name']
-        else:
-            return None
-
-    @property
-    def author_username(self):
-        if 'username' in self.message['from']:
-            return self.message['from']['username']
-        else:
-            return None
-
-    @property
-    def callback_author_username(self):
-        if self.is_callback:
-            if 'username' in self.data['callback_query']:
-                return self.data['callback_query']['from']['username']
-            else:
-                return None
-        else:
-            return None
-
-    @property
-    def chat_id(self):
-        return self.message['chat']['id']
-
-    @property
-    def chat_type(self):
-        return self.message['chat']['type']
-
-    @property
-    def chat_title(self):
-        return self.message['chat']['title']
-
-    @property
-    def new_member(self):
-        if 'new_chat_members' in self.message:
-            return True
-        else:
-            return False
-
-    @property
-    def new_member_id(self):
-        if self.new_member:
-            return self.message['new_chat_members'][0]['id']
-        else:
-            return None
-
-    @property
-    def new_member_is_bot(self):
-        if self.new_member:
-            return self.message['new_chat_members'][0]['is_bot']
-        else:
-            return None
-
-    @property
-    def new_memberr_first_name(self):
-        if self.new_member:
-            return self.message['new_chat_members'][0]['first_name']
-        else:
-            return None
-
-    @property
-    def new_member_last_name(self):
-        if self.new_member:
-            return self.message['new_chat_members'][0]['last_name']
-        else:
-            return None
-
-    @property
-    def new_member_username(self):
-        if self.new_member and 'username' in self.message['new_chat_members'][0]:
-            return self.message['new_chat_members'][0]['username']
-        else:
-            return None
-
-    @property
-    def left_member(self):
-        if 'left_chat_member' in self.message:
-            return True
-        else:
-            return False
-
-    @property
-    def left_member_id(self):
-        if self.left_member:
-            return self.message['left_chat_member']['id']
-        else:
-            return None
-
-    @property
-    def left_member_is_bot(self):
-        if self.left_member:
-            return self.message['left_chat_member']['is_bot']
-        else:
-            return None
-
-    @property
-    def left_member_first_name(self):
-        if self.left_member:
-            return self.message['left_chat_member']['first_name']
-        else:
-            return None
-
-    @property
-    def left_member_last_name(self):
-        if self.left_member:
-            return self.message['left_chat_member']['last_name']
-        else:
-            return None
-
-    @property
-    def left_member_username(self):
-        if self.left_member and 'username' in self.message['left_chat_member']:
-            return self.message['left_chat_member']['username']
-        else:
-            return None
-
-    @property
-    def is_reply(self):
-        if 'reply_to_message' in self.message:
-            return True
-        else:
-            return False
-
-    @property
-    def reply_message_id(self):
-        if 'reply_to_message' in self.message:
-            return self.message['reply_to_message']['message_id']
-        else:
-            return False
-
-    @property
-    def reply_data(self):
-        if 'reply_to_message' in self.message:
-            return self.message['reply_to_message']
-        else:
-            return False
-
-    @property
-    def is_forward(self):
-        if 'forward_from' in self.message:
-            return True
-        elif 'forward_from_chat' in self.message:
-            return True
-        else:
-            return False
-
-    @property
-    def forward_from_id(self):
-        if 'forward_from' in self.message:
-            return self.message['forward_from']['id']
-        elif 'forward_from_chat' in self.message:
-            return self.message['forward_from_chat']['id']
-        else:
-            return None
-
-    @property
-    def forward_from_message_id(self):
-        if 'forward_from_message_id' in self.message:
-            return self.message['forward_from_message_id']
-        else:
-            return None
-
-    @property
-    def forward_from_is_bot(self):
-        if 'forward_from' in self.message:
-            return self.message['forward_from']['is_bot']
-        else:
-            return None
-
-    @property
-    def forward_from_is_bot(self):
-        if self.is_forward:
-            return self.message['forward_from']['is_bot']
-        else:
-            return None
-
-    @property
-    def text(self):
-        if 'text' in self.message:
-            return self.message['text']
-        elif 'caption' in self.message:
-            return self.message['caption']
-        else:
-            return None
-
-    @property
-    def callback_data_send(self):
-        if self.is_callback:
-            return self.data['callback_query']['data']
-        else:
-            return None
-
-    @property
-    def file_data(self):
-        if 'photo' in self.message:
-            return self.message['photo']
-        elif 'video' in self.message:
-            return self.message['video']
-        elif 'document' in self.message:
-            return self.message['document']
-        elif 'audio' in self.message:
-            return self.message['audio']
-        else:
-            return None
-
-    @property
-    def message_type(self):
-        if 'text' in self.message:
-            return 'text'
-        elif 'photo' in self.message:
-            if 'caption' in self.message:
-                return 'photoCaption'
-            else:
-                return 'photo'
-        elif 'video' in self.message:
-            if 'caption' in self.message:
-                return 'videoCaption'
-            else:
-                return 'video'
-        elif 'document' in self.message:
-            if 'caption' in self.message:
-                return 'documentCaption'
-            else:
-                return 'document'
-        elif 'audio' in self.message:
-            if 'caption' in self.message:
-                return 'audioCaption'
-            else:
-                return 'audio'
-        else:
-            return None
+from .network import Network
+
+class message:
+
+    def __init__(self, data: dict, token: str, timeout: float):
+        self.network = Network(token=token, timeout=timeout)
+        self.data = data
+
+    @property
+    def message(self):
+        if 'callback_query' in self.data:
+            return self.data['callback_query']['message']
+        elif 'message' in self.data:
+            return self.data['message']
+
+    @property
+    def is_callback(self):
+        if 'callback_query' in self.data:
+            return True
+        else:
+            return False
+
+    @property
+    def update_id(self):
+        return self.data['update_id']
+
+    @property
+    def message_id(self):
+        return self.message['message_id']
+
+    @property
+    def author_id(self):
+        return self.message['from']['id']
+
+    @property
+    def callback_author_id(self):
+        if self.is_callback:
+            return self.data['callback_query']['from']['id']
+        else:
+            return None
+
+    @property
+    def is_bot(self):
+        return self.message['from']['is_bot']
+
+    @property
+    def callback_is_bot(self):
+        if self.is_callback:
+            return self.data['callback_query']['from']['is_bot']
+        else:
+            return None
+
+    @property
+    def author_first_name(self):
+        return self.message['from']['first_name']
+
+    @property
+    def callback_author_first_name(self):
+        if self.is_callback:
+            return self.data['callback_query']['from']['first_name']
+        else:
+            return None
+
+    @property
+    def author_last_name(self):
+        return self.message['from']['last_name']
+
+    @property
+    def callback_author_last_name(self):
+        if self.is_callback:
+            return self.data['callback_query']['from']['last_name']
+        else:
+            return None
+
+    @property
+    def author_username(self):
+        if 'username' in self.message['from']:
+            return self.message['from']['username']
+        else:
+            return None
+
+    @property
+    def callback_author_username(self):
+        if self.is_callback:
+            if 'username' in self.data['callback_query']:
+                return self.data['callback_query']['from']['username']
+            else:
+                return None
+        else:
+            return None
+
+    @property
+    def chat_id(self):
+        return self.message['chat']['id']
+
+    @property
+    def chat_type(self):
+        return self.message['chat']['type']
+
+    @property
+    def chat_title(self):
+        return self.message['chat']['title']
+
+    @property
+    def new_member(self):
+        if 'new_chat_members' in self.message:
+            return True
+        else:
+            return False
+
+    @property
+    def new_member_id(self):
+        if self.new_member:
+            return self.message['new_chat_members'][0]['id']
+        else:
+            return None
+
+    @property
+    def new_member_is_bot(self):
+        if self.new_member:
+            return self.message['new_chat_members'][0]['is_bot']
+        else:
+            return None
+
+    @property
+    def new_memberr_first_name(self):
+        if self.new_member:
+            return self.message['new_chat_members'][0]['first_name']
+        else:
+            return None
+
+    @property
+    def new_member_last_name(self):
+        if self.new_member:
+            return self.message['new_chat_members'][0]['last_name']
+        else:
+            return None
+
+    @property
+    def new_member_username(self):
+        if self.new_member and 'username' in self.message['new_chat_members'][0]:
+            return self.message['new_chat_members'][0]['username']
+        else:
+            return None
+
+    @property
+    def left_member(self):
+        if 'left_chat_member' in self.message:
+            return True
+        else:
+            return False
+
+    @property
+    def left_member_id(self):
+        if self.left_member:
+            return self.message['left_chat_member']['id']
+        else:
+            return None
+
+    @property
+    def left_member_is_bot(self):
+        if self.left_member:
+            return self.message['left_chat_member']['is_bot']
+        else:
+            return None
+
+    @property
+    def left_member_first_name(self):
+        if self.left_member:
+            return self.message['left_chat_member']['first_name']
+        else:
+            return None
+
+    @property
+    def left_member_last_name(self):
+        if self.left_member:
+            return self.message['left_chat_member']['last_name']
+        else:
+            return None
+
+    @property
+    def left_member_username(self):
+        if self.left_member and 'username' in self.message['left_chat_member']:
+            return self.message['left_chat_member']['username']
+        else:
+            return None
+
+    @property
+    def is_reply(self):
+        if 'reply_to_message' in self.message:
+            return True
+        else:
+            return False
+
+    @property
+    def reply_message_id(self):
+        if 'reply_to_message' in self.message:
+            return self.message['reply_to_message']['message_id']
+        else:
+            return False
+
+    @property
+    def reply_data(self):
+        if 'reply_to_message' in self.message:
+            return self.message['reply_to_message']
+        else:
+            return False
+
+    @property
+    def is_forward(self):
+        if 'forward_from' in self.message:
+            return True
+        elif 'forward_from_chat' in self.message:
+            return True
+        else:
+            return False
+
+    @property
+    def forward_from_id(self):
+        if 'forward_from' in self.message:
+            return self.message['forward_from']['id']
+        elif 'forward_from_chat' in self.message:
+            return self.message['forward_from_chat']['id']
+        else:
+            return None
+
+    @property
+    def forward_from_message_id(self):
+        if 'forward_from_message_id' in self.message:
+            return self.message['forward_from_message_id']
+        else:
+            return None
+
+    @property
+    def forward_from_is_bot(self):
+        if 'forward_from' in self.message:
+            return self.message['forward_from']['is_bot']
+        else:
+            return None
+
+    @property
+    def forward_from_is_bot(self):
+        if self.is_forward:
+            return self.message['forward_from']['is_bot']
+        else:
+            return None
+
+    @property
+    def text(self):
+        if 'text' in self.message:
+            return self.message['text']
+        elif 'caption' in self.message:
+            return self.message['caption']
+        else:
+            return None
+
+    @property
+    def callback_data_send(self):
+        if self.is_callback:
+            return self.data['callback_query']['data']
+        else:
+            return None
+
+    @property
+    def file_data(self):
+        if 'photo' in self.message:
+            return self.message['photo']
+        elif 'video' in self.message:
+            return self.message['video']
+        elif 'document' in self.message:
+            return self.message['document']
+        elif 'audio' in self.message:
+            return self.message['audio']
+        else:
+            return None
+
+    @property
+    def message_type(self):
+        if 'text' in self.message:
+            return 'text'
+        elif 'photo' in self.message:
+            if 'caption' in self.message:
+                return 'photoCaption'
+            else:
+                return 'photo'
+        elif 'video' in self.message:
+            if 'caption' in self.message:
+                return 'videoCaption'
+            else:
+                return 'video'
+        elif 'document' in self.message:
+            if 'caption' in self.message:
+                return 'documentCaption'
+            else:
+                return 'document'
+        elif 'audio' in self.message:
+            if 'caption' in self.message:
+                return 'audioCaption'
+            else:
+                return 'audio'
+        else:
+            return None
+
+    async def reply(self, text: str) -> dict:
+        payload: dict = {
+            'text': text,
+            'chat_id': self.chat_id,
+            'reply_to_message_id': self.message_id
+        }
+        return await self.network.connect('sendmessage', data=payload)
+
+    @property
+    def groups(self):
+        if self.message["chat"]["type"] == 'group':
+            return self.message
+        
+
+    @property
+    def channel(self):
+        if self.message["chat"]["type"] == 'channel':
+            return self.message
+        
+    @property
+    def private(self):
+        if self.message["chat"]["type"] == 'private':
+            return self.message
```

### Comparing `balepy-1.3.7.4/balepy.egg-info/PKG-INFO` & `balepy-1.3.8/balepy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,57 @@
-Metadata-Version: 2.1
-Name: balepy
-Version: 1.3.7.4
-Summary: balepy a Library Python for create bots API in bale application
-Home-page: https://github.com/OnlyRad/balepy
-Author: Mohammad, AmirAli
-Author-email: mohammadmehrabi175@gmail.com
-Keywords: bot,Bot,bale,robot,messangers
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: ~=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-
-# balepy
-
-<h3 align="center"> balepy a Library Python for create bot API in bale application </h3>
-
-## Install and Update:
-```bash
-pip install -U balepy
-```
-
-## For See Docs:
-- <a href="https://balepy.github.io">WebSite</a>
-- <a href="https://t.me/TheCommit">Telegram</a>
-
-## START:
-```python
-from bale import Client
-import asyncio
-
-
-__token = 'your-token-here'
-client = Client(__token, timeout=10)
-
-async def main():
-    for update in client.on_message():
-        await client.send_message(
-            chat_id=update.chat_id,
-            text='Hello __from__ *balepy*',
-            reply_to_message_id=update.message_id
-        )
-
-if __name__ == '__main__':
-    asyncio.run(main())
-```
-
-
-## Thanks To:
-### <a href="https://github.com/metect">AmirAli</a>
-
-## Social Media:
-#### <a href="https://t.me/TheCommit">TELEGRAM</a>
-#### <a href="https://rubika.ir/TheBalepy">RUBIKA</a>
+Metadata-Version: 2.1
+Name: balepy
+Version: 1.3.8
+Summary: balepy a Library Python for create bots API in bale application
+Home-page: https://github.com/OnlyRad/balepy
+Author: Mohammad, AmirAli
+Author-email: mohammadmehrabi175@gmail.com
+Keywords: bot,Bot,bale,robot,messangers
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: ~=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
+# balepy
+
+<p align=center>
+<img src="https://s8.uupload.ir/files/balethon_uvi2_esnh.png" style="width: 300px; height: 300px;" align=center alt="background">
+</p>
+<h3 align="center"> balepy a Library Python for create bot API in bale application <br> <h5 align=center> <a href="https://balepy.github.io"> Docs</a> | <a href="https://t.me/TheLinuxGP">Community</a> | <a href="https://t.me/TheCommit">Telegram Channel</a> | <a href="https://github.com/OnlyRad">Owner</a></h5></h3>
+
+
+## Install and Update:
+```bash
+pip install -U balepy
+```
+
+## START:
+```python
+from bale import Client
+from asyncio import run
+
+
+__token = 'your-token-here'
+client = Client(__token, timeout=10)
+
+async def main():
+    async for message in client.on_message():
+        await message.reply('hello __from__ **balepy**')
+
+
+if __name__ == '__main__':
+    run(main())
+```
+
+
+## Thanks To:
+### <a href="https://github.com/metect">AmirAli</a>
+
+<p>Thanks to all those who contributed directly or indirectly to the development of the module</p>
```

### Comparing `balepy-1.3.7.4/setup.py` & `balepy-1.3.8/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup, find_packages
-
-setup(
-    name = 'balepy',
-    version = '1.3.7.4',
-    author='Mohammad, AmirAli',
-    author_email = 'mohammadmehrabi175@gmail.com',
-    description = 'balepy a Library Python for create bots API in bale application',
-    keywords = ['bot' , 'Bot' , 'bale' , 'robot', 'messangers'],
-    long_description = open("README.md", encoding="utf-8").read(),
-    python_requires="~=3.6",
-    long_description_content_type = 'text/markdown',
-    url = 'https://github.com/OnlyRad/balepy',
-    packages = find_packages(),
-    install_requires = ['requests'],
-    classifiers = [
-    	'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'License :: OSI Approved :: MIT License',
-    ]
-)
+from setuptools import setup, find_packages
+
+setup(
+    name = 'balepy',
+    version = '1.3.8',
+    author='Mohammad, AmirAli',
+    author_email = 'mohammadmehrabi175@gmail.com',
+    description = 'balepy a Library Python for create bots API in bale application',
+    keywords = ['bot' , 'Bot' , 'bale' , 'robot', 'messangers'],
+    long_description = open("README.md", encoding="utf-8").read(),
+    python_requires="~=3.6",
+    long_description_content_type = 'text/markdown',
+    url = 'https://github.com/OnlyRad/balepy',
+    packages = find_packages(),
+    install_requires = ['requests'],
+    classifiers = [
+    	'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'License :: OSI Approved :: MIT License',
+    ]
+)
```

