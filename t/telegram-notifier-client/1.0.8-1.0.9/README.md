# Comparing `tmp/telegram_notifier_client-1.0.8.tar.gz` & `tmp/telegram_notifier_client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_notifier_client-1.0.8.tar", last modified: Sun Mar 24 14:42:46 2024, max compression
+gzip compressed data, was "telegram_notifier_client-1.0.9.tar", last modified: Sat Apr 20 11:46:10 2024, max compression
```

## Comparing `telegram_notifier_client-1.0.8.tar` & `telegram_notifier_client-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 rorschach  (1000) rorschach  (1000)        0 2024-03-24 14:42:46.083066 telegram_notifier_client-1.0.8/
--rw-r--r--   0 rorschach  (1000) rorschach  (1000)      822 2024-03-24 14:42:46.079065 telegram_notifier_client-1.0.8/PKG-INFO
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)      106 2023-08-12 14:44:16.000000 telegram_notifier_client-1.0.8/README.md
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)      605 2024-03-24 14:39:43.000000 telegram_notifier_client-1.0.8/pyproject.toml
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)       79 2024-03-24 14:42:46.083066 telegram_notifier_client-1.0.8/setup.cfg
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)      401 2024-03-24 14:39:42.000000 telegram_notifier_client-1.0.8/setup.py
-drwxrwxr-x   0 rorschach  (1000) rorschach  (1000)        0 2024-03-24 14:42:46.079065 telegram_notifier_client-1.0.8/src/
-drwxrwxr-x   0 rorschach  (1000) rorschach  (1000)        0 2024-03-24 14:42:46.079065 telegram_notifier_client-1.0.8/src/notifier_client/
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)        0 2023-08-12 14:44:16.000000 telegram_notifier_client-1.0.8/src/notifier_client/__init__.py
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)    19061 2024-03-24 14:39:42.000000 telegram_notifier_client-1.0.8/src/notifier_client/web_app_notifier_client.py
-drwxrwxr-x   0 rorschach  (1000) rorschach  (1000)        0 2024-03-24 14:42:46.079065 telegram_notifier_client-1.0.8/src/telegram_notifier_client.egg-info/
--rw-r--r--   0 rorschach  (1000) rorschach  (1000)      822 2024-03-24 14:42:46.000000 telegram_notifier_client-1.0.8/src/telegram_notifier_client.egg-info/PKG-INFO
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)      381 2024-03-24 14:42:46.000000 telegram_notifier_client-1.0.8/src/telegram_notifier_client.egg-info/SOURCES.txt
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)        1 2024-03-24 14:42:46.000000 telegram_notifier_client-1.0.8/src/telegram_notifier_client.egg-info/dependency_links.txt
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)       49 2024-03-24 14:42:46.000000 telegram_notifier_client-1.0.8/src/telegram_notifier_client.egg-info/requires.txt
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)       16 2024-03-24 14:42:46.000000 telegram_notifier_client-1.0.8/src/telegram_notifier_client.egg-info/top_level.txt
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-20 11:46:10.151797 telegram_notifier_client-1.0.9/
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-04-20 11:46:10.151797 telegram_notifier_client-1.0.9/PKG-INFO
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      106 2023-11-27 16:14:13.000000 telegram_notifier_client-1.0.9/README.md
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      605 2024-04-20 11:43:55.000000 telegram_notifier_client-1.0.9/pyproject.toml
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       79 2024-04-20 11:46:10.151797 telegram_notifier_client-1.0.9/setup.cfg
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      396 2024-04-20 11:43:55.000000 telegram_notifier_client-1.0.9/setup.py
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-20 11:46:10.147796 telegram_notifier_client-1.0.9/src/
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-20 11:46:10.147796 telegram_notifier_client-1.0.9/src/notifier_client/
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        0 2023-11-27 16:14:13.000000 telegram_notifier_client-1.0.9/src/notifier_client/__init__.py
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)    18780 2024-04-20 11:05:45.000000 telegram_notifier_client-1.0.9/src/notifier_client/web_app_notifier_client.py
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-20 11:46:10.151797 telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-04-20 11:46:10.000000 telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/PKG-INFO
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      381 2024-04-20 11:46:10.000000 telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        1 2024-04-20 11:46:10.000000 telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       49 2024-04-20 11:46:10.000000 telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/requires.txt
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       16 2024-04-20 11:46:10.000000 telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/top_level.txt
```

### Comparing `telegram_notifier_client-1.0.8/PKG-INFO` & `telegram_notifier_client-1.0.9/src/telegram_notifier_client.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
-Name: telegram_notifier_client
-Version: 1.0.8
+Name: telegram-notifier-client
+Version: 1.0.9
 Summary: telegram_notifier_client
 Home-page: https://github.com/deusfinance/notifier-client.git
-Author: Ali Ghorbani
+Author: Metalica
 Author-email: rorschach <rorschach45001@gmail.com>
 Project-URL: Homepage, https://github.com/deusfinance/notifier-client
 Project-URL: Issues, https://github.com/deusfinance/notifier-client/issues
