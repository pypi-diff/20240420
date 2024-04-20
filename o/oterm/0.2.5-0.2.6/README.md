# Comparing `tmp/oterm-0.2.5.tar.gz` & `tmp/oterm-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oterm-0.2.5.tar", max compression
+gzip compressed data, was "oterm-0.2.6.tar", max compression
```

## Comparing `oterm-0.2.5.tar` & `oterm-0.2.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1064 2024-04-02 09:23:57.938553 oterm-0.2.5/LICENSE
--rw-r--r--   0        0        0     3802 2024-04-02 09:23:57.938553 oterm-0.2.5/README.md
--rw-r--r--   0        0        0        0 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/__init__.py
--rw-r--r--   0        0        0     7129 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/chat_edit.py
--rw-r--r--   0        0        0     1593 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/chat_export.py
--rw-r--r--   0        0        0      734 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/chat_rename.py
--rw-r--r--   0        0        0     2313 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/image_browser.py
--rw-r--r--   0        0        0     3238 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/oterm.py
--rw-r--r--   0        0        0     3239 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/oterm.tcss
--rw-r--r--   0        0        0     1058 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/prompt_history.py
--rw-r--r--   0        0        0     1947 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/splash.py
--rw-r--r--   0        0        0       46 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/widgets/__init__.py
--rw-r--r--   0        0        0     9680 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/widgets/chat.py
--rw-r--r--   0        0        0     1823 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/widgets/image.py
--rw-r--r--   0        0        0      627 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/widgets/monkey.py
--rw-r--r--   0        0        0     5569 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/widgets/prompt.py
--rw-r--r--   0        0        0      879 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/app/widgets/text_area.py
--rw-r--r--   0        0        0        0 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/cli/__init__.py
--rw-r--r--   0        0        0      724 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/cli/oterm.py
--rw-r--r--   0        0        0     3135 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/config.py
--rw-r--r--   0        0        0     1651 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/ollama.py
--rw-r--r--   0        0        0        0 2024-04-02 09:23:57.938553 oterm-0.2.5/oterm/store/__init__.py
--rw-r--r--   0        0        0      892 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/chat.py
--rw-r--r--   0        0        0      572 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/setup.py
--rw-r--r--   0        0        0     5769 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/store.py
--rw-r--r--   0        0        0      359 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/upgrades/__init__.py
--rw-r--r--   0        0        0      574 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/upgrades/v0_1_11.py
--rw-r--r--   0        0        0      514 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/upgrades/v0_1_6.py
--rw-r--r--   0        0        0      522 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/upgrades/v0_2_0.py
--rw-r--r--   0        0        0      533 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/store/upgrades/v0_2_4.py
--rw-r--r--   0        0        0     1408 2024-04-02 09:23:57.942553 oterm-0.2.5/oterm/utils.py
--rw-r--r--   0        0        0     2040 2024-04-02 09:23:57.942553 oterm-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     5246 1970-01-01 00:00:00.000000 oterm-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-20 06:48:32.686512 oterm-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3798 2024-04-20 06:48:32.686512 oterm-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/__init__.py
+-rw-r--r--   0        0        0     7129 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/chat_edit.py
+-rw-r--r--   0        0        0     1593 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/chat_export.py
+-rw-r--r--   0        0        0      734 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/chat_rename.py
+-rw-r--r--   0        0        0     2313 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/image_browser.py
+-rw-r--r--   0        0        0     3244 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/oterm.py
+-rw-r--r--   0        0        0     3239 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/oterm.tcss
+-rw-r--r--   0        0        0     1058 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/prompt_history.py
+-rw-r--r--   0        0        0     1947 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/splash.py
+-rw-r--r--   0        0        0       46 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/widgets/__init__.py
+-rw-r--r--   0        0        0     9680 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/widgets/chat.py
+-rw-r--r--   0        0        0     1823 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/widgets/image.py
+-rw-r--r--   0        0        0      627 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/widgets/monkey.py
+-rw-r--r--   0        0        0     5569 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/widgets/prompt.py
+-rw-r--r--   0        0        0      879 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/widgets/text_area.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/cli/__init__.py
+-rw-r--r--   0        0        0      724 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/cli/oterm.py
+-rw-r--r--   0        0        0     3131 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/config.py
+-rw-r--r--   0        0        0     1763 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/ollama.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/__init__.py
+-rw-r--r--   0        0        0      892 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/chat.py
+-rw-r--r--   0        0        0      572 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/setup.py
+-rw-r--r--   0        0        0     5769 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/store.py
+-rw-r--r--   0        0        0      359 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/upgrades/__init__.py
+-rw-r--r--   0        0        0      574 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/upgrades/v0_1_11.py
+-rw-r--r--   0        0        0      514 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/upgrades/v0_1_6.py
+-rw-r--r--   0        0        0      522 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/upgrades/v0_2_0.py
+-rw-r--r--   0        0        0      533 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/upgrades/v0_2_4.py
+-rw-r--r--   0        0        0     1408 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/utils.py
+-rw-r--r--   0        0        0     2040 2024-04-20 06:48:32.690512 oterm-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 oterm-0.2.6/PKG-INFO
```

### Comparing `oterm-0.2.5/LICENSE` & `oterm-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/README.md` & `oterm-0.2.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 ```bash
 pip install oterm
 ```
 
 ## Using
 
