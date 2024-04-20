# Comparing `tmp/django-feed-reader-2.0.0b1.tar.gz` & `tmp/django_feed_reader-2.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-feed-reader-2.0.0b1.tar", last modified: Wed Feb 28 13:40:26 2024, max compression
+gzip compressed data, was "django_feed_reader-2.0.1b1.tar", last modified: Sat Apr 20 09:43:37 2024, max compression
```

## Comparing `django-feed-reader-2.0.0b1.tar` & `django_feed_reader-2.0.1b1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-02-28 13:40:26.605566 django-feed-reader-2.0.0b1/
--rw-r--r--   0 g          (501) staff       (20)     1071 2023-01-28 17:47:47.000000 django-feed-reader-2.0.0b1/LICENSE
--rw-r--r--   0 g          (501) staff       (20)       87 2023-01-28 17:47:47.000000 django-feed-reader-2.0.0b1/MANIFEST.in
--rw-r--r--   0 g          (501) staff       (20)     4757 2024-02-28 13:40:26.605505 django-feed-reader-2.0.0b1/PKG-INFO
--rw-r--r--   0 g          (501) staff       (20)     4152 2024-02-25 20:00:43.000000 django-feed-reader-2.0.0b1/README.md
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-02-28 13:40:26.605263 django-feed-reader-2.0.0b1/django_feed_reader.egg-info/
--rw-r--r--   0 g          (501) staff       (20)     4757 2024-02-28 13:40:26.000000 django-feed-reader-2.0.0b1/django_feed_reader.egg-info/PKG-INFO
--rw-r--r--   0 g          (501) staff       (20)     1202 2024-02-28 13:40:26.000000 django-feed-reader-2.0.0b1/django_feed_reader.egg-info/SOURCES.txt
--rw-r--r--   0 g          (501) staff       (20)        1 2024-02-28 13:40:26.000000 django-feed-reader-2.0.0b1/django_feed_reader.egg-info/dependency_links.txt
--rw-r--r--   0 g          (501) staff       (20)       74 2024-02-28 13:40:26.000000 django-feed-reader-2.0.0b1/django_feed_reader.egg-info/requires.txt
--rw-r--r--   0 g          (501) staff       (20)        6 2024-02-28 13:40:26.000000 django-feed-reader-2.0.0b1/django_feed_reader.egg-info/top_level.txt
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-02-28 13:40:26.601413 django-feed-reader-2.0.0b1/feeds/
--rw-r--r--   0 g          (501) staff       (20)      442 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/__init__.py
--rw-r--r--   0 g          (501) staff       (20)     1528 2024-02-24 14:36:21.000000 django-feed-reader-2.0.0b1/feeds/admin.py
--rw-r--r--   0 g          (501) staff       (20)      139 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/apps.py
--rw-r--r--   0 g          (501) staff       (20)       17 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/cloudflare.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-02-28 13:40:26.601559 django-feed-reader-2.0.0b1/feeds/management/
--rw-r--r--   0 g          (501) staff       (20)        1 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/management/__init__.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-02-28 13:40:26.601837 django-feed-reader-2.0.0b1/feeds/management/commands/
--rw-r--r--   0 g          (501) staff       (20)        1 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/management/commands/__init__.py
--rw-r--r--   0 g          (501) staff       (20)      298 2024-02-24 14:37:34.000000 django-feed-reader-2.0.0b1/feeds/management/commands/refreshfeeds.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-02-28 13:40:26.605117 django-feed-reader-2.0.0b1/feeds/migrations/
--rw-r--r--   0 g          (501) staff       (20)     3384 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0001_initial.py
--rw-r--r--   0 g          (501) staff       (20)      395 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0002_auto_20190604_0845.py
--rw-r--r--   0 g          (501) staff       (20)      407 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0003_post_image_url.py
--rw-r--r--   0 g          (501) staff       (20)      513 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0004_webproxy.py
--rw-r--r--   0 g          (501) staff       (20)      385 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0005_source_description.py
--rw-r--r--   0 g          (501) staff       (20)      921 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0006_auto_20190901_1644.py
--rw-r--r--   0 g          (501) staff       (20)     1098 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0007_auto_20210502_0716.py
--rw-r--r--   0 g          (501) staff       (20)      419 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0008_allow_longer_post_guid.py
--rw-r--r--   0 g          (501) staff       (20)      576 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py
--rw-r--r--   0 g          (501) staff       (20)      626 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0010_enclosure_description_enclosure_medium.py
--rw-r--r--   0 g          (501) staff       (20)      439 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0011_alter_post_guid.py
--rw-r--r--   0 g          (501) staff       (20)     1383 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/0012_source_last_read_subscription.py
--rw-r--r--   0 g          (501) staff       (20)      474 2024-02-24 22:48:14.000000 django-feed-reader-2.0.0b1/feeds/migrations/0013_delete_webproxy_enclosure_is_current.py
--rw-r--r--   0 g          (501) staff       (20)      561 2024-02-25 01:08:43.000000 django-feed-reader-2.0.0b1/feeds/migrations/0014_post_json_source_json.py
--rw-r--r--   0 g          (501) staff       (20)        0 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/migrations/__init__.py
--rw-r--r--   0 g          (501) staff       (20)     8560 2024-02-25 01:43:17.000000 django-feed-reader-2.0.0b1/feeds/models.py
--rw-r--r--   0 g          (501) staff       (20)    27558 2024-02-25 01:41:59.000000 django-feed-reader-2.0.0b1/feeds/tests.py
--rw-r--r--   0 g          (501) staff       (20)    32167 2024-02-25 01:12:25.000000 django-feed-reader-2.0.0b1/feeds/utils.py
--rw-r--r--   0 g          (501) staff       (20)       63 2024-02-16 11:42:34.000000 django-feed-reader-2.0.0b1/feeds/views.py
--rw-r--r--   0 g          (501) staff       (20)       38 2024-02-28 13:40:26.605732 django-feed-reader-2.0.0b1/setup.cfg
--rw-r--r--   0 g          (501) staff       (20)      875 2024-02-28 13:34:16.000000 django-feed-reader-2.0.0b1/setup.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-20 09:43:37.723745 django_feed_reader-2.0.1b1/
+-rw-r--r--   0 g          (501) staff       (20)     1071 2023-01-28 17:47:47.000000 django_feed_reader-2.0.1b1/LICENSE
+-rw-r--r--   0 g          (501) staff       (20)       87 2023-01-28 17:47:47.000000 django_feed_reader-2.0.1b1/MANIFEST.in
+-rw-r--r--   0 g          (501) staff       (20)     6869 2024-04-20 09:43:37.723680 django_feed_reader-2.0.1b1/PKG-INFO
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-20 09:43:37.723263 django_feed_reader-2.0.1b1/django_feed_reader.egg-info/
+-rw-r--r--   0 g          (501) staff       (20)     6869 2024-04-20 09:43:37.000000 django_feed_reader-2.0.1b1/django_feed_reader.egg-info/PKG-INFO
+-rw-r--r--   0 g          (501) staff       (20)     1236 2024-04-20 09:43:37.000000 django_feed_reader-2.0.1b1/django_feed_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 g          (501) staff       (20)        1 2024-04-20 09:43:37.000000 django_feed_reader-2.0.1b1/django_feed_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 g          (501) staff       (20)       90 2024-04-20 09:43:37.000000 django_feed_reader-2.0.1b1/django_feed_reader.egg-info/requires.txt
+-rw-r--r--   0 g          (501) staff       (20)        6 2024-04-20 09:43:37.000000 django_feed_reader-2.0.1b1/django_feed_reader.egg-info/top_level.txt
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-20 09:43:37.720103 django_feed_reader-2.0.1b1/feeds/
+-rw-r--r--   0 g          (501) staff       (20)      442 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)     1528 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/admin.py
+-rw-r--r--   0 g          (501) staff       (20)      139 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/apps.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-20 09:43:37.720245 django_feed_reader-2.0.1b1/feeds/management/
+-rw-r--r--   0 g          (501) staff       (20)        1 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/management/__init__.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-20 09:43:37.720540 django_feed_reader-2.0.1b1/feeds/management/commands/
+-rw-r--r--   0 g          (501) staff       (20)        1 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/management/commands/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)      415 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/management/commands/refreshfeeds.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-20 09:43:37.723119 django_feed_reader-2.0.1b1/feeds/migrations/
+-rw-r--r--   0 g          (501) staff       (20)     3384 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0001_initial.py
+-rw-r--r--   0 g          (501) staff       (20)      395 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0002_auto_20190604_0845.py
+-rw-r--r--   0 g          (501) staff       (20)      407 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0003_post_image_url.py
+-rw-r--r--   0 g          (501) staff       (20)      513 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0004_webproxy.py
+-rw-r--r--   0 g          (501) staff       (20)      385 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0005_source_description.py
+-rw-r--r--   0 g          (501) staff       (20)      921 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0006_auto_20190901_1644.py
+-rw-r--r--   0 g          (501) staff       (20)     1098 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0007_auto_20210502_0716.py
+-rw-r--r--   0 g          (501) staff       (20)      419 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0008_allow_longer_post_guid.py
+-rw-r--r--   0 g          (501) staff       (20)      576 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py
+-rw-r--r--   0 g          (501) staff       (20)      626 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0010_enclosure_description_enclosure_medium.py
+-rw-r--r--   0 g          (501) staff       (20)      439 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0011_alter_post_guid.py
+-rw-r--r--   0 g          (501) staff       (20)     1383 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0012_source_last_read_subscription.py
+-rw-r--r--   0 g          (501) staff       (20)      474 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0013_delete_webproxy_enclosure_is_current.py
+-rw-r--r--   0 g          (501) staff       (20)      561 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0014_post_json_source_json.py
+-rw-r--r--   0 g          (501) staff       (20)      393 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0015_source_alt_url.py
+-rw-r--r--   0 g          (501) staff       (20)        0 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)    17419 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/models.py
+-rw-r--r--   0 g          (501) staff       (20)    34044 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/tests.py
+-rw-r--r--   0 g          (501) staff       (20)    14197 2024-04-20 09:41:43.000000 django_feed_reader-2.0.1b1/feeds/utils.py
+-rw-r--r--   0 g          (501) staff       (20)    20969 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/utils_internal.py
+-rw-r--r--   0 g          (501) staff       (20)       63 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/views.py
+-rw-r--r--   0 g          (501) staff       (20)       38 2024-04-20 09:43:37.723925 django_feed_reader-2.0.1b1/setup.cfg
+-rw-r--r--   0 g          (501) staff       (20)      903 2024-04-20 09:43:34.000000 django_feed_reader-2.0.1b1/setup.py
```

### Comparing `django-feed-reader-2.0.0b1/LICENSE` & `django_feed_reader-2.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-feed-reader-2.0.0b1/django_feed_reader.egg-info/SOURCES.txt` & `django_feed_reader-2.0.1b1/django_feed_reader.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 LICENSE
 MANIFEST.in
