# Comparing `tmp/cloudpy_org-1.4.6.tar.gz` & `tmp/cloudpy_org-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.4.6.tar", last modified: Thu Feb 29 00:57:52 2024, max compression
+gzip compressed data, was "dist\cloudpy_org-1.4.7.tar", last modified: Sat Apr 20 06:30:19 2024, max compression
```

## Comparing `cloudpy_org-1.4.6.tar` & `cloudpy_org-1.4.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 00:57:52.353180 cloudpy_org-1.4.6/
--rw-rw-rw-   0        0        0      935 2024-02-29 00:57:52.352681 cloudpy_org-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-02-29 00:57:52.230451 cloudpy_org-1.4.6/cloudpy_org/
--rw-rw-rw-   0        0        0      473 2024-02-29 00:56:35.000000 cloudpy_org-1.4.6/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    29322 2024-02-29 00:56:59.000000 cloudpy_org-1.4.6/cloudpy_org/aws.py
--rw-rw-rw-   0        0        0    13614 2024-02-29 00:57:04.000000 cloudpy_org-1.4.6/cloudpy_org/docs.py
--rw-rw-rw-   0        0        0     3924 2024-02-29 00:22:40.000000 cloudpy_org-1.4.6/cloudpy_org/imgedit.py
--rw-rw-rw-   0        0        0    47871 2024-02-29 00:57:11.000000 cloudpy_org-1.4.6/cloudpy_org/tools.py
--rw-rw-rw-   0        0        0     4998 2024-02-29 00:57:15.000000 cloudpy_org-1.4.6/cloudpy_org/web.py
-drwxrwxrwx   0        0        0        0 2024-02-29 00:57:52.327835 cloudpy_org-1.4.6/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2024-02-29 00:57:51.000000 cloudpy_org-1.4.6/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-02-29 00:57:51.000000 cloudpy_org-1.4.6/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 00:57:51.000000 cloudpy_org-1.4.6/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-02-29 00:57:51.000000 cloudpy_org-1.4.6/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-02-29 00:57:51.000000 cloudpy_org-1.4.6/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-29 00:57:52.353681 cloudpy_org-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1324 2024-02-29 00:56:00.000000 cloudpy_org-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 06:30:19.006675 cloudpy_org-1.4.7/
+-rw-rw-rw-   0        0        0      935 2024-04-20 06:30:19.006174 cloudpy_org-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 06:30:18.862113 cloudpy_org-1.4.7/cloudpy_org/
+-rw-rw-rw-   0        0        0     1819 2024-04-20 05:15:05.000000 cloudpy_org-1.4.7/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    31391 2024-04-20 05:38:00.000000 cloudpy_org-1.4.7/cloudpy_org/aws.py
+-rw-rw-rw-   0        0        0    12316 2024-02-26 22:47:47.000000 cloudpy_org-1.4.7/cloudpy_org/docs.py
+-rw-rw-rw-   0        0        0     2618 2024-02-22 21:16:50.000000 cloudpy_org-1.4.7/cloudpy_org/imgedit.py
+-rw-rw-rw-   0        0        0    49191 2024-04-19 17:14:28.000000 cloudpy_org-1.4.7/cloudpy_org/tools.py
+-rw-rw-rw-   0        0        0     3701 2023-12-20 02:08:16.000000 cloudpy_org-1.4.7/cloudpy_org/web.py
+drwxrwxrwx   0        0        0        0 2024-04-20 06:30:18.983904 cloudpy_org-1.4.7/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2024-04-20 06:30:16.000000 cloudpy_org-1.4.7/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-20 06:30:17.000000 cloudpy_org-1.4.7/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 06:30:16.000000 cloudpy_org-1.4.7/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-20 06:30:16.000000 cloudpy_org-1.4.7/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-20 06:30:16.000000 cloudpy_org-1.4.7/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 06:30:19.007179 cloudpy_org-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2024-04-20 03:03:10.000000 cloudpy_org-1.4.7/setup.py
```

### Comparing `cloudpy_org-1.4.6/PKG-INFO` & `cloudpy_org-1.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.4.6
+Version: 1.4.7
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.4.6/cloudpy_org/aws.py` & `cloudpy_org-1.4.7/cloudpy_org/aws.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-"""
-███████████████████████████aws of cloudpy_org███████████████████████████
-Copyright © 2023-2024 Cloudpy.org
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Find documentation at https://www.cloudpy.org
-"""
-from cloudpy_org import cloudpy_org_version,gsep,processing_tools
+from cloudpy_org_base import cloudpy_org_version,gsep,processing_tools,aws_regions,subscription_url,msh
 import requests
 import inspect
 import json
 import os
 import random
 import time
 unique_id = lambda: int(round(time.time() * 100000))
 xpt = processing_tools()
 xpt.environment = "s3"
 class aws_framework_manager:
     def __init__(self,secret_key:str,aws_auth_token:str="",aws_namespace:str=""):
