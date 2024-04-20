# Comparing `tmp/gtsystem-0.1.3.tar.gz` & `tmp/gtsystem-0.1.4.tar.gz`

## Comparing `gtsystem-0.1.3.tar` & `gtsystem-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/__init__.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/anthropic.py
--rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/bedrock.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/benchmark.py
--rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/chat.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/groq.py
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/instrument.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/leaderboard.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/ollama.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/openai.py
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/render.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 gtsystem-0.1.3/gtsystem/tasks.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 gtsystem-0.1.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.1.3/LICENSE
--rw-r--r--   0        0        0     8350 2020-02-02 00:00:00.000000 gtsystem-0.1.3/README.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 gtsystem-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.1.4/gtsystem/__init__.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 gtsystem-0.1.4/gtsystem/anthropic.py
+-rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 gtsystem-0.1.4/gtsystem/bedrock.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 gtsystem-0.1.4/gtsystem/benchmark.py
+-rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 gtsystem-0.1.4/gtsystem/chat.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gtsystem-0.1.4/gtsystem/groq.py
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 gtsystem-0.1.4/gtsystem/instrument.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 gtsystem-0.1.4/gtsystem/leaderboard.py
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 gtsystem-0.1.4/gtsystem/ollama.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 gtsystem-0.1.4/gtsystem/openai.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 gtsystem-0.1.4/gtsystem/render.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 gtsystem-0.1.4/gtsystem/tasks.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 gtsystem-0.1.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.1.4/LICENSE
+-rw-r--r--   0        0        0     8481 2020-02-02 00:00:00.000000 gtsystem-0.1.4/README.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 gtsystem-0.1.4/PKG-INFO
```

### Comparing `gtsystem-0.1.3/gtsystem/anthropic.py` & `gtsystem-0.1.4/gtsystem/anthropic.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,37 +12,37 @@
         messages=[
             {"role": "user", "content": prompt}
         ]
     )
 
     return message.content[0].text
 
-CHAT_CONTEXT = ClaudeChat()
+CHAT = ClaudeChat()
 
 def _claude3_chat(prompt, system='', temperature=0.0, topP=1, tokens=4096, model="", image_url="", reset=False):
     if reset:
-        CHAT_CONTEXT.reset_context()
+        CHAT.reset_context()
     
     if system != "":
-        CHAT_CONTEXT.set_system(system)
+        CHAT.set_system(system)
     
     if image_url != "":
-        CHAT_CONTEXT.add_image_message(prompt=prompt, image_url=image_url)
+        CHAT.add_image_message(prompt=prompt, image_url=image_url)
     else:
-        CHAT_CONTEXT.add_message("user", prompt)
+        CHAT.add_message("user", prompt)
 
     message  = anthropic.Anthropic().messages.create(
         model=model,
-        system=CHAT_CONTEXT.get_system(),
+        system=CHAT.get_system(),
         temperature=temperature,
         top_p=topP,
         max_tokens=tokens,
-        messages=CHAT_CONTEXT.get_messages()
+        messages=CHAT.get_messages()
     )
