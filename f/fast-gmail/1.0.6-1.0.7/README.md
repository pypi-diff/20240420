# Comparing `tmp/fast_gmail-1.0.6.tar.gz` & `tmp/fast_gmail-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_gmail-1.0.6.tar", last modified: Fri Apr 19 12:12:04 2024, max compression
+gzip compressed data, was "fast_gmail-1.0.7.tar", last modified: Sat Apr 20 07:02:21 2024, max compression
```

## Comparing `fast_gmail-1.0.6.tar` & `fast_gmail-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-19 12:12:04.316816 fast_gmail-1.0.6/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.0.6/LICENSE
--rw-r--r--   0 aleti     (1000) aleti     (1000)    15007 2024-04-19 12:12:04.316816 fast_gmail-1.0.6/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    14247 2024-04-19 12:06:14.000000 fast_gmail-1.0.6/README.md
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-19 12:12:04.316816 fast_gmail-1.0.6/fast_gmail/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       30 2024-04-15 08:44:02.000000 fast_gmail-1.0.6/fast_gmail/__init__.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.0.6/fast_gmail/draft.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    21216 2024-04-19 12:05:26.000000 fast_gmail-1.0.6/fast_gmail/gmail.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     7203 2024-04-19 12:04:22.000000 fast_gmail-1.0.6/fast_gmail/helpers.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    25047 2024-04-19 11:46:36.000000 fast_gmail-1.0.6/fast_gmail/message.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.0.6/fast_gmail/search.py
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-19 12:12:04.316816 fast_gmail-1.0.6/fast_gmail.egg-info/
--rw-r--r--   0 aleti     (1000) aleti     (1000)    15007 2024-04-19 12:12:04.000000 fast_gmail-1.0.6/fast_gmail.egg-info/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-04-19 12:12:04.000000 fast_gmail-1.0.6/fast_gmail.egg-info/SOURCES.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-04-19 12:12:04.000000 fast_gmail-1.0.6/fast_gmail.egg-info/dependency_links.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-04-19 12:12:04.000000 fast_gmail-1.0.6/fast_gmail.egg-info/requires.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-04-19 12:12:04.000000 fast_gmail-1.0.6/fast_gmail.egg-info/top_level.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-04-19 12:12:04.316816 fast_gmail-1.0.6/setup.cfg
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1074 2024-04-19 12:11:51.000000 fast_gmail-1.0.6/setup.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-20 07:02:21.575887 fast_gmail-1.0.7/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.0.7/LICENSE
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    15592 2024-04-20 07:02:21.575887 fast_gmail-1.0.7/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    14832 2024-04-20 07:00:13.000000 fast_gmail-1.0.7/README.md
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-20 07:02:21.575887 fast_gmail-1.0.7/fast_gmail/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       30 2024-04-15 08:44:02.000000 fast_gmail-1.0.7/fast_gmail/__init__.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.0.7/fast_gmail/draft.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    21980 2024-04-20 06:58:56.000000 fast_gmail-1.0.7/fast_gmail/gmail.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     7203 2024-04-19 12:04:22.000000 fast_gmail-1.0.7/fast_gmail/helpers.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    25047 2024-04-19 11:46:36.000000 fast_gmail-1.0.7/fast_gmail/message.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.0.7/fast_gmail/search.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-20 07:02:21.575887 fast_gmail-1.0.7/fast_gmail.egg-info/
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    15592 2024-04-20 07:02:21.000000 fast_gmail-1.0.7/fast_gmail.egg-info/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-04-20 07:02:21.000000 fast_gmail-1.0.7/fast_gmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-04-20 07:02:21.000000 fast_gmail-1.0.7/fast_gmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-04-20 07:02:21.000000 fast_gmail-1.0.7/fast_gmail.egg-info/requires.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-04-20 07:02:21.000000 fast_gmail-1.0.7/fast_gmail.egg-info/top_level.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-04-20 07:02:21.575887 fast_gmail-1.0.7/setup.cfg
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1074 2024-04-20 07:02:06.000000 fast_gmail-1.0.7/setup.py
```

### Comparing `fast_gmail-1.0.6/LICENSE` & `fast_gmail-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.6/PKG-INFO` & `fast_gmail-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: fast_gmail
-Version: 1.0.6
-Summary: GmailApi wrapper
-Home-page: https://github.com/aleti1/fast_gmail
-Author: Aleti
-Author-email: aleti.open.source@gmail.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: google-api-python-client==2.125.0
-Requires-Dist: google-auth-httplib2==0.2.0
-Requires-Dist: google-auth-oauthlib==1.2.0
-Requires-Dist: typing-extensions==4.11.0
-
 # Fast-gmail a simple python wrapper for gmailapi
 
 ---
 ## Functionalities:
 - Send text/html messages
 - Send messages with signature & attachments
 - Get messages with pagination
