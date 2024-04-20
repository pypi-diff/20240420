# Comparing `tmp/fast_gmail-1.0.5.tar.gz` & `tmp/fast_gmail-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_gmail-1.0.5.tar", last modified: Wed Apr 17 12:07:46 2024, max compression
+gzip compressed data, was "fast_gmail-1.0.6.tar", last modified: Fri Apr 19 12:12:04 2024, max compression
```

## Comparing `fast_gmail-1.0.5.tar` & `fast_gmail-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-17 12:07:46.498422 fast_gmail-1.0.5/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.0.5/LICENSE
--rw-r--r--   0 aleti     (1000) aleti     (1000)    14792 2024-04-17 12:07:46.498422 fast_gmail-1.0.5/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    14032 2024-04-17 12:07:20.000000 fast_gmail-1.0.5/README.md
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-17 12:07:46.494423 fast_gmail-1.0.5/fast_gmail/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       30 2024-04-15 08:44:02.000000 fast_gmail-1.0.5/fast_gmail/__init__.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.0.5/fast_gmail/draft.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    21074 2024-04-17 11:51:01.000000 fast_gmail-1.0.5/fast_gmail/gmail.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     7199 2024-04-15 06:26:53.000000 fast_gmail-1.0.5/fast_gmail/helpers.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    25018 2024-04-17 11:49:05.000000 fast_gmail-1.0.5/fast_gmail/message.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.0.5/fast_gmail/search.py
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-17 12:07:46.498422 fast_gmail-1.0.5/fast_gmail.egg-info/
--rw-r--r--   0 aleti     (1000) aleti     (1000)    14792 2024-04-17 12:07:46.000000 fast_gmail-1.0.5/fast_gmail.egg-info/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-04-17 12:07:46.000000 fast_gmail-1.0.5/fast_gmail.egg-info/SOURCES.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-04-17 12:07:46.000000 fast_gmail-1.0.5/fast_gmail.egg-info/dependency_links.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-04-17 12:07:46.000000 fast_gmail-1.0.5/fast_gmail.egg-info/requires.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-04-17 12:07:46.000000 fast_gmail-1.0.5/fast_gmail.egg-info/top_level.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-04-17 12:07:46.498422 fast_gmail-1.0.5/setup.cfg
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1074 2024-04-17 12:07:33.000000 fast_gmail-1.0.5/setup.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-19 12:12:04.316816 fast_gmail-1.0.6/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.0.6/LICENSE
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    15007 2024-04-19 12:12:04.316816 fast_gmail-1.0.6/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    14247 2024-04-19 12:06:14.000000 fast_gmail-1.0.6/README.md
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-19 12:12:04.316816 fast_gmail-1.0.6/fast_gmail/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       30 2024-04-15 08:44:02.000000 fast_gmail-1.0.6/fast_gmail/__init__.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.0.6/fast_gmail/draft.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    21216 2024-04-19 12:05:26.000000 fast_gmail-1.0.6/fast_gmail/gmail.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     7203 2024-04-19 12:04:22.000000 fast_gmail-1.0.6/fast_gmail/helpers.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    25047 2024-04-19 11:46:36.000000 fast_gmail-1.0.6/fast_gmail/message.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.0.6/fast_gmail/search.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-19 12:12:04.316816 fast_gmail-1.0.6/fast_gmail.egg-info/
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    15007 2024-04-19 12:12:04.000000 fast_gmail-1.0.6/fast_gmail.egg-info/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-04-19 12:12:04.000000 fast_gmail-1.0.6/fast_gmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-04-19 12:12:04.000000 fast_gmail-1.0.6/fast_gmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-04-19 12:12:04.000000 fast_gmail-1.0.6/fast_gmail.egg-info/requires.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-04-19 12:12:04.000000 fast_gmail-1.0.6/fast_gmail.egg-info/top_level.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-04-19 12:12:04.316816 fast_gmail-1.0.6/setup.cfg
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1074 2024-04-19 12:11:51.000000 fast_gmail-1.0.6/setup.py
```

### Comparing `fast_gmail-1.0.5/LICENSE` & `fast_gmail-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.5/PKG-INFO` & `fast_gmail-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.0.5
+Version: 1.0.6
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -37,15 +37,15 @@
 `pip install fast-gmail`
 
 ---
 
 ## Usage:
 
 ### Initialization
