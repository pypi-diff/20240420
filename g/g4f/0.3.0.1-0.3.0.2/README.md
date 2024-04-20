# Comparing `tmp/g4f-0.3.0.1.tar.gz` & `tmp/g4f-0.3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.3.0.1.tar", last modified: Fri Apr 19 13:39:10 2024, max compression
+gzip compressed data, was "g4f-0.3.0.2.tar", last modified: Sat Apr 20 18:13:41 2024, max compression
```

## Comparing `g4f-0.3.0.1.tar` & `g4f-0.3.0.2.tar`

### file list

```diff
@@ -1,243 +1,244 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.041218 g4f-0.3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-19 13:39:06.000000 g4f-0.3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 13:39:06.000000 g4f-0.3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    50356 2024-04-19 13:39:10.041218 g4f-0.3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    47160 2024-04-19 13:39:06.000000 g4f-0.3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.005218 g4f-0.3.0.1/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.009218 g4f-0.3.0.1/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    21001 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Ecosia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.009218 g4f-0.3.0.1/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.017218 g4f-0.3.0.1/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.017218 g4f-0.3.0.1/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.017218 g4f-0.3.0.1/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)     8972 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/needs_auth/OpenaiAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    32305 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.021218 g4f-0.3.0.1/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.021218 g4f-0.3.0.1/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.021218 g4f-0.3.0.1/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.021218 g4f-0.3.0.1/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.021218 g4f-0.3.0.1/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/openai/har_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.025218 g4f-0.3.0.1/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.025218 g4f-0.3.0.1/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/unfinished/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.025218 g4f-0.3.0.1/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.025218 g4f-0.3.0.1/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.025218 g4f-0.3.0.1/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.029218 g4f-0.3.0.1/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.029218 g4f-0.3.0.1/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12815 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.001217 g4f-0.3.0.1/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.029218 g4f-0.3.0.1/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    22654 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.029218 g4f-0.3.0.1/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.029218 g4f-0.3.0.1/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    45680 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.029218 g4f-0.3.0.1/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.033218 g4f-0.3.0.1/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.033218 g4f-0.3.0.1/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.033218 g4f-0.3.0.1/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.033218 g4f-0.3.0.1/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.033218 g4f-0.3.0.1/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-19 13:39:06.000000 g4f-0.3.0.1/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:39:10.037218 g4f-0.3.0.1/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50356 2024-04-19 13:39:09.000000 g4f-0.3.0.1/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-19 13:39:09.000000 g4f-0.3.0.1/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:39:09.000000 g4f-0.3.0.1/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 13:39:09.000000 g4f-0.3.0.1/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-19 13:39:09.000000 g4f-0.3.0.1/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 13:39:09.000000 g4f-0.3.0.1/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:39:10.041218 g4f-0.3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-19 13:39:06.000000 g4f-0.3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.588012 g4f-0.3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-20 18:13:30.000000 g4f-0.3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-20 18:13:30.000000 g4f-0.3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    50356 2024-04-20 18:13:41.588012 g4f-0.3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    47160 2024-04-20 18:13:30.000000 g4f-0.3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.552012 g4f-0.3.0.2/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.560012 g4f-0.3.0.2/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21001 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/MetaAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.560012 g4f-0.3.0.2/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.568012 g4f-0.3.0.2/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.568012 g4f-0.3.0.2/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.568012 g4f-0.3.0.2/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8972 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32305 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.572012 g4f-0.3.0.2/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.572012 g4f-0.3.0.2/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.572012 g4f-0.3.0.2/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.572012 g4f-0.3.0.2/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.572012 g4f-0.3.0.2/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/openai/har_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.572012 g4f-0.3.0.2/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/unfinished/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    12815 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.548012 g4f-0.3.0.2/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.576012 g4f-0.3.0.2/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22655 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.580012 g4f-0.3.0.2/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.580012 g4f-0.3.0.2/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    45822 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.580012 g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.580012 g4f-0.3.0.2/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.584012 g4f-0.3.0.2/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.584012 g4f-0.3.0.2/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.584012 g4f-0.3.0.2/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.584012 g4f-0.3.0.2/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-20 18:13:30.000000 g4f-0.3.0.2/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:13:41.584012 g4f-0.3.0.2/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50356 2024-04-20 18:13:41.000000 g4f-0.3.0.2/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-20 18:13:41.000000 g4f-0.3.0.2/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:13:41.000000 g4f-0.3.0.2/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-20 18:13:41.000000 g4f-0.3.0.2/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-20 18:13:41.000000 g4f-0.3.0.2/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-20 18:13:41.000000 g4f-0.3.0.2/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:13:41.588012 g4f-0.3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-20 18:13:30.000000 g4f-0.3.0.2/setup.py
```

### Comparing `g4f-0.3.0.1/LICENSE` & `g4f-0.3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/PKG-INFO` & `g4f-0.3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.0.1
+Version: 0.3.0.2
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.0.1 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.2 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.3.0.1/README.md` & `g4f-0.3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/Aichatos.py` & `g4f-0.3.0.2/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/Aura.py` & `g4f-0.3.0.2/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/Bing.py` & `g4f-0.3.0.2/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/BingCreateImages.py` & `g4f-0.3.0.2/g4f/Provider/BingCreateImages.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from .bing.create_images import create_images, create_session, get_cookies_from_browser
 
 class BingCreateImages(AsyncGeneratorProvider, ProviderModelMixin):
     label = "Microsoft Designer"
     url = "https://www.bing.com/images/create"
     working = True