-README.md
 setup.cfg
 setup.py
 django_feed_reader.egg-info/PKG-INFO
 django_feed_reader.egg-info/SOURCES.txt
 django_feed_reader.egg-info/dependency_links.txt
 django_feed_reader.egg-info/requires.txt
 django_feed_reader.egg-info/top_level.txt
 feeds/__init__.py
 feeds/admin.py
 feeds/apps.py
-feeds/cloudflare.py
 feeds/models.py
 feeds/tests.py
 feeds/utils.py
+feeds/utils_internal.py
 feeds/views.py
 feeds/management/__init__.py
 feeds/management/commands/__init__.py
 feeds/management/commands/refreshfeeds.py
 feeds/migrations/0001_initial.py
 feeds/migrations/0002_auto_20190604_0845.py
 feeds/migrations/0003_post_image_url.py
@@ -29,8 +28,9 @@
 feeds/migrations/0008_allow_longer_post_guid.py
 feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py
 feeds/migrations/0010_enclosure_description_enclosure_medium.py
 feeds/migrations/0011_alter_post_guid.py
 feeds/migrations/0012_source_last_read_subscription.py
 feeds/migrations/0013_delete_webproxy_enclosure_is_current.py
 feeds/migrations/0014_post_json_source_json.py
+feeds/migrations/0015_source_alt_url.py
 feeds/migrations/__init__.py
