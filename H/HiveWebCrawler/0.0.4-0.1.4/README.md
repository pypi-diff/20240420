# Comparing `tmp/hivewebcrawler-0.0.4.tar.gz` & `tmp/hivewebcrawler-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivewebcrawler-0.0.4.tar", last modified: Mon Apr 15 15:20:34 2024, max compression
+gzip compressed data, was "hivewebcrawler-0.1.4.tar", last modified: Sat Apr 20 13:32:44 2024, max compression
```

## Comparing `hivewebcrawler-0.0.4.tar` & `hivewebcrawler-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 15:20:34.755711 hivewebcrawler-0.0.4/
-drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 15:20:34.751711 hivewebcrawler-0.0.4/HiveWebCrawler/
--rw-r--r--   0 delta     (1000) delta     (1000)    12384 2024-04-15 09:46:49.000000 hivewebcrawler-0.0.4/HiveWebCrawler/Crawler.py
--rw-r--r--   0 delta     (1000) delta     (1000)       24 2024-04-15 12:55:31.000000 hivewebcrawler-0.0.4/HiveWebCrawler/__init__.py
-drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 15:20:34.755711 hivewebcrawler-0.0.4/HiveWebCrawler.egg-info/
--rw-r--r--   0 delta     (1000) delta     (1000)     5934 2024-04-15 15:20:34.000000 hivewebcrawler-0.0.4/HiveWebCrawler.egg-info/PKG-INFO
--rw-r--r--   0 delta     (1000) delta     (1000)      273 2024-04-15 15:20:34.000000 hivewebcrawler-0.0.4/HiveWebCrawler.egg-info/SOURCES.txt
--rw-r--r--   0 delta     (1000) delta     (1000)        1 2024-04-15 15:20:34.000000 hivewebcrawler-0.0.4/HiveWebCrawler.egg-info/dependency_links.txt
--rw-r--r--   0 delta     (1000) delta     (1000)       24 2024-04-15 15:20:34.000000 hivewebcrawler-0.0.4/HiveWebCrawler.egg-info/requires.txt
--rw-r--r--   0 delta     (1000) delta     (1000)       15 2024-04-15 15:20:34.000000 hivewebcrawler-0.0.4/HiveWebCrawler.egg-info/top_level.txt
--rw-r--r--   0 delta     (1000) delta     (1000)     5934 2024-04-15 15:20:34.755711 hivewebcrawler-0.0.4/PKG-INFO
--rw-r--r--   0 delta     (1000) delta     (1000)     5274 2024-04-15 15:19:37.000000 hivewebcrawler-0.0.4/README.md
--rw-r--r--   0 delta     (1000) delta     (1000)       38 2024-04-15 15:20:34.755711 hivewebcrawler-0.0.4/setup.cfg
--rw-r--r--   0 delta     (1000) delta     (1000)      981 2024-04-15 15:20:11.000000 hivewebcrawler-0.0.4/setup.py
-drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-15 15:20:34.755711 hivewebcrawler-0.0.4/test/
--rw-r--r--   0 delta     (1000) delta     (1000)      559 2024-04-15 13:15:46.000000 hivewebcrawler-0.0.4/test/test.py
+drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-20 13:32:44.709672 hivewebcrawler-0.1.4/
+drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-20 13:32:44.705672 hivewebcrawler-0.1.4/HiveWebCrawler/
+-rw-r--r--   0 delta     (1000) delta     (1000)    15738 2024-04-20 13:27:46.000000 hivewebcrawler-0.1.4/HiveWebCrawler/Crawler.py
+-rw-r--r--   0 delta     (1000) delta     (1000)       24 2024-04-15 12:55:31.000000 hivewebcrawler-0.1.4/HiveWebCrawler/__init__.py
+drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-20 13:32:44.709672 hivewebcrawler-0.1.4/HiveWebCrawler.egg-info/
+-rw-r--r--   0 delta     (1000) delta     (1000)     6086 2024-04-20 13:32:44.000000 hivewebcrawler-0.1.4/HiveWebCrawler.egg-info/PKG-INFO
+-rw-r--r--   0 delta     (1000) delta     (1000)      273 2024-04-20 13:32:44.000000 hivewebcrawler-0.1.4/HiveWebCrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 delta     (1000) delta     (1000)        1 2024-04-20 13:32:44.000000 hivewebcrawler-0.1.4/HiveWebCrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 delta     (1000) delta     (1000)       31 2024-04-20 13:32:44.000000 hivewebcrawler-0.1.4/HiveWebCrawler.egg-info/requires.txt
+-rw-r--r--   0 delta     (1000) delta     (1000)       15 2024-04-20 13:32:44.000000 hivewebcrawler-0.1.4/HiveWebCrawler.egg-info/top_level.txt
+-rw-r--r--   0 delta     (1000) delta     (1000)     6086 2024-04-20 13:32:44.709672 hivewebcrawler-0.1.4/PKG-INFO
+-rw-r--r--   0 delta     (1000) delta     (1000)     5404 2024-04-20 13:32:20.000000 hivewebcrawler-0.1.4/README.md
+-rw-r--r--   0 delta     (1000) delta     (1000)       38 2024-04-20 13:32:44.709672 hivewebcrawler-0.1.4/setup.cfg
+-rw-r--r--   0 delta     (1000) delta     (1000)      990 2024-04-20 13:30:19.000000 hivewebcrawler-0.1.4/setup.py
+drwxr-xr-x   0 delta     (1000) delta     (1000)        0 2024-04-20 13:32:44.709672 hivewebcrawler-0.1.4/test/
+-rw-r--r--   0 delta     (1000) delta     (1000)      559 2024-04-15 13:15:46.000000 hivewebcrawler-0.1.4/test/test.py
```

### Comparing `hivewebcrawler-0.0.4/HiveWebCrawler/Crawler.py` & `hivewebcrawler-0.1.4/HiveWebCrawler/Crawler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from bs4 import BeautifulSoup
 import requests
