# Comparing `tmp/bilibili_dl-3.0.0.tar.gz` & `tmp/bilibili-dl-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilibili_dl-3.0.0.tar", last modified: Wed Apr 17 13:23:36 2024, max compression
+gzip compressed data, was "bilibili-dl-3.1.0.tar", last modified: Sat Apr 20 07:42:32 2024, max compression
```

## Comparing `bilibili_dl-3.0.0.tar` & `bilibili-dl-3.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 youguang   (501) staff       (20)        0 2024-04-17 13:23:36.878344 bilibili_dl-3.0.0/
--rw-r--r--   0 youguang   (501) staff       (20)    19363 2024-04-17 12:57:30.000000 bilibili_dl-3.0.0/LICENSE
--rw-r--r--   0 youguang   (501) staff       (20)     1427 2024-04-17 13:23:36.878153 bilibili_dl-3.0.0/PKG-INFO
--rw-r--r--   0 youguang   (501) staff       (20)     1080 2024-04-17 12:57:30.000000 bilibili_dl-3.0.0/README.md
-drwxr-xr-x   0 youguang   (501) staff       (20)        0 2024-04-17 13:23:36.877136 bilibili_dl-3.0.0/bilibili_dl/
--rw-r--r--   0 youguang   (501) staff       (20)        0 2024-04-17 12:57:30.000000 bilibili_dl-3.0.0/bilibili_dl/__init__.py
--rw-r--r--   0 youguang   (501) staff       (20)       58 2024-04-17 13:13:19.000000 bilibili_dl-3.0.0/bilibili_dl/cli.py
--rw-r--r--   0 youguang   (501) staff       (20)     3476 2024-04-17 13:13:23.000000 bilibili_dl-3.0.0/bilibili_dl/downloader.py
--rw-r--r--   0 youguang   (501) staff       (20)     1408 2024-04-17 13:13:26.000000 bilibili_dl-3.0.0/bilibili_dl/main.py
--rw-r--r--   0 youguang   (501) staff       (20)     2012 2024-04-17 13:14:08.000000 bilibili_dl-3.0.0/bilibili_dl/utils.py
-drwxr-xr-x   0 youguang   (501) staff       (20)        0 2024-04-17 13:23:36.877958 bilibili_dl-3.0.0/bilibili_dl.egg-info/
--rw-r--r--   0 youguang   (501) staff       (20)     1427 2024-04-17 13:23:36.000000 bilibili_dl-3.0.0/bilibili_dl.egg-info/PKG-INFO
--rw-r--r--   0 youguang   (501) staff       (20)      348 2024-04-17 13:23:36.000000 bilibili_dl-3.0.0/bilibili_dl.egg-info/SOURCES.txt
--rw-r--r--   0 youguang   (501) staff       (20)        1 2024-04-17 13:23:36.000000 bilibili_dl-3.0.0/bilibili_dl.egg-info/dependency_links.txt
--rw-r--r--   0 youguang   (501) staff       (20)       56 2024-04-17 13:23:36.000000 bilibili_dl-3.0.0/bilibili_dl.egg-info/entry_points.txt
--rw-r--r--   0 youguang   (501) staff       (20)       26 2024-04-17 13:23:36.000000 bilibili_dl-3.0.0/bilibili_dl.egg-info/requires.txt
--rw-r--r--   0 youguang   (501) staff       (20)       12 2024-04-17 13:23:36.000000 bilibili_dl-3.0.0/bilibili_dl.egg-info/top_level.txt
--rw-r--r--   0 youguang   (501) staff       (20)       38 2024-04-17 13:23:36.878380 bilibili_dl-3.0.0/setup.cfg
--rw-r--r--   0 youguang   (501) staff       (20)      605 2024-04-17 12:58:39.000000 bilibili_dl-3.0.0/setup.py
+drwxr-xr-x   0 youguang   (501) staff       (20)        0 2024-04-20 07:42:32.724332 bilibili-dl-3.1.0/
+-rw-r--r--   0 youguang   (501) staff       (20)    19363 2024-04-20 06:05:37.000000 bilibili-dl-3.1.0/LICENSE
+-rw-r--r--   0 youguang   (501) staff       (20)     1427 2024-04-20 07:42:32.724089 bilibili-dl-3.1.0/PKG-INFO
+-rw-r--r--   0 youguang   (501) staff       (20)     1080 2024-04-20 06:05:37.000000 bilibili-dl-3.1.0/README.md
+drwxr-xr-x   0 youguang   (501) staff       (20)        0 2024-04-20 07:42:32.723078 bilibili-dl-3.1.0/bilibili_dl/
+-rw-r--r--   0 youguang   (501) staff       (20)        0 2024-04-20 06:05:37.000000 bilibili-dl-3.1.0/bilibili_dl/__init__.py
+-rw-r--r--   0 youguang   (501) staff       (20)       58 2024-04-20 06:05:37.000000 bilibili-dl-3.1.0/bilibili_dl/cli.py
+-rw-r--r--   0 youguang   (501) staff       (20)     3476 2024-04-20 07:29:03.000000 bilibili-dl-3.1.0/bilibili_dl/downloader.py
+-rw-r--r--   0 youguang   (501) staff       (20)     1408 2024-04-20 06:44:45.000000 bilibili-dl-3.1.0/bilibili_dl/main.py
+-rw-r--r--   0 youguang   (501) staff       (20)     2339 2024-04-20 06:27:14.000000 bilibili-dl-3.1.0/bilibili_dl/utils.py
+drwxr-xr-x   0 youguang   (501) staff       (20)        0 2024-04-20 07:42:32.723827 bilibili-dl-3.1.0/bilibili_dl.egg-info/
+-rw-r--r--   0 youguang   (501) staff       (20)     1427 2024-04-20 07:42:32.000000 bilibili-dl-3.1.0/bilibili_dl.egg-info/PKG-INFO
+-rw-r--r--   0 youguang   (501) staff       (20)      348 2024-04-20 07:42:32.000000 bilibili-dl-3.1.0/bilibili_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 youguang   (501) staff       (20)        1 2024-04-20 07:42:32.000000 bilibili-dl-3.1.0/bilibili_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 youguang   (501) staff       (20)       56 2024-04-20 07:42:32.000000 bilibili-dl-3.1.0/bilibili_dl.egg-info/entry_points.txt
+-rw-r--r--   0 youguang   (501) staff       (20)       26 2024-04-20 07:42:32.000000 bilibili-dl-3.1.0/bilibili_dl.egg-info/requires.txt
+-rw-r--r--   0 youguang   (501) staff       (20)       12 2024-04-20 07:42:32.000000 bilibili-dl-3.1.0/bilibili_dl.egg-info/top_level.txt
+-rw-r--r--   0 youguang   (501) staff       (20)       38 2024-04-20 07:42:32.724381 bilibili-dl-3.1.0/setup.cfg
+-rw-r--r--   0 youguang   (501) staff       (20)      605 2024-04-20 07:31:25.000000 bilibili-dl-3.1.0/setup.py
```

### Comparing `bilibili_dl-3.0.0/LICENSE` & `bilibili-dl-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bilibili_dl-3.0.0/PKG-INFO` & `bilibili-dl-3.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibili-dl
-Version: 3.0.0
+Version: 3.1.0
 Summary: Bilibili-dl 是一个下载B站音视频的工具（目前视频下载最高只支持720P）
 Home-page: https://github.com/Youguang-Zhou/bilibili-dl
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: progressbar
```

### Comparing `bilibili_dl-3.0.0/README.md` & `bilibili-dl-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bilibili_dl-3.0.0/bilibili_dl/downloader.py` & `bilibili-dl-3.1.0/bilibili_dl/downloader.py`

 * *Files identical despite different names*

### Comparing `bilibili_dl-3.0.0/bilibili_dl/main.py` & `bilibili-dl-3.1.0/bilibili_dl/main.py`

 * *Files identical despite different names*

### Comparing `bilibili_dl-3.0.0/bilibili_dl/utils.py` & `bilibili-dl-3.1.0/bilibili_dl/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,13 +59,20 @@
     根据BV号获取视频详细信息(bvid, cid, title, up_name, pic)
     '''
     try:
         print('[bilibili-dl] 获取视频详细信息中...')
         if type(bvids) == str:
             bvids = [bvids]
         videos = []
-        for bvid in tqdm(bvids):
+        for bvid in tqdm(bvids, leave=False):
             res = send_request(URL_VIDEO_INFO, params={'bvid': bvid})
-            videos.append((res['bvid'], res['cid'], res['title'], res['owner']['name'], res['pic']))
+            # 检查该视频是否为分p视频
+            if res['videos'] == 1:
+                videos.append((res['bvid'], res['cid'], res['title'], res['owner']['name'], res['pic']))
+            else:
+                # 分p列表
+                pages = res['pages']
+                for p in pages:
+                    videos.append((res['bvid'], p['cid'], p['part'], res['owner']['name'], p['first_frame']))
         return videos
     except Exception:
         raise Exception('获取视频详细信息失败！')
```

### Comparing `bilibili_dl-3.0.0/bilibili_dl.egg-info/PKG-INFO` & `bilibili-dl-3.1.0/bilibili_dl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibili-dl
-Version: 3.0.0
+Version: 3.1.0
 Summary: Bilibili-dl 是一个下载B站音视频的工具（目前视频下载最高只支持720P）
 Home-page: https://github.com/Youguang-Zhou/bilibili-dl
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: progressbar
```

### Comparing `bilibili_dl-3.0.0/setup.py` & `bilibili-dl-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='bilibili-dl',
-    version='3.0.0',
+    version='3.1.0',
     description='Bilibili-dl 是一个下载B站音视频的工具（目前视频下载最高只支持720P）',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Youguang-Zhou/bilibili-dl',
     packages=setuptools.find_packages(),
     entry_points={'console_scripts': ['bilibili-dl=bilibili_dl.cli:run_cli']},
     install_requires=['tqdm', 'requests', 'progressbar'],
```