```

### Comparing `django-feed-reader-2.0.0b1/feeds/admin.py` & `django_feed_reader-2.0.1b1/feeds/admin.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-2.0.0b1/feeds/migrations/0001_initial.py` & `django_feed_reader-2.0.1b1/feeds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-2.0.0b1/feeds/migrations/0004_webproxy.py` & `django_feed_reader-2.0.1b1/feeds/migrations/0004_webproxy.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-2.0.0b1/feeds/migrations/0006_auto_20190901_1644.py` & `django_feed_reader-2.0.1b1/feeds/migrations/0006_auto_20190901_1644.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-2.0.0b1/feeds/migrations/0007_auto_20210502_0716.py` & `django_feed_reader-2.0.1b1/feeds/migrations/0007_auto_20210502_0716.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-2.0.0b1/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py` & `django_feed_reader-2.0.1b1/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-2.0.0b1/feeds/migrations/0010_enclosure_description_enclosure_medium.py` & `django_feed_reader-2.0.1b1/feeds/migrations/0010_enclosure_description_enclosure_medium.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-2.0.0b1/feeds/migrations/0012_source_last_read_subscription.py` & `django_feed_reader-2.0.1b1/feeds/migrations/0012_source_last_read_subscription.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-2.0.0b1/feeds/migrations/0014_post_json_source_json.py` & `django_feed_reader-2.0.1b1/feeds/migrations/0014_post_json_source_json.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-2.0.0b1/feeds/tests.py` & `django_feed_reader-2.0.1b1/feeds/tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,48 @@
-from django.test import TestCase, TransactionTestCase
+
+from datetime import timedelta
+from importlib import reload
+import os
+
 from django.conf import settings