-    CHAT_CONTEXT.add_message("assistant", message.content[0].text)
+    CHAT.add_message("assistant", message.content[0].text)
     return message.content[0].text
 
 @metrics.track
 def sonnet_chat(prompt, system='', temperature=0.0, topP=1.0, tokens=512, image_url="", reset=False):
     return _claude3_chat(prompt, system=system, 
                          temperature=temperature, topP=topP, tokens=tokens, 
                          model='claude-3-sonnet-20240229',
```

### Comparing `gtsystem-0.1.3/gtsystem/bedrock.py` & `gtsystem-0.1.4/gtsystem/bedrock.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,49 +74,49 @@
 
 def list_models(vendor):
     if BEDROCK is None:
         _init()
     listModels = BEDROCK.list_foundation_models(byProvider=vendor)
     print("\n".join(list(map(lambda x: f"{x['modelName']} : { x['modelId'] }", listModels['modelSummaries']))))
 
-CHAT_CONTEXT = ClaudeChat()
+CHAT = ClaudeChat()
 
 def _claude3_chat(prompt, system='', temperature=0.0, topP=1, tokens=4096, model="", image_url="", reset=False):
     if reset:
-        CHAT_CONTEXT.reset_context()
+        CHAT.reset_context()
     
     if system != "":
-        CHAT_CONTEXT.set_system(system)
+        CHAT.set_system(system)
     
     if image_url != "":
-        CHAT_CONTEXT.add_image_message(image_url=image_url, prompt=prompt)
+        CHAT.add_image_message(image_url=image_url, prompt=prompt)
     else:
-        CHAT_CONTEXT.add_message("user", prompt)
+        CHAT.add_message("user", prompt)
 
     try:
         if BEDROCK_RUNTIME is None:
             _init_runtime()
 
         response = BEDROCK_RUNTIME.invoke_model(
             modelId=model,
             body=json.dumps(
                 {
                     "anthropic_version": "bedrock-2023-05-31",
-                    "system": CHAT_CONTEXT.get_system(),
+                    "system": CHAT.get_system(),
                     "max_tokens": tokens,
                     "temperature": temperature,
                     "top_p": topP,
                     "max_tokens": tokens,
-                    "messages": CHAT_CONTEXT.get_messages(),
+                    "messages": CHAT.get_messages(),
                 }
             ),
         )
 
         result = json.loads(response.get('body').read())
-        CHAT_CONTEXT.add_message("assistant", result['content'][0]['text'])
+        CHAT.add_message("assistant", result['content'][0]['text'])
 
         return result['content'][0]['text']
 
     except ClientError as err:
         logger.error(
             "Couldn't invoke Claude 3. Here's why: %s: %s",
             err.response["Error"]["Code"],
```

### Comparing `gtsystem-0.1.3/gtsystem/benchmark.py` & `gtsystem-0.1.4/gtsystem/benchmark.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.3/gtsystem/chat.py` & `gtsystem-0.1.4/gtsystem/chat.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.3/gtsystem/groq.py` & `gtsystem-0.1.4/gtsystem/groq.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.3/gtsystem/instrument.py` & `gtsystem-0.1.4/gtsystem/instrument.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.3/gtsystem/leaderboard.py` & `gtsystem-0.1.4/gtsystem/leaderboard.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.3/gtsystem/ollama.py` & `gtsystem-0.1.4/gtsystem/ollama.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 import ollama
 
 from .instrument import metrics
 
 @metrics.track
-def llama_text(prompt, system='', temperature=0.0, topP=1.0, model='llama2'):
+def llama3_text(prompt, system='', temperature=0.0, topP=1.0, model='llama3'):
+    response = ollama.generate(model=model, prompt=prompt, system=system, 
+                               options={
+                                   "temperature": temperature,
+                                   "top_p": topP
+                               })
+    return response['response']
+
+@metrics.track
+def llama2_text(prompt, system='', temperature=0.0, topP=1.0, model='llama2'):
     response = ollama.generate(model=model, prompt=prompt, system=system, 
                                options={
                                    "temperature": temperature,
                                    "top_p": topP
                                })
     return response['response']
 
@@ -34,19 +43,21 @@
     response = ollama.generate(model=model, prompt=prompt, system=system, 
                                options={
                                    "temperature": temperature,
                                    "top_p": topP
                                })
     return response['response']
 
-def text(prompt, system='', temperature=0.0, topP=1.0, model='gemma'):
+def text(prompt, system='', temperature=0.0, topP=1.0, model='llama3'):
     match model:
         case 'gemma':
             return gemma_text(prompt, system, temperature, topP)
+        case 'llama3':
+            return llama3_text(prompt, system, temperature, topP)
         case 'llama2':
-            return llama_text(prompt, system, temperature, topP)
+            return llama2_text(prompt, system, temperature, topP)
         case 'codellama':
             return codellama_text(prompt, system, temperature, topP)
         case 'mistral':
             return mistral_text(prompt, system, temperature, topP)
         case _:
             return 'Please specify a valid model name'
```

### Comparing `gtsystem-0.1.3/gtsystem/openai.py` & `gtsystem-0.1.4/gtsystem/openai.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,69 @@
 from openai import OpenAI
 from .chat import GptChat
 from .instrument import metrics
+from IPython.display import clear_output
 
 OPENAI = None
 
 def init():
     global OPENAI
     OPENAI = OpenAI()
 
-CHAT_CONTEXT = GptChat()
+CHAT = GptChat()
 
-def _gpt_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", model="", reset=False):
+def _gpt_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", reset=False, stream=False, model=""):
     if OPENAI is None:
         init()
 
     if reset:
-        CHAT_CONTEXT.reset_context()
+        CHAT.reset_context()
     
     if system != "":
-        CHAT_CONTEXT.add_message("system", system)
+        CHAT.add_message("system", system)
     
     if image_url != "":
-        CHAT_CONTEXT.add_image_message(prompt=prompt, image_url=image_url)
+        CHAT.add_image_message(prompt=prompt, image_url=image_url)
     else:
-        CHAT_CONTEXT.add_message("user", prompt)
+        CHAT.add_message("user", prompt)
 
     response = OPENAI.chat.completions.create(
         model=model,
-        messages=CHAT_CONTEXT.get_messages(),
+        messages=CHAT.get_messages(),
         temperature=temperature,
         top_p=topP,
         max_tokens=tokens,
+        stream=stream
     )
-    response_text = response.choices[0].message.content.strip()
-    CHAT_CONTEXT.add_message("assistant", response_text)
+    if stream:
+        all_chunks = ""
+        for chunk in response:
+            part = chunk.choices[0].delta.content
+            if part:
+                print(part, end='')
+                all_chunks += part
+        response_text = all_chunks
+    else:
+        response_text = response.choices[0].message.content.strip()
+    CHAT.add_message("assistant", response_text)
+    clear_output()
     return response_text
 
 @metrics.track
-def gpt4_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", reset=False):
+def gpt4_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", reset=False, stream=False):
     return _gpt_chat(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, model="gpt-4-turbo", image_url=image_url, reset=reset)
+                topP=topP, tokens=tokens, image_url=image_url, reset=reset, 
+                stream=stream, model="gpt-4-turbo")
 
 @metrics.track
-def gpt3_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, reset=False):
+def gpt3_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, reset=False, stream=False):
     return _gpt_chat(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, model="gpt-3.5-turbo", reset=reset)