+        self.msh = subscription_url.replace('w'*3,msh) + '/'
+        self.regions = aws_regions
         self.aws_namespace = aws_namespace
         self.__deconstructor_token = 'JQxrs8sWqn3JIWlIL8nTlw-302SfmV7RmlZ-T-gB5c4=oiwn8TU5-NcDKzVq'
         uuu = "1V44bjdzKODcN50jdz00c4="
         self.__sc = secret_key[::-1].split(uuu)
         self.__at = aws_auth_token[::-1].split(uuu)
         self.cppt_construction(self.__sc[1])
         self.cppt.environment = "s3"
@@ -138,16 +129,14 @@
     def _decorator(decorator_param):
         def inner_func(self,dk):
             k = dk + "_is_function"
             dc = "self.dx['@k'] = self.dynamic_exec(dynamic_key='@dynamic_key'@these_args)"
             dc = dc.replace("@dynamic_key",dk)\
             .replace("@k",k)\
             .replace("@these_args",self.__args_applied[dk])
-            #print("dcx:")
-            #print(dc)
             exec(dc)
             is_function = self.dx[k]
             self.dx.pop(k, None)
             rslt = None
             if dk in set(self.dx.keys()):
                 if is_function:
                     rslt = self.dx[dk]
@@ -255,36 +244,53 @@
             dk=str(inspect.getframeinfo(inspect.currentframe()).function)
             self.__args_applied[dk]= self.__args_applied[dk]\
             .replace("@bucket_name","'" + bucket_name + "'")
             return self.deco(dk=dk)
         else:
             return self.__not_initialized_message
     #___________________________________________________________________
-    def create_new_user(self,username:str,email:str,pwd:str,bucket_name:str):
-        if self.__service_initialized:
-            dk=str(inspect.getframeinfo(inspect.currentframe()).function)
-            self.__args_applied[dk]= self.__args_applied[dk]\
-            .replace("@username","'" + username + "'")\
-            .replace("@email","'" + email + "'")\
-            .replace("@pwd","'" + pwd + "'")\
-            .replace("@bucket_name","'" + bucket_name + "'")
-            return self.deco(dk=dk)
+    def create_new_user(self,sufix:str=None,region:str=None,username:str=None,email:str=None,pwd:str=None):
+        if sufix != None and region != None and username != None and email != None and pwd != None:
+            if self.__service_initialized:
+                dk=str(inspect.getframeinfo(inspect.currentframe()).function)
+                self.__args_applied[dk]= self.__args_applied[dk]\
+                .replace("@sufix","'" + sufix + "'")\
+                .replace("@region","'" + region + "'")\
+                .replace("@username","'" + username + "'")\
+                .replace("@email","'" + email + "'")\
+                .replace("@pwd","'" + pwd + "'")
+                return self.deco(dk=dk)
+            else:
+                return self.__not_initialized_message
         else:
-            return self.__not_initialized_message
+            return 'Wrong parameters input.'
+    #___________________________________________________________________
+    def treat_none_strings(self,object_str:str,paramName:str,paramValue:str):
+        if paramValue != None:
+            object_str = object_str.replace("@" + paramName,"'" + paramValue + "'")
+        else:
+            object_str = object_str.replace("@" + paramName,str(paramValue))
+        return object_str
     #___________________________________________________________________
-    def check_if_user_exists_and_was_confirmed(self,username_or_email:list,bucket_name:str):
+    def check_if_user_exists_and_was_confirmed(self,username_or_email:list,bucket_name:str=None,sufix:str=None,region:str=None):
+        if type(username_or_email) == str:
+            username_or_email = [username_or_email]
         if self.__service_initialized:
             dk=str(inspect.getframeinfo(inspect.currentframe()).function)