@@ -45,35 +23,39 @@
 - Setup Oauth consent screen
 - Create new credentials with OAuth client ID for web or installed app
 - Set Authorized redirect URIs to http://localhost:3000/ (Notice the trailing slash)
 - Download the credentials.json file
 - Go to Enable APIs & services and enable GmailAPI
 
 With credentials.json file downloaded we can connect to Gmail
-```
+```python
 gmail = GmailApi(
     credentials_file_path = __path_to_credentials_json_file__,  # Defaults to ./credentials.json
     port = 3000, # Defaults to 3000  !IMPORTANT: if you change this default value don't forget to also changed on Authorized redirect URIs
 )
 ```
+### Examples
+- FastAPI
+- Django
+- Flask (comming soon)
 
 ### Send message
-``` 
+```python
     from fast_gmail import GmailApi
 
     messages = GmailApi().send_message(
         sender: str,
         to: str,
         subject: str,
         html: Optional[str]=None,
         text: Optional[str]=None,
         cc: Optional[List[str] | str]=None,
         bcc: Optional[List[str] | str]=None,
         attachments: Optional[List[str] | str]=None,
-		in_reply_to: Optional[str] = None,
+        in_reply_to: Optional[str] = None,
         signature: bool = True
     )
     """Sends an email message.
         Args:
             sender (str): Email address of the message sender.
             to (str): Email address of the recipient.
             subject (str): Subject line of the email.
@@ -86,15 +68,15 @@
             signature (bool, optional): Whether to include a signature (if configured). Defaults to True.
         Returns:
             Optional[Message]: An object representing the sent message, or None on error.
     """
 ```
 
 ### Get messages