+                topP=topP, tokens=tokens, reset=reset, stream=stream, model="gpt-3.5-turbo")
 
-def _gpt_text(prompt, system='', temperature=0.0, topP=1, tokens=512, model=""):
+def _gpt_text(prompt, system='', temperature=0.0, topP=1, tokens=512, stream=False, model=""):
     if OPENAI is None:
         init()
 
     response = OPENAI.chat.completions.create(
         model=model,
         messages=[
             {
@@ -61,30 +74,54 @@
             "role": "user",
             "content": prompt
             }
         ],
         temperature=temperature,
         top_p=topP,
         max_tokens=tokens,
+        stream=stream
     )
-    response_text = response.choices[0].message.content.strip()
+    if stream:
+        all_chunks = ""
+        for chunk in response:
+            part = chunk.choices[0].delta.content
+            if part:
+                print(part, end='')
+                all_chunks += part
+        response_text = all_chunks
+    else:
+        response_text = response.choices[0].message.content.strip()
+    clear_output()
     return response_text
 
 @metrics.track
-def gpt3_text(prompt, system='', temperature=0.0, topP=1, tokens=512):
+def gpt3_text(prompt, system='', temperature=0.0, topP=1, tokens=512, stream=False):
     return _gpt_text(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, model="gpt-3.5-turbo")
+                topP=topP, tokens=tokens, stream=stream, model="gpt-3.5-turbo")
 
 @metrics.track
-def gpt4_text(prompt, system='', temperature=0.0, topP=1, tokens=512):
+def gpt4_text(prompt, system='', temperature=0.0, topP=1, tokens=512, stream=False):
     return _gpt_text(prompt, system=system, temperature=temperature, 
-                topP=topP, tokens=tokens, model="gpt-4-turbo-preview")
+                topP=topP, tokens=tokens, stream=stream, model="gpt-4-turbo-preview")
 
-def text(prompt, system='', temperature=0.0, topP=1, tokens=512, model="gpt4"):
+def text(prompt, system='', temperature=0.0, topP=1, tokens=512, stream=False, model="gpt4"):
     match model:
         case 'gpt3':
-            return gpt3_text(prompt, system, temperature, topP, tokens)
+            return gpt3_text(prompt, system, temperature, topP, tokens, stream)
         case 'gpt4':
-            return gpt4_text(prompt, system, temperature, topP, tokens)
+            return gpt4_text(prompt, system, temperature, topP, tokens, stream)
         case _:
             return 'Please specify a valid model name'
 