+Keywords: telegram notifier client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: certifi
-Requires-Dist: charset-normalizer
-Requires-Dist: idna
-Requires-Dist: requests
-Requires-Dist: urllib3
 
 # notifier-client
 https://pypi.org/project/telegram-notifier-client/
 
 pip install telegram-notifier-client
```

### Comparing `telegram_notifier_client-1.0.8/pyproject.toml` & `telegram_notifier_client-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "telegram_notifier_client"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="rorschach", email="rorschach45001@gmail.com" },
 ]
 description = "telegram_notifier_client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `telegram_notifier_client-1.0.8/src/notifier_client/web_app_notifier_client.py` & `telegram_notifier_client-1.0.9/src/notifier_client/web_app_notifier_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,37 +10,36 @@
 
 @dataclass
 class Message:
     page: int
     content: str
     emergency: str = ''
     amend: dict = None
-    has_html_tag: bool = False
 
     def message(self) -> str:
-        if self.emergency and not self.has_html_tag:
+        if self.emergency:
             self.emergency = self.emergency.replace("<", "&lt;").replace(">", "&gt;")
-        if not self.has_html_tag:
-            self.content = self.content.replace("<", "&lt;").replace(">", "&gt;")
+        self.content = self.content.replace("<", "&lt;").replace(">", "&gt;")
         emergency = f"<b>Emergency Message</b><blockquote>{self.emergency}</blockquote>\n" if self.emergency else ""
         return f"<blockquote>{self.content}</blockquote>\n{emergency}<b>Page: {self.page}</b>\n"
 
 
 @dataclass
 class ErrorMessage:
     title: str
     apm_reference: str
     amend: dict = None
     mentions: str = None
 
     def message(self):
         self.title = self.title.replace("<", "&lt;").replace(">", "&gt;")
+        developers = f'\n👨‍💻    {self.mentions}' if self.mentions else ''
         return (f'<blockquote>🔵 Message:    <code class="language-python">{self.title}</code>\n'
-                f'📊 APM Reference:   <code>{self.apm_reference}</code>\n'
-                f'👨‍💻 Developers:    {self.mentions}</blockquote>\n')
+                f'📊 APM Reference:   <code>{self.apm_reference}</code>'
+                f'{developers}</blockquote>\n')
 
 
 class WebAppNotifierClient:
     def __init__(self, receiver_id: int, server_url: str, auth_token: str, topic_id: int = None):
         """
         Initializes a new instance of the WebAppNotifierClient.
         Parameters:
@@ -178,33 +177,30 @@
             server_url: str,
             auth_token: str,
             retrying_number: int = 5,
             telegram_bot_token=None,
             test_env=False,
             test_env_logger: Optional[Logger] = None,
             topic_id: Optional[int] = None,
-            max_msg_size: int = 3000,
-            message_html_tag: bool = False
+            max_msg_size: int = 3000
     ):
         """
            Initializes a new instance of the SendNotification.
 
            Parameters:
                - receiver_id (int): The receiver ID for sending notifications.
                - server_url (str): The server URL for the WebAppNotifierClient.
                - auth_token (str): The authentication token for the WebAppNotifierClient.
                - retrying_number (int): The number of times to retry sending a notification upon failure.
                - telegram_bot_token (str, optional): The bot token for the Telegram bot.
                - test_env (bool): Flag indicating if the notification is being sent in a test environment.
                - test_env_logger (logging.Logger, optional): The logger to use in the test environment.
                - topic_id (int, optional):
                - max_msg_size (int): The maximum allowed size for a message to be sent.
-               - message_html_tag: bool define if message has html or not
            """
-        self.message_html_tag = message_html_tag
         self.receiver_id = receiver_id
         self.server_url = server_url
         self.retiring_number = retrying_number
         self.telegram_bot_token = telegram_bot_token
         self.notifier_client = WebAppNotifierClient(self.receiver_id, server_url, auth_token, topic_id)
         self.test_env = test_env
         self.max_msg_size = max_msg_size
@@ -226,29 +222,31 @@
             - amend (dict, optional): Additional data to amend the alert message.
             - emergency_msg (str, optional): An emergency message to include, such as mentioning a user.
 
         Returns:
             - Optional[int]: The HTTP status code of the response (200 indicates that the message has been queued).
                               Returns None if in test environment.
         """
+        message = message.replace('<', '&lt;').replace('>', '&gt;')
         if self.test_env:
             self.test_env_logger.info(message)
             return
         return self.__send_message_pagination(message, self.notifier_client.send_alert, amend, emergency_msg)
 
-    def send_message(self, message: str, amend: dict = None, emergency_msg: str = None) -> Optional[int]:
+    def send_message(self, message: str, amend: dict = None, emergency_msg: str = '') -> Optional[int]:
         """
         Parameters:
             -message: the message to send
             -amend: to amend the message
             -emergency_msg: emergency message like mentioning someone
         Returns:
             -the status code of the response (200 means the message added to
                                                   the queue for sending not the message sent)
         """
