# Comparing `tmp/xvideos_api-1.2.tar.gz` & `tmp/xvideos_api-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xvideos_api-1.2.tar", last modified: Mon Apr  1 23:50:48 2024, max compression
+gzip compressed data, was "xvideos_api-1.3.tar", last modified: Sat Apr 20 18:35:14 2024, max compression
```

## Comparing `xvideos_api-1.2.tar` & `xvideos_api-1.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:50:48.342865 xvideos_api-1.2/
--rw-r--r--   0 asuna     (1000) asuna     (1000)     7369 2024-03-28 01:24:01.000000 xvideos_api-1.2/LICENSE
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2542 2024-04-01 23:50:48.342865 xvideos_api-1.2/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-04-01 23:50:48.342865 xvideos_api-1.2/setup.cfg
--rw-r--r--   0 asuna     (1000) asuna     (1000)      918 2024-04-01 23:49:55.000000 xvideos_api-1.2/setup.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:50:48.339532 xvideos_api-1.2/xvideos_api/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/__init__.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:50:48.339532 xvideos_api-1.2/xvideos_api/modules/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/modules/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1204 2024-03-29 11:49:46.000000 xvideos_api-1.2/xvideos_api/modules/consts.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)       81 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/modules/exceptions.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)      672 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/modules/sorting.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:50:48.342865 xvideos_api-1.2/xvideos_api/tests/
--rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/tests/__init__.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2981 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/tests/test_search.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)     1550 2024-02-08 17:27:58.000000 xvideos_api-1.2/xvideos_api/tests/test_video.py
--rw-r--r--   0 asuna     (1000) asuna     (1000)    10191 2024-03-29 12:19:12.000000 xvideos_api-1.2/xvideos_api/xvideos_api.py
-drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-01 23:50:48.342865 xvideos_api-1.2/xvideos_api.egg-info/
--rw-r--r--   0 asuna     (1000) asuna     (1000)     2542 2024-04-01 23:50:48.000000 xvideos_api-1.2/xvideos_api.egg-info/PKG-INFO
--rw-r--r--   0 asuna     (1000) asuna     (1000)      470 2024-04-01 23:50:48.000000 xvideos_api-1.2/xvideos_api.egg-info/SOURCES.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-04-01 23:50:48.000000 xvideos_api-1.2/xvideos_api.egg-info/dependency_links.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       53 2024-04-01 23:50:48.000000 xvideos_api-1.2/xvideos_api.egg-info/requires.txt
--rw-r--r--   0 asuna     (1000) asuna     (1000)       12 2024-04-01 23:50:48.000000 xvideos_api-1.2/xvideos_api.egg-info/top_level.txt
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-20 18:35:14.198195 xvideos_api-1.3/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     7369 2024-03-28 01:24:01.000000 xvideos_api-1.3/LICENSE
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2644 2024-04-20 18:35:14.198195 xvideos_api-1.3/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       38 2024-04-20 18:35:14.198195 xvideos_api-1.3/setup.cfg
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      960 2024-04-20 18:35:09.000000 xvideos_api-1.3/setup.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-20 18:35:14.194862 xvideos_api-1.3/xvideos_api/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 17:27:58.000000 xvideos_api-1.3/xvideos_api/__init__.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-20 18:35:14.194862 xvideos_api-1.3/xvideos_api/modules/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 17:27:58.000000 xvideos_api-1.3/xvideos_api/modules/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1204 2024-04-20 18:23:35.000000 xvideos_api-1.3/xvideos_api/modules/consts.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       81 2024-02-08 17:27:58.000000 xvideos_api-1.3/xvideos_api/modules/exceptions.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      672 2024-02-08 17:27:58.000000 xvideos_api-1.3/xvideos_api/modules/sorting.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-20 18:35:14.194862 xvideos_api-1.3/xvideos_api/tests/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        0 2024-02-08 17:27:58.000000 xvideos_api-1.3/xvideos_api/tests/__init__.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      414 2024-04-20 18:34:36.000000 xvideos_api-1.3/xvideos_api/tests/test_pornstar.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2981 2024-02-08 17:27:58.000000 xvideos_api-1.3/xvideos_api/tests/test_search.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     1550 2024-02-08 17:27:58.000000 xvideos_api-1.3/xvideos_api/tests/test_video.py
+-rw-r--r--   0 asuna     (1000) asuna     (1000)    13027 2024-04-20 18:23:52.000000 xvideos_api-1.3/xvideos_api/xvideos_api.py
+drwxr-xr-x   0 asuna     (1000) asuna     (1000)        0 2024-04-20 18:35:14.198195 xvideos_api-1.3/xvideos_api.egg-info/
+-rw-r--r--   0 asuna     (1000) asuna     (1000)     2644 2024-04-20 18:35:14.000000 xvideos_api-1.3/xvideos_api.egg-info/PKG-INFO
+-rw-r--r--   0 asuna     (1000) asuna     (1000)      543 2024-04-20 18:35:14.000000 xvideos_api-1.3/xvideos_api.egg-info/SOURCES.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)        1 2024-04-20 18:35:14.000000 xvideos_api-1.3/xvideos_api.egg-info/dependency_links.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       61 2024-04-20 18:35:14.000000 xvideos_api-1.3/xvideos_api.egg-info/entry_points.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       53 2024-04-20 18:35:14.000000 xvideos_api-1.3/xvideos_api.egg-info/requires.txt
+-rw-r--r--   0 asuna     (1000) asuna     (1000)       12 2024-04-20 18:35:14.000000 xvideos_api-1.3/xvideos_api.egg-info/top_level.txt
```

### Comparing `xvideos_api-1.2/LICENSE` & `xvideos_api-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xvideos_api-1.2/PKG-INFO` & `xvideos_api-1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xvideos_api
-Version: 1.2
+Version: 1.3
 Summary: A Python API for the Porn Site xvideos.com
 Home-page: https://github.com/EchterAlsFake/xvideos_api
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
@@ -55,14 +55,16 @@
 # Download the video
 
 video_object.download(downloader=threaded, quality=Quality.BEST, path="your_output_path + filename")
 
 # SEE DOCUMENTATION FOR MORE
 ```
 
+> [!NOTE]
+> XVideos API can also be used from the command line. Do: xvideos_api -h to see the options
 # Changelog
 See [Changelog](https://github.com/EchterAlsFake/xvideos_api/blob/master/README/Changelog.md) for more details.
 
 # Contribution
 Do you see any issues or having some feature requests? Simply open an Issue or talk
 in the discussions.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xvideos_api Version: 1.2 Summary: A Python API for
+Metadata-Version: 2.1 Name: xvideos_api Version: 1.3 Summary: A Python API for
 the Porn Site xvideos.com Home-page: https://github.com/EchterAlsFake/
 xvideos_api Author: Johannes Habel Author-email: EchterAlsFake@proton.me
 License: LGPLv3 Classifier: License :: OSI Approved :: GNU Lesser General
 Public License v3 (LGPLv3) Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: bs4 Requires-Dist: lxml Requires-Dist: ffmpeg-progress-
 yield Requires-Dist: eaf_base_api
@@ -17,13 +17,14 @@
 blob/master/README/Documentation.md) for more details - Install the library
 with `pip install xvideos_api` ```python from xvideos_api.xvideos_api import
 Client, Quality from base_api.modules.download import threaded, default, FFMPEG
 # Initialize a Client object client = Client() # Fetch a video video_object =
 client.get_video("") # Information from Video objects print(video_object.title)
 print(video_object.likes) # Download the video video_object.download
 (downloader=threaded, quality=Quality.BEST, path="your_output_path + filename")