+    needs_auth = True
 
     def __init__(self, cookies: Cookies = None, proxy: str = None) -> None:
         self.cookies: Cookies = cookies
         self.proxy: str = proxy
 
     @classmethod
     async def create_async_generator(
```

### Comparing `g4f-0.3.0.1/g4f/Provider/Blackbox.py` & `g4f-0.3.0.2/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/ChatForAi.py` & `g4f-0.3.0.2/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.0.2/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/ChatgptAi.py` & `g4f-0.3.0.2/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/ChatgptFree.py` & `g4f-0.3.0.2/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/ChatgptNext.py` & `g4f-0.3.0.2/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/ChatgptX.py` & `g4f-0.3.0.2/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/Cnote.py` & `g4f-0.3.0.2/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/Cohere.py` & `g4f-0.3.0.2/g4f/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/DeepInfra.py` & `g4f-0.3.0.2/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.0.2/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.0.2/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/Ecosia.py` & `g4f-0.3.0.2/g4f/Provider/Ecosia.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,37 +11,37 @@
 from .helper import get_connector
 
 class Ecosia(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://www.ecosia.org"
     working = True
     supports_gpt_35_turbo = True
     default_model = "gpt-3.5-turbo-0125"
-    model_aliases = {"gpt-3.5-turbo": "gpt-3.5-turbo-0125"}
+    models = [default_model, "green"]
+    model_aliases = {"gpt-3.5-turbo": default_model}
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         connector: BaseConnector = None,
-        green: bool = False,
         proxy: str = None,
         **kwargs
     ) -> AsyncResult:
-        cls.get_model(model)
+        model = cls.get_model(model)
         headers = {
             "authority": "api.ecosia.org",
             "accept": "*/*",
             "origin": cls.url,
             "referer": f"{cls.url}/",
             "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36",
         }
         async with ClientSession(headers=headers, connector=get_connector(connector, proxy)) as session:
             data = {
                 "messages": base64.b64encode(json.dumps(messages).encode()).decode()
             }
-            api_url = f"https://api.ecosia.org/v2/chat/?sp={'eco' if green else 'productivity'}"
+            api_url = f"https://api.ecosia.org/v2/chat/?sp={'eco' if model == 'green' else 'productivity'}"
             async with session.post(api_url, json=data) as response:
                 await raise_for_status(response)
                 async for chunk in response.content.iter_any():
                     if chunk:
                         yield chunk.decode(errors="ignore")
```

### Comparing `g4f-0.3.0.1/g4f/Provider/Feedough.py` & `g4f-0.3.0.2/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/FlowGpt.py` & `g4f-0.3.0.2/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.0.2/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/FreeGpt.py` & `g4f-0.3.0.2/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/GeminiPro.py` & `g4f-0.3.0.2/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/GeminiProChat.py` & `g4f-0.3.0.2/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/GigaChat.py` & `g4f-0.3.0.2/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/GptTalkRu.py` & `g4f-0.3.0.2/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/HuggingChat.py` & `g4f-0.3.0.2/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/HuggingFace.py` & `g4f-0.3.0.2/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/Koala.py` & `g4f-0.3.0.2/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/Liaobots.py` & `g4f-0.3.0.2/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/Llama.py` & `g4f-0.3.0.2/g4f/Provider/Llama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/Local.py` & `g4f-0.3.0.2/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.0.2/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/Pi.py` & `g4f-0.3.0.2/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/ReplicateImage.py` & `g4f-0.3.0.2/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/Vercel.py` & `g4f-0.3.0.2/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.0.2/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/You.py` & `g4f-0.3.0.2/g4f/Provider/You.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/__init__.py` & `g4f-0.3.0.2/g4f/Provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from .GptTalkRu        import GptTalkRu
 from .HuggingChat      import HuggingChat
 from .HuggingFace      import HuggingFace
 from .Koala            import Koala
 from .Liaobots         import Liaobots
 from .Llama            import Llama
 from .Local            import Local
+from .MetaAI           import MetaAI
 from .PerplexityLabs   import PerplexityLabs
 from .Pi               import Pi
 from .ReplicateImage   import ReplicateImage
 from .Vercel           import Vercel
 from .WhiteRabbitNeo   import WhiteRabbitNeo
 from .You              import You
```

### Comparing `g4f-0.3.0.1/g4f/Provider/bing/conversation.py` & `g4f-0.3.0.2/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/bing/create_images.py` & `g4f-0.3.0.2/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/bing/upload_image.py` & `g4f-0.3.0.2/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/V50.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.0.2/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.0.2/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.0.2/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.0.2/g4f/Provider/needs_auth/Groq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from .Openai import Openai
 from ...typing import AsyncResult, Messages
 
 class Groq(Openai):
-    lebel = "Groq"
+    label = "Groq"
     url = "https://console.groq.com/playground"
     working = True
     default_model = "mixtral-8x7b-32768"
     models = ["mixtral-8x7b-32768", "llama2-70b-4096", "gemma-7b-it"]
     model_aliases = {"mixtral-8x7b": "mixtral-8x7b-32768", "llama2-70b": "llama2-70b-4096"}
 
     @classmethod
```

### Comparing `g4f-0.3.0.1/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.0.2/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.0.2/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.0.2/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.0.2/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.0.2/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.0.2/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.0.2/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.0.2/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.0.2/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.0.2/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.0.2/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.0.2/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.0.2/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.0.2/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.0.2/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.0.2/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.0.2/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.0.2/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.0.2/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.0.2/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.0.2/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.0.2/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/npm/package-lock.json` & `g4f-0.3.0.2/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/openai/crypt.py` & `g4f-0.3.0.2/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/openai/har_file.py` & `g4f-0.3.0.2/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.0.2/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/selenium/Bard.py` & `g4f-0.3.0.2/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.0.2/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.0.2/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/selenium/Phind.py` & `g4f-0.3.0.2/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.0.2/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.3.0.2/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.0.2/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.0.2/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.0.2/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/unfinished/Replicate.py` & `g4f-0.3.0.2/g4f/Provider/unfinished/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/Provider/you/har_file.py` & `g4f-0.3.0.2/g4f/Provider/you/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/__init__.py` & `g4f-0.3.0.2/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/api/__init__.py` & `g4f-0.3.0.2/g4f/api/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,99 +11,92 @@
 from typing import List, Union, Optional
 
 import g4f
 import g4f.debug
 from g4f.client import AsyncClient
 from g4f.typing import Messages
 
+app = FastAPI()
+
 class ChatCompletionsConfig(BaseModel):
     messages: Messages
     model: str
     provider: Optional[str] = None
     stream: bool = False
     temperature: Optional[float] = None
     max_tokens: Optional[int] = None
     stop: Union[list[str], str, None] = None
     api_key: Optional[str] = None
     web_search: Optional[bool] = None
+    proxy: Optional[str] = None
 
 class Api:
-    def __init__(self, engine: g4f, debug: bool = True, sentry: bool = False,
-                 list_ignored_providers: List[str] = None) -> None:
-        self.engine = engine
-        self.debug = debug
-        self.sentry = sentry
+    def __init__(self, list_ignored_providers: List[str] = None) -> None:
         self.list_ignored_providers = list_ignored_providers
-
-        if debug:
-            g4f.debug.logging = True
         self.client = AsyncClient()
-        self.app = FastAPI()
-
-        self.routes()
-        self.register_validation_exception_handler()
+    
+    def set_list_ignored_providers(self, list: list):
+        self.list_ignored_providers = list
 
     def register_validation_exception_handler(self):
-        @self.app.exception_handler(RequestValidationError)
+        @app.exception_handler(RequestValidationError)
         async def validation_exception_handler(request: Request, exc: RequestValidationError):
             details = exc.errors()
             modified_details = []
             for error in details:
-                modified_details.append(
-                    {
-                        "loc": error["loc"],
-                        "message": error["msg"],
-                        "type": error["type"],
-                    }
-                )
+                modified_details.append({
+                    "loc": error["loc"],
+                    "message": error["msg"],
+                    "type": error["type"],
+                })
             return JSONResponse(
                 status_code=HTTP_422_UNPROCESSABLE_ENTITY,
                 content=jsonable_encoder({"detail": modified_details}),
             )
 
-    def routes(self):
-        @self.app.get("/")
+    def register_routes(self):
+        @app.get("/")
         async def read_root():
             return RedirectResponse("/v1", 302)
 
-        @self.app.get("/v1")
+        @app.get("/v1")
         async def read_root_v1():
             return HTMLResponse('g4f API: Go to '
                                 '<a href="/v1/chat/completions">chat/completions</a> '
                                 'or <a href="/v1/models">models</a>.')
 
-        @self.app.get("/v1/models")
+        @app.get("/v1/models")
         async def models():
             model_list = dict(
                 (model, g4f.models.ModelUtils.convert[model])
                 for model in g4f.Model.__all__()
             )
             model_list = [{
                 'id': model_id,
                 'object': 'model',
                 'created': 0,
                 'owned_by': model.base_provider
             } for model_id, model in model_list.items()]
             return JSONResponse(model_list)
 
-        @self.app.get("/v1/models/{model_name}")
+        @app.get("/v1/models/{model_name}")
         async def model_info(model_name: str):
             try:
                 model_info = g4f.models.ModelUtils.convert[model_name]
                 return JSONResponse({
                     'id': model_name,
                     'object': 'model',
                     'created': 0,
                     'owned_by': model_info.base_provider
                 })
             except:
                 return JSONResponse({"error": "The model does not exist."})
 
-        @self.app.post("/v1/chat/completions")
-        async def chat_completions(config: ChatCompletionsConfig = None, request: Request = None, provider: str = None):
+        @app.post("/v1/chat/completions")
+        async def chat_completions(config: ChatCompletionsConfig, request: Request = None, provider: str = None):
             try:
                 config.provider = provider if config.provider is None else config.provider
                 if config.api_key is None and request is not None:
                     auth_header = request.headers.get("Authorization")
                     if auth_header is not None:
                         auth_header = auth_header.split(None, 1)[-1]
                         if auth_header and auth_header != "Bearer":
@@ -128,27 +121,39 @@
                 except Exception as e:
                     logging.exception(e)
                     yield f'data: {format_exception(e, config)}\n\n'
                 yield "data: [DONE]\n\n"
 
             return StreamingResponse(streaming(), media_type="text/event-stream")
 
-        @self.app.post("/v1/completions")
+        @app.post("/v1/completions")
         async def completions():
             return Response(content=json.dumps({'info': 'Not working yet.'}, indent=4), media_type="application/json")
 
-    def run(self, ip, use_colors : bool = False):
-        split_ip = ip.split(":")
-        uvicorn.run(app=self.app, host=split_ip[0], port=int(split_ip[1]), use_colors=use_colors)
+api = Api()
+api.register_routes()
+api.register_validation_exception_handler()
 
 def format_exception(e: Exception, config: ChatCompletionsConfig) -> str:
     last_provider = g4f.get_last_provider(True)
     return json.dumps({
         "error": {"message": f"{e.__class__.__name__}: {e}"},
         "model": last_provider.get("model") if last_provider else config.model,
         "provider": last_provider.get("name") if last_provider else config.provider
     })
 
-def run_api(host: str = '0.0.0.0', port: int = 1337, debug: bool = False, use_colors=True) -> None:
-    print(f'Starting server... [g4f v-{g4f.version.utils.current_version}]')
-    app = Api(engine=g4f, debug=debug)
-    app.run(f"{host}:{port}", use_colors=use_colors)
+def run_api(
+    host: str = '0.0.0.0',
+    port: int = 1337,
+    bind: str = None,
+    debug: bool = False,
+    workers: int = None,
+    use_colors: bool = None
+) -> None:
+    print(f'Starting server... [g4f v-{g4f.version.utils.current_version}]' + (" (debug)" if debug else ""))
+    if use_colors is None:
+        use_colors = debug
+    if bind is not None:
+        host, port = bind.split(":")
+    if debug:
+        g4f.debug.logging = True
+    uvicorn.run("g4f.api:app", host=host, port=int(port), workers=workers, use_colors=use_colors)#
```

### Comparing `g4f-0.3.0.1/g4f/api/_logging.py` & `g4f-0.3.0.2/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/cli.py` & `g4f-0.3.0.2/g4f/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import argparse
-from enum import Enum
 
-import g4f
 from g4f import Provider
-
 from g4f.gui.run import gui_parser, run_gui_args
 
-def run_gui(args):
-    print("Running GUI...")
-
 def main():
-    IgnoredProviders = Enum("ignore_providers", {key: key for key in Provider.__all__})
     parser = argparse.ArgumentParser(description="Run gpt4free")
     subparsers = parser.add_subparsers(dest="mode", help="Mode to run the g4f in.")
-    api_parser=subparsers.add_parser("api")
+    api_parser = subparsers.add_parser("api")
     api_parser.add_argument("--bind", default="0.0.0.0:1337", help="The bind string.")
-    api_parser.add_argument("--debug", type=bool, default=False, help="Enable verbose logging")
-    api_parser.add_argument("--ignored-providers", nargs="+", choices=[provider.name for provider in IgnoredProviders],
+    api_parser.add_argument("--debug", action="store_true", help="Enable verbose logging.")
+    api_parser.add_argument("--workers", type=int, default=None, help="Number of workers.")
+    api_parser.add_argument("--disable_colors", action="store_true", help="Don't use colors.")
+    api_parser.add_argument("--ignored-providers", nargs="+", choices=[provider for provider in Provider.__map__],
                             default=[], help="List of providers to ignore when processing request.")
     subparsers.add_parser("gui", parents=[gui_parser()], add_help=False)
 
     args = parser.parse_args()
     if args.mode == "api":
-        from g4f.api import Api
-        controller=Api(engine=g4f, debug=args.debug, list_ignored_providers=args.ignored_providers)
-        controller.run(args.bind)
+        import g4f.api
+        g4f.api.api.set_list_ignored_providers(
+            args.ignored_providers
+        )
+        g4f.api.run_api(
+            bind=args.bind,
+            debug=args.debug,
+            workers=args.workers,
+            use_colors=not args.disable_colors
+        )
     elif args.mode == "gui":
         run_gui_args(args)
     else:
         parser.print_help()
         exit(1)
 
 if __name__ == "__main__":
```

### Comparing `g4f-0.3.0.1/g4f/client/async_client.py` & `g4f-0.3.0.2/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/client/client.py` & `g4f-0.3.0.2/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/client/helper.py` & `g4f-0.3.0.2/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/client/image_models.py` & `g4f-0.3.0.2/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/client/service.py` & `g4f-0.3.0.2/g4f/client/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,9 +107,10 @@
     if isinstance(last, BaseRetryProvider):
         last = last.last_provider
     if last and as_dict:
         return {
             "name": last.__name__,
             "url": last.url,
             "model": debug.last_model,
+            "label": last.label if hasattr(last, "label") else None
         }
     return last
```

### Comparing `g4f-0.3.0.1/g4f/client/stubs.py` & `g4f-0.3.0.2/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/client/types.py` & `g4f-0.3.0.2/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/cookies.py` & `g4f-0.3.0.2/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/errors.py` & `g4f-0.3.0.2/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/__init__.py` & `g4f-0.3.0.2/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/client/index.html` & `g4f-0.3.0.2/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/css/style.css` & `g4f-0.3.0.2/g4f/gui/client/static/css/style.css`

 * *Files 0% similar despite different names*

```diff
@@ -886,15 +886,15 @@
     background: none;
     border: none;
     outline: none;
     color: var(--colour-3);
 
     resize: vertical;
     max-height: 200px;
-    min-height: 80px;
+    min-height: 100px;
 }
 
 /* style for hljs copy */
 .hljs-copy-wrapper {
     position: relative;
     overflow: hidden
 }
```

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.0.2/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.0.2/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.0.2/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.0.2/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.0.2/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/img/user.png` & `g4f-0.3.0.2/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.0.2/g4f/gui/client/static/js/chat.v1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -299,15 +299,15 @@
 async function add_message_chunk(message) {
     if (message.type == "conversation") {
         console.info("Conversation used:", message.conversation)
     } else if (message.type == "provider") {
         window.provider_result = message.provider;
         content.querySelector('.provider').innerHTML = `
             <a href="${message.provider.url}" target="_blank">
-                ${message.provider.name}
+                ${message.provider.label ? message.provider.label : message.provider.name}
             </a>
             ${message.provider.model ? ' with ' + message.provider.model : ''}
         `
     } else if (message.type == "message") {
         console.error(message.message)
     } else if (message.type == "error") {
         window.error = message.error
@@ -545,15 +545,16 @@
     let elements = "";
     let last_model = null;
     for (i in messages) {
         let item = messages[i];
         last_model = item.provider?.model;
         let next_i = parseInt(i) + 1;
         let next_provider = item.provider ? item.provider : (messages.length > next_i ? messages[next_i].provider : null);
-        let provider_link = item.provider?.name ? `<a href="${item.provider.url}" target="_blank">${item.provider.name}</a>` : "";
+        let provider_label = item.provider?.label ? item.provider?.label : item.provider?.name;
+        let provider_link = item.provider?.name ? `<a href="${item.provider.url}" target="_blank">${provider_label}</a>` : "";
         let provider = provider_link ? `
             <div class="provider">
                 ${provider_link}
                 ${item.provider.model ? ' with ' + item.provider.model : ''}
             </div>
         ` : "";
         elements += `
```

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.0.2/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.0.2/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/js/icons.js` & `g4f-0.3.0.2/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.0.2/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/server/android_gallery.py` & `g4f-0.3.0.2/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/server/api.py` & `g4f-0.3.0.2/g4f/gui/server/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         model = json_data.get('model') or models.default
         provider = json_data.get('provider')
         messages = json_data['messages']
         api_key = json_data.get("api_key")
         if api_key is not None:
             kwargs["api_key"] = api_key
         if json_data.get('web_search'):
-            if provider == "Bing":
+            if provider in ("Bing", "HuggingChat"):
                 kwargs['web_search'] = True
             else:
                 from .internet import get_search_message
                 messages[-1]["content"] = get_search_message(messages[-1]["content"])
 
         conversation_id = json_data.get("conversation_id")
         if conversation_id and provider in conversations and conversation_id in conversations[provider]:
```

### Comparing `g4f-0.3.0.1/g4f/gui/server/backend.py` & `g4f-0.3.0.2/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/server/config.py` & `g4f-0.3.0.2/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/server/internet.py` & `g4f-0.3.0.2/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/server/js_api.py` & `g4f-0.3.0.2/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/server/website.py` & `g4f-0.3.0.2/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/gui/webview.py` & `g4f-0.3.0.2/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/image.py` & `g4f-0.3.0.2/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/local/__init__.py` & `g4f-0.3.0.2/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/locals/models.py` & `g4f-0.3.0.2/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/locals/provider.py` & `g4f-0.3.0.2/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/models.py` & `g4f-0.3.0.2/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/providers/base_provider.py` & `g4f-0.3.0.2/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/providers/create_images.py` & `g4f-0.3.0.2/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/providers/helper.py` & `g4f-0.3.0.2/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/providers/retry_provider.py` & `g4f-0.3.0.2/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/providers/types.py` & `g4f-0.3.0.2/g4f/providers/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,8 +98,15 @@
     supports_stream: bool = True
     last_provider: Type[BaseProvider] = None
 
 ProviderType = Union[Type[BaseProvider], BaseRetryProvider]
 
 class FinishReason():
     def __init__(self, reason: str):
-        self.reason = reason
+        self.reason = reason
+
+class Streaming():
+    def __init__(self, data: str) -> None:
+        self.data = data
+
+    def __str__(self) -> str:
+        return self.data
```

### Comparing `g4f-0.3.0.1/g4f/requests/__init__.py` & `g4f-0.3.0.2/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/requests/aiohttp.py` & `g4f-0.3.0.2/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/requests/curl_cffi.py` & `g4f-0.3.0.2/g4f/requests/curl_cffi.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,18 +75,18 @@
     ) -> StreamResponse:
         if isinstance(kwargs.get("data"), CurlMime):
             kwargs["multipart"] = kwargs.pop("data")
         """Create and return a StreamResponse object for the given HTTP request."""
         return StreamResponse(super().request(method, url, stream=True, **kwargs))
 
     def ws_connect(self, url, *args, **kwargs):
