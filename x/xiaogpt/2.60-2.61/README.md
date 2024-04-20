# Comparing `tmp/xiaogpt-2.60.tar.gz` & `tmp/xiaogpt-2.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.60.tar", last modified: Thu Apr 18 13:20:09 2024, max compression
+gzip compressed data, was "xiaogpt-2.61.tar", last modified: Fri Apr 19 09:59:28 2024, max compression
```

## Comparing `xiaogpt-2.60.tar` & `xiaogpt-2.61.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1063 2024-04-18 13:20:05.908612 xiaogpt-2.60/LICENSE
--rw-r--r--   0        0        0    20871 2024-04-18 13:20:05.912612 xiaogpt-2.60/README.md
--rw-r--r--   0        0        0     3938 2024-04-18 13:20:09.456638 xiaogpt-2.60/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/__main__.py
--rw-r--r--   0        0        0      919 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0     1467 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3656 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1840 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     1944 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0     2289 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3657 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0     4409 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/cli.py
--rw-r--r--   0        0        0     5896 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      145 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     4656 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1095 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1903 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/tts/tetos.py
--rw-r--r--   0        0        0     2072 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/utils.py
--rw-r--r--   0        0        0    15821 2024-04-18 13:20:05.912612 xiaogpt-2.60/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    26836 1970-01-01 00:00:00.000000 xiaogpt-2.60/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-19 09:59:25.115830 xiaogpt-2.61/LICENSE
+-rw-r--r--   0        0        0    22048 2024-04-19 09:59:25.115830 xiaogpt-2.61/README.md
+-rw-r--r--   0        0        0     3938 2024-04-19 09:59:28.943861 xiaogpt-2.61/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/__main__.py
+-rw-r--r--   0        0        0     1006 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0     1467 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3656 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     2773 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/doubao_bot.py
+-rw-r--r--   0        0        0     2516 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1944 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0     2289 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3657 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0     4696 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/cli.py
+-rw-r--r--   0        0        0     6444 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-04-19 09:59:25.115830 xiaogpt-2.61/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      145 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     4656 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1095 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1903 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/tts/tetos.py
+-rw-r--r--   0        0        0     2072 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/utils.py
+-rw-r--r--   0        0        0    15821 2024-04-19 09:59:25.119830 xiaogpt-2.61/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    28013 1970-01-01 00:00:00.000000 xiaogpt-2.61/PKG-INFO
```

### Comparing `xiaogpt-2.60/LICENSE` & `xiaogpt-2.61/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/README.md` & `xiaogpt-2.61/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 xiaogpt --hardware LX06 --account ${your_xiaomi_account} --password ${your_password} --use_chatgpt_api
 # 如果你想 mute 小米的回答
 xiaogpt --hardware LX06  --mute_xiaoai --use_chatgpt_api
 # 使用流式响应，获得更快的响应
 xiaogpt --hardware LX06  --mute_xiaoai --stream
 # 如果你想使用 google 的 gemini
 xiaogpt --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key}
+# 如果你想使用自己的 google gemini 服务
+python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key} --gemini_api_domain ${gemini_api_domain}
 # 如果你想使用阿里的通义千问
 xiaogpt --hardware LX06  --mute_xiaoai --use_qwen --qen_key ${qwen_key}
 # 如果你想用 edge-tts
 xiaogpt --hardware LX06 --cookie ${cookie} --use_chatgpt_api --tts edge
 # 如果你想使用 LangChain + SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