-# SEE DOCUMENTATION FOR MORE ``` # Changelog See [Changelog](https://
-github.com/EchterAlsFake/xvideos_api/blob/master/README/Changelog.md) for more
-details. # Contribution Do you see any issues or having some feature requests?
-Simply open an Issue or talk in the discussions. Pull requests are also
-welcome. # License Licensed under the LGPLv3 License Copyright (C) 2023â2024
-Johannes Habel
+# SEE DOCUMENTATION FOR MORE ``` > [!NOTE] > XVideos API can also be used from
+the command line. Do: xvideos_api -h to see the options # Changelog See
+[Changelog](https://github.com/EchterAlsFake/xvideos_api/blob/master/README/
+Changelog.md) for more details. # Contribution Do you see any issues or having
+some feature requests? Simply open an Issue or talk in the discussions. Pull
+requests are also welcome. # License Licensed under the LGPLv3 License
+Copyright (C) 2023â2024 Johannes Habel
```

### Comparing `xvideos_api-1.2/setup.py` & `xvideos_api-1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="xvideos_api",
-    version="1.2",
+    version="1.3",
     packages=find_packages(),
     install_requires=[
         "requests", "bs4", "lxml", "ffmpeg-progress-yield", "eaf_base_api"
     ],
     entry_points={
-        'console_scripts': [
+        'console_scripts': ['xvideos_api=xvideos_api.xvideos_api:main'
             # If you want to create any executable scripts
         ],
     },
     author="Johannes Habel",
     author_email="EchterAlsFake@proton.me",
     description="A Python API for the Porn Site xvideos.com",
     long_description=open('/home/asuna/PycharmProjects/xvideos_api/README.md').read(),
```

### Comparing `xvideos_api-1.2/xvideos_api/modules/consts.py` & `xvideos_api-1.3/xvideos_api/modules/consts.py`

 * *Files identical despite different names*

### Comparing `xvideos_api-1.2/xvideos_api/modules/sorting.py` & `xvideos_api-1.3/xvideos_api/modules/sorting.py`

 * *Files identical despite different names*

### Comparing `xvideos_api-1.2/xvideos_api/tests/test_search.py` & `xvideos_api-1.3/xvideos_api/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `xvideos_api-1.2/xvideos_api/tests/test_video.py` & `xvideos_api-1.3/xvideos_api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `xvideos_api-1.2/xvideos_api/xvideos_api.py` & `xvideos_api-1.3/xvideos_api/xvideos_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import json
 import html
 import logging
+import argparse
 
 from bs4 import BeautifulSoup
 from functools import cached_property
 from base_api.base import Core, threaded, default, FFMPEG
 from base_api.modules.download import legacy_download
 from base_api.modules.quality import Quality
 
@@ -55,15 +56,15 @@
         :return: (str) The URL of the video, if valid, otherwise raises InvalidUrl Exception
         """
         match = REGEX_VIDEO_CHECK_URL.match(url)
         if match:
             return url
 
         else:
-            raise InvalidUrl
+            raise InvalidUrl("Invalid Video URL")
 
     @classmethod
     def is_desired_script(cls, tag):
         if tag.name != "script":
             return False
         script_contents = ['html5player', 'setVideoTitle', 'setVideoUrlLow']
         return all(content in tag.text for content in script_contents)
@@ -242,14 +243,46 @@
         return REGEX_IFRAME.search(html.unescape(self.html_content)).group(1)
 
     @cached_property
     def cdn_url(self) -> str:
         return self.json_data["contentUrl"]
 
 
+class Pornstar:
+    def __init__(self, url):
+        self.url = url
+        base_content = Core().get_content(f"{self.url}/videos/best/0").decode("utf-8")
+        self.data = json.loads(base_content)
+
+    @cached_property
+    def total_videos(self):
+        return int(self.data["nb_videos"])
+
+    @cached_property
+    def per_page(self):
+        return int(self.data["nb_per_page"])
+
+    @cached_property
+    def total_pages(self):
+        return round(self.total_videos / self.per_page)
+
+    @cached_property
+    def videos(self):
+        for idx in range(0, self.total_pages):
+            url_dynamic_javascript = Core().get_content(f"{self.url}/videos/best/{idx}").decode("utf-8")
+            data = json.loads(url_dynamic_javascript)
+
+            u_values = [video["u"] for video in data["videos"]]
+            for video in u_values:
+                url = str(video).split("/")
+                id = url[4]
+                part_two = url[5]
+                yield Video(f"https://www.xvideos.com/video.{id}/{part_two}")
+
+
 class Client:
 
     @classmethod
     def get_video(cls, url):
         """
         :param url: (str) The video URL
         :return: (Video) The video object
@@ -290,7 +323,51 @@
                 url = f"https://www.xvideos.com{url}"
 
                 if REGEX_VIDEO_CHECK_URL.match(url):
                     urls.append(url)
 
         for id in urls:
             yield Video(id)
+
+    @classmethod
+    def get_pornstar(self, url):
+        return Pornstar(url)
+
+
+def main():
+    parser = argparse.ArgumentParser(description="API Command Line Interface")
+    parser.add_argument("--download", metavar="URL (str)", type=str, help="URL to download from")
+    parser.add_argument("--quality", metavar="best,half,worst", type=str, help="The video quality (best,half,worst)",
+                        required=True)
+    parser.add_argument("--file", metavar="Source to .txt file", type=str,
+                        help="(Optional) Specify a file with URLs (separated with new lines)")
+    parser.add_argument("--output", metavar="Output directory", type=str, help="The output path (with filename)",
+                        required=True)
+    parser.add_argument("--downloader", type=str, help="The Downloader (threaded,ffmpeg,default)", required=True)
+    parser.add_argument("--use-title", metavar="True,False", type=bool,
+                        help="Whether to apply video title automatically to output path or not", required=True)
+
+    args = parser.parse_args()
+
+    if args.download:
+        client = Client()
+        video = client.get_video(args.download)
+        path = Core().return_path(args=args, video=video)
+        video.download(quality=args.quality, path=path, downloader=args.downloader)
+
+    if args.file:
+        videos = []
+        client = Client()
+
+        with open(args.file, "r") as file:
+            content = file.read().splitlines()
+
+        for url in content:
+            videos.append(client.get_video(url))
+
+        for video in videos:
+            path = Core().return_path(args=args, video=video)
+            video.download(quality=args.quality, path=path, downloader=args.downloader)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `xvideos_api-1.2/xvideos_api.egg-info/PKG-INFO` & `xvideos_api-1.3/xvideos_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xvideos_api
-Version: 1.2
+Version: 1.3
 Summary: A Python API for the Porn Site xvideos.com
 Home-page: https://github.com/EchterAlsFake/xvideos_api
 Author: Johannes Habel
 Author-email: EchterAlsFake@proton.me
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
@@ -55,14 +55,16 @@
 # Download the video
 
 video_object.download(downloader=threaded, quality=Quality.BEST, path="your_output_path + filename")
 
 # SEE DOCUMENTATION FOR MORE
 ```
 
+> [!NOTE]
+> XVideos API can also be used from the command line. Do: xvideos_api -h to see the options
 # Changelog
 See [Changelog](https://github.com/EchterAlsFake/xvideos_api/blob/master/README/Changelog.md) for more details.
 
 # Contribution
 Do you see any issues or having some feature requests? Simply open an Issue or talk
 in the discussions.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xvideos_api Version: 1.2 Summary: A Python API for
+Metadata-Version: 2.1 Name: xvideos_api Version: 1.3 Summary: A Python API for
 the Porn Site xvideos.com Home-page: https://github.com/EchterAlsFake/
 xvideos_api Author: Johannes Habel Author-email: EchterAlsFake@proton.me
 License: LGPLv3 Classifier: License :: OSI Approved :: GNU Lesser General
 Public License v3 (LGPLv3) Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: bs4 Requires-Dist: lxml Requires-Dist: ffmpeg-progress-
 yield Requires-Dist: eaf_base_api
@@ -17,13 +17,14 @@
 blob/master/README/Documentation.md) for more details - Install the library
 with `pip install xvideos_api` ```python from xvideos_api.xvideos_api import
 Client, Quality from base_api.modules.download import threaded, default, FFMPEG
 # Initialize a Client object client = Client() # Fetch a video video_object =
 client.get_video("") # Information from Video objects print(video_object.title)
 print(video_object.likes) # Download the video video_object.download
 (downloader=threaded, quality=Quality.BEST, path="your_output_path + filename")
-# SEE DOCUMENTATION FOR MORE ``` # Changelog See [Changelog](https://
-github.com/EchterAlsFake/xvideos_api/blob/master/README/Changelog.md) for more
-details. # Contribution Do you see any issues or having some feature requests?
-Simply open an Issue or talk in the discussions. Pull requests are also
-welcome. # License Licensed under the LGPLv3 License Copyright (C) 2023â2024
-Johannes Habel
+# SEE DOCUMENTATION FOR MORE ``` > [!NOTE] > XVideos API can also be used from
+the command line. Do: xvideos_api -h to see the options # Changelog See
+[Changelog](https://github.com/EchterAlsFake/xvideos_api/blob/master/README/
+Changelog.md) for more details. # Contribution Do you see any issues or having
+some feature requests? Simply open an Issue or talk in the discussions. Pull
+requests are also welcome. # License Licensed under the LGPLv3 License
+Copyright (C) 2023â2024 Johannes Habel
```

