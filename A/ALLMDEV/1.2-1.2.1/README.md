# Comparing `tmp/ALLMDEV-1.2-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 5553 bytes, number of entries: 9
+Zip file size: 6736 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
--rw-rw-rw-  2.0 fat     2034 b- defN 24-Apr-19 13:18 ALLMDEV/api.py
+-rw-rw-rw-  2.0 fat     1904 b- defN 24-Apr-20 05:31 ALLMDEV/api.py
 -rw-rw-rw-  2.0 fat      757 b- defN 24-Apr-17 06:35 ALLMDEV/cli.py
--rw-rw-rw-  2.0 fat    10394 b- defN 24-Apr-19 06:20 ALLMDEV/instruct.py
--rw-rw-rw-  2.0 fat     2354 b- defN 24-Apr-19 13:20 ALLMDEV-1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-19 13:20 ALLMDEV-1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       76 b- defN 24-Apr-19 13:20 ALLMDEV-1.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-19 13:20 ALLMDEV-1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      674 b- defN 24-Apr-19 13:20 ALLMDEV-1.2.dist-info/RECORD
-9 files, 16428 bytes uncompressed, 4399 bytes compressed:  73.2%
+-rw-rw-rw-  2.0 fat     2416 b- defN 24-Apr-20 10:05 ALLMDEV/generate.py
+-rw-rw-rw-  2.0 fat    10334 b- defN 24-Apr-19 14:10 ALLMDEV/instruct.py
+-rw-rw-rw-  2.0 fat     2372 b- defN 24-Apr-20 10:05 ALLMDEV-1.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-20 10:05 ALLMDEV-1.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       81 b- defN 24-Apr-20 10:05 ALLMDEV-1.2.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-20 10:05 ALLMDEV-1.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      760 b- defN 24-Apr-20 10:05 ALLMDEV-1.2.1.dist-info/RECORD
+10 files, 18763 bytes uncompressed, 5448 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -3,26 +3,29 @@
 
 Filename: ALLMDEV/api.py
 Comment: 
 
 Filename: ALLMDEV/cli.py
 Comment: 
 
+Filename: ALLMDEV/generate.py
+Comment: 
+
 Filename: ALLMDEV/instruct.py
 Comment: 
 
-Filename: ALLMDEV-1.2.dist-info/METADATA
+Filename: ALLMDEV-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.2.dist-info/WHEEL
+Filename: ALLMDEV-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: ALLMDEV-1.2.dist-info/entry_points.txt
+Filename: ALLMDEV-1.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLMDEV-1.2.dist-info/top_level.txt
+Filename: ALLMDEV-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLMDEV-1.2.dist-info/RECORD
+Filename: ALLMDEV-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ALLMDEV/api.py

```diff
@@ -8,58 +8,52 @@
 parser.add_argument("--host", type=str, default="127.0.0.1", help="Host on which you wish to run the API server")
 parser.add_argument("--port", type=str, default='5000', help="Host on which you wish to run the API server")
 
 app = Flask(__name__)
 app.config['DEBUG'] = False
 
 model_files = [f for f in os.listdir('model') if f.endswith('.gguf')]
-model_path = load_model(model_files[0])
+model_path = load_model(model_files[0]) if model_files else None
 
 def generate(model):
-    prompt_template = "<s>[INST] {prompt} [/INST]"
     llm = LlamaCPP(
             model_path=model,
             temperature=0.5,
             max_new_tokens=512,
             context_window=3900,
-            # model_kwargs=model_kwargs,
             verbose=False,
         )
     return llm
 
 def infer(llm, prompt):
-    prompt_template = "<s>[INST] {prompt} [/INST]"
-    prompt = prompt_template.format(prompt=prompt)
-    response = llm.complete(prompt)
-    return str(response)
-
+    if prompt.lower() == "exit":
+        return "Exiting chat."
+    response_iter = llm.stream_complete(prompt)
+    response_text = ''.join(response.delta for response in response_iter)
+    return response_text
 
 @app.route('/')
 def index():
     return "Welcome to the allmdev API!"
 
 @app.route('/v1/chat/completions', methods=['POST'])
 def infer_text():
-    data = request.json
-    user_input = data.get('user_input')
-    
-    # Verify if the model is loaded and initialized
-    # Assuming load_model() returns the model path if it's loaded and None otherwise
+    user_input = request.data.decode('utf-8')
+    print("Received input:", user_input)  # Debug statement
+
     if model_path is None:
-        return jsonify({"error": "Model is not loaded or initialized. Kindly run 'allm-run --name model_name_or_path' to initialize the model"})
+        return "Model is not loaded or initialized. Kindly run 'allm-run --name model_name_or_path' to initialize the model"
 
-    # Perform inference
-    llm=generate(model_path)
+    llm = generate(model_path)
     response = infer(llm, user_input)
-    return jsonify({"response": response})
+    print("Generated response:", response)  # Debug statement
+    return response
 
 def main():
     args = parser.parse_args()
     host = args.host
     port = args.port
     print(f"Inference is working on http://{host}:{port}/v1/chat/completions")
     app.run(host=host, port=port)
     
-
-
 if __name__ == '__main__':
     main()
```