-In order to use `oterm` you will need to have the Ollama server running. By default it expects to find the Ollama API running on `http://0.0.0.0:11434/api`. If you are running Ollama inside docker or on a different host/port, use the `OLLAMA_HOST` environment variable to customize the host/port. Alternatively you can use `OLLAMA_URL` to specify the full http(s) url. Setting `OTERM_VERIFY_SSL` to `False` will disable SSL verification.
+In order to use `oterm` you will need to have the Ollama server running. By default it expects to find the Ollama API running on `http://0.0.0.0:11434`. If you are running Ollama inside docker or on a different host/port, use the `OLLAMA_HOST` environment variable to customize the host/port. Alternatively you can use `OLLAMA_URL` to specify the full http(s) url. Setting `OTERM_VERIFY_SSL` to `False` will disable SSL verification.
 
 ```bash
 OLLAMA_URL=http://host:port/api
 ```
 
 The following keyboard shortcuts are supported:
```

### Comparing `oterm-0.2.5/oterm/app/chat_edit.py` & `oterm-0.2.6/oterm/app/chat_edit.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/app/chat_export.py` & `oterm-0.2.6/oterm/app/chat_export.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/app/chat_rename.py` & `oterm-0.2.6/oterm/app/chat_rename.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/app/image_browser.py` & `oterm-0.2.6/oterm/app/image_browser.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/app/oterm.py` & `oterm-0.2.6/oterm/app/oterm.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                     chat_name=name,
                     model=model["name"],
                     system=model["system"],
                     format=model["format"],
                     messages=[],
                 )
             )
-            tabs.add_pane(pane)
+            await tabs.add_pane(pane)
             tabs.active = f"chat-{id}"
 
         self.push_screen(ChatEdit(), on_model_select)
 
     async def on_mount(self) -> None:
         self.store = await Store.create()
         self.dark = appConfig.get("theme") == "dark"
```

### Comparing `oterm-0.2.5/oterm/app/oterm.tcss` & `oterm-0.2.6/oterm/app/oterm.tcss`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/app/prompt_history.py` & `oterm-0.2.6/oterm/app/prompt_history.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/app/splash.py` & `oterm-0.2.6/oterm/app/splash.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/app/widgets/chat.py` & `oterm-0.2.6/oterm/app/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/app/widgets/image.py` & `oterm-0.2.6/oterm/app/widgets/image.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/app/widgets/monkey.py` & `oterm-0.2.6/oterm/app/widgets/monkey.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/app/widgets/prompt.py` & `oterm-0.2.6/oterm/app/widgets/prompt.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/app/widgets/text_area.py` & `oterm-0.2.6/oterm/app/widgets/text_area.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/cli/oterm.py` & `oterm-0.2.6/oterm/cli/oterm.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/config.py` & `oterm-0.2.6/oterm/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             except ValueError:
                 raise EnvConfigError(
                     'Unable to cast value of "{}" to type "{}" for "{}" field'.format(
                         env[field], var_type, field  # type: ignore
                     )
                 )
         if self.OLLAMA_URL == "":
-            self.OLLAMA_URL = f"http://{self.OLLAMA_HOST}/api"
+            self.OLLAMA_URL = f"http://{self.OLLAMA_HOST}"
 
     def __repr__(self):
         return str(self.__dict__)
 
 
 # Expose EnvConfig object for app to import
 envConfig = EnvConfig(os.environ)
```