+def chat(prompt, system='', temperature=0.0, topP=1, tokens=512, reset=False, stream=False, 
+         image_url="", model="gpt4"):
+    match model:
+        case 'gpt3':
+            return gpt3_chat(prompt, system=system, temperature=temperature, 
+                topP=topP, tokens=tokens, reset=reset, 
+                stream=stream)
+        case 'gpt4':
+            return gpt4_chat(prompt, system=system, temperature=temperature, 
+                topP=topP, tokens=tokens, reset=reset, image_url=image_url,
+                stream=stream)
+        case _:
+            return 'Please specify a valid model name'
```

### Comparing `gtsystem-0.1.3/gtsystem/render.py` & `gtsystem-0.1.4/gtsystem/render.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def md(text):
     display(Markdown(text))
 
 def img(url):
     return Image(url=url)
 
-def display_base64_image(base64_string):
+def _display_base64_image(base64_string):
     image_data = base64.b64decode(base64_string)
     display(Image(data=image_data))
 
 def chat(chat_json):
     # Define role to emoji mapping
     role_emoji = {
         "system": "⚙️ ",
@@ -33,15 +33,15 @@
             text_lines = []
             for item in content:
                 if item['type'] == 'text':
                     text_lines.append(f"{role_emoji[role]}**{item['text']}**")
                 elif item['type'] == 'image_url':
                     display(Image(url=item['image_url']['url']))
                 elif item['type'] == 'image' and item['source']['type'] == 'base64':
-                    display_base64_image(item['source']['data'])
+                    _display_base64_image(item['source']['data'])
             markdown_line = '\n'.join(text_lines)
         elif role == "system":
             # System messages in italics
             markdown_line = f"{role_emoji[role]} *{content}*"
         elif role == "user":
             # Simple user messages in bold
             markdown_line = f"{role_emoji[role]}**{content}**"
```

### Comparing `gtsystem-0.1.3/.gitignore` & `gtsystem-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.3/LICENSE` & `gtsystem-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.3/README.md` & `gtsystem-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,20 @@
 
 10. **Visual chat on Anthropic:** Explore `10-chat-anthropic.ipynb` for visual chat using Anthropic hosted models.
 
 11. **Visual chat on OpenAI:** Explore `11-chat-openai.ipynb` for visual chat using OpenAI GPT4-Turbo.
 
 ## What's New
 
+### 2024-04-19 (Release 0.1.4)
+
+- Stream chat and text for OpenAI
+- openai.chat() simplifier API
+- GenAI Advisor - Trends feature
+
 ### 2024-04-17 (Release 0.1.3)
 
 - Save, list, load, and render chat for Bedrock/Claude3
 - Save, list, load, and render chat for Anthropic
 - Save, list, load, and render chat for OpenAI
 
 ### 2024-04-15 (Release 0.1.2)
```

### Comparing `gtsystem-0.1.3/pyproject.toml` & `gtsystem-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gtsystem"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="GenAI Techne", email="team@genaitechne.com" },
 ]
 description = "GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gtsystem-0.1.3/PKG-INFO` & `gtsystem-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gtsystem
-Version: 0.1.3
+Version: 0.1.4
 Summary: GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly
 Project-URL: Homepage, https://github.com/GenaiTechne/gtsystem
 Project-URL: Issues, https://github.com/GenaiTechne/gtsystem/issues
 Author-email: GenAI Techne <team@genaitechne.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Jupyter
@@ -87,14 +87,20 @@
 
 10. **Visual chat on Anthropic:** Explore `10-chat-anthropic.ipynb` for visual chat using Anthropic hosted models.
 
 11. **Visual chat on OpenAI:** Explore `11-chat-openai.ipynb` for visual chat using OpenAI GPT4-Turbo.
 
 ## What's New
 
+### 2024-04-19 (Release 0.1.4)
+
+- Stream chat and text for OpenAI
+- openai.chat() simplifier API
+- GenAI Advisor - Trends feature
+
 ### 2024-04-17 (Release 0.1.3)
 
 - Save, list, load, and render chat for Bedrock/Claude3
 - Save, list, load, and render chat for Anthropic
 - Save, list, load, and render chat for OpenAI
 
 ### 2024-04-15 (Release 0.1.2)
```