## ALLMDEV/instruct.py

```diff
@@ -165,15 +165,14 @@
                 # Perform inference
                 response_iter = llm.stream_complete(prompt)
                 # print("ALLM:", end='')
                 
                 # Print the assistant's response
                 for response in response_iter:
                     print(response.delta, end="", flush=True)
-                    return response
-                print()
+
             except KeyboardInterrupt:
                 print("\nExiting...")
                 break
```

## Comparing `ALLMDEV-1.2.dist-info/METADATA` & `ALLMDEV-1.2.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLMDEV
-Version: 1.2
+Version: 1.2.1
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Soham Ghadge
 Maintainer-email: soham.ghadge@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
@@ -41,21 +41,17 @@
 
 ```bash
 allm-run --name model_name_or_path
 ```
 
 ## API
 
-After initialising or downloading the model you can start inference API with a simple 'allm-serve' command. The command takes host and port as optional arguments, if not provided, the API will run on the default 127.0.0.1:5000 host.
+After initialising or downloading the model you can start inference API with a simple 'allm-serve' command. The command starts the API server on the default 127.0.0.1:5000 host. If you want to run the API server on a different port and host, you can customize the apiconfig,txt file in your model directory.
 
 ```bash
 allm-serve
 ```
 
-```bash
-allm-serve --host 192.168.0.1 --port 8000
-```
-
 
 ## Supported Model names
 Llama2, llama, llama2_chat, Llama_chat, Mistral, Mistral_instruct
```

## Comparing `ALLMDEV-1.2.dist-info/RECORD` & `ALLMDEV-1.2.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ALLMDEV/__init__.py,sha256=8XSO2SVH9cZ_Iut8rNwcDxtEaBp4LIdXP6hAKGRgeaI,39
-ALLMDEV/api.py,sha256=GLAgApGFlOh9daU6OhR8NjWgy3M4G9DHUrYjhQa8RDc,2034
+ALLMDEV/api.py,sha256=Y69wMrLgODKsoiWQRH9CCVLU4IA8QYO9rX3C0fciEGI,1904
 ALLMDEV/cli.py,sha256=wWOt7Uv_DmQKT821rEIaEVh9MFJVz0n19BXgwTHsdDY,757
-ALLMDEV/instruct.py,sha256=RVxJJhwlGy7q2a3NgwPZi35qB9wnll5Yf2ifDGJ1unQ,10394
-ALLMDEV-1.2.dist-info/METADATA,sha256=vCDKyn_dOu8fHEk0hUn7fcCHnXbx7IQTz8EzGwdv0Vg,2354
-ALLMDEV-1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ALLMDEV-1.2.dist-info/entry_points.txt,sha256=He_WB4819TTsETEoQ7J82TTyF1qChfyKmGNAR6evCy0,76
-ALLMDEV-1.2.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
-ALLMDEV-1.2.dist-info/RECORD,,
+ALLMDEV/generate.py,sha256=Hyp2rsQjjg7jnbykOB3Xr_oaGXLeCfyrTRn2DyDx0gU,2416
+ALLMDEV/instruct.py,sha256=9cjx7CnIc-C-LXxVl2THdlrNX3WXcZ0rXKXWVpZ0BXY,10334
+ALLMDEV-1.2.1.dist-info/METADATA,sha256=warn4PXhbq46xrwS9lJw1wyLjsfBAHI3WaB0WBlarm0,2372
+ALLMDEV-1.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ALLMDEV-1.2.1.dist-info/entry_points.txt,sha256=Vg1PNkMT6_InD8pcRNpouHe5eJ-VSb9lWSb7XeeJr1o,81
+ALLMDEV-1.2.1.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
+ALLMDEV-1.2.1.dist-info/RECORD,,
```