-            self.__args_applied[dk]= self.__args_applied[dk]\
-            .replace("@username_or_email",str(username_or_email))\
-            .replace("@bucket_name","'" + bucket_name + "'")
+            self.__args_applied[dk] = self.__args_applied[dk]\
+            .replace("@username_or_email",str(username_or_email))
+            self.__args_applied[dk] = self.treat_none_strings(self.__args_applied[dk],'bucket_name',bucket_name)
+            self.__args_applied[dk] = self.treat_none_strings(self.__args_applied[dk],'sufix',sufix)
+            self.__args_applied[dk] = self.treat_none_strings(self.__args_applied[dk],'region',region)
             return self.deco(dk=dk)
         else:
             return self.__not_initialized_message
     def service_check_if_user_exists_and_was_confirmed(self,username_or_email:list,bucket_name:str):
+        if type(username_or_email) == str:
+            username_or_email = [username_or_email]
         if self.__service_initialized:
             dk=str(inspect.getframeinfo(inspect.currentframe()).function)
             self.__args_applied[dk]= self.__args_applied[dk]\
             .replace("@username_or_email",str(username_or_email))\
             .replace("@bucket_name","'" + bucket_name + "'")
             return self.deco(dk=dk)
         else:
@@ -337,14 +343,40 @@
             .replace("@username","'" + username + "'")\
             .replace("@token","'" + token + "'")\
             .replace("@bucket_name","'" + bucket_name + "'")
             return self.deco(dk=dk)
         else:
             return self.__not_initialized_message
 
+#*format_bucket_name*begin
+    #___________________________________________________________________
+    def format_bucket_name(self,sufix:str,region:str):
+        if self.__service_initialized:
+            dk=str(inspect.getframeinfo(inspect.currentframe()).function)
+            self.__args_applied[dk]= self.__args_applied[dk]\
+            .replace("@sufix","'" + sufix + "'")\
+            .replace("@region","'" + region + "'")
+            return self.deco(dk=dk)
+        else:
+            return self.__not_initialized_message
+
+#*format_bucket_name*end
+#*get_bucket_name*begin
+    #___________________________________________________________________
+    def get_bucket_name(self,sufix:str,region:str):
+        if self.__service_initialized:
+            dk=str(inspect.getframeinfo(inspect.currentframe()).function)
+            self.__args_applied[dk]= self.__args_applied[dk]\
+            .replace("@sufix","'" + sufix + "'")\
+            .replace("@region","'" + region + "'")
+            return self.deco(dk=dk)
+        else:
+            return self.__not_initialized_message
+
+#*get_bucket_name*end
 #new function here
     
     #*******************************************************************
     
     #___________________________________________________________________
     def get_s3_reference_name(self,username:str,email:str):
         referenceName = username + self.general_separators["user_email_sep"] + email
@@ -423,15 +455,15 @@
     ,local:bool=False
     ,print_results:bool=False
     ,version:str=cloudpy_org_version
     ,test_file_name:str=None
     ,test_folder_path:str=None):
     if aws_namespace != None and aws_namespace != "" and aws_account_tagname == "":
         aws_account_tagname = aws_namespace
-    url_base = "https://www.cloudpy.org/"
+    url_base = subscription_url.replace('w'*3,msh) + '/'
     if local:
         url_base = "http://localhost/"
     url_1 = url_base + "gen_authentication_token"
     url_2 = url_base + "authenticate_with_token"
     url_3 = url_base + "gen_service_token"
     url_4 = url_base + "gtud"
     udata = {}
@@ -494,75 +526,90 @@
             print(message)
         except:
             fm = None
     return fm
 
 def gen_aws_auth_token(user_key:str,secret:str,local:bool=False,minutes_to_expire:float=5):
     ks = "1V44bjdzKODcN50jdz00c4="
-    url_base = "https://www.cloudpy.org/"
+    url_base = subscription_url.replace('w'*3,msh) + '/'
     if local:
         url_base = "http://localhost/"
     url = url_base + "gen_secret_key"
+    #print('url at gen_aws_auth_token:',url)
     data = xpt.gen_encrypted_data_with_expiration(
         original_message=user_key + ks + secret
         ,minutes_to_expire=minutes_to_expire)
     json_to_post = {}
     json_to_post["data"] = str(data)
     json_to_post["minutes_to_expire"] = minutes_to_expire