-- Go to https://console.developers.google.com/apis/credentials and login to correct account
+- Go to https://console.developers.google.com/apis/credentials and login with correct account
 - Setup Oauth consent screen
 - Create new credentials with OAuth client ID for web or installed app
 - Set Authorized redirect URIs to http://localhost:3000/ (Notice the trailing slash)
 - Download the credentials.json file
 - Go to Enable APIs & services and enable GmailAPI
 
 With credentials.json file downloaded we can connect to Gmail
@@ -210,14 +210,16 @@
 ###### Attributes:
 
 - **credentials (Optional[Credentials])**: Stores user credentials (OAuth tokens) for accessing Gmail.
 - **google_service (GoogleService)**: An instance of GoogleService used for making API requests.
 - **max_results (int)**: Maximum number of messages to retrieve per request (default 10).
 - **SEPARATOR_SYMBOL (str)**: String used for separating page tokens during pagination.
 - **profile_data (Optional[GmailProfile])**: Caches the user's Gmail profile information.
+- **application_type: ApplicationType = ApplicationType.WEB**: Type of application WEB or INSTALLED,
+- **code: Optional[str] = None**: gmail oAuth response code for creating token.json file after successful login
 
 ###### Constructor (__init__):
 - Initializes the GmailApi object.
 - Reads credentials from token and credentials files.
 - Handles refreshing expired tokens.
 - Creates a GoogleService instance for making API calls.
```

### Comparing `fast_gmail-1.0.5/README.md` & `fast_gmail-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 `pip install fast-gmail`
 
 ---
 
 ## Usage:
 
 ### Initialization
-- Go to https://console.developers.google.com/apis/credentials and login to correct account
+- Go to https://console.developers.google.com/apis/credentials and login with correct account
 - Setup Oauth consent screen
 - Create new credentials with OAuth client ID for web or installed app
 - Set Authorized redirect URIs to http://localhost:3000/ (Notice the trailing slash)
 - Download the credentials.json file
 - Go to Enable APIs & services and enable GmailAPI
 
 With credentials.json file downloaded we can connect to Gmail
@@ -188,14 +188,16 @@
 ###### Attributes:
 
 - **credentials (Optional[Credentials])**: Stores user credentials (OAuth tokens) for accessing Gmail.
 - **google_service (GoogleService)**: An instance of GoogleService used for making API requests.
 - **max_results (int)**: Maximum number of messages to retrieve per request (default 10).
 - **SEPARATOR_SYMBOL (str)**: String used for separating page tokens during pagination.
 - **profile_data (Optional[GmailProfile])**: Caches the user's Gmail profile information.
+- **application_type: ApplicationType = ApplicationType.WEB**: Type of application WEB or INSTALLED,
+- **code: Optional[str] = None**: gmail oAuth response code for creating token.json file after successful login
 
 ###### Constructor (__init__):
 - Initializes the GmailApi object.
 - Reads credentials from token and credentials files.
 - Handles refreshing expired tokens.
 - Creates a GoogleService instance for making API calls.
```

### Comparing `fast_gmail-1.0.5/fast_gmail/gmail.py` & `fast_gmail-1.0.6/fast_gmail/gmail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional
 from typing import Union
 from typing import List
+from typing import Any
 import mimetypes
 import base64
 import os
 import json
 
 from email.message import EmailMessage
 from email.header import Header
@@ -38,16 +39,16 @@
 	profile_data: Optional[GmailProfile] = None
 
 	def __init__(
 		self,
 		token_file_path: str = "token.json",
 		credentials_file_path: str = "credentials.json",
 		port: int = 3000, # set the local server port for Authorized redirect URI
-		separator_symbol: Optional[str] = ", ",
-		user_id: Optional[str] = "me",
+		separator_symbol: str = ", ",
+		user_id: str = "me",
 		application_type: ApplicationType = ApplicationType.WEB,
 		code: Optional[str] = None
 	)-> None:
 		"""https://github.com/googleapis/google-api-python-client/blob/main/docs/oauth-installed.md"""
 
 		# set separator for spliting/joining the array of existing previous_page_tokens for pagination
 		self.SEPARATOR_SYMBOL = separator_symbol