-        return WebSocket(self, url)
+        return WebSocket(self, url, **kwargs)
 
-    def _ws_connect(self, url):
-        return super().ws_connect(url)
+    def _ws_connect(self, url, **kwargs):
+        return super().ws_connect(url, **kwargs)
 
     # Defining HTTP methods as partial methods of the request method.
     head = partialmethod(request, "HEAD")
     get = partialmethod(request, "GET")
     post = partialmethod(request, "POST")
     put = partialmethod(request, "PUT")
     patch = partialmethod(request, "PATCH")
@@ -98,26 +98,28 @@
             self.addpart(name, content_type=content_type, filename=filename, data=data)
 else:
     class FormData():
         def __init__(self) -> None:
             raise RuntimeError("CurlMimi in curl_cffi is missing | pip install -U g4f[curl_cffi]")
 
 class WebSocket():
-    def __init__(self, session, url) -> None:
+    def __init__(self, session, url, **kwargs) -> None:
         if not has_curl_ws:
             raise RuntimeError("CurlWsFlag in curl_cffi is missing | pip install -U g4f[curl_cffi]")
         self.session: StreamSession = session
         self.url: str = url
+        del kwargs["autoping"]
+        self.options: dict = kwargs
 
     async def __aenter__(self):
-        self.inner = await self.session._ws_connect(self.url)
+        self.inner = await self.session._ws_connect(self.url, **self.options)
         return self
 
     async def __aexit__(self, *args):