+from django.contrib.auth import get_user_model
+from django.test import TestCase, TransactionTestCase
+from django.utils import timezone
+import requests_mock
+
 
 # Create your tests here.
-from feeds.models import Source, Subscription
-from feeds.utils import (
-    read_feed,
+from feeds.models import Source, Subscription, Post
+from feeds.utils_internal import (
     fix_relative,
     hash_body,
+)
+from feeds.utils import (
+    read_feed,
     get_subscription_list_for_user,
     get_unread_subscription_list_for_user
 )
 
 from feeds import utils
-from importlib import reload
-
-from django.contrib.auth import get_user_model
-from django.utils import timezone
-
-from datetime import timedelta
-
-import os
+from feeds import utils_internal
 
-import requests_mock
 
 User = get_user_model()
 
 TEST_FILES_FOLDER = os.path.join(os.path.dirname(os.path.abspath(__file__)), "testdata")
 BASE_URL = 'http://feed.com/'
 
 
+class NullOutput(object):
+
+    # little class to stop the tests filling the console window
+    def write(self, strin: str):
+        pass
+
+
 class UtilsTest(TestCase):
 
     def test_fix_relative(self):
 
         url = "https://example.com/rss.xml"
         html = "<a href='/'><img src='/image.jpg'></a>"
 
@@ -48,17 +58,16 @@
         content = open(os.path.join(TEST_FILES_FOLDER, test_file), "rb").read()
 
         ret_headers = {"Content-Type": content_type, "etag": "an-etag"}
         if headers is not None:
             ret_headers = {**ret_headers, **headers}
 
         if is_cloudflare:
-            agent = "{user_agent} (+{server}; Updater; {subs} subscribers)".format(user_agent=settings.FEEDS_USER_AGENT, server=settings.FEEDS_SERVER, subs=1)
-
-            mock.register_uri('GET', url, request_headers={"User-Agent": agent}, status_code=status, content=content, headers=ret_headers)
+            ret_headers["Server"] = "Some cloudflare thing"
+            mock.register_uri('GET', url, status_code=status, content=content, headers=ret_headers)
         else:
             if etag is None:
                 mock.register_uri('GET', url, status_code=status, content=content, headers=ret_headers)
             else:
                 mock.register_uri('GET', url, request_headers={'If-None-Match': etag}, status_code=status, content=content, headers=ret_headers)
 
 
@@ -70,25 +79,29 @@
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/rss+xml")
 
         ls = timezone.now()
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.unread_count, 1)
 
+        self.assertEqual(len(src.get_unread_posts()), 1)
+
         src.mark_read()
 
         src.refresh_from_db()
 
         self.assertEqual(src.unread_count, 0)
 
+        self.assertEqual(len(src.get_unread_posts()), 0)
+
     def test_subscriber_count(self, mock):
 
         ls = timezone.now()
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
         src.save()
         src.refresh_from_db()
         # If we don't use Subscriptions then the default is 1
@@ -127,15 +140,15 @@
         ls = timezone.now()
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
         src.save()
 
         user = User(email='x@example.com')
         user.save()
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
 
         sub = Subscription(user=user, source=src)
         sub.save()
         sub.refresh_from_db()
 
         self.assertEqual(src.unread_count, 1)
 
@@ -192,116 +205,157 @@
         all_subs_and_folder = Subscription.objects.filter(user=user).count()
 
         sub_list = get_subscription_list_for_user(user)
 
         self.assertEqual(all_subs_and_folder, 11)
         self.assertEqual(len(sub_list), 6)
 
