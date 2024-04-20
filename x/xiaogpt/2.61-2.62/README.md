# Comparing `tmp/xiaogpt-2.61.tar.gz` & `tmp/xiaogpt-2.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.61.tar", last modified: Fri Apr 19 09:59:28 2024, max compression
+gzip compressed data, was "xiaogpt-2.62.tar", last modified: Sat Apr 20 03:50:28 2024, max compression
```

## Comparing `xiaogpt-2.61.tar` & `xiaogpt-2.62.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1063 2024-04-19 09:59:25.115830 xiaogpt-2.61/LICENSE
--rw-r--r--   0        0        0    22048 2024-04-19 09:59:25.115830 xiaogpt-2.61/README.md
--rw-r--r--   0        0        0     3938 2024-04-19 09:59:28.943861 xiaogpt-2.61/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/__main__.py
--rw-r--r--   0        0        0     1006 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0     1467 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3656 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     2773 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/doubao_bot.py
--rw-r--r--   0        0        0     2516 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     1944 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0     2289 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3657 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0     4696 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/cli.py
--rw-r--r--   0        0        0     6444 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      145 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     4656 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1095 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1903 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/tts/tetos.py
--rw-r--r--   0        0        0     2072 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/utils.py
--rw-r--r--   0        0        0    15821 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    28013 1970-01-01 00:00:00.000000 xiaogpt-2.61/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-20 03:50:22.151328 xiaogpt-2.62/LICENSE
+-rw-r--r--   0        0        0    22048 2024-04-20 03:50:22.151328 xiaogpt-2.62/README.md
+-rw-r--r--   0        0        0     3938 2024-04-20 03:50:28.167413 xiaogpt-2.62/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/__main__.py
+-rw-r--r--   0        0        0     1006 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0     1467 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3656 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     2773 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/bot/doubao_bot.py
+-rw-r--r--   0        0        0     2516 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1944 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0     2289 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3657 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0     4696 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/cli.py
+-rw-r--r--   0        0        0     6444 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      145 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     4656 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1095 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1903 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/tts/tetos.py
+-rw-r--r--   0        0        0     2072 2024-04-20 03:50:22.151328 xiaogpt-2.62/xiaogpt/utils.py
+-rw-r--r--   0        0        0    15826 2024-04-20 03:50:22.155328 xiaogpt-2.62/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    28013 1970-01-01 00:00:00.000000 xiaogpt-2.62/PKG-INFO
```

### Comparing `xiaogpt-2.61/LICENSE` & `xiaogpt-2.62/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/README.md` & `xiaogpt-2.62/README.md`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/pyproject.toml` & `xiaogpt-2.62/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "google-search-results>=2.4.2",
     "google-generativeai",
     "numexpr>=2.8.6",
     "dashscope>=1.10.0",
     "tetos>=0.1.1",
 ]
 dynamic = []
-version = "2.61"
+version = "2.62"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-2.61/xiaogpt/bot/__init__.py` & `xiaogpt-2.62/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/bot/base_bot.py` & `xiaogpt-2.62/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.62/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/bot/doubao_bot.py` & `xiaogpt-2.62/xiaogpt/bot/doubao_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.62/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.62/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.62/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/bot/newbing_bot.py` & `xiaogpt-2.62/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.62/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/cli.py` & `xiaogpt-2.62/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/config.py` & `xiaogpt-2.62/xiaogpt/config.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.62/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/langchain/chain.py` & `xiaogpt-2.62/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.62/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.62/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/tts/base.py` & `xiaogpt-2.62/xiaogpt/tts/base.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/tts/mi.py` & `xiaogpt-2.62/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/tts/tetos.py` & `xiaogpt-2.62/xiaogpt/tts/tetos.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/utils.py` & `xiaogpt-2.62/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.61/xiaogpt/xiaogpt.py` & `xiaogpt-2.62/xiaogpt/xiaogpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
             else:
                 print("回答完毕")
             if self.in_conversation:
                 print(f"继续对话, 或用`{self.config.end_conversation}`结束对话")
                 await self.wakeup_xiaoai()
 
     async def speak(self, text_stream: AsyncIterator[str]) -> None:
-        text = await anext(text_stream)
+        text = await text_stream.__anext__()
         # See if the first part contains language code(e.g. en-US|Hello world)
         lang, _, first_chunk = text.rpartition("|")
         if len(lang) > 7:
             # It is not a legal language code, discard it
             lang, first_chunk = "", text
 
         async def gen():  # reconstruct the generator
```

### Comparing `xiaogpt-2.61/PKG-INFO` & `xiaogpt-2.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.61
+Version: 2.62
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
```