-
+from urllib.parse import urlparse
 """
             Prime Security | ThiHive @ WebCrawler 
 
 Version         :   __VERSION__
 Author          :   __AUTHOR__
 
 """
@@ -12,20 +12,20 @@
 
 __VERSION__ = "0.0.1"
 __AUTHOR__ = "Prime Security"
 
 class WebCrawler():    
     def __init__(self) -> None:
         self.HREF_BLACKLIST = [
-            "javascript:;", "_banlk", "__blank"
+            "javascript:;", "_banlk", "__blank","#","javascript:__doPostBack","javascript:void(0);"
         ]    
     
         self.IMAGE_BLACKLIST = ["data:image/svg+xml;",]
         self.IMAGE_EXTENSION_BLACKLIST = [".svg"]
-        
+        self.IMAGE_LINK_EXTENSIONS = [".png",".jpg",".jpeg",".webm",".tiff",".psd",".eps",".raw"]
         
         
     def prepare_string(self, target_str:str) -> str:
         first_numeric_detected = False
         detected_data = ""
         
         for single_char in target_str:
@@ -72,15 +72,17 @@
 
         if detected_data[0:4].lower() != "tel:":
             return [False, "No phone in string"]
         
         detected_data = detected_data.lower()
         detected_data = detected_data.replace("tel:","")
         detected_data = detected_data.replace(" ","")
-        
+        detected_data = detected_data.replace("(","")
+        detected_data = detected_data.replace(")","")
+            
         if len(detected_data) == 0:
             return [False, "No phone in string"]
 
         return [True, detected_data]
     
     def crawl_email_address_from_response_href(self,response_text:str) -> dict:
 