-    def test_basic_subscription_unread_counts(self, mock):
+    def test_basic_subscription_read(self, mock):
 
         user = User(email='x@example.com')
         user.save()
 
         for i in range(5):
             ls = timezone.now()
             src = Source(name="test{i}".format(i=i), feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
             src.max_index = 1
+            src.last_read
             src.save()
 
             sub = Subscription(user=user, source=src)
             sub.save()
 
         folder = Subscription(user=user, source=None, name="Folder")
         folder.save()
 
         for i in range(5):
             ls = timezone.now()
             src = Source(name="folder_test{i}".format(i=i), feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
             src.max_index = 1
             src.save()
 
+            # make the posts get created earlier as they increase in index to check the ordering below
+            p = Post(source=src, title=f"post{i}", created=timezone.now() - timedelta(days=i), index=1, guid=f"src-{src.id}-post-{i}")
+            p.save()
+
             sub = Subscription(user=user, source=src, parent=folder)
+            src.last_read = 0
             sub.save()
 
         all_subs_and_folder = Subscription.objects.filter(user=user).count()
 
         sub_list = get_unread_subscription_list_for_user(user)
 
         self.assertEqual(all_subs_and_folder, 11)
         self.assertEqual(len(sub_list), 6)
 
         for s in sub_list:
             if s.source is None:
                 self.assertEqual(s.unread_count, 5)
 
-    def test_nested_subscription_unread_counts(self, mock):
+                self.assertEqual(len(s.get_unread_posts()), 5)
+
+                i = 5
+                for p in s.get_unread_posts():
+                    i -= 1
+                    self.assertEqual(p.title, f"post{i}")
+
+    def test_nested_subscription_read(self, mock):
 
         user = User(email='x@example.com')
         user.save()
 
+        pcount = 0
+
         for i in range(3):
             ls = timezone.now()
             src = Source(name="test{i}".format(i=i), feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
-            src.max_index = 1
             src.save()
 
+            for j in range(3):
+                p = Post(source=src, title="post", created=timezone.now())
+                p.save()
+
             sub = Subscription(user=user, source=src)
             sub.save()
 
         folder = Subscription(user=user, source=None, name="Folder")
         folder.save()
 
         for i in range(3):
             ls = timezone.now()
             src = Source(name="folder1_test{i}".format(i=i), feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
-            src.max_index = 1
             src.save()
 
+            for j in range(3):
+                p = Post(source=src, title=f"post-{pcount}", created=timezone.now()-timedelta(days=pcount))
+                p.save()
+                pcount += 1
+
             sub = Subscription(user=user, source=src, parent=folder)
+            sub.name = f"Sub-1-{i}"
             sub.save()
 
         folder2 = Subscription(user=user, source=None, name="AFolder2", parent=folder)
         folder2.save()
 
         for i in range(3):
             ls = timezone.now()
             src = Source(name="folder2_test{i}".format(i=i), feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
-            src.max_index = 1
             src.save()
 
+            for j in range(3):
+                p = Post(source=src, title=f"post-{pcount}", created=timezone.now()-timedelta(days=pcount))
+                p.save()
+                pcount += 1
+
             sub = Subscription(user=user, source=src, parent=folder2)
             sub.save()
 
         all_subs_and_folder = Subscription.objects.filter(user=user).count()
 
         sub_list = get_unread_subscription_list_for_user(user)
 
         self.assertEqual(all_subs_and_folder, 11)
         self.assertEqual(len(sub_list), 4)
 
         for s in sub_list:
             if s.source is None:
-                self.assertEqual(s.unread_count, 6)
+                self.assertEqual(s.unread_count, 18)
+                self.assertEqual(len(s.get_unread_posts()), 18)
+                last = None
+                for p in s.get_unread_posts():
+                    if last:
+                        self.assertGreater(p.created, last.created)
+                    last = p
+
+        (posts, paginator) = folder.get_paginated_posts(1, posts_per_page=10)
+        self.assertEqual(len(posts), 10)
+        self.assertEqual(paginator.num_pages, 2)
+        self.assertEqual(posts[0].subscription.name, "Sub-1-0")
+
+        (posts, paginator) = folder.get_paginated_posts(2, posts_per_page=10)
+        self.assertEqual(len(posts), 8)
 
     def test_get_unread(self, mock):
 
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/rss+xml")
 
         ls = timezone.now()
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
-        self.assertEqual(src.unread_posts.count(), 1)
+        self.assertEqual(len(src.get_unread_posts()), 1)
         src.mark_read()
         src.refresh_from_db()
-        self.assertEqual(src.unread_posts.count(), 0)
+        self.assertEqual(len(src.get_unread_posts()), 0)
 
     def test_get_unread_count_for_single_folder(self, mock):
 
         user = User(email='x@example.com')
         user.save()
 
         for i in range(3):
@@ -352,15 +406,15 @@
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/rss+xml")
 
         ls = timezone.now()
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.posts.count(), 1)  # got the one post
         self.assertEqual(src.interval, 60)
         self.assertEqual(src.etag, "an-etag")
         self.assertNotEqual(src.last_success, ls)
@@ -370,15 +424,15 @@
 
         self._populate_mock(mock, status=200, test_file="podcast.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.description, 'SU: Three nerds discussing tech, Apple, programming, and loosely related matters.')
 
         self.assertEqual(src.posts.all()[0].enclosures.count(), 1)
 
         enc = src.posts.all()[0].enclosures.all()[0]
@@ -388,29 +442,29 @@
     def test_mastodon(self, mock):
 
         self._populate_mock(mock, status=200, test_file="mastodon.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.description, 'Public posts from @xurble@toot.community')
 
         self.assertEqual(src.posts.all()[0].enclosures.count(), 1)
 
     def test_media_content(self, mock):
 
         self._populate_mock(mock, status=200, test_file="media_content.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         post = src.posts.all()[0]
         self.assertEqual(post.enclosures.count(), 1)
 
         self.assertEqual(post.body, "<p>New job, new Mac.</p>")
 
@@ -421,25 +475,26 @@
 
     def test_keep_old_enclosure(self, mock):
 
         settings.FEEDS_KEEP_OLD_ENCLOSURES = True
 
         # to pick up the settings change
         reload(utils)
+        reload(utils_internal)
 
         self._populate_mock(mock, status=200, test_file="media_content.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
 
         self._populate_mock(mock, status=200, test_file="media_content_changed.xml", content_type="application/rss+xml")
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         post = src.posts.all()[0]
         self.assertEqual(post.enclosures.count(), 2)
 
         self.assertEqual(post.current_enclosures.count(), 1)
         self.assertEqual(post.old_enclosures.count(), 1)
@@ -450,21 +505,22 @@
 
     def test_save_json(self, mock):
 
         settings.FEEDS_SAVE_JSON = True
 
         # to pick up the settings change
         reload(utils)
+        reload(utils_internal)
 
         self._populate_mock(mock, status=200, test_file="media_content.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
         self.assertEqual(src.json["feed"]["link"], "https://toot.community/@xurble")
 
         post = src.posts.all()[0]
         self.assertEqual(post.json["summary"], post.body)
 
     def test_sanitize_1(self, mock):
@@ -475,15 +531,15 @@
 
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         p = src.posts.all()[0]
 
         self.assertFalse("<script>" in p.body)
 
@@ -495,29 +551,29 @@
 
         self._populate_mock(mock, status=200, test_file="sanitizer_bad_comment.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # read the feed to update the name
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.name, "safe")
 
     def test_sanitize_attrs(self, mock):
 
         self._populate_mock(mock, status=200, test_file="sanitizer_img_attrs.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # read the feed to update the name
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
 
         body = src.posts.all()[0].body
 
         self.assertTrue("<img" in body)
@@ -527,15 +583,15 @@
     def create_source(self, mock, test_name, test_fn):
         self._populate_mock(mock, status=200,
                             test_file=test_fn,
                             content_type="application/rss+xml")
         src = Source(name=test_name, feed_url=BASE_URL, interval=0)
         src.save()
         # read the feed to update the name
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
         self.assertEqual(src.status_code, 200)
         return src
 
     def test_catch_long_guid_short_url(self, mock):
         test_name = "long guid short url"
         src = self.create_source(mock, test_name, "long_guid_tests.xml")
@@ -560,15 +616,15 @@
 
         ls = timezone.now()
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls, last_change=ls)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.posts.count(), 2)  # got the one post
         self.assertEqual(src.interval, 60)
         self.assertEqual(src.etag, "an-etag")
         self.assertNotEqual(src.last_success, ls)
@@ -576,36 +632,37 @@
 
     def test_save_json(self, mock):
 
         settings.FEEDS_SAVE_JSON = True
 
         # to pick up the settings change
         reload(utils)
+        reload(utils_internal)
 
         self._populate_mock(mock, status=200, test_file="json_simple_two_entry.json", content_type="application/json")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
         self.assertEqual(src.json["title"], src.name)
 
         post = src.posts.all()[0]
         self.assertEqual(post.json["url"], post.link)
 
     def test_sanitize_1(self, mock):
 
         self._populate_mock(mock, status=200, test_file="json_simple_two_entry.json", content_type="application/json")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         p = src.posts.all()[0]
 
         self.assertFalse("<script>" in p.body)
 
@@ -617,29 +674,29 @@
 
         self._populate_mock(mock, status=200, test_file="sanitizer_bad_comment.json", content_type="application/json")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # read the feed to update the name
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.name, "safe")
 
     def test_podcast(self, mock):
 
         self._populate_mock(mock, status=200, test_file="podcast.json", content_type="application/json")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # read the feed to update the name
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
 
         post = src.posts.all()[0]
 
         self.assertEqual(post.enclosures.count(), 1)
@@ -653,39 +710,39 @@
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/xml+rss")
         self._populate_mock(mock, status=304, test_file="empty_file.txt", content_type="application/xml+rss", etag="an-etag")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         # Read the feed once to get the 1 post  and the etag
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.posts.count(), 1)  # got the one post
         self.assertEqual(src.interval, 60)
         self.assertEqual(src.etag, "an-etag")
 
         # Read the feed again to get a 304 and a small increment to the interval
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.posts.count(), 1)  # should have no more
         self.assertEqual(src.status_code, 304)
         self.assertEqual(src.interval, 70)
         self.assertTrue(src.live)
 
     def test_not_a_feed(self, mock):
 
         self._populate_mock(mock, status=200, test_file="spurious_text_file.txt", content_type="text/plain")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)  # it returned a page, but not a  feed
         self.assertEqual(src.posts.count(), 0)  # can't have got any
         self.assertEqual(src.interval, 120)
         self.assertTrue(src.live)
 
@@ -694,43 +751,120 @@
         self._populate_mock(mock, status=403, test_file="empty_file.txt", content_type="text/plain")
 
         ls = timezone.now()
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls)
         src.save()
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 403)  # it returned a page, but not a  feed
         self.assertEqual(src.posts.count(), 0)  # can't have got any
         self.assertFalse(src.live)
 
+    def test_cloudflared_standard(self, mock):
+
+        settings.FEEDS_DRIPFEED_KEY = "Key"
+
+        # to pick up the settings change
+        reload(utils)
+
+        self._populate_mock(mock, status=403, test_file="empty_file.txt", content_type="text/plain", is_cloudflare=True)
+
+        mock.register_uri('PUT', "https://dripfeed.app/api/v1/feeds/", content=b"""{"feed": {"uuid": "aa48333e-c40d-47ac-8a46-a13352dd8505", "name": "Elephant", "source_url": "http://feed.com/", "status_code": 200, "last_polled": "2024-03-17T18:48:19Z", "next_poll": "2024-03-25T03:06:08.991Z", "content_type": "text/plain", "etag": "06b06eb5", "error_code": "not-feed", "last_result": "Server response was not a feed", "dripfeed_url": "https://dripfeed.app/feed/aa48333e-c40d-47ac-8a46-a13352dd8505/", "live": true}, "detail": "OK"}""")
+
+        ls = timezone.now()
+
+        src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls)
+        src.save()
+
+        read_feed(src, output=NullOutput())
+        src.refresh_from_db()
+
+        self.assertEqual(src.status_code, 403)  # it returned a page, but not a  feed
+        self.assertEqual(src.posts.count(), 0)  # can't have got any
+        self.assertTrue(src.live)
+        self.assertTrue(src.is_cloudflare)
+        self.assertEqual(src.alt_url, "https://dripfeed.app/feed/aa48333e-c40d-47ac-8a46-a13352dd8505/")
+
+    def test_cloudflared_already_dripfed(self, mock):
+
+        settings.FEEDS_DRIPFEED_KEY = "Key"
+
+        # to pick up the settings change
+        reload(utils)
+
+        self._populate_mock(mock, status=403, test_file="empty_file.txt", content_type="text/plain", is_cloudflare=True)
+
+        mock.register_uri('PUT', "https://dripfeed.app/api/v1/feeds/", status_code=400, content=b"""{"detail": "Already subscribed to this feed."}""")
+        mock.register_uri('GET', "https://dripfeed.app/api/v1/feeds/", content=b"""{"feeds": [{"uuid": "aa48333e-c40d-47ac-8a46-a13352dd8505", "name": "Elephant", "source_url": "http://feed.com/", "status_code": 200, "last_polled": "2024-03-17T18:48:19Z", "next_poll": "2024-03-25T03:06:08.991Z", "content_type": "text/plain", "etag": "06b06eb5", "error_code": "not-feed", "last_result": "Server response was not a feed", "dripfeed_url": "https://dripfeed.app/feed/aa48333e-c40d-47ac-8a46-a13352dd8505/", "live": true}], "detail": "OK"}""")
+
+        ls = timezone.now()
+
+        src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls)
+        src.save()
+
+        read_feed(src, output=NullOutput())
+        src.refresh_from_db()
+
+        self.assertEqual(src.status_code, 403)  # it returned a page, but not a  feed
+        self.assertEqual(src.posts.count(), 0)  # can't have got any
+        self.assertTrue(src.live)
+        self.assertTrue(src.is_cloudflare)
+        self.assertEqual(src.alt_url, "https://dripfeed.app/feed/aa48333e-c40d-47ac-8a46-a13352dd8505/")
+
+    def test_cloudflared_cant_dripfeed(self, mock):
+
+        settings.FEEDS_DRIPFEED_KEY = "Key"
+
+        # to pick up the settings change
+        reload(utils)
+
+        self._populate_mock(mock, status=403, test_file="empty_file.txt", content_type="text/plain", is_cloudflare=True)
+
+        mock.register_uri('PUT', "https://dripfeed.app/api/v1/feeds/", status_code=403, content=b"""{"detail": "Maximum number of feeds reached."}""")
+
+        ls = timezone.now()
+
+        src = Source(name="test1", feed_url=BASE_URL, interval=0, last_success=ls)
+        src.save()
+
+        read_feed(src, output=NullOutput())
+        src.refresh_from_db()
+
+        self.assertEqual(src.status_code, 403)  # it returned a page, but not a  feed
+        self.assertEqual(src.posts.count(), 0)  # can't have got any
+        self.assertTrue(src.live)
+        self.assertTrue(src.is_cloudflare)
+        self.assertIsNone(src.alt_url)
+        self.assertEqual(src.last_result, "Failed add to Dripfeed: Maximum number of feeds reached.")
+
     def test_feed_gone(self, mock):
 
         self._populate_mock(mock, status=410, test_file="empty_file.txt", content_type="text/plain")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 410)  # it returned a page, but not a  feed
         self.assertEqual(src.posts.count(), 0)  # can't have got any
         self.assertFalse(src.live)
 
     def test_feed_not_found(self, mock):
 
         self._populate_mock(mock, status=404, test_file="empty_file.txt", content_type="text/plain")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 404)  # it returned a page, but not a  feed
         self.assertEqual(src.posts.count(), 0)  # can't have got any
         self.assertTrue(src.live)
         self.assertEqual(src.interval, 120)
 