+        message = message.replace('<', '&lt;').replace('>', '&gt;')
         if self.test_env:
             self.test_env_logger.info(message)
             return
         return self.__send_message_pagination(message, self.notifier_client.send_message, amend, emergency_msg)
 
     def send_message_by_threshold(
             self, message: str, amend: dict = None, emergency_msg: str = ''
@@ -257,14 +255,15 @@
         Parameters:
             -message: the message to send
             -amend: to amend the message
             -emergency_msg: emergency message like mentioning someone
         Returns:
             -the status code of the response and that the message was added to queue for sending or not
         """
+        message = message.replace('<', '&lt;').replace('>', '&gt;')
         if self.test_env:
             self.test_env_logger.info(message)
             return
         return self.__send_message_pagination(
             message, self.notifier_client.send_message_by_threshold, amend, emergency_msg
         )
 
@@ -278,14 +277,15 @@
             -message: the message want to set a sending thresh hole to
             -sending_threshold_number: the number of the message that need to be added to send one
                         of them (threshold value)
             -sending_threshold_time: the threshold boundary
         Returns:
              the status code
         """
+        message = message.replace('<', '&lt;').replace('>', '&gt;')
         return self.notifier_client.set_threshold_setting(
             message,
             sending_threshold_number,
             sending_threshold_time
         )
 
     def send_message_once(self,
@@ -344,16 +344,16 @@
         mandatory_msg = f"\nemergency_msg: {emergency_msg}\namend: {amend}"
         first_message_size = self.max_msg_size - len(mandatory_msg)
         if first_message_size < 0:
             raise Exception("Max size is to low")
         first_message = message[:first_message_size]
         rest_of_message = message[first_message_size:]
 
-        return [Message(1, first_message, emergency_msg, amend, has_html_tag=self.message_html_tag)] + [
-            Message(page + 2, rest_of_message[i:i + self.max_msg_size], has_html_tag=self.message_html_tag)
+        return [Message(1, first_message, emergency_msg, amend)] + [
+            Message(page + 2, rest_of_message[i:i + self.max_msg_size])
             for page, i in enumerate(range(0, len(rest_of_message), self.max_msg_size))
         ]
 
     def __send_message_pagination(
             self, message: str, send_func: callable, amend: dict = None, emergency_msg: str = ''
     ) -> Union[int, Optional[Tuple[int, bool]]]:
         """
@@ -365,16 +365,15 @@
             - message (str): The message to be sent.
             - send_func (callable): The function to be used to send the message.
             - amend (dict, optional): A dictionary of amendments to be included in the message.
             - emergency_msg (str, optional): An emergency message to be appended to each message part.
         Returns:
             - Union[int, Optional[Tuple[int, bool]]]: The result of the last message attempt to send.
         """
-        if not self.message_html_tag:
-            message = message.replace('<', '&lt;').replace('>', '&gt;')
+        message = message.replace('<', '&lt;').replace('>', '&gt;')
         msg_list = self.__split_msg(message, amend, emergency_msg)
         res = 0
         for msg in msg_list:
             break_flag = False
             try:
                 for _ in range(self.retiring_number):
                     res = send_func(msg.message(), msg.amend)
@@ -404,18 +403,15 @@
 
     def __send_emergency_message(self, message: str, amend: dict = None, retrying=5):
         """
         Sends an emergency message to a specified receiver, with optional retries.
         If the message fails to send, the function retries the sending up to a specified number of times.
         Parameters:
             - message (str): The emergency message to be sent.
-            - receiver_id (int): The ID of the receiver to whom the message should be sent.
-            - topic_id (int, optional):
             - amend (dict, optional): A dictionary of amendments to be appended to the message.
-            - emergency_msg (str, optional): An additional emergency message to be included.
             - retrying (int): The number of times to retry sending the message.
         Returns:
             - None
         """
         for _ in range(retrying):
             logger.info(f'{message}, {self.receiver_id}')
             url = f'https://api.telegram.org/bot{self.telegram_bot_token}/sendMessage'
```

### Comparing `telegram_notifier_client-1.0.8/src/telegram_notifier_client.egg-info/PKG-INFO` & `telegram_notifier_client-1.0.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: telegram_notifier_client
-Version: 1.0.8
+Version: 1.0.9
 Summary: telegram_notifier_client
 Home-page: https://github.com/deusfinance/notifier-client.git
-Author: Ali Ghorbani
+Author: Metalica
 Author-email: rorschach <rorschach45001@gmail.com>
 Project-URL: Homepage, https://github.com/deusfinance/notifier-client
 Project-URL: Issues, https://github.com/deusfinance/notifier-client/issues
+Keywords: telegram notifier client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: certifi
-Requires-Dist: charset-normalizer
-Requires-Dist: idna
-Requires-Dist: requests
-Requires-Dist: urllib3
 
 # notifier-client
 https://pypi.org/project/telegram-notifier-client/
 
 pip install telegram-notifier-client
```