@@ -214,16 +216,28 @@
             if href_target is not None:
                 if href_target.startswith("/"):
                     href_target = original_target_url + href_target[1:]
         
                 if only_address:
                     href_target = href_target.split("?")
                     href_target = href_target[0]
-                    
-            
+                
+                if href_target.startswith("www."):
+                    href_target = "https://" + href_target
+
+                if href_target.startswith("#"):
+                    href_target = None
+                
+
+                analysed_url = urlparse(href_target)
+                
+                
+                if not analysed_url.scheme and href_target != None:
+                    href_target = original_target_url + href_target
+                
             if href_target is not None:
                 results_dict["data_array"].append( [ href_target, href_title ])
 
         if len(results_dict["data_array"]) == 0:
             results_dict["success"] = False
             results_dict["message"] = "No link detected in url"
         else:
@@ -340,19 +354,94 @@
                 exluce_parser = image_url
                 if "?" in image_url:
                     exluce_parser = image_url.split("?")
                     exluce_parser = exluce_parser[0]
                 if exluce_parser.endswith(".svg")  or "data:image/svg+xml;" in exluce_parser:
                     image_url = None
                     
-                
+            
             if image_url is not None:
+                if image_url.startswith("/"):
+                    image_url = original_url + image_url[1:]
                 
+                if image_url.startswith("www."):
+                    image_url = "https://" + image_url
+
+                if image_url.startswith("#"):
+                    image_url = None
+                
+                analysed_url = urlparse(image_url)
+                
+                
+                if not analysed_url.scheme and image_url != None:
+                    image_url = original_url + image_url
+
+
+
+            if image_url is not None:    
                 results_dict["data_array"].append( [ image_url, image_alt, image_title ])
 
+
+        # Direct image link detections ( Direcyory index etc..)
+        
+        for single_link in soup_data.select("a"):
+            
+            href_target = None
+            href_title = None
+            
+            if "href" in single_link.attrs.keys():
+                check_href_target = single_link.attrs["href"]
+                if not self.is_null(check_href_target) and check_href_target not in self.HREF_BLACKLIST:
+                    href_target = check_href_target
+            
+            if "title" in single_link.attrs.keys():
+                check_href_title = single_link.attrs["title"]
+                if not self.is_null(check_href_title):
+                    href_title = check_href_title
+
+            if href_target is not None:
+                if href_target.startswith("/"):
+                    href_target = original_url + href_target[1:]
+        
+                
+                href_target = href_target.split("?")
+                href_target = href_target[0]
+                
+                if href_target.startswith("www."):
+                    href_target = "https://" + href_target
+
+                if href_target.startswith("#"):
+                    href_target = None
+                
+
+                analysed_url = urlparse(href_target)
+                
+                
+                if not analysed_url.scheme and href_target != None:
+                    href_target = original_url + href_target
+            
+            
+            if href_target is not None:
+                for extensions in self.IMAGE_LINK_EXTENSIONS:
+                    if href_target.lower().endswith(extensions):
+                        results_dict["data_array"].append( [ href_target, href_title ])
+                        break
+
+        if len(results_dict["data_array"]) == 0:
+            results_dict["success"] = False
+            results_dict["message"] = "No link detected in url"
+        else:
+            results_dict["success"] = True
+            results_dict["message"] = "Proccess successfuly"
+        return results_dict
+        
+
+
+
+
         results_dict["success"] = True
 
         return results_dict
 
 
 
 if __name__ =="__main__":
```

### Comparing `hivewebcrawler-0.0.4/HiveWebCrawler.egg-info/PKG-INFO` & `hivewebcrawler-0.1.4/HiveWebCrawler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: HiveWebCrawler
-Version: 0.0.4
+Version: 0.1.4
 Summary: Python 3.x Web Crawler, Images, Urls, Emails, Phone numbers
 Home-page: https://github.com/MehmetYukselSekeroglu/HiveWebCrawler
 Author: MehmetYukselSekeroglu
 Author-email: dijital_evren@protonmail.com
 Project-URL: Bug Reports, https://github.com/MehmetYukselSekeroglu/HiveWebCrawler/issues
 Project-URL: Source Code, https://github.com/MehmetYukselSekeroglu/HiveWebCrawler
 Keywords: PyPi,Web Crawler,Web Image Crawler,Web URL Crawler,Web Email Crawler,Web Phone Number Crawler
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
+Requires-Dist: urllib
 
 # How To Install
 
 `pip install HiveWebCrawler`
 
 