@@ -741,39 +875,39 @@
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/xml+rss",  url=new_url)
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
         self.assertIsNone(src.last_302_start)
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.last_302_url, new_url)  # this is where  went
         self.assertIsNotNone(src.last_302_start)
         self.assertEqual(src.posts.count(), 1)  # after following redirect will have 1 post
         self.assertEqual(src.interval, 60)
         self.assertTrue(src.live)
 
         # do it all again -  shouldn't change
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)  # it returned a page, but not a  feed
         self.assertEqual(src.last_302_url, new_url)  # this is where  went
         self.assertIsNotNone(src.last_302_start)
         self.assertEqual(src.posts.count(), 1)  # after following redirect will have 1 post
         self.assertEqual(src.interval, 80)
         self.assertTrue(src.live)
 
         # now we test making it permaent
         src.last_302_start = timezone.now() - timedelta(days=365)
         src.save()
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.last_302_url, ' ')
         self.assertIsNone(src.last_302_start)
         self.assertEqual(src.posts.count(), 1)
         self.assertEqual(src.interval, 100)
@@ -785,51 +919,51 @@
         new_url = "http://new.feed.com/"
         self._populate_mock(mock, status=301, test_file="empty_file.txt", content_type="text/plain", headers={"Location": new_url})
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/xml+rss",  url=new_url)
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 301)
         self.assertEqual(src.interval, 60)
         self.assertEqual(src.feed_url, new_url)
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 200)
         self.assertEqual(src.posts.count(), 1)
         self.assertEqual(src.interval, 60)
         self.assertTrue(src.live)
 
     def test_server_error_1(self, mock):
 
         self._populate_mock(mock, status=500, test_file="empty_file.txt", content_type="text/plain")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 500)  # error
         self.assertEqual(src.posts.count(), 0)  # can't have got any
         self.assertTrue(src.live)
         self.assertEqual(src.interval, 120)
 
     def test_server_error_2(self, mock):
 
         self._populate_mock(mock, status=503, test_file="empty_file.txt", content_type="text/plain")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
-        read_feed(src)
+        read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 503)  # error!
         self.assertEqual(src.posts.count(), 0)  # can't have got any
         self.assertTrue(src.live)
         self.assertEqual(src.interval, 120)
```

### Comparing `django-feed-reader-2.0.0b1/setup.py` & `django_feed_reader-2.0.1b1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import setuptools
 
 
-with open('readme.md', encoding='utf-8') as f:
+with open('readme.rst', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name='django-feed-reader',
-    version='2.0.0-beta.1',
+    version='2.0.1-beta.1',
     description='An RSS feed reading library for Django.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Gareth Simpson',
     author_email='g@xurble.org',
     url='https://github.com/xurble/django-feed-reader',
     license='MIT',
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
+        'dripfeed-client',
         'sgmllib3k',
         'requests',
         'feedparser>=6.0.0',
         'beautifulsoup4',
         'pyrfc3339',
         'Django>=2.2'
     ],
```

