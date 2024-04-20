# Comparing `tmp/twikit-1.5.3.tar.gz` & `tmp/twikit-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.5.3.tar", last modified: Thu Apr 18 16:56:08 2024, max compression
+gzip compressed data, was "twikit-1.5.4.tar", last modified: Sat Apr 20 04:21:46 2024, max compression
```

## Comparing `twikit-1.5.3.tar` & `twikit-1.5.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 16:56:08.106277 twikit-1.5.3/
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.3/LICENSE
--rw-rw-rw-   0        0        0     3863 2024-04-18 16:56:08.104282 twikit-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 16:56:08.106277 twikit-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 16:56:08.022503 twikit-1.5.3/twikit/
--rw-rw-rw-   0        0        0      620 2024-04-18 16:53:11.000000 twikit-1.5.3/twikit/__init__.py
--rw-rw-rw-   0        0        0   134560 2024-04-18 16:54:24.000000 twikit-1.5.3/twikit/client.py
--rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.3/twikit/community.py
--rw-rw-rw-   0        0        0     2626 2024-04-14 11:15:08.000000 twikit-1.5.3/twikit/errors.py
--rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.3/twikit/group.py
--rw-rw-rw-   0        0        0     2095 2024-04-14 11:11:34.000000 twikit-1.5.3/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.3/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.3/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.3/twikit/notification.py
--rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.3/twikit/trend.py
--rw-rw-rw-   0        0        0    22342 2024-04-18 16:51:18.000000 twikit-1.5.3/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-18 16:56:08.100294 twikit-1.5.3/twikit/twikit_async/
--rw-rw-rw-   0        0        0      572 2024-04-15 14:48:54.000000 twikit-1.5.3/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0   136855 2024-04-18 16:48:21.000000 twikit-1.5.3/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.3/twikit/twikit_async/community.py
--rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.3/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.3/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.3/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.3/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.3/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.3/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.3/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    22211 2024-04-18 16:51:47.000000 twikit-1.5.3/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14740 2024-04-16 15:30:17.000000 twikit-1.5.3/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.3/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14517 2024-04-16 15:30:25.000000 twikit-1.5.3/twikit/user.py
--rw-rw-rw-   0        0        0    24789 2024-04-15 12:37:05.000000 twikit-1.5.3/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-18 16:56:08.045442 twikit-1.5.3/twikit.egg-info/
--rw-rw-rw-   0        0        0     3863 2024-04-18 16:56:07.000000 twikit-1.5.3/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      790 2024-04-18 16:56:07.000000 twikit-1.5.3/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 16:56:07.000000 twikit-1.5.3/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-18 16:56:07.000000 twikit-1.5.3/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 16:56:07.000000 twikit-1.5.3/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 04:21:46.206078 twikit-1.5.4/
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.4/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-04-20 04:21:46.203087 twikit-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 04:21:46.206078 twikit-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 04:21:46.129282 twikit-1.5.4/twikit/
+-rw-rw-rw-   0        0        0      620 2024-04-20 03:59:36.000000 twikit-1.5.4/twikit/__init__.py
+-rw-rw-rw-   0        0        0   135693 2024-04-20 03:58:46.000000 twikit-1.5.4/twikit/client.py
+-rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.4/twikit/community.py
+-rw-rw-rw-   0        0        0     2626 2024-04-14 11:15:08.000000 twikit-1.5.4/twikit/errors.py
+-rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.4/twikit/group.py
+-rw-rw-rw-   0        0        0     2095 2024-04-14 11:11:34.000000 twikit-1.5.4/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.4/twikit/notification.py
+-rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/trend.py
+-rw-rw-rw-   0        0        0    22342 2024-04-20 03:51:37.000000 twikit-1.5.4/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-20 04:21:46.199097 twikit-1.5.4/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      572 2024-04-15 14:48:54.000000 twikit-1.5.4/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0   137981 2024-04-20 03:59:02.000000 twikit-1.5.4/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.4/twikit/twikit_async/community.py
+-rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.4/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    22211 2024-04-18 16:51:47.000000 twikit-1.5.4/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14740 2024-04-16 15:30:17.000000 twikit-1.5.4/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14517 2024-04-16 15:30:25.000000 twikit-1.5.4/twikit/user.py
+-rw-rw-rw-   0        0        0    26321 2024-04-20 03:22:02.000000 twikit-1.5.4/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 04:21:46.149231 twikit-1.5.4/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-04-20 04:21:45.000000 twikit-1.5.4/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2024-04-20 04:21:45.000000 twikit-1.5.4/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 04:21:45.000000 twikit-1.5.4/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-20 04:21:45.000000 twikit-1.5.4/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-20 04:21:45.000000 twikit-1.5.4/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.5.3/LICENSE` & `twikit-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/PKG-INFO` & `twikit-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.3
+Version: 1.5.4
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.3/README.md` & `twikit-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/setup.py` & `twikit-1.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/__init__.py` & `twikit-1.5.4/twikit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ==========================
 Twikit Twitter API Wrapper
 ==========================
 
 A Python library for interacting with the Twitter API.
 """
 
-__version__ = '1.5.3'
+__version__ = '1.5.4'
 
 from .client import Client
 from .community import (Community, CommunityCreator, CommunityMember,
                         CommunityRule)
 from .errors import *
 from .group import Group, GroupMessage
 from .list import List
```

### Comparing `twikit-1.5.3/twikit/client.py` & `twikit-1.5.4/twikit/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     COMMUNITY_TWEETS_FEATURES,
     COMMUNITY_NOTE_FEATURES,
     JOIN_COMMUNITY_FEATURES,
     LIST_FEATURES,
     FEATURES,
     TOKEN,
     USER_FEATURES,
+    NOTE_TWEET_FEATURES,
     Endpoint,
     Flow,
     Result,
     build_tweet_data,
     build_user_data,
     find_dict,
     flatten_params,
@@ -903,15 +904,18 @@
         media_ids: list[str] | None = None,
         poll_uri: str | None = None,
         reply_to: str | None = None,
         conversation_control: Literal[
             'followers', 'verified', 'mentioned'] | None = None,
         attachment_url: str | None = None,
         community_id: str | None = None,
-        share_with_followers: bool = False
+        share_with_followers: bool = False,
+        is_note_tweet: bool = False,
+        richtext_options: list[dict] | None = None,
+        edit_tweet_id: str | None = None
     ) -> Tweet:
         """
         Creates a new tweet on Twitter with the specified
         text, media, and poll.
 
         Parameters
         ----------