+    #print('json_to_post:\n',json_to_post)
     auth_token = requests.post(url,json=json_to_post,verify=False).text
+    #print('auth_token at gen_aws_auth_token:\n',auth_token)
     return auth_token
 
 def store_cloudpy_org_aws_token():
     fm = co.aws_framework_manager(secret_key=sc,aws_auth_token=sc)
 
 def gen_cloudpy_org_aws_token(user_key:str,secret:str,email:str,pwd:str,local:bool=False):
     minutes_to_expire = 525600
     ks = "1V44bjdzKODcN50jdz00c4="
-    url_base = "https://www.cloudpy.org/"
+    url_base = subscription_url.replace('w'*3,msh) + '/'
     if local:
         url_base = "http://localhost/"
     url = url_base + "gen_secret_key"
     data = xpt.gen_encrypted_data_with_expiration(
         original_message=user_key + ks + secret
         ,minutes_to_expire=minutes_to_expire)
     json_to_post = {}
     json_to_post["data"] = str(data)
     json_to_post["minutes_to_expire"] = minutes_to_expire
     auth_token = requests.post(url,json=json_to_post,verify=False).text
     return auth_token
-
-def configure_aws(service_token:str,aws_namespace:str,access_key_id:str,secret_access_key:str,local:bool=False):
-    url_base = "https://www.cloudpy.org/"
+def post_it(json_data:dict,endpoint:str,local:bool,expects_json:bool=False):
+    url_base = subscription_url.replace('w'*3,msh) + '/'
     if local:
         url_base = "http://localhost/"
-    url_1 = url_base + 'special_enc'
-    url_2 = url_base +'update_aws_auth_token'
-    enc1 = requests.post(url=url_1,json = {"val":access_key_id,"case":1} ,verify=False).text
-    enc2 = requests.post(url=url_1,json = {"val":secret_access_key,"case":2} ,verify=False).text
-    x = requests.post(url=url_2,json = {"service_token":service_token,"enc1":enc1,"enc2":enc2,"aws_account_tagname":aws_namespace,"active":True} ,verify=False).text
-    return x
+    url_1 = url_base + endpoint
+    this_response = requests.post(url=url_1,json=json_data,verify=False)
+    if expects_json:
+        try:
+            return this_response.json()
+        except Exception as e:
+            return {"error":"this returned: " + this_response.text, "json_data":json_data}
+    else:
+        return this_response.text
+def configure_aws(service_token:str,aws_namespace:str,access_key_id:str,secret_access_key:str,local:bool=False):
+    enc1 = post_it(json_data={"val":access_key_id,"case":1},endpoint='special_enc',local=local)
+    enc2 = post_it(json_data={"val":secret_access_key,"case":2},endpoint='special_enc',local=local)
+    this_json_data = {"service_token":service_token,"enc1":enc1,"enc2":enc2,"aws_account_tagname":aws_namespace,"active":True}
+    return post_it(json_data=this_json_data,endpoint='update_aws_auth_token',local=local)
 
 def gen_new_service_token(username_or_email:str,pwd:str,local:bool=False):
-    url_base = "https://www.cloudpy.org/"
-    if local:
-        url_base = "http://localhost/"
-    url_1 = url_base + 'tek_enc'
-    url_2 = url_base + 'temp_token'
-    url_3 = url_base +'gst'
     case = random.randint(1, 100)
-    enc_pwd = requests.post(url=url_1,json = {"val":pwd,"case":case} ,verify=False).text
-    temp_token = requests.post(url=url_2,json = {"username_or_email":username_or_email,"enc_pwd":enc_pwd,"case":case} ,verify=False).json() 
-    x = requests.post(url=url_3,json = {"token":xpt.decrypt_before_expiration(temp_token)} ,verify=False).text
-    return x
+    enc_pwd = post_it(json_data={"val":pwd,"case":case},endpoint='tek_enc',local=local)
+    temp_token = post_it(json_data={"username_or_email":username_or_email,"enc_pwd":enc_pwd,"case":case},endpoint='temp_token',local=local,expects_json=True)
+    return post_it(json_data={"token":xpt.decrypt_before_expiration(temp_token)},endpoint='gst',local=local)
 
 def get_my_aws_service_token(username_or_email:str,pwd:str,aws_namespace:str,local:bool=False):
