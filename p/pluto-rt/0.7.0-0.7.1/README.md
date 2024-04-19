# Comparing `tmp/pluto_rt-0.7.0.tar.gz` & `tmp/pluto_rt-0.7.1.tar.gz`

## Comparing `pluto_rt-0.7.0.tar` & `pluto_rt-0.7.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/MANIFEST.in
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/Dockerfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/asgi.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/compose.yaml
--rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/manage.py
--rw-r--r--   0        0        0  2281154 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/pluto_rt_demo.gif
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/requirements.txt
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/settings.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/tasks.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/urls.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/views.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/wsgi.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/demo/demo_index.html
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/demo/demo_list.html
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/demo/demo_messages.html
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/demo/demo_progress.html
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/pluto_rt/list_item.html
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/pluto_rt/progress_item.html
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/pluto_rt/toast_item.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/apps.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/ops.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/urls.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/views.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/templates/pluto_rt/polling.html
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/templates/pluto_rt/sse.html
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/templates/pluto_rt/table.html
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/templates/pluto_rt/table_item.html
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt.egg-info/PKG-INFO
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt.egg-info/top_level.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/tests/tests.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/.gitignore
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/LICENSE
--rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/README.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/MANIFEST.in
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/Dockerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/asgi.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/compose.yaml
+-rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/manage.py
+-rw-r--r--   0        0        0  2281154 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/pluto_rt_demo.gif
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/requirements.txt
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/settings.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/tasks.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/urls.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/views.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/wsgi.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/demo/demo_index.html
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/demo/demo_list.html
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/demo/demo_messages.html
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/demo/demo_progress.html
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/pluto_rt/list_item.html
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/pluto_rt/progress_item.html
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/pluto_rt/toast_item.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/apps.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/ops.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/urls.py
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/views.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/templates/pluto_rt/polling.html
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/templates/pluto_rt/sse.html
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/templates/pluto_rt/table.html
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/templates/pluto_rt/table_item.html
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt.egg-info/top_level.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/tests/tests.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/.gitignore
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6945 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/README.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/PKG-INFO
```

### Comparing `pluto_rt-0.7.0/demo/compose.yaml` & `pluto_rt-0.7.1/demo/compose.yaml`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/demo/manage.py` & `pluto_rt-0.7.1/demo/manage.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/demo/pluto_rt_demo.gif` & `pluto_rt-0.7.1/demo/pluto_rt_demo.gif`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/demo/settings.py` & `pluto_rt-0.7.1/demo/settings.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/demo/tasks.py` & `pluto_rt-0.7.1/demo/tasks.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/demo/views.py` & `pluto_rt-0.7.1/demo/views.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/demo/templates/demo/demo_index.html` & `pluto_rt-0.7.1/demo/templates/demo/demo_index.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/demo/templates/demo/demo_list.html` & `pluto_rt-0.7.1/demo/templates/demo/demo_list.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/demo/templates/demo/demo_messages.html` & `pluto_rt-0.7.1/demo/templates/demo/demo_messages.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/demo/templates/demo/demo_progress.html` & `pluto_rt-0.7.1/demo/templates/demo/demo_progress.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/src/pluto_rt/ops.py` & `pluto_rt-0.7.1/src/pluto_rt/ops.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/src/pluto_rt/urls.py` & `pluto_rt-0.7.1/src/pluto_rt/urls.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/src/pluto_rt/views.py` & `pluto_rt-0.7.1/src/pluto_rt/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import time
 from typing import AsyncGenerator
 
 from asgiref.sync import sync_to_async
 from django.http import (
     HttpRequest,
     HttpResponseBase,
     HttpResponse,
@@ -18,20 +19,27 @@
 async def rt_sse_content(
     request: HttpRequest, queue_name: str, item_template: str
 ) -> AsyncGenerator[str, None]:
     """Deliver event stream of formatted messages from the item template."""
     mqueue = get_rt_queue_handle(queue_name)
     queue_index = 0
     count = 100
+    keepalive_interval = 10  # seconds
+    last_message_time = time.time()
 
     while True:
         items = await sync_to_async(mqueue.range)(queue_index, queue_index + count)
+        now = time.time()
         if not items:
+            if now - last_message_time > keepalive_interval:
+                last_message_time = now
+                yield "event: keepalive\ndata: \n\n"
             await asyncio.sleep(0.1)
             continue
+        last_message_time = now
         queue_index += len(items)
         for item in items:
             if item == mqueue.QUEUE_EXHAUSTED:
                 yield SSE_CLOSE
                 return
             try:
                 lines = loader.render_to_string(item_template, {"item": item}).strip().split("\n")
```

### Comparing `pluto_rt-0.7.0/src/pluto_rt/templates/pluto_rt/table.html` & `pluto_rt-0.7.1/src/pluto_rt/templates/pluto_rt/table.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/src/pluto_rt.egg-info/PKG-INFO` & `pluto_rt-0.7.1/src/pluto_rt.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.0/README.md` & `pluto_rt-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -172,7 +172,9 @@
 0.4.0 Feb 21, 2024: Server-sent events, more flexible templates
 
 0.5.0 Mar 3, 2024: Improved template inclusion, added demos
 
 0.6.0 Mar 9, 2024: Use modes, add replace
 
 0.7.0 Apr 9, 2024: Support multiple consumers
+
+0.7.1 Apr 19, 20204: Keepalive every 10 seconds
```

### Comparing `pluto_rt-0.7.0/pyproject.toml` & `pluto_rt-0.7.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pluto_rt"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
   { name="Scot Hacker", email="shacker@energy-solution.com" },
   { name="Rob Harvey", email="rharvey@energy-solution.com" },
 ]
 description = "A reusable Django app providing a kit for storing and displaying messages from a background processor into a web view in real time, as the processor works."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `pluto_rt-0.7.0/PKG-INFO` & `pluto_rt-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pluto_rt
-Version: 0.7.0
+Version: 0.7.1
 Summary: A reusable Django app providing a kit for storing and displaying messages from a background processor into a web view in real time, as the processor works.
 Project-URL: Homepage, https://github.com/energy-solution/pluto-rt
 Author-email: Scot Hacker <shacker@energy-solution.com>, Rob Harvey <rharvey@energy-solution.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -185,7 +185,9 @@
 0.4.0 Feb 21, 2024: Server-sent events, more flexible templates
 
 0.5.0 Mar 3, 2024: Improved template inclusion, added demos
 
 0.6.0 Mar 9, 2024: Use modes, add replace
 
 0.7.0 Apr 9, 2024: Support multiple consumers
+
+0.7.1 Apr 19, 20204: Keepalive every 10 seconds
```