@@ -928,14 +932,21 @@
         conversation_control : {'followers', 'verified', 'mentioned'}
             The type of conversation control for the tweet:
             - 'followers': Limits replies to followers only.
             - 'verified': Limits replies to verified accounts only.
             - 'mentioned': Limits replies to mentioned accounts only.
         attachment_url : :class:`str`
             URL of the tweet to be quoted.
+        is_note_tweet : class`bool`, default=False
+            If this option is set to True, tweets longer than 280 characters
+            can be posted (Twitter Premium only).
+        richtext_options : list[:class:`dict`], default=None
+            Options for decorating text (Twitter Premium only).
+        edit_tweet_id : :class:`str` | None, default=None
+            ID of the tweet to edit (Twitter Premium only).
 
         Raises
         ------
         :exc:`DuplicateTweet` : If the tweet is a duplicate of another tweet.
 
         Returns
         -------
@@ -1013,21 +1024,38 @@
             variables['semantic_annotation_ids'] = [{
                 'entity_id': community_id,
                 'group_id': '8',
                 'domain_id': '31'
             }]
             variables['broadcast'] = share_with_followers
 
+        if richtext_options is not None:
+            is_note_tweet = True
+            variables['richtext_options'] = {
+                'richtext_tags': richtext_options
+            }
+
+        if edit_tweet_id is not None:
+            variables['edit_options'] = {
+                'previous_tweet_id': edit_tweet_id
+            }
+
+        if is_note_tweet:
+            endpoint = Endpoint.CREATE_NOTE_TWEET
+            features = NOTE_TWEET_FEATURES
+        else:
+            endpoint = Endpoint.CREATE_TWEET
+            features = FEATURES
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_TWEET),
-            'features': FEATURES,
+            'features': features,
         }
         response = self.http.post(
-            Endpoint.CREATE_TWEET,
+            endpoint,
             json=data,
             headers=self._base_headers,
         ).json()
 
         _result = find_dict(response, 'result')
         if not _result:
             raise_exceptions_from_response(response['errors'])