### Comparing `oterm-0.2.5/oterm/ollama.py` & `oterm-0.2.6/oterm/ollama.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,30 +15,34 @@
     ):
         self.model = model
         self.system = system
         self.context = context
         self.format = format
 
     async def completion(self, prompt: str, images: list[str] = []) -> str:
-        client = AsyncClient(host=envConfig.OLLAMA_HOST)
+        client = AsyncClient(
+            host=envConfig.OLLAMA_URL, verify=envConfig.OTERM_VERIFY_SSL
+        )
         response: dict = await client.generate(
             model=self.model,
             prompt=prompt,
             context=self.context,
             system=self.system,  # type: ignore
             format=self.format,  # type: ignore
             images=images,
         )
         self.context = response.get("context", [])
         return response.get("response", "")
 
     async def stream(
         self, prompt: str, images: list[str] = []
     ) -> AsyncGenerator[str, Any]:
-        client = AsyncClient(host=envConfig.OLLAMA_HOST)
+        client = AsyncClient(
+            host=envConfig.OLLAMA_URL, verify=envConfig.OTERM_VERIFY_SSL
+        )
         stream: AsyncIterator[dict] = await client.generate(
             model=self.model,
             prompt=prompt,
             context=self.context,
             system=self.system,  # type: ignore
             format=self.format,  # type: ignore
             images=images,
```

### Comparing `oterm-0.2.5/oterm/store/chat.py` & `oterm-0.2.6/oterm/store/chat.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/store/setup.py` & `oterm-0.2.6/oterm/store/setup.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/store/store.py` & `oterm-0.2.6/oterm/store/store.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/store/upgrades/v0_1_11.py` & `oterm-0.2.6/oterm/store/upgrades/v0_1_11.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/store/upgrades/v0_1_6.py` & `oterm-0.2.6/oterm/store/upgrades/v0_1_6.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/store/upgrades/v0_2_0.py` & `oterm-0.2.6/oterm/store/upgrades/v0_2_0.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/store/upgrades/v0_2_4.py` & `oterm-0.2.6/oterm/store/upgrades/v0_2_4.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/oterm/utils.py` & `oterm-0.2.6/oterm/utils.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.5/pyproject.toml` & `oterm-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oterm"
-version = "0.2.5"
+version = "0.2.6"
 description = "A text-based terminal client for Ollama."
 authors = ["Yiorgis Gozadinos <ggozadinos@gmail.com>"]
 homepage = "https://github.com/ggozad/oterm"
 repository = "https://github.com/ggozad/oterm"
 license = "MIT"
 readme = "README.md"
 classifiers = [
```

### Comparing `oterm-0.2.5/PKG-INFO` & `oterm-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oterm
-Version: 0.2.5
+Version: 0.2.6
 Summary: A text-based terminal client for Ollama.
 Home-page: https://github.com/ggozad/oterm
 License: MIT
 Author: Yiorgis Gozadinos
 Author-email: ggozadinos@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -58,15 +58,15 @@
 
 ```bash
 pip install oterm
 ```
 
 ## Using
 
-In order to use `oterm` you will need to have the Ollama server running. By default it expects to find the Ollama API running on `http://0.0.0.0:11434/api`. If you are running Ollama inside docker or on a different host/port, use the `OLLAMA_HOST` environment variable to customize the host/port. Alternatively you can use `OLLAMA_URL` to specify the full http(s) url. Setting `OTERM_VERIFY_SSL` to `False` will disable SSL verification.
+In order to use `oterm` you will need to have the Ollama server running. By default it expects to find the Ollama API running on `http://0.0.0.0:11434`. If you are running Ollama inside docker or on a different host/port, use the `OLLAMA_HOST` environment variable to customize the host/port. Alternatively you can use `OLLAMA_URL` to specify the full http(s) url. Setting `OTERM_VERIFY_SSL` to `False` will disable SSL verification.
 
 ```bash
 OLLAMA_URL=http://host:port/api
 ```
 
 The following keyboard shortcuts are supported:
```