-```
+```python
     messages = GmailApi().get_messages(
         includeSpamTrash: bool = False,
         max_results: int = 10,
         labels: Union[List[Labels], List[str], None] = None,
         next_page_token: str = None,
         existing_pages: Optional[List[str] | str] = None,
         previous_page_token: Optional[str] = None,
@@ -111,36 +93,36 @@
             query (Union[SearchParams, str], optional): Search query to filter messages. Can be a string or a SearchParams object. 
         Returns:
             GetMessagesResponse: An object containing the retrieved messages and pagination information.
     """
 ```
 
 ### Get INBOX/SPAM/TRASH messages
-```
+```python
     messages = GmailApi().get_inbox_messages(
         max_results: int = MAX_RESULTS,
         next_page_token: str = None,
         existing_pages: Optional[List[str] | str] = None,
         previous_page_token: Optional[str] = None,
         query: Union[SearchParams, str] = None
     )
 
     # helpers for spam or trash
     messages = GmailApi().get_spam_messages()
     messages = GmailApi().get_trash_messages()
 ```
 
 ### GET message
-```
+```python
     message = GmailApi().get_message(id)
     # returns a Message object
 ```
 
 ### GET attachment
-```
+```python
     message = GmailApi().get_message(id)
     attachment_id = None
     attachment_name = None
     for attacment in message.attachments:
         attachment_id = attachment.part_id
         attachment_name = attachment.filename
 
@@ -149,16 +131,32 @@
     # or by filename
     by_name = message.get_attachment(filename=attachment_name) # returns an Attachment object
 
     # save file to disk
     by_id.save(filepath=f"/tmp/{attachment.filename}", overwrite=True)
 ```
 
-### Message actions
+### GET contacts
+```python
+    contacts = GmailApi().get_contacts()
+    for contact in contacts:
+        if "emailAddresses" in contact and contact["emailAddresses"]:
+            print(contact["emailAddresses"][0]["value"])
+```
+
+### Search contacts
+```python
+    contacts = GmailApi().search_contacts(query="example@gmail.com")
+    for contact in contacts:
+        if "person" in contact and contact["person"]:
+            print(contact["person"]["emailAddresses"][0]["value"])
 ```
+
+### Message actions
+```python
     message = GmailApi().get_message(id)
 
     # mark read or unread
     message.toggle_read_unread
     # or
     message.mark_as_read
     # or
@@ -315,8 +313,8 @@
 ---
 
 ### class GetMessagesResponse:
 ###### Attributes:
 - **next_page_token (Optional[str], optional)**: Token for fetching the next page of results. Defaults to None.
 - **existing_pages (Optional[str], optional)**: Used internally for pagination. Defaults to None. List like string of page tokens separated by GmailApi.SEPARATOR_SYMBOL
 - **previous_page_token (Optional[List[str | None]], optional)**: Token for fetching the previous page of results (may be empty list). Defaults to [].
-- **messages (List[Message])**: List of retrieved message objects.
+- **messages (List[Message])**: List of retrieved message objects.
```

### Comparing `fast_gmail-1.0.6/README.md` & `fast_gmail-1.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: fast_gmail
+Version: 1.0.7
+Summary: GmailApi wrapper
+Home-page: https://github.com/aleti1/fast_gmail
+Author: Aleti
+Author-email: aleti.open.source@gmail.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: google-api-python-client==2.125.0
+Requires-Dist: google-auth-httplib2==0.2.0
+Requires-Dist: google-auth-oauthlib==1.2.0
+Requires-Dist: typing-extensions==4.11.0
+
 # Fast-gmail a simple python wrapper for gmailapi
 
 ---
 ## Functionalities:
 - Send text/html messages
 - Send messages with signature & attachments
 - Get messages with pagination
@@ -23,35 +45,39 @@
 - Setup Oauth consent screen
 - Create new credentials with OAuth client ID for web or installed app
 - Set Authorized redirect URIs to http://localhost:3000/ (Notice the trailing slash)
 - Download the credentials.json file
 - Go to Enable APIs & services and enable GmailAPI
 
 With credentials.json file downloaded we can connect to Gmail
-```
+```python
 gmail = GmailApi(
     credentials_file_path = __path_to_credentials_json_file__,  # Defaults to ./credentials.json
     port = 3000, # Defaults to 3000  !IMPORTANT: if you change this default value don't forget to also changed on Authorized redirect URIs
 )
 ```
+### Examples
+- FastAPI
+- Django
+- Flask (comming soon)
 
 ### Send message
-``` 
+```python
     from fast_gmail import GmailApi
 
     messages = GmailApi().send_message(
         sender: str,
         to: str,
         subject: str,
         html: Optional[str]=None,
         text: Optional[str]=None,
         cc: Optional[List[str] | str]=None,
         bcc: Optional[List[str] | str]=None,
         attachments: Optional[List[str] | str]=None,
-		in_reply_to: Optional[str] = None,
+        in_reply_to: Optional[str] = None,
         signature: bool = True
     )
     """Sends an email message.
         Args:
             sender (str): Email address of the message sender.
             to (str): Email address of the recipient.
             subject (str): Subject line of the email.
@@ -64,15 +90,15 @@
             signature (bool, optional): Whether to include a signature (if configured). Defaults to True.
         Returns:
             Optional[Message]: An object representing the sent message, or None on error.
     """
 ```
 
 ### Get messages
-```
+```python
     messages = GmailApi().get_messages(
         includeSpamTrash: bool = False,
         max_results: int = 10,
         labels: Union[List[Labels], List[str], None] = None,
         next_page_token: str = None,
         existing_pages: Optional[List[str] | str] = None,
         previous_page_token: Optional[str] = None,
@@ -89,36 +115,36 @@
             query (Union[SearchParams, str], optional): Search query to filter messages. Can be a string or a SearchParams object. 
         Returns:
             GetMessagesResponse: An object containing the retrieved messages and pagination information.
     """
 ```
 
 ### Get INBOX/SPAM/TRASH messages
-```
+```python
     messages = GmailApi().get_inbox_messages(
         max_results: int = MAX_RESULTS,
         next_page_token: str = None,
         existing_pages: Optional[List[str] | str] = None,
         previous_page_token: Optional[str] = None,
         query: Union[SearchParams, str] = None
     )
 
     # helpers for spam or trash
     messages = GmailApi().get_spam_messages()
     messages = GmailApi().get_trash_messages()
 ```
 
 ### GET message
-```
+```python
     message = GmailApi().get_message(id)
     # returns a Message object
 ```
 
 ### GET attachment
-```
+```python
     message = GmailApi().get_message(id)
     attachment_id = None
     attachment_name = None
     for attacment in message.attachments:
         attachment_id = attachment.part_id
         attachment_name = attachment.filename
 
@@ -127,16 +153,32 @@
     # or by filename
     by_name = message.get_attachment(filename=attachment_name) # returns an Attachment object
 
     # save file to disk
     by_id.save(filepath=f"/tmp/{attachment.filename}", overwrite=True)
 ```
 
-### Message actions
+### GET contacts
+```python
+    contacts = GmailApi().get_contacts()
+    for contact in contacts:
+        if "emailAddresses" in contact and contact["emailAddresses"]:
+            print(contact["emailAddresses"][0]["value"])
+```
+
+### Search contacts
+```python
+    contacts = GmailApi().search_contacts(query="example@gmail.com")
+    for contact in contacts:
+        if "person" in contact and contact["person"]:
+            print(contact["person"]["emailAddresses"][0]["value"])
 ```
+
+### Message actions
+```python
     message = GmailApi().get_message(id)
 
     # mark read or unread
     message.toggle_read_unread
     # or
     message.mark_as_read
     # or
@@ -293,8 +335,8 @@
 ---
 
 ### class GetMessagesResponse:
 ###### Attributes:
 - **next_page_token (Optional[str], optional)**: Token for fetching the next page of results. Defaults to None.
 - **existing_pages (Optional[str], optional)**: Used internally for pagination. Defaults to None. List like string of page tokens separated by GmailApi.SEPARATOR_SYMBOL
 - **previous_page_token (Optional[List[str | None]], optional)**: Token for fetching the previous page of results (may be empty list). Defaults to [].
-- **messages (List[Message])**: List of retrieved message objects.
+- **messages (List[Message])**: List of retrieved message objects.
```

### Comparing `fast_gmail-1.0.6/fast_gmail/gmail.py` & `fast_gmail-1.0.7/fast_gmail/gmail.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 from fast_gmail.draft import Draft
 from fast_gmail.helpers import *
 
 
 # If modifying these scopes, delete the file token.json.
 SCOPES = [
 	"https://www.googleapis.com/auth/gmail.modify",
-	"https://www.googleapis.com/auth/gmail.settings.basic"
+	"https://www.googleapis.com/auth/gmail.settings.basic",
+	"https://www.googleapis.com/auth/contacts.readonly",
+	"https://www.googleapis.com/auth/contacts.other.readonly"
 ]
 
 
 class GmailApi(object):
 	"""https://googleapis.github.io/google-api-python-client/docs/dyn/gmail_v1.users.html"""
 	credentials: Optional[Credentials] = None
 	google_service: GoogleService
@@ -608,7 +610,27 @@
 		finally:
 			# close connection
 			self.google_service.service.close()
 			if request:
 				return DraftsList(**request)
 			return DraftsList(resultSizeEstimate=0, drafts=[], nextPageToken=None)
 
+	def get_contacts(self)-> Optional[list]:
+		try:
+			request = build("people", "v1", credentials = self.credentials).otherContacts().list(
+				pageSize=1000,
+				readMask="emailAddresses"
+			).execute()
+			return request["otherContacts"] if "otherContacts" in request else None
+		except HttpError as e:
+			raise e
+		
+	def search_contacts(self, query: str)-> Optional[list]:
+		try:
+			request = build("people", "v1", credentials = self.credentials).otherContacts().search(
+				pageSize=30,
+				readMask="emailAddresses",
+				query = query
+			).execute()
+			return request["results"] if "results" in request else None
+		except HttpError as e:
+			raise e
```

### Comparing `fast_gmail-1.0.6/fast_gmail/helpers.py` & `fast_gmail-1.0.7/fast_gmail/helpers.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.6/fast_gmail/message.py` & `fast_gmail-1.0.7/fast_gmail/message.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.6/fast_gmail/search.py` & `fast_gmail-1.0.7/fast_gmail/search.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.6/fast_gmail.egg-info/PKG-INFO` & `fast_gmail-1.0.7/fast_gmail.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.0.6
+Version: 1.0.7
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -45,35 +45,39 @@
 - Setup Oauth consent screen
 - Create new credentials with OAuth client ID for web or installed app
 - Set Authorized redirect URIs to http://localhost:3000/ (Notice the trailing slash)
 - Download the credentials.json file
 - Go to Enable APIs & services and enable GmailAPI
 
 With credentials.json file downloaded we can connect to Gmail
-```
+```python
 gmail = GmailApi(
     credentials_file_path = __path_to_credentials_json_file__,  # Defaults to ./credentials.json
     port = 3000, # Defaults to 3000  !IMPORTANT: if you change this default value don't forget to also changed on Authorized redirect URIs
 )
 ```
+### Examples
+- FastAPI
+- Django
+- Flask (comming soon)
 
 ### Send message
-``` 
+```python
     from fast_gmail import GmailApi
 
     messages = GmailApi().send_message(
         sender: str,
         to: str,
         subject: str,
         html: Optional[str]=None,
         text: Optional[str]=None,
         cc: Optional[List[str] | str]=None,
         bcc: Optional[List[str] | str]=None,
         attachments: Optional[List[str] | str]=None,
-		in_reply_to: Optional[str] = None,
+        in_reply_to: Optional[str] = None,
         signature: bool = True
     )
     """Sends an email message.
         Args:
             sender (str): Email address of the message sender.
             to (str): Email address of the recipient.
             subject (str): Subject line of the email.
@@ -86,15 +90,15 @@
             signature (bool, optional): Whether to include a signature (if configured). Defaults to True.
         Returns:
             Optional[Message]: An object representing the sent message, or None on error.
     """
 ```
 
 ### Get messages
-```
+```python
     messages = GmailApi().get_messages(
         includeSpamTrash: bool = False,
         max_results: int = 10,
         labels: Union[List[Labels], List[str], None] = None,
         next_page_token: str = None,
         existing_pages: Optional[List[str] | str] = None,
         previous_page_token: Optional[str] = None,
@@ -111,36 +115,36 @@
             query (Union[SearchParams, str], optional): Search query to filter messages. Can be a string or a SearchParams object. 
         Returns:
             GetMessagesResponse: An object containing the retrieved messages and pagination information.
     """
 ```
 
 ### Get INBOX/SPAM/TRASH messages
-```
+```python
     messages = GmailApi().get_inbox_messages(
         max_results: int = MAX_RESULTS,
         next_page_token: str = None,
         existing_pages: Optional[List[str] | str] = None,
         previous_page_token: Optional[str] = None,
         query: Union[SearchParams, str] = None
     )
 
     # helpers for spam or trash
     messages = GmailApi().get_spam_messages()
     messages = GmailApi().get_trash_messages()
 ```
 
 ### GET message
-```
+```python
     message = GmailApi().get_message(id)
     # returns a Message object
 ```
 
 ### GET attachment
-```
+```python
     message = GmailApi().get_message(id)
     attachment_id = None
     attachment_name = None
     for attacment in message.attachments:
         attachment_id = attachment.part_id
         attachment_name = attachment.filename
 
@@ -149,16 +153,32 @@
     # or by filename
     by_name = message.get_attachment(filename=attachment_name) # returns an Attachment object
 
     # save file to disk
     by_id.save(filepath=f"/tmp/{attachment.filename}", overwrite=True)
 ```
 
-### Message actions
+### GET contacts
+```python
+    contacts = GmailApi().get_contacts()
+    for contact in contacts:
+        if "emailAddresses" in contact and contact["emailAddresses"]:
+            print(contact["emailAddresses"][0]["value"])
+```
+
+### Search contacts
+```python
+    contacts = GmailApi().search_contacts(query="example@gmail.com")
+    for contact in contacts:
+        if "person" in contact and contact["person"]:
+            print(contact["person"]["emailAddresses"][0]["value"])
 ```
+
+### Message actions
+```python
     message = GmailApi().get_message(id)
 
     # mark read or unread
     message.toggle_read_unread
     # or
     message.mark_as_read
     # or
```

### Comparing `fast_gmail-1.0.6/setup.py` & `fast_gmail-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as f:
     long_descrition=f.read()
 
 setup(
     name="fast_gmail",
-    version="1.0.6",
+    version="1.0.7",
     description="GmailApi wrapper",
     long_description=long_descrition,
     long_description_content_type='text/markdown',
     author="Aleti",
     author_email="aleti.open.source@gmail.com",
     url="https://github.com/aleti1/fast_gmail",
     license="MIT",
```