```

### Comparing `twikit-1.5.3/twikit/community.py` & `twikit-1.5.4/twikit/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/errors.py` & `twikit-1.5.4/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/group.py` & `twikit-1.5.4/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/http.py` & `twikit-1.5.4/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/list.py` & `twikit-1.5.4/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/message.py` & `twikit-1.5.4/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/notification.py` & `twikit-1.5.4/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/trend.py` & `twikit-1.5.4/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/tweet.py` & `twikit-1.5.4/twikit/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/twikit_async/__init__.py` & `twikit-1.5.4/twikit/twikit_async/__init__.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/twikit_async/client.py` & `twikit-1.5.4/twikit/twikit_async/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     COMMUNITY_TWEETS_FEATURES,
     COMMUNITY_NOTE_FEATURES,
     FEATURES,
     JOIN_COMMUNITY_FEATURES,
     LIST_FEATURES,
     TOKEN,
     USER_FEATURES,
+    NOTE_TWEET_FEATURES,
     Endpoint,
     build_tweet_data,
     build_user_data,
     find_dict,
     flatten_params,
     get_query_id,
     urlencode
@@ -917,15 +918,18 @@
         media_ids: list[str] | None = None,
         poll_uri: str | None = None,
         reply_to: str | None = None,
         conversation_control: Literal[
             'followers', 'verified', 'mentioned'] | None = None,
         attachment_url: str | None = None,
         community_id: str | None = None,