-    url_base = "https://www.cloudpy.org/"
-    if local:
-        url_base = "http://localhost/"
-    url_1 = url_base + 'tek_enc'
-    url_2 = url_base + 'temp_token'
-    url_3 = url_base +'gst'
     case = random.randint(1, 100)
-    enc_pwd = requests.post(url=url_1,json = {"val":pwd,"case":case} ,verify=False).text
-    temp_token = requests.post(url=url_2,json = {"username_or_email":username_or_email,"enc_pwd":enc_pwd,"case":case} ,verify=False).json()
-    x = requests.post(url=url_3,json = {"token":xpt.decrypt_before_expiration(temp_token),"aws_namespace":aws_namespace} ,verify=False).text
-    return x
+    enc_pwd = post_it(json_data={"val":pwd,"case":case},endpoint='tek_enc',local=local)
+    temp_token = post_it(json_data={"username_or_email":username_or_email,"enc_pwd":enc_pwd,"case":case},endpoint='temp_token',local=local,expects_json=True)
+    this_json_data = {"token":xpt.decrypt_before_expiration(temp_token),"aws_namespace":aws_namespace}
+    return post_it(json_data=this_json_data,endpoint='gst',local=local)
+
+def authenticate_with_token(json_data:dict,local:bool=False):
+    if "token" in set(json_data.keys()):
+        return post_it(json_data=json_data,endpoint='authenticate_with_token',local=local)
+    else:
+        return "No token provided."
+
+def delete_biscuit(json_data:dict,local:bool=False):
+    if "tk" in set(json_data.keys()):
+        tk = json_data["tk"].replace('"','')
+        return post_it(json_data={"tk":tk},endpoint='clear',local=local)
+    else:
+        return "No tk provided."
+def co_token_auth(json_data:dict,local:bool=False):
+    if "token" in set(json_data.keys()):
+        return post_it(json_data=json_data,endpoint='co_token_auth',local=local,expects_json=True)
+    else:
+        return {"error_message":"No token provided."}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cloudpy_org-1.4.6/cloudpy_org/docs.py` & `cloudpy_org-1.4.7/cloudpy_org/docs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,8 @@
-"""
-███████████████████████████docs of cloudpy_org███████████████████████████
-Copyright © 2023-2024 Cloudpy.org
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Find documentation at https://www.cloudpy.org
-"""
-from cloudpy_org import cloudpy_org_version,processing_tools
+from cloudpy_org_base import cloudpy_org_version,processing_tools
 from typing import Union
 import inspect
 import os
 pt = processing_tools()
 class auto_document:
     def __init__(self):
         self.load_classes_and_methods()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cloudpy_org-1.4.6/cloudpy_org/tools.py` & `cloudpy_org-1.4.7/cloudpy_org/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Find documentation at https://www.cloudpy.org
 """
-from cloudpy_org import cloudpy_org_version
+from cloudpy_org_base import cloudpy_org_version,subscription_url,msh
 import os
 import json
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.filterwarnings('ignore')
 warnings.simplefilter('ignore')
 import pandas as pd
@@ -63,14 +63,15 @@
         self.settings = self.main_bucket + 'settings/'
         self.secrets = self.settings + 'secrets/'
         self.metadata = self.settings + 'metadata/'
         self.datalake = self.s3_bucket + 'datalake-demo-01/'
         self.hive = self.s3_bucket + 'default_hive/'
         self.dl_crypto = self.datalake + 'crypto/'
         self.dl_crypto_intraday = self.dl_crypto + 'intraday/'
+        self.log_path = self.local_directory + 'log/'
         try:
             self.fs = s3fs.S3FileSystem()
         except:
             self.fs = None
         try:
             self.load_metadata()
         except:
@@ -251,38 +252,41 @@
                 third_part = "gCfJUHLD7Y60ekf6qm_Y=Fl9pT5Fl9pT5gAAAAABkm_us4VOEmkDGp38wL5Jka5UGJzLnKJ9d7RCs110oM-c_kR4iAa1rLNH98ILTdWMf4wUwOozHEn34X5g6ITG7Q5InPQJPj_hyUaHVbe8RC_r7EPvJ1QGTUhFl_jOzz5RztN5zKdyuLw_XraiVpRzlS7gIscIpFdXCr3NQSWndyUASbr6VR2Rm1HQaYQTfQYS6LDflq57fXY1nGmpzz__COVQ60SsOwuYsQSKYpMOCc3nWNPDkEenJautpp50RfRmBs1GyWKEiRv-l7IAnu9VlQrayVFNI-GKEF7svIYOORZso7KXXHWK_1hKCMpI4kgH8L1_481R6TrBEfz9vdOQvdm6CBVoYFa-ifMULx3Ul7ZbYetZjMWKdQTidMzWaYy9MQxBz-GGfhaihTKLuq7KUbMkxQkUZ_RX0Xx07j65eSRMYoExophuknTI74bkbtx5t2_X31uTuMksTe7VWl6s2BHnzH_EzqH1ERVYUukyETuTkZq6_H3o6LpYN0zAIiCcM-x10wvkJz9f6bNg1ElaxoWKz7FUIVVI7vJP3HtIchRrDmus6jM_LWae00z7gpaOw7ysljEut6y7NXQ1nNmOAOQr6Z5XTR3X1dwcI66Xe1tPEm30bRgxblQS3IntVanjrJUY8"
         dc = self.decrypt(third_part.split("Fl9pT5Fl9pT5")[1], url.split(url_base)[1] + third_part.split("Fl9pT5Fl9pT5")[0])
         """
         #print("self.xtdata:",self.xtdata)
         if type(self.xtdata) == dict and self.xtdata != {}:
             try:
                 spd = self.dx(self.decrypt_before_expiration(self.xtdata),10)