@@ -67,41 +68,47 @@
 					client_id=self.credentials.client_id,
 					client_secret=self.credentials.client_secret
 				)
 			else:
 				if not os.path.exists(credentials_file_path):
 					raise FileNotFoundError(f"{credentials_file_path=} NOT FOUND!")
 				match application_type:
-					case ApplicationType.DESKTOP:
+					case ApplicationType.INSTALLED:
 						flow = InstalledAppFlow.from_client_secrets_file(
 							credentials_file_path, SCOPES
 						)
 						self.credentials = flow.run_local_server(port=port)
 					case ApplicationType.WEB:
 						cred_payload: Optional[dict] = None
 						with open(credentials_file_path, "r") as f:
 							cred_payload = json.loads(f.read())
 						if not cred_payload:
 							raise Exception(f"Could't read {credentials_file_path=}")
 						if not "web" in cred_payload:
-							raise Exception(f"{cred_payload=} content missing. \n\033[91mDid you create credentials for Web app?\033[0m")
-						if not "redirect_uris" in cred_payload["web"]:
-							raise Exception(f"Missing `redirect_uris` key from {cred_payload['web']}. \n\033[91mDid you define Authorized redirect URIs?\033[0m")
+							raise Exception(
+								f"{cred_payload=} content missing."
+								"\n\033[91mDid you create credentials for Web app?\033[0m"
+							)
+						if not "redirect_uris" in cred_payload["web"] or not cred_payload["web"]["redirect_uris"]:
+							raise Exception(
+								f"Missing `redirect_uris` key from {cred_payload['web']}."
+								"\n\033[91mDid you define Authorized redirect URIs?\033[0m"
+							)
 						
 						redirect_uris = cred_payload["web"]["redirect_uris"]
 						for uri in redirect_uris:
 							if str(port) in uri:
 								self.redirect_uri = uri
 						if not self.redirect_uri:
 							self.redirect_uri = redirect_uris[0]
 						self.flow = Flow.from_client_secrets_file(
 							credentials_file_path,
 							SCOPES,
-							redirect_uri=self.redirect_uri
-						)
+                            redirect_uri=self.redirect_uri
+                        )
 						if code:
 							self.flow.fetch_token(code=code)
 							self.credentials: str = self.flow.credentials
 						else:
 							self.auth_url = f"{self.flow.authorization_url()[0]}&prompt=consent"
 							return
 			# Save the credentials for the next run
```

### Comparing `fast_gmail-1.0.5/fast_gmail/helpers.py` & `fast_gmail-1.0.6/fast_gmail/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 	REMOVE = "remove"
 	ADD = "add"
 	TOGGLE = "toggle"
 
 
 class ApplicationType(str, Enum):
 	WEB = "web"
-	DESKTOP = "installed"
+	INSTALLED = "installed"
 
 
 class LabelMessageVisibility(str, Enum):
 	SHOW = "show"
 	HIDE = "hide"
 
 
@@ -261,16 +261,16 @@
 			previous_page_token (Optional[List[str | None]], optional): Token for fetching the previous page of results (may be empty list). Defaults to [].
 			messages (List[Message]): List of retrieved message objects.
 
 		This dataclass also provides list-like methods for iterating, checking membership, length, and accessing/modifying elements within the `messages` list.  
     """
 	next_page_token: Optional[str] = None
 	existing_pages: Optional[str] = None
-	previous_page_token: Optional[List[str | None]] = field(default_factory=lambda: [])
-	messages: List['Message'] = field(default_factory=lambda: [])
+	previous_page_token: Optional[List[str | None]] = field(default_factory = lambda: [])
+	messages: List['Message'] = field(default_factory = lambda: [])
 
 	def __iter__(self):
 		for message in self.messages:
 			yield message
 
 	def __contains__(self, value):
 		return value in self.messages
@@ -285,15 +285,15 @@
 			return self.messages[idx]
 
 	def __setitem__(self, idx, value):
 		self.messages[idx] = value
 
 	def __delitem__(self, idx):
 		del self.messages[idx]
-		
+
 	def count(self):
 		return len(self.messages)
 	
 	def index(self, idx, *args):
 		return self.messages.index(idx, *args)
 	
 	def append(self, value):
```

### Comparing `fast_gmail-1.0.5/fast_gmail/message.py` & `fast_gmail-1.0.6/fast_gmail/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,21 +23,20 @@
 
 @dataclass
 class MessagePartBody(object):
 	size: int
 	attachmentId: Optional[str] = None
 	data: Optional[str] = None
 
-
 @dataclass
 class MessageHeader(object):
 	name: str
 	value: str
 
-
+@dataclass
 class Attachment(object):
 	"""Represents an attachment associated with a Gmail message.
 		Attributes:
 			filename (str): Name of the attachment file.
 			mimeType (str): MIME type of the attachment content.
 			part_id (str): Internal identifier for the attachment within the message parts. Used for download with the Gmail API.
 			google_service (GoogleService): Reference to the Google service object used for downloading the attachment.
