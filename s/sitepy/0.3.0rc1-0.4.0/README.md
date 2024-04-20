# Comparing `tmp/sitepy-0.3.0rc1.tar.gz` & `tmp/sitepy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitepy-0.3.0rc1.tar", last modified: Thu Apr 18 23:00:17 2024, max compression
+gzip compressed data, was "sitepy-0.4.0.tar", last modified: Sat Apr 20 02:33:38 2024, max compression
```

## Comparing `sitepy-0.3.0rc1.tar` & `sitepy-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 23:00:17.402061 sitepy-0.3.0rc1/
--rw-rw-rw-   0        0        0      566 2024-04-18 20:48:30.000000 sitepy-0.3.0rc1/LICENSE
--rw-rw-rw-   0        0        0     1813 2024-04-18 23:00:17.401061 sitepy-0.3.0rc1/PKG-INFO
--rw-rw-rw-   0        0        0      920 2024-04-18 18:57:48.000000 sitepy-0.3.0rc1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 23:00:17.402061 sitepy-0.3.0rc1/setup.cfg
--rw-rw-rw-   0        0        0     1086 2024-04-18 22:58:11.000000 sitepy-0.3.0rc1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 23:00:17.387058 sitepy-0.3.0rc1/sitepy/
--rw-rw-rw-   0        0        0       88 2024-04-18 20:59:01.000000 sitepy-0.3.0rc1/sitepy/__init__.py
--rw-rw-rw-   0        0        0    11932 2024-04-18 22:57:43.000000 sitepy-0.3.0rc1/sitepy/core.py
--rw-rw-rw-   0        0        0      236 2024-04-18 22:58:21.000000 sitepy-0.3.0rc1/sitepy/gpt.py
--rw-rw-rw-   0        0        0    28925 2024-04-18 22:58:26.000000 sitepy-0.3.0rc1/sitepy/profanity.py
--rw-rw-rw-   0        0        0      318 2024-04-18 22:59:08.000000 sitepy-0.3.0rc1/sitepy/recaptcha.py
-drwxrwxrwx   0        0        0        0 2024-04-18 23:00:17.398061 sitepy-0.3.0rc1/sitepy.egg-info/
--rw-rw-rw-   0        0        0     1813 2024-04-18 23:00:16.000000 sitepy-0.3.0rc1/sitepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-18 23:00:17.000000 sitepy-0.3.0rc1/sitepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 23:00:16.000000 sitepy-0.3.0rc1/sitepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 23:00:16.000000 sitepy-0.3.0rc1/sitepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 02:33:38.878552 sitepy-0.4.0/
+-rw-rw-rw-   0        0        0      566 2024-04-18 20:48:30.000000 sitepy-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1817 2024-04-20 02:33:38.877552 sitepy-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2024-04-18 18:57:48.000000 sitepy-0.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 02:33:38.878552 sitepy-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1074 2024-04-20 02:33:08.000000 sitepy-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 02:33:38.863549 sitepy-0.4.0/sitepy/
+-rw-rw-rw-   0        0        0      125 2024-04-19 00:15:25.000000 sitepy-0.4.0/sitepy/__init__.py
+-rw-rw-rw-   0        0        0    12175 2024-04-20 02:22:50.000000 sitepy-0.4.0/sitepy/core.py
+-rw-rw-rw-   0        0        0     1010 2024-04-18 23:46:26.000000 sitepy-0.4.0/sitepy/db.py
+-rw-rw-rw-   0        0        0      236 2024-04-18 22:58:21.000000 sitepy-0.4.0/sitepy/gpt.py
+-rw-rw-rw-   0        0        0      457 2024-04-20 02:11:02.000000 sitepy-0.4.0/sitepy/log.py
+-rw-rw-rw-   0        0        0    28925 2024-04-18 22:58:26.000000 sitepy-0.4.0/sitepy/profanity.py
+-rw-rw-rw-   0        0        0      318 2024-04-18 22:59:08.000000 sitepy-0.4.0/sitepy/recaptcha.py
+drwxrwxrwx   0        0        0        0 2024-04-20 02:33:38.874552 sitepy-0.4.0/sitepy.egg-info/
+-rw-rw-rw-   0        0        0     1817 2024-04-20 02:33:38.000000 sitepy-0.4.0/sitepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-04-20 02:33:38.000000 sitepy-0.4.0/sitepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 02:33:38.000000 sitepy-0.4.0/sitepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-20 02:33:38.000000 sitepy-0.4.0/sitepy.egg-info/top_level.txt
```

### Comparing `sitepy-0.3.0rc1/LICENSE` & `sitepy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sitepy-0.3.0rc1/PKG-INFO` & `sitepy-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.3.0rc1
+Version: 0.4.0
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -61,8 +61,8 @@
 - Static file serving: Files in the static directory are served at /static.
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
-[Apache](LICENSE)
+[Apache](sitepy/LICENSE)
```

### Comparing `sitepy-0.3.0rc1/README.md` & `sitepy-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sitepy-0.3.0rc1/setup.py` & `sitepy-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sitepy',
-    version='0.3.0-pre1',
+    version='0.4.0',
     description='A simple web framework.',
     author='WolfTheDev',
     author_email='wolfthedev@gmail.com',
     url='https://github.com/WolfTheDeveloper/sitepy',
     license='Apache 2.0',
     packages=find_packages(),