@@ -97,14 +99,16 @@
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai
 # 使用流式响应，获得更快的响应
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --stream
 # 如果你想使用 ChatGLM api
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_glm --glm_key ${glm_key}
 # 如果你想使用 google 的 gemini
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key}
+# 如果你想使用自己的 google gemini 服务
+python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key} --gemini_api_domain ${gemini_api_domain}
 # 如果你想使用阿里的通义千问
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_qwen --qen_key ${qwen_key}
 # 如果你想使用 LangChain+SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
 python3 xiaogpt.py --hardware Lx06 --use_langchain --mute_xiaoai --stream --openai_key ${your_api_key} --serpapi_api_key ${your_serpapi_key}
 ```
@@ -151,14 +155,15 @@
 | hardware              | 设备型号                                                                                    |                                                                                                           |                                                       |
 | account               | 小爱账户                                                                                    |                                                                                                           |                                                       |
 | password              | 小爱账户密码                                                                                |                                                                                                           |                                                       |
 | openai_key            | openai的apikey                                                                              |                                                                                                           |                                                       |
 | serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                       |
 | glm_key               | chatglm 的 apikey                                                                           |                                                                                                           |                                                       |
 | gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                       |
+| gemini_api_domain            | gemini 的自定义域名 [参考](https://github.com/antergone/palm-netlify-proxy)                                                      |                                                                                                           |
 | qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                       |
 | cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                       |
 | mi_did                | 设备did                                                                                     |                                                                                                           |                                                       |
 | use_command           | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                       |
 | mute_xiaoai           | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                       |
 | verbose               | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                       |
 | bot                   | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                  | `chatgptapi`                                                                                              |                                                       |
@@ -171,17 +176,17 @@
 | end_conversation      | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                       |
 | stream                | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                       |
 | proxy                 | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                       |
 | gpt_options           | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                       |
 | bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                       |
 | bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                       |
 | deployment_id         | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                       |
-| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |                                                       |
-
-
+| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 | 
+| volc_access_key       | 火山引擎的 access key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                       |
+| volc_secret_key       | 火山引擎的 secret key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                       |
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
 3. 目前已知 LX04、X10A 和 L05B L05C 可能需要使用 `--use_command`，否则可能会出现终端能输出GPT的回复但小爱同学不回答GPT的情况。这几个型号也只支持小爱原本的 tts.
```

### Comparing `xiaogpt-2.60/pyproject.toml` & `xiaogpt-2.61/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     "EdgeGPT==0.1.26",
     "langchain>=0.0.343",
     "beautifulsoup4>=4.12.0",
     "google-search-results>=2.4.2",
     "google-generativeai",
     "numexpr>=2.8.6",
     "dashscope>=1.10.0",
-    "tetos>=0.1.0",
+    "tetos>=0.1.1",
 ]
 dynamic = []
-version = "2.60"
+version = "2.61"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
 
@@ -116,15 +116,15 @@
     "rich==13.7.1",
     "rsa==4.9",
     "sniffio==1.3.0",
     "socksio==1.0.0",
     "soupsieve==2.5",
     "sqlalchemy==2.0.25",
     "tenacity==8.2.3",
-    "tetos==0.1.0",
+    "tetos==0.1.1",
     "tqdm==4.66.1",
     "typing-extensions==4.9.0",
     "typing-inspect==0.9.0",
     "uritemplate==4.1.1",
     "urllib3==2.1.0",
     "wcwidth==0.2.13",
     "websockets==12.0",
```

### Comparing `xiaogpt-2.60/xiaogpt/bot/__init__.py` & `xiaogpt-2.61/xiaogpt/bot/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 
 from xiaogpt.bot.base_bot import BaseBot
 from xiaogpt.bot.chatgptapi_bot import ChatGPTBot
-from xiaogpt.bot.newbing_bot import NewBingBot
-from xiaogpt.bot.glm_bot import GLMBot
+from xiaogpt.bot.doubao_bot import DoubaoBot
 from xiaogpt.bot.gemini_bot import GeminiBot
-from xiaogpt.bot.qwen_bot import QwenBot
+from xiaogpt.bot.glm_bot import GLMBot
 from xiaogpt.bot.langchain_bot import LangChainBot
+from xiaogpt.bot.newbing_bot import NewBingBot
+from xiaogpt.bot.qwen_bot import QwenBot
 from xiaogpt.config import Config
 
 BOTS: dict[str, type[BaseBot]] = {
     "newbing": NewBingBot,
     "chatgptapi": ChatGPTBot,
     "glm": GLMBot,
     "gemini": GeminiBot,
     "qwen": QwenBot,
     "langchain": LangChainBot,
+    "doubao": DoubaoBot,
 }
 
 
 def get_bot(config: Config) -> BaseBot:
     try:
         return BOTS[config.bot].from_config(config)
     except KeyError:
@@ -30,8 +32,9 @@
     "ChatGPTBot",
     "NewBingBot",
     "GLMBot",
     "GeminiBot",
     "QwenBot",
     "get_bot",
     "LangChainBot",
+    "DoubaoBot",
 ]
