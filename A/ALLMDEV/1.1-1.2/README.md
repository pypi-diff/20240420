# Comparing `tmp/ALLMDEV-1.1-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 4346 bytes, number of entries: 8
+Zip file size: 5553 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
+-rw-rw-rw-  2.0 fat     2034 b- defN 24-Apr-19 13:18 ALLMDEV/api.py
 -rw-rw-rw-  2.0 fat      757 b- defN 24-Apr-17 06:35 ALLMDEV/cli.py
--rw-rw-rw-  2.0 fat    10332 b- defN 24-Apr-17 15:17 ALLMDEV/instruct.py
--rw-rw-rw-  2.0 fat     1995 b- defN 24-Apr-17 15:21 ALLMDEV-1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-17 15:21 ALLMDEV-1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       46 b- defN 24-Apr-17 15:21 ALLMDEV-1.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-17 15:21 ALLMDEV-1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      603 b- defN 24-Apr-17 15:21 ALLMDEV-1.1.dist-info/RECORD
-8 files, 13872 bytes uncompressed, 3296 bytes compressed:  76.2%
+-rw-rw-rw-  2.0 fat    10394 b- defN 24-Apr-19 06:20 ALLMDEV/instruct.py
+-rw-rw-rw-  2.0 fat     2354 b- defN 24-Apr-19 13:20 ALLMDEV-1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-19 13:20 ALLMDEV-1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       76 b- defN 24-Apr-19 13:20 ALLMDEV-1.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-19 13:20 ALLMDEV-1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      674 b- defN 24-Apr-19 13:20 ALLMDEV-1.2.dist-info/RECORD
+9 files, 16428 bytes uncompressed, 4399 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: ALLMDEV/__init__.py
 Comment: 
 
+Filename: ALLMDEV/api.py
+Comment: 
+
 Filename: ALLMDEV/cli.py
 Comment: 
 
 Filename: ALLMDEV/instruct.py
 Comment: 
 
-Filename: ALLMDEV-1.1.dist-info/METADATA
+Filename: ALLMDEV-1.2.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.1.dist-info/WHEEL
+Filename: ALLMDEV-1.2.dist-info/WHEEL
 Comment: 
 
-Filename: ALLMDEV-1.1.dist-info/entry_points.txt
+Filename: ALLMDEV-1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLMDEV-1.1.dist-info/top_level.txt
+Filename: ALLMDEV-1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLMDEV-1.1.dist-info/RECORD
+Filename: ALLMDEV-1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ALLMDEV/instruct.py

```diff
@@ -165,13 +165,15 @@
                 # Perform inference
                 response_iter = llm.stream_complete(prompt)
                 # print("ALLM:", end='')
                 
                 # Print the assistant's response
                 for response in response_iter:
                     print(response.delta, end="", flush=True)
+                    return response
+                print()
             except KeyboardInterrupt:
                 print("\nExiting...")
                 break
```

## Comparing `ALLMDEV-1.1.dist-info/METADATA` & `ALLMDEV-1.2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ALLMDEV
-Version: 1.1
+Version: 1.2
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Soham Ghadge
 Maintainer-email: soham.ghadge@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
+Requires-Dist: Flask
 Requires-Dist: click
 Requires-Dist: llama-index
 Requires-Dist: llama-cpp-python
 Requires-Dist: aiohttp
 Requires-Dist: llama-index-llms-llama-cpp
 Requires-Dist: huggingface-hub
 
@@ -37,10 +38,24 @@
 ## Usage
 
 You can start inference with a simple 'allm-run' command. The command takes name or path, temperature(optional), max new tokens(optional) and additional model kwargs(optional) as arguments.
 
 ```bash
 allm-run --name model_name_or_path
 ```
+
+## API
+
+After initialising or downloading the model you can start inference API with a simple 'allm-serve' command. The command takes host and port as optional arguments, if not provided, the API will run on the default 127.0.0.1:5000 host.
+
+```bash
+allm-serve
+```
+
+```bash
+allm-serve --host 192.168.0.1 --port 8000
+```
+
+
 ## Supported Model names
 Llama2, llama, llama2_chat, Llama_chat, Mistral, Mistral_instruct
```

## Comparing `ALLMDEV-1.1.dist-info/RECORD` & `ALLMDEV-1.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ALLMDEV/__init__.py,sha256=8XSO2SVH9cZ_Iut8rNwcDxtEaBp4LIdXP6hAKGRgeaI,39
+ALLMDEV/api.py,sha256=GLAgApGFlOh9daU6OhR8NjWgy3M4G9DHUrYjhQa8RDc,2034
 ALLMDEV/cli.py,sha256=wWOt7Uv_DmQKT821rEIaEVh9MFJVz0n19BXgwTHsdDY,757
-ALLMDEV/instruct.py,sha256=P-8bzeYoF6huaYFq2kN0NDOZfB_U7nxYEKelNWmgdaM,10332
-ALLMDEV-1.1.dist-info/METADATA,sha256=Gan9JLBJTswKcIXjWTos1zeos9lZI-1MIQ-foIarRZY,1995
-ALLMDEV-1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ALLMDEV-1.1.dist-info/entry_points.txt,sha256=ekZkHoIao3UZTqmxa3h99Cdve_c5t9CG4FiqORIsjN4,46
-ALLMDEV-1.1.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
-ALLMDEV-1.1.dist-info/RECORD,,
+ALLMDEV/instruct.py,sha256=RVxJJhwlGy7q2a3NgwPZi35qB9wnll5Yf2ifDGJ1unQ,10394
+ALLMDEV-1.2.dist-info/METADATA,sha256=vCDKyn_dOu8fHEk0hUn7fcCHnXbx7IQTz8EzGwdv0Vg,2354
+ALLMDEV-1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ALLMDEV-1.2.dist-info/entry_points.txt,sha256=He_WB4819TTsETEoQ7J82TTyF1qChfyKmGNAR6evCy0,76
+ALLMDEV-1.2.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
+ALLMDEV-1.2.dist-info/RECORD,,
```