-    long_description=open('sitepy/README.md').read(),
+    long_description=open('README.md').read(),
     long_description_content_type='text/markdown',  # Add this line
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `sitepy-0.3.0rc1/sitepy/core.py` & `sitepy-0.4.0/sitepy/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from urllib.parse import parse_qs
 from wsgiref.simple_server import make_server
 import inspect
+from jinja2 import Environment, FileSystemLoader
 
 fof = """
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
     <meta charset="UTF-8">
@@ -341,34 +342,27 @@
 </body>
 </html>
 """
 
 
 class SitePy:
     def __init__(
-        self,
-        static_dir="static",
-        templates_dir="templates",
-        custom_404_page=None,
-        custom_500_page=None,
+        self, static_dir="static", templates_dir="templates", custom_404_page=None, custom_500_page=None
     ):
         self.routes = {}
         self.middleware = [self.logger_middleware]
         self.static_dir = static_dir
         self.templates_dir = templates_dir
         self.custom_404_page = custom_404_page
         self.custom_500_page = custom_500_page
 
-    def render_template(self, template_name, context={}):
-        template_path = os.path.join(self.templates_dir, template_name)
-        with open(template_path, "r") as f:
-            template = f.read()
-        for key, value in context.items():
-            template = template.replace(f"{{{{ {key} }}}}", value)
-        return template
+    def render_template(self, template_name, **context):
+        env = Environment(loader=FileSystemLoader(self.templates_dir))
+        template = env.get_template(template_name)
+        return template.render(**context)
 
     def route(self, path, methods=["GET"]):
         def wrapper(handler):
             self.routes[(path, tuple(methods))] = handler
             return handler
 
         return wrapper
@@ -447,14 +441,24 @@
             return [
                 (
                     self.custom_500_page.encode()
                     if self.custom_500_page
                     else f00.encode()
                 )
             ]
+    
+    def json_response(self, data):
+        import json
+        response_body = json.dumps(data)
+        def response(start_response):
+            status = "200 OK"
+            headers = [("Content-type", "application/json")]
+            start_response(status, headers)
+            return [response_body.encode()]
+        return response
 
     def run(self, host="localhost", port=8080):
         try:
             server = make_server(host, port, self)
             print(f"Serving on {host}:{port}")
             server.serve_forever()
         except KeyboardInterrupt:
```

#### html2text {}