-            except:
+            except Exception as e:
+                self.aws_auth_error_message = 'Error at __set_aws_session:' + str(e) + '\nwith data:\n' + str(self.xtdata)
                 spd = []
             if len(spd) > 1 and spd[1] == 'deripxe noitpyrcne':
                 self.aws_auth_token_expired = True
                 self.aws_auth_error_message = "AWS authentication token expired."
             elif len(spd) > 1 and len(spd[0]) == 20 and len(spd[1]) == 40:
                 self.aws_auth_token_expired = False
                 try:
                     self.xsession = boto3.Session(aws_access_key_id=spd[0],aws_secret_access_key=spd[1])
                     self.xs3_client = boto3.client("s3",aws_access_key_id=spd[0],aws_secret_access_key=spd[1],region_name=region_name)
                     self.aws_authenticated = True
                     self.aws_auth_error_message = ""
+                    del spd
                 except Exception as e:
                     self.aws_authenticated = False
                     self.xsession = None
                     self.xs3_client = None
                     self.aws_auth_error_message = "Invalid AWS credentials."
+                    
             else:
                 self.aws_authenticated = False
                 self.aws_auth_token_expired = False
-                self.aws_auth_error_message = "Invalid AWS authentication token."
+                #self.aws_auth_error_message = "Invalid AWS authentication token."
                 self.xsession = None
                 self.xs3_client = None
-                
+
         self.__session = self.xsession
         self.__s3_client = self.xs3_client
         self.s3_client = self.__s3_client
         if self.__session != None:
             self.__resource = self.__session.resource('s3')
         else:
             self.__resource=boto3.resource('s3')
