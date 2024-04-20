# Comparing `tmp/kellyapi-0.0.1.7.tar.gz` & `tmp/kellyapi-0.0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kellyapi-0.0.1.7.tar", last modified: Thu Apr 18 19:15:42 2024, max compression
+gzip compressed data, was "kellyapi-0.0.1.8.tar", last modified: Sat Apr 20 03:37:55 2024, max compression
```

## Comparing `kellyapi-0.0.1.7.tar` & `kellyapi-0.0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:15:42.363669 kellyapi-0.0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-18 19:15:38.000000 kellyapi-0.0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-18 19:15:42.363669 kellyapi-0.0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-18 19:15:38.000000 kellyapi-0.0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:15:42.359668 kellyapi-0.0.1.7/kellyapi/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 19:15:38.000000 kellyapi-0.0.1.7/kellyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-04-18 19:15:38.000000 kellyapi-0.0.1.7/kellyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-18 19:15:38.000000 kellyapi-0.0.1.7/kellyapi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:15:42.363669 kellyapi-0.0.1.7/kellyapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-18 19:15:42.000000 kellyapi-0.0.1.7/kellyapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-18 19:15:42.000000 kellyapi-0.0.1.7/kellyapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:15:42.000000 kellyapi-0.0.1.7/kellyapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 19:15:42.000000 kellyapi-0.0.1.7/kellyapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 19:15:42.000000 kellyapi-0.0.1.7/kellyapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:15:42.363669 kellyapi-0.0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-18 19:15:38.000000 kellyapi-0.0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:37:55.436704 kellyapi-0.0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-20 03:37:50.000000 kellyapi-0.0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-20 03:37:55.436704 kellyapi-0.0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-20 03:37:50.000000 kellyapi-0.0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:37:55.432704 kellyapi-0.0.1.8/kellyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-20 03:37:50.000000 kellyapi-0.0.1.8/kellyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-20 03:37:50.000000 kellyapi-0.0.1.8/kellyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-20 03:37:50.000000 kellyapi-0.0.1.8/kellyapi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:37:55.436704 kellyapi-0.0.1.8/kellyapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-20 03:37:55.000000 kellyapi-0.0.1.8/kellyapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-20 03:37:55.000000 kellyapi-0.0.1.8/kellyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 03:37:55.000000 kellyapi-0.0.1.8/kellyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-20 03:37:55.000000 kellyapi-0.0.1.8/kellyapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 03:37:55.000000 kellyapi-0.0.1.8/kellyapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 03:37:55.436704 kellyapi-0.0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-20 03:37:50.000000 kellyapi-0.0.1.8/setup.py
```

### Comparing `kellyapi-0.0.1.7/LICENSE` & `kellyapi-0.0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1.7/PKG-INFO` & `kellyapi-0.0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.1.7
+Version: 0.0.1.8
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.1.7/README.md` & `kellyapi-0.0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1.7/kellyapi/api.py` & `kellyapi-0.0.1.8/kellyapi/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -96,23 +96,23 @@
             raise InvalidContent
         except ClientConnectorError:
             raise ConnectionError
         return response
 
     async def sd_models(self):
         content = await self._fetch("sd-models")
-        return content.models
+        return content
 
     async def sdxl_models(self):
         content = await self._fetch("sdxl-models")
-        return content.models
+        return content
 
     async def get_styles(self):
         content = await self._fetch("styles")
-        return content.styles
+        return content
 
     async def generate(
         self,
         prompt: str,
         negative_prompt: str = None,
         model: str = "DreamShaper",
         style: str = "cinematic",
@@ -128,15 +128,15 @@
             height=height,
         )
         content = await self._post_data("generate", data=kwargs)
         return content
 
     async def llm_models(self):
         content = await self._fetch("llm-models")
-        return content.models
+        return content
 
     async def llm(self, prompt: str, model: str = "ChatGPT", character: str = "KelyAI"):
         kwargs = dict(prompt=prompt, model=model, character=character)
         content = await self._post_json("llm", data=kwargs)
         return content.message
 
     async def upscale(self, image: str):
@@ -147,15 +147,15 @@
     async def rmbg(self, image: str):
         kwargs = dict(image=image)
         content = await self._post_data("rmbg", data=kwargs)
         return content
 
     async def voice_models(self):
         content = await self._fetch("voice-models")
-        return content.models
+        return content
 
     async def text2voice(self, text: str, model: str = "en-US_LisaExpressive"):
         kwargs = dict(text=text, model=model)
         content = await self._post_data("text2voice", data=kwargs)
         return content
 
     async def voice2text(self, audio: str):
```

### Comparing `kellyapi-0.0.1.7/kellyapi/errors.py` & `kellyapi-0.0.1.8/kellyapi/errors.py`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1.7/kellyapi.egg-info/PKG-INFO` & `kellyapi-0.0.1.8/kellyapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.1.7
+Version: 0.0.1.8
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.1.7/setup.py` & `kellyapi-0.0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="kellyapi",
     packages=setuptools.find_packages(),
-    version="0.0.1.7",
+    version="0.0.1.8",
     license="MIT",
     description="A Project Made To Centralize Various APIs 📖 No Authorization Needed :)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="NotReallyPrince",
     author_email="princebots3011@gmail.com",
     url="https://github.com/NotReallyPrince/Prince-Api",
```