```diff
@@ -1,55 +1,58 @@
 import os from urllib.parse import parse_qs from wsgiref.simple_server import
-make_server import inspect fof = """
+make_server import inspect from jinja2 import Environment, FileSystemLoader fof
+= """
 ************ EErrrroorr 440044 ************
 The page you are looking for might have been removed, had its name changed or
 is temporarily unavailable.
 Please _r_e_t_u_r_n_ _t_o_ _t_h_e_ _h_o_m_e_p_a_g_e.
 Good luck.
 Credits to _R_i_t_h_i_k_ _S_a_m_a_n_t_h_u_l_a_ _(_@_c_o_d_e_2_r_i_t_h_i_k_)_!
 """ f00 = """
 **** IInntteerrnnaall SSeerrvveerr eerrrroorr !! ****
 ************ 55 ************
 ************ 0000 ************
 We're unable to find out what's happening! We suggest you to
 _G_o_ _H_o_m_e or visit here later. Credits to _A_M_A_N_ _(_@_a_d_s_i_n_g_h_1_4_)_!
 """ class SitePy: def __init__( self, static_dir="static",
-templates_dir="templates", custom_404_page=None, custom_500_page=None, ):
+templates_dir="templates", custom_404_page=None, custom_500_page=None ):
 self.routes = {} self.middleware = [self.logger_middleware] self.static_dir =
 static_dir self.templates_dir = templates_dir self.custom_404_page =
 custom_404_page self.custom_500_page = custom_500_page def render_template
-(self, template_name, context={}): template_path = os.path.join
-(self.templates_dir, template_name) with open(template_path, "r") as f:
-template = f.read() for key, value in context.items(): template =
-template.replace(f"{{{{ {key} }}}}", value) return template def route(self,
-path, methods=["GET"]): def wrapper(handler): self.routes[(path, tuple
-(methods))] = handler return handler return wrapper def use(self, middleware):
-self.middleware.append(middleware) def logger_middleware(self, environ): print
-(f"Request received for {environ['PATH_INFO']}") def __call__(self, environ,
-start_response): try: path = environ["PATH_INFO"] method = environ
-["REQUEST_METHOD"] for middleware in self.middleware: middleware(environ)
-handler = None for route, methods in self.routes.keys(): match = route.match
-(path) if match and method in methods: handler = self.routes[(route, methods)]
-params = match.groupdict() break if handler: try: request_body_size = int
-(environ.get("CONTENT_LENGTH", 0)) except ValueError: request_body_size = 0
-request_body = environ["wsgi.input"].read(request_body_size) body_params =
-parse_qs(request_body.decode()) if request_body else {} params = parse_qs
-(request_body.decode()) if request_body else {} params.update(body_params)
-handler_args = inspect.signature(handler).parameters response_body = handler
-(params) if handler_args else handler() status = "200 OK" headers = [("Content-
-type", "text/html")] start_response(status, headers) return
-[response_body.encode()] elif path.startswith("/" + self.static_dir): try: with
-open(path[1:], "rb") as f: response_body = f.read() status = "200 OK" headers =
-[("Content-type", "application/octet-stream")] start_response(status, headers)
-return [response_body] except FileNotFoundError: status = "404 NOT FOUND"
-headers = [("Content-type", "text/html")] start_response(status, headers)
-return [ ( self.custom_404_page.encode() if self.custom_404_page else
-fof.encode() ) ] else: status = "404 NOT FOUND" headers = [("Content-type",
-"text/html")] start_response(status, headers) return [
+(self, template_name, **context): env = Environment(loader=FileSystemLoader
+(self.templates_dir)) template = env.get_template(template_name) return
+template.render(**context) def route(self, path, methods=["GET"]): def wrapper
+(handler): self.routes[(path, tuple(methods))] = handler return handler return
+wrapper def use(self, middleware): self.middleware.append(middleware) def
+logger_middleware(self, environ): print(f"Request received for {environ
+['PATH_INFO']}") def __call__(self, environ, start_response): try: path =
+environ["PATH_INFO"] method = environ["REQUEST_METHOD"] for middleware in
+self.middleware: middleware(environ) handler = None for route, methods in
+self.routes.keys(): match = route.match(path) if match and method in methods:
+handler = self.routes[(route, methods)] params = match.groupdict() break if
+handler: try: request_body_size = int(environ.get("CONTENT_LENGTH", 0)) except
+ValueError: request_body_size = 0 request_body = environ["wsgi.input"].read
+(request_body_size) body_params = parse_qs(request_body.decode()) if
+request_body else {} params = parse_qs(request_body.decode()) if request_body
+else {} params.update(body_params) handler_args = inspect.signature
+(handler).parameters response_body = handler(params) if handler_args else
+handler() status = "200 OK" headers = [("Content-type", "text/html")]
+start_response(status, headers) return [response_body.encode()] elif
+path.startswith("/" + self.static_dir): try: with open(path[1:], "rb") as f:
+response_body = f.read() status = "200 OK" headers = [("Content-type",
+"application/octet-stream")] start_response(status, headers) return
+[response_body] except FileNotFoundError: status = "404 NOT FOUND" headers = [
+("Content-type", "text/html")] start_response(status, headers) return [
 ( self.custom_404_page.encode() if self.custom_404_page else fof.encode() ) ]
-except KeyboardInterrupt: print("\nServer shutting down...") except Exception
-as e: status = "500 INTERNAL SERVER ERROR" headers = [("Content-type", "text/
-html")] start_response(status, headers) print(e) return [
-( self.custom_500_page.encode() if self.custom_500_page else f00.encode() ) ]
+else: status = "404 NOT FOUND" headers = [("Content-type", "text/html")]
+start_response(status, headers) return [ ( self.custom_404_page.encode() if
+self.custom_404_page else fof.encode() ) ] except KeyboardInterrupt: print
+("\nServer shutting down...") except Exception as e: status = "500 INTERNAL
+SERVER ERROR" headers = [("Content-type", "text/html")] start_response(status,
+headers) print(e) return [ ( self.custom_500_page.encode() if
+self.custom_500_page else f00.encode() ) ] def json_response(self, data):
+import json response_body = json.dumps(data) def response(start_response):
+status = "200 OK" headers = [("Content-type", "application/json")]
+start_response(status, headers) return [response_body.encode()] return response
 def run(self, host="localhost", port=8080): try: server = make_server(host,
 port, self) print(f"Serving on {host}:{port}") server.serve_forever() except
 KeyboardInterrupt: print("\nServer shutting down...") server.server_close()
```

### Comparing `sitepy-0.3.0rc1/sitepy/profanity.py` & `sitepy-0.4.0/sitepy/profanity.py`

 * *Files identical despite different names*

### Comparing `sitepy-0.3.0rc1/sitepy.egg-info/PKG-INFO` & `sitepy-0.4.0/sitepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.3.0rc1
+Version: 0.4.0
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -61,8 +61,8 @@
 - Static file serving: Files in the static directory are served at /static.
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
-[Apache](LICENSE)
+[Apache](sitepy/LICENSE)
```