@@ -123,15 +122,15 @@
 			)
 		with open(filepath, "wb") as f:
 			f.write(self.data)
 
 	def __str__(self):
 		return self.filename
 
-
+@dataclass
 class MessagePart(object):
 	"""Represents a single part of a Gmail message.
 		A message part can be the main body content, an attachment, or a nested structure
 		containing further parts.
 		Attributes:
 			mimeType (Optional[str]): MIME type of the message part content.
 			headers (List[MessageHeader]): List of message headers associated with this part.
@@ -228,15 +227,15 @@
 		if not key:
 			return self.headers
 		for header in self.headers:
 			if key == header.name:
 				return header
 		return None
 
-
+@dataclass
 class Message(object):
 	"""Represents a single email message within a Gmail account.
 		This class provides access to various message properties and functionalities,
 		including content retrieval, attachment handling, label management, and
 		common actions like marking as read/unread or starring.
 
 		Attributes:
```

### Comparing `fast_gmail-1.0.5/fast_gmail/search.py` & `fast_gmail-1.0.6/fast_gmail/search.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.5/fast_gmail.egg-info/PKG-INFO` & `fast_gmail-1.0.6/fast_gmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.0.5
+Version: 1.0.6
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -37,15 +37,15 @@
 `pip install fast-gmail`
 
 ---
 
 ## Usage:
 
 ### Initialization
-- Go to https://console.developers.google.com/apis/credentials and login to correct account
+- Go to https://console.developers.google.com/apis/credentials and login with correct account
 - Setup Oauth consent screen
 - Create new credentials with OAuth client ID for web or installed app
 - Set Authorized redirect URIs to http://localhost:3000/ (Notice the trailing slash)
 - Download the credentials.json file
 - Go to Enable APIs & services and enable GmailAPI
 
 With credentials.json file downloaded we can connect to Gmail
@@ -210,14 +210,16 @@
 ###### Attributes:
 
 - **credentials (Optional[Credentials])**: Stores user credentials (OAuth tokens) for accessing Gmail.
 - **google_service (GoogleService)**: An instance of GoogleService used for making API requests.
 - **max_results (int)**: Maximum number of messages to retrieve per request (default 10).
 - **SEPARATOR_SYMBOL (str)**: String used for separating page tokens during pagination.
 - **profile_data (Optional[GmailProfile])**: Caches the user's Gmail profile information.
+- **application_type: ApplicationType = ApplicationType.WEB**: Type of application WEB or INSTALLED,
+- **code: Optional[str] = None**: gmail oAuth response code for creating token.json file after successful login
 
 ###### Constructor (__init__):
 - Initializes the GmailApi object.
 - Reads credentials from token and credentials files.
 - Handles refreshing expired tokens.
 - Creates a GoogleService instance for making API calls.
```

### Comparing `fast_gmail-1.0.5/setup.py` & `fast_gmail-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as f:
     long_descrition=f.read()
 
 setup(
     name="fast_gmail",
-    version="1.0.5",
+    version="1.0.6",
     description="GmailApi wrapper",
     long_description=long_descrition,
     long_description_content_type='text/markdown',
     author="Aleti",
     author_email="aleti.open.source@gmail.com",
     url="https://github.com/aleti1/fast_gmail",
     license="MIT",
```