-        self.inner.aclose()
+        await self.inner.aclose()
 
-    async def receive_str(self) -> str:
+    async def receive_str(self, **kwargs) -> str:
         bytes, _ = await self.inner.arecv()
         return bytes.decode(errors="ignore")
 
     async def send_str(self, data: str):
         await self.inner.asend(data.encode(), CurlWsFlag.TEXT)
```

### Comparing `g4f-0.3.0.1/g4f/requests/defaults.py` & `g4f-0.3.0.2/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/requests/raise_for_status.py` & `g4f-0.3.0.2/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/stubs.py` & `g4f-0.3.0.2/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/typing.py` & `g4f-0.3.0.2/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/version.py` & `g4f-0.3.0.2/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/g4f/webdriver.py` & `g4f-0.3.0.2/g4f/webdriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         proxy (str, optional): Proxy settings for the browser. Defaults to None.
         options (ChromeOptions, optional): ChromeOptions object with specific browser options. Defaults to None.
 
     Returns:
         WebDriver: An instance of WebDriver configured with the specified options.
     """
     if not has_requirements:
-        raise MissingRequirementsError('Webdriver packages are not installed | pip install -U g4f[webdriver]')
+        raise MissingRequirementsError('Install Webdriver packages | pip install -U g4f[webdriver]')
     browser = find_chrome_executable()
     if browser is None:
         raise MissingRequirementsError('Install "Google Chrome" browser')
     if user_data_dir is None:
         user_data_dir = user_config_dir("g4f")
     if user_data_dir and debug.logging:
         print("Open browser with config dir:", user_data_dir)
```

### Comparing `g4f-0.3.0.1/g4f.egg-info/PKG-INFO` & `g4f-0.3.0.2/g4f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.0.1
+Version: 0.3.0.2
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.0.1 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.2 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.3.0.1/g4f.egg-info/SOURCES.txt` & `g4f-0.3.0.2/g4f.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 g4f/Provider/GptTalkRu.py
 g4f/Provider/HuggingChat.py
 g4f/Provider/HuggingFace.py
 g4f/Provider/Koala.py
 g4f/Provider/Liaobots.py
 g4f/Provider/Llama.py
 g4f/Provider/Local.py
+g4f/Provider/MetaAI.py
 g4f/Provider/PerplexityLabs.py
 g4f/Provider/Pi.py
 g4f/Provider/ReplicateImage.py
 g4f/Provider/Vercel.py
 g4f/Provider/WhiteRabbitNeo.py
 g4f/Provider/You.py
 g4f/Provider/__init__.py
```

### Comparing `g4f-0.3.0.1/g4f.egg-info/requires.txt` & `g4f-0.3.0.2/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.1/setup.py` & `g4f-0.3.0.2/setup.py`

 * *Files identical despite different names*