+# v0.1.4 News
+
+- With v0.1.4, erroneous scraping scenarios have been significantly reduced.
+- Image scraping has been improved.
+
+
 # Example:
 
 ## Sending requests:
 
 ```python
 # Code
 from HiveWebCrawler.Crawler import WebCrawler
```

### Comparing `hivewebcrawler-0.0.4/PKG-INFO` & `hivewebcrawler-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: HiveWebCrawler
-Version: 0.0.4
+Version: 0.1.4
 Summary: Python 3.x Web Crawler, Images, Urls, Emails, Phone numbers
 Home-page: https://github.com/MehmetYukselSekeroglu/HiveWebCrawler
 Author: MehmetYukselSekeroglu
 Author-email: dijital_evren@protonmail.com
 Project-URL: Bug Reports, https://github.com/MehmetYukselSekeroglu/HiveWebCrawler/issues
 Project-URL: Source Code, https://github.com/MehmetYukselSekeroglu/HiveWebCrawler
 Keywords: PyPi,Web Crawler,Web Image Crawler,Web URL Crawler,Web Email Crawler,Web Phone Number Crawler
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
+Requires-Dist: urllib
 
 # How To Install
 
 `pip install HiveWebCrawler`
 
 
+# v0.1.4 News
+
+- With v0.1.4, erroneous scraping scenarios have been significantly reduced.
+- Image scraping has been improved.
+
+
 # Example:
 
 ## Sending requests:
 
 ```python
 # Code
 from HiveWebCrawler.Crawler import WebCrawler
```

### Comparing `hivewebcrawler-0.0.4/README.md` & `hivewebcrawler-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # How To Install
 
 `pip install HiveWebCrawler`
 
 
+# v0.1.4 News
+
+- With v0.1.4, erroneous scraping scenarios have been significantly reduced.
+- Image scraping has been improved.
+
+
 # Example:
 
 ## Sending requests:
 
 ```python
 # Code
 from HiveWebCrawler.Crawler import WebCrawler
```

### Comparing `hivewebcrawler-0.0.4/setup.py` & `hivewebcrawler-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 with open('README.md','r') as readmeFile:
     long_describe = readmeFile.read()
 
 setuptools.setup(
     name='HiveWebCrawler',
     author='MehmetYukselSekeroglu',
-    version='0.0.4',
+    version='0.1.4',
     author_email='dijital_evren@protonmail.com',
     description='Python 3.x Web Crawler, Images, Urls, Emails, Phone numbers',
     long_description=long_describe,
     long_description_content_type=long_describe_format,
     keywords='PyPi, Web Crawler, Web Image Crawler, Web URL Crawler, Web Email Crawler, Web Phone Number Crawler',
     project_urls={
         'Bug Reports':'https://github.com/MehmetYukselSekeroglu/HiveWebCrawler/issues',
         'Source Code':'https://github.com/MehmetYukselSekeroglu/HiveWebCrawler'
     },
     url='https://github.com/MehmetYukselSekeroglu/HiveWebCrawler',
     packages=setuptools.find_packages(),
     python_requires='>=3.8',
-    install_requires=['requests','beautifulsoup4'], 
+    install_requires=['requests','beautifulsoup4','urllib'], 
 )
```

### Comparing `hivewebcrawler-0.0.4/test/test.py` & `hivewebcrawler-0.1.4/test/test.py`

 * *Files identical despite different names*