```

### Comparing `xiaogpt-2.60/xiaogpt/bot/base_bot.py` & `xiaogpt-2.61/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.61/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.61/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.61/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/bot/newbing_bot.py` & `xiaogpt-2.61/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.61/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/cli.py` & `xiaogpt-2.61/xiaogpt/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,19 @@
     )
     parser.add_argument(
         "--gemini_key",
         dest="gemini_key",
         help="gemini api key",
     )
     parser.add_argument(
+        "--gemini_api_domain",
+        dest="gemini_api_domain",
+        help="custom gemini api domain",
+    )
+    parser.add_argument(
         "--qwen_key",
         dest="qwen_key",
         help="Alibaba Qwen api key",
     )
     parser.add_argument(
         "--serpapi_api_key",
         dest="serpapi_api_key",
@@ -74,14 +79,16 @@
     parser.add_argument(
         "--mute_xiaoai",
         dest="mute_xiaoai",
         action="store_true",
         default=None,
         help="try to mute xiaoai answer",
     )
+    parser.add_argument("--volc-access-key", help="Volcengine access key")
+    parser.add_argument("--volc-secret-key", help="Volcengine secret key")
     parser.add_argument(
         "--verbose",
         dest="verbose",
         action="store_true",
         default=None,
         help="show info",
     )
```

### Comparing `xiaogpt-2.60/xiaogpt/config.py` & `xiaogpt-2.61/xiaogpt/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,19 @@
     account: str = os.getenv("MI_USER", "")
     password: str = os.getenv("MI_PASS", "")
     openai_key: str = os.getenv("OPENAI_API_KEY", "")
     glm_key: str = os.getenv("CHATGLM_KEY", "")
     gemini_key: str = os.getenv("GEMINI_KEY", "")  # keep the old rule
     qwen_key: str = os.getenv("DASHSCOPE_API_KEY", "")  # keep the old rule
     serpapi_api_key: str = os.getenv("SERPAPI_API_KEY", "")
+    gemini_api_domain: str = os.getenv(
+        "GEMINI_API_DOMAIN", ""
+    )  # 自行部署的 Google Gemini 代理
+    volc_access_key: str = os.getenv("VOLC_ACCESS_KEY", "")
+    volc_secret_key: str = os.getenv("VOLC_SECRET_KEY", "")
     proxy: str | None = None
     mi_did: str = os.getenv("MI_DID", "")
     keyword: Iterable[str] = KEY_WORD
     change_prompt_keyword: Iterable[str] = CHANGE_PROMPT_KEY_WORD
     prompt: str = PROMPT
     mute_xiaoai: bool = False
     bot: str = "chatgptapi"
@@ -113,14 +118,21 @@
     def from_options(cls, options: argparse.Namespace) -> Config:
         config = {}
         if options.config:
             config = cls.read_from_file(options.config)
         for key, value in vars(options).items():
             if value is not None and key in cls.__dataclass_fields__:
                 config[key] = value
+        if config.get("tts") == "volc":
+            config.setdefault("tts_options", {}).setdefault(
+                "access_key", config.get("volc_access_key")
+            )
+            config.setdefault("tts_options", {}).setdefault(
+                "secret_key", config.get("volc_secret_key")
+            )
         return cls(**config)
 
     @classmethod
     def read_from_file(cls, config_path: str) -> dict:
         result = {}
         with open(config_path, "rb") as f:
             config = json.load(f)
```

### Comparing `xiaogpt-2.60/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.61/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/langchain/chain.py` & `xiaogpt-2.61/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.61/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.61/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/tts/base.py` & `xiaogpt-2.61/xiaogpt/tts/base.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/tts/mi.py` & `xiaogpt-2.61/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/tts/tetos.py` & `xiaogpt-2.61/xiaogpt/tts/tetos.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/utils.py` & `xiaogpt-2.61/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/xiaogpt/xiaogpt.py` & `xiaogpt-2.61/xiaogpt/xiaogpt.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.60/PKG-INFO` & `xiaogpt-2.61/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.60
+Version: 2.61
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
@@ -18,15 +18,15 @@
 Requires-Dist: EdgeGPT==0.1.26
 Requires-Dist: langchain>=0.0.343
 Requires-Dist: beautifulsoup4>=4.12.0
 Requires-Dist: google-search-results>=2.4.2
 Requires-Dist: google-generativeai
 Requires-Dist: numexpr>=2.8.6
 Requires-Dist: dashscope>=1.10.0
-Requires-Dist: tetos>=0.1.0
+Requires-Dist: tetos>=0.1.1
 Requires-Dist: aiohttp==3.9.5; extra == "locked"
 Requires-Dist: aiosignal==1.3.1; extra == "locked"
 Requires-Dist: annotated-types==0.6.0; extra == "locked"
 Requires-Dist: anyio==4.3.0; extra == "locked"
 Requires-Dist: async-timeout==4.0.3; python_version < "3.11" and extra == "locked"
 Requires-Dist: attrs==23.2.0; extra == "locked"
 Requires-Dist: azure-cognitiveservices-speech==1.37.0; extra == "locked"
@@ -98,15 +98,15 @@
 Requires-Dist: rich==13.7.1; extra == "locked"
 Requires-Dist: rsa==4.9; extra == "locked"
 Requires-Dist: sniffio==1.3.0; extra == "locked"
 Requires-Dist: socksio==1.0.0; extra == "locked"
 Requires-Dist: soupsieve==2.5; extra == "locked"
 Requires-Dist: sqlalchemy==2.0.25; extra == "locked"
 Requires-Dist: tenacity==8.2.3; extra == "locked"
-Requires-Dist: tetos==0.1.0; extra == "locked"
+Requires-Dist: tetos==0.1.1; extra == "locked"
 Requires-Dist: tqdm==4.66.1; extra == "locked"
 Requires-Dist: typing-extensions==4.9.0; extra == "locked"
 Requires-Dist: typing-inspect==0.9.0; extra == "locked"
 Requires-Dist: uritemplate==4.1.1; extra == "locked"
 Requires-Dist: urllib3==2.1.0; extra == "locked"
 Requires-Dist: wcwidth==0.2.13; extra == "locked"
 Requires-Dist: websockets==12.0; extra == "locked"
@@ -187,14 +187,16 @@
 xiaogpt --hardware LX06 --account ${your_xiaomi_account} --password ${your_password} --use_chatgpt_api
 # 如果你想 mute 小米的回答
 xiaogpt --hardware LX06  --mute_xiaoai --use_chatgpt_api
 # 使用流式响应，获得更快的响应
 xiaogpt --hardware LX06  --mute_xiaoai --stream
 # 如果你想使用 google 的 gemini
 xiaogpt --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key}