-        share_with_followers: bool = False
+        share_with_followers: bool = False,
+        is_note_tweet: bool = False,
+        richtext_options: list[dict] = None,
+        edit_tweet_id: str | None = None
     ) -> Tweet:
         """
         Creates a new tweet on Twitter with the specified
         text, media, and poll.
 
         Parameters
         ----------
@@ -942,14 +946,21 @@
         conversation_control : {'followers', 'verified', 'mentioned'}
             The type of conversation control for the tweet:
             - 'followers': Limits replies to followers only.
             - 'verified': Limits replies to verified accounts only.
             - 'mentioned': Limits replies to mentioned accounts only.
         attachment_url : :class:`str`
             URL of the tweet to be quoted.
+        is_note_tweet : :class:`bool`, default=False
+            If this option is set to True, tweets longer than 280 characters
+            can be posted (Twitter Premium only).
+        richtext_options : list[:class:`dict`], default=None
+            Options for decorating text (Twitter Premium only).
+        edit_tweet_id : :class:`str` | None, default=None
+            ID of the tweet to edit (Twitter Premium only).
 
         Raises
         ------
         :exc:`DuplicateTweet` : If the tweet is a duplicate of another tweet.
 
         Returns
         -------
@@ -1027,21 +1038,37 @@
             variables['semantic_annotation_ids'] = [{
                 'entity_id': community_id,
                 'group_id': '8',
                 'domain_id': '31'
             }]
             variables['broadcast'] = share_with_followers
 
+        if richtext_options is not None:
+            is_note_tweet = True
+            variables['richtext_options'] = {
+                'richtext_tags': richtext_options
+            }
+        if edit_tweet_id is not None:
+            variables['edit_options'] = {
+                'previous_tweet_id': edit_tweet_id
+            }
+
+        if is_note_tweet:
+            endpoint = Endpoint.CREATE_NOTE_TWEET
+            features = NOTE_TWEET_FEATURES
+        else:
+            endpoint = Endpoint.CREATE_TWEET
+            features = FEATURES
         data = {
             'variables': variables,
             'queryId': get_query_id(Endpoint.CREATE_TWEET),
-            'features': FEATURES,
+            'features': features,
         }
         response = (await self.http.post(
-            Endpoint.CREATE_TWEET,
+            endpoint,
             json=data,
             headers=self._base_headers,
         )).json()
 
         _result = find_dict(response, 'result')
         if not _result:
             raise_exceptions_from_response(response['errors'])
```

### Comparing `twikit-1.5.3/twikit/twikit_async/community.py` & `twikit-1.5.4/twikit/twikit_async/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/twikit_async/errors.py` & `twikit-1.5.4/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/twikit_async/group.py` & `twikit-1.5.4/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/twikit_async/http.py` & `twikit-1.5.4/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/twikit_async/list.py` & `twikit-1.5.4/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/twikit_async/message.py` & `twikit-1.5.4/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/twikit_async/notification.py` & `twikit-1.5.4/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/twikit_async/trend.py` & `twikit-1.5.4/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/twikit_async/tweet.py` & `twikit-1.5.4/twikit/twikit_async/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/twikit_async/user.py` & `twikit-1.5.4/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/twikit_async/utils.py` & `twikit-1.5.4/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/user.py` & `twikit-1.5.4/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.3/twikit/utils.py` & `twikit-1.5.4/twikit/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,22 +105,50 @@
     'rweb_tipjar_consumption_enabled': True,
     'responsive_web_graphql_exclude_directive_enabled': True,
     'verified_phone_label_enabled': False,
     'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
     'responsive_web_graphql_timeline_navigation_enabled': True
 }
 
+NOTE_TWEET_FEATURES = {
+    "communities_web_enable_tweet_community_results_fetch": True,
+    "c9s_tweet_anatomy_moderator_badge_enabled": True,
+    "tweetypie_unmention_optimization_enabled": True,
+    "responsive_web_edit_tweet_api_enabled": True,
+    "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True,
+    "view_counts_everywhere_api_enabled": True,
+    "longform_notetweets_consumption_enabled": True,
+    "responsive_web_twitter_article_tweet_consumption_enabled": True,
+    "tweet_awards_web_tipping_enabled": False,
+    "creator_subscriptions_quote_tweet_preview_enabled": False,
+    "longform_notetweets_rich_text_read_enabled": True,
+    "longform_notetweets_inline_media_enabled": True,
+    "articles_preview_enabled": False,
+    "rweb_video_timestamps_enabled": True,
+    "rweb_tipjar_consumption_enabled": True,
+    "responsive_web_graphql_exclude_directive_enabled": True,
+    "verified_phone_label_enabled": False,
+    "freedom_of_speech_not_reach_fetch_enabled": True,
+    "standardized_nudges_misinfo": True,
+    "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": True,
+    "tweet_with_visibility_results_prefer_gql_media_interstitial_enabled": True,
+    "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
+    "responsive_web_graphql_timeline_navigation_enabled": True,
+    "responsive_web_enhance_cards_enabled": False
+}
+
 
 class Endpoint:
     """
     A class containing Twitter API endpoints.
     """
     LOGIN_FLOW = 'https://api.twitter.com/1.1/onboarding/task.json'
     LOGOUT = 'https://api.twitter.com/1.1/account/logout.json'
     CREATE_TWEET = 'https://twitter.com/i/api/graphql/SiM_cAu83R0wnrpmKQQSEw/CreateTweet'
+    CREATE_NOTE_TWEET = 'https://twitter.com/i/api/graphql/iCUB42lIfXf9qPKctjE5rQ/CreateNoteTweet'
     DELETE_TWEET = 'https://twitter.com/i/api/graphql/VaenaVgh5q5ih7kvyVjgtg/DeleteTweet'
     SEARCH_TIMELINE = 'https://twitter.com/i/api/graphql/flaR-PUMshxFWZWPNpq4zA/SearchTimeline'
     UPLOAD_MEDIA = 'https://upload.twitter.com/i/media/upload.json'
     CREATE_MEDIA_METADATA = 'https://api.twitter.com/1.1/media/metadata/create.json'
     GUEST_TOKEN = 'https://api.twitter.com/1.1/guest/activate.json'
     CREATE_CARD = 'https://caps.twitter.com/v2/cards/create.json'
     USER_BY_SCREEN_NAME = 'https://twitter.com/i/api/graphql/NimuplG1OB7Fd2btCLdBOw/UserByScreenName'
```

### Comparing `twikit-1.5.3/twikit.egg-info/PKG-INFO` & `twikit-1.5.4/twikit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.3
+Version: 1.5.4
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.3/twikit.egg-info/SOURCES.txt` & `twikit-1.5.4/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