@@ -613,27 +617,29 @@
         ,[5. volume] [volume],[date],[capture_date_id],[capture_time_id] from df) a
         order by 1 asc;
         """
         rslt_df = sqldf(q)
         file_name = symbol.lower() + "_" + str(date_id) + "_"+ str(time_id) + ".parquet"
         rslt_df.to_parquet(file_name)
         return rslt_df
-    def decrypt_before_expiration(self,data:dict)->str:
+    def decrypt_before_expiration(self,data:dict,save:bool=True)->str:
         '''
         ***
         Returns the decryption of the "encrypted_content" node of the encrypted_data_with_expiration() output dict as long as it's "keystr_with_expiration" value has not expired.
         ***
         '''
+        #_______________________
         encrypted_string=data["encrypted_content"]
         exp_seconds,keystr_with_expiration=self.extract_seconds_from_encrypted_input(data["keystr_with_expiration"])
         piece = keystr_with_expiration[0:12]
         spx = keystr_with_expiration.replace(piece,'')[0:14]
         if self.validate_special_phrase(spx,exp_seconds) == True:
             k = piece[::-1] + keystr_with_expiration.replace(spx,'').replace(piece,'')
-            a,b = self.date_time_id()
+            #a,b = self.date_time_id()
+            a = data['date_id']
             w = 0
             for i in str(a):
                 w+=int(i)
             u = str(w) + '*-*'
             i = -1
             xx = ""
             ol = k.split(u)
@@ -651,18 +657,19 @@
                             x = self.alpha_ofuscate(intx)
                             y = o[::-1][2:len(o)][::-1]
                             new_piece = y + x
                         except:
                             new_piece = o
                     new_keystr += new_piece
                 else:
-                    new_keystr += o 
-            return self.decrypt(inputStr=encrypted_string,keyStr=new_keystr)
+                    new_keystr += o
+            rslt = self.decrypt(inputStr=encrypted_string,keyStr=new_keystr)
         else:
-            return "encryption expired"
+            rslt = "encryption expired"
+        return rslt
     #__________________________________________________________________________
     def pre_gen_encrypted_data_with_expiration(self,inputStr:str)->dict:
         '''
         ***
         Description not available.
         ***
         '''
@@ -792,15 +799,15 @@
         Description not available.
         ***
         '''
         a = strInput[0:7]
         b = strInput[7:len(strInput)]
         keystr =  self.gen_enc_key() 
         encrypted_message = self.encrypt("<*seconds*>" +str(seconds) +"</*seconds*>",keystr) 
-        rslt = a+keystr[::-1] + b + "<****>" + encrypted_message
+        rslt = a + keystr[::-1] + b + "<****>" + encrypted_message
         return rslt
     #__________________________________________________________________________
     def extract_seconds_from_encrypted_input(self,strInput:str)->Union[int,str]:
         '''
         ***
         Description not available.
         ***
@@ -819,33 +826,53 @@
                 if "<*seconds*>" in decrypted_seconds and "</*seconds*>" in decrypted_seconds:
                     decrypted_seconds = decrypted_seconds.replace("<*seconds*>","").replace("</*seconds*>","")
                     rslt = int(decrypted_seconds)
                     break
             except:
                 ...
         return rslt,w.replace(key_reverse,"")
+    def date_id_time_str(self):
+        date_id,time_id = self.date_time_id()
+        time_str = self.seconds_to_timestr(time_id)
+        this_rslt = str(date_id) + " | " + time_str
+        return this_rslt
     #__________________________________________________________________________ 
     def gen_encrypted_data_with_expiration(self,original_message:str,minutes_to_expire:int)->dict:
         '''
         ***
         Generates an encrypted dictionary which work as the input of decrypt_before_expiration() function and which
         expires after the minutes_to_expire here provided.
         Once the expiration time has passed, the message won´t be able to be decrypted again.
         The output dict has information about when the encryption took place was created, however the information to validate that is actually encrypted within it, so modifying the "date_id" or "timestr" values has no effect on the expiration time of the "keystr_with_expiration" value. The "date_id" and "timestr" values are only informative and play no effect on the expiration validation. The real time of expiration can't change.
         ***
         '''
         data = {}
+        #_______________________ERASE THIS
+        #json_path = self.log_path + 'encrypted_with_expiration.json'
+        #try:
+        #    with open(json_path, 'r') as f:
+        #        this_dict = json.loads(f.read())
+        #except:
+        #    this_dict = {}
+        #_______________________
         for a in range(100):
             try:
                 data = self.pre_gen_encrypted_data_with_expiration(original_message)
                 data["keystr_with_expiration"] = self.add_encrypted_seconds(
                     data["keystr_with_expiration"]
                     ,int(minutes_to_expire*60))
-                decrypted_message = self.decrypt_before_expiration(data=data)
-
+                decrypted_message = self.decrypt_before_expiration(data=data,save=False)
+                #_______________________ERASE THIS
+                #k = self.date_id_time_str()
+                #this_dict[k] = {}
+                #this_dict[k]['data'] = data
+                #this_dict[k]['minutes_to_expire'] = minutes_to_expire
+                #this_dict[k]['original_message'] = original_message
+                #self.store_dict_as_json(dictionary_input=this_dict,writing_path=json_path)
+                #_______________________
                 break
             except:
                 ...
         return data
     #__________________________________________________________________________
     def popsql(self,df_input_name:str,df_output_name:str,column_names:object,action_expression:str,new_column_names:object=None)->pd.DataFrame:
         '''
```

### Comparing `cloudpy_org-1.4.6/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.4.7/cloudpy_org.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.4.6
+Version: 1.4.7
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.4.6/setup.py` & `cloudpy_org-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.4.6",
+    version="1.4.7",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