+# 如果你想使用自己的 google gemini 服务
+python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key} --gemini_api_domain ${gemini_api_domain}
 # 如果你想使用阿里的通义千问
 xiaogpt --hardware LX06  --mute_xiaoai --use_qwen --qen_key ${qwen_key}
 # 如果你想用 edge-tts
 xiaogpt --hardware LX06 --cookie ${cookie} --use_chatgpt_api --tts edge
 # 如果你想使用 LangChain + SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
@@ -214,14 +216,16 @@
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai
 # 使用流式响应，获得更快的响应
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --stream
 # 如果你想使用 ChatGLM api
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_glm --glm_key ${glm_key}
 # 如果你想使用 google 的 gemini
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key}
+# 如果你想使用自己的 google gemini 服务
+python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key} --gemini_api_domain ${gemini_api_domain}
 # 如果你想使用阿里的通义千问
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_qwen --qen_key ${qwen_key}
 # 如果你想使用 LangChain+SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
 python3 xiaogpt.py --hardware Lx06 --use_langchain --mute_xiaoai --stream --openai_key ${your_api_key} --serpapi_api_key ${your_serpapi_key}
 ```
@@ -268,14 +272,15 @@
 | hardware              | 设备型号                                                                                    |                                                                                                           |                                                       |
 | account               | 小爱账户                                                                                    |                                                                                                           |                                                       |
 | password              | 小爱账户密码                                                                                |                                                                                                           |                                                       |
 | openai_key            | openai的apikey                                                                              |                                                                                                           |                                                       |
 | serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                       |
 | glm_key               | chatglm 的 apikey                                                                           |                                                                                                           |                                                       |
 | gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                       |
+| gemini_api_domain            | gemini 的自定义域名 [参考](https://github.com/antergone/palm-netlify-proxy)                                                      |                                                                                                           |
 | qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                       |
 | cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                       |
 | mi_did                | 设备did                                                                                     |                                                                                                           |                                                       |
 | use_command           | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                       |
 | mute_xiaoai           | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                       |
 | verbose               | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                       |
 | bot                   | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                  | `chatgptapi`                                                                                              |                                                       |
@@ -288,17 +293,17 @@
 | end_conversation      | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                       |
 | stream                | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                       |
 | proxy                 | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                       |
 | gpt_options           | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                       |
 | bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                       |
 | bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                       |
 | deployment_id         | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                       |
-| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |                                                       |
-
-
+| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 | 
+| volc_access_key       | 火山引擎的 access key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                       |
+| volc_secret_key       | 火山引擎的 secret key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                       |
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
 3. 目前已知 LX04、X10A 和 L05B L05C 可能需要使用 `--use_command`，否则可能会出现终端能输出GPT的回复但小爱同学不回答GPT的情况。这几个型号也只支持小爱原本的 tts.
```

