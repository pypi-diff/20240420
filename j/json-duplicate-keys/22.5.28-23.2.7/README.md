# Comparing `tmp/json_duplicate_keys-22.5.28.tar.gz` & `tmp/json_duplicate_keys-23.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_duplicate_keys-22.5.28.tar", last modified: Sat May 28 15:27:54 2022, max compression
+gzip compressed data, was "json_duplicate_keys-23.2.7.tar", last modified: Tue Feb  7 04:40:26 2023, max compression
```

## Comparing `json_duplicate_keys-22.5.28.tar` & `json_duplicate_keys-23.2.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-05-28 15:27:54.740042 json_duplicate_keys-22.5.28/
--rw-rw-rw-   0        0        0     1077 2022-05-27 07:21:58.000000 json_duplicate_keys-22.5.28/LICENSE.txt
--rw-rw-rw-   0        0        0     3094 2022-05-28 15:27:54.739042 json_duplicate_keys-22.5.28/PKG-INFO
--rw-rw-rw-   0        0        0     2499 2022-05-27 07:21:58.000000 json_duplicate_keys-22.5.28/README.md
-drwxrwxrwx   0        0        0        0 2022-05-28 15:27:54.724477 json_duplicate_keys-22.5.28/json_duplicate_keys/
--rw-rw-rw-   0        0        0    13703 2022-05-28 15:19:22.000000 json_duplicate_keys-22.5.28/json_duplicate_keys/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-28 15:27:54.736013 json_duplicate_keys-22.5.28/json_duplicate_keys.egg-info/
--rw-rw-rw-   0        0        0     3094 2022-05-28 15:27:54.000000 json_duplicate_keys-22.5.28/json_duplicate_keys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2022-05-28 15:27:54.000000 json_duplicate_keys-22.5.28/json_duplicate_keys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-28 15:27:54.000000 json_duplicate_keys-22.5.28/json_duplicate_keys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2022-05-28 15:27:54.000000 json_duplicate_keys-22.5.28/json_duplicate_keys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-28 15:27:54.740042 json_duplicate_keys-22.5.28/setup.cfg
--rw-rw-rw-   0        0        0      866 2022-05-28 15:20:35.000000 json_duplicate_keys-22.5.28/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-07 04:40:26.556110 json_duplicate_keys-23.2.7/
+-rw-rw-rw-   0        0        0     1077 2022-06-07 06:40:42.000000 json_duplicate_keys-23.2.7/LICENSE
+-rw-rw-rw-   0        0        0     3105 2023-02-07 04:40:26.555109 json_duplicate_keys-23.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2023-02-06 16:14:11.000000 json_duplicate_keys-23.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-02-07 04:40:26.540408 json_duplicate_keys-23.2.7/json_duplicate_keys/
+-rw-rw-rw-   0        0        0    14424 2023-02-07 04:39:52.000000 json_duplicate_keys-23.2.7/json_duplicate_keys/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-07 04:40:26.550925 json_duplicate_keys-23.2.7/json_duplicate_keys.egg-info/
+-rw-rw-rw-   0        0        0     3105 2023-02-07 04:40:26.000000 json_duplicate_keys-23.2.7/json_duplicate_keys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-02-07 04:40:26.000000 json_duplicate_keys-23.2.7/json_duplicate_keys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-07 04:40:26.000000 json_duplicate_keys-23.2.7/json_duplicate_keys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-02-07 04:40:26.000000 json_duplicate_keys-23.2.7/json_duplicate_keys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-02-07 04:40:26.556110 json_duplicate_keys-23.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      873 2023-02-06 16:13:44.000000 json_duplicate_keys-23.2.7/setup.py
```

### Comparing `json_duplicate_keys-22.5.28/LICENSE.txt` & `json_duplicate_keys-23.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `json_duplicate_keys-22.5.28/PKG-INFO` & `json_duplicate_keys-23.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: json_duplicate_keys
-Version: 22.5.28
-Summary: Flatten / Unflatten and Loads / Dumps JSON object with Duplicate Keys
+Version: 23.2.7
+Summary: Flatten/ Unflatten and Load(s)/ Dump(s) JSON File/ Object with Duplicate Keys
 Home-page: https://github.com/truocphan/json_duplicate_keys
 Author: Truoc Phan
 Author-email: truocphan112017@gmail.com
 License: MIT
 Keywords: json,duplicate keys,json duplicate keys,flatten,unflatten
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: Implementation :: Jython
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 
 # JSON Duplicate Keys
-Flatten / Unflatten and Loads / Dumps JSON object with Duplicate Keys
+Flatten/ Unflatten and Load(s)/ Dump(s) JSON File/ Object with Duplicate Keys
 
 ## Installation
 ```console
 pip install json-duplicate-keys
 ```
 
 ## Usage
```

### Comparing `json_duplicate_keys-22.5.28/README.md` & `json_duplicate_keys-23.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # JSON Duplicate Keys
-Flatten / Unflatten and Loads / Dumps JSON object with Duplicate Keys
+Flatten/ Unflatten and Load(s)/ Dump(s) JSON File/ Object with Duplicate Keys
 
 ## Installation
 ```console
 pip install json-duplicate-keys
 ```
 
 ## Usage
```

### Comparing `json_duplicate_keys-22.5.28/json_duplicate_keys/__init__.py` & `json_duplicate_keys-23.2.7/json_duplicate_keys/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,62 +2,70 @@
 # # # # # # # # # # loads # # # # # # # # # #
 # # # # # # # # # # # # # # # # # # # # # # #
 """
 >>> INPUT: '{"author": "truocphan", "version": "22.3.3", "version": "latest", "release": [{"version": "22.3.3", "version": "latest"}], "snapshot": {"author": "truocphan", "version": "22.3.3", "release": [{"version": "latest"}]}}'
 
 <<< OUTPUT: {'author': 'truocphan', 'version': '22.3.3', 'version{{{_2_}}}': 'latest', 'release': [{'version': '22.3.3', 'version{{{_2_}}}': 'latest'}], 'snapshot': {'author': 'truocphan', 'version': '22.3.3', 'release': [{'version': 'latest'}]}}
 """
-def loads(Jstr, dupSign_start="{", dupSign_end="}", _isDebug_=False):
+def loads(Jstr, dupSign_start="{", dupSign_end="}", ordered_dict=False, _isDebug_=False):
 	import json
 	import re
 	from collections import OrderedDict
 	import traceback
 
 	def __convert_Jloads_to_Jobj(Jloads, Jobj):
-		if type(Jloads) == OrderedDict:
+		if type(Jloads) in [dict, OrderedDict]:
 			for k in Jloads.keys():
 				_key = re.split(dupSign_start_escape_regex*3+"_\d+_"+dupSign_end_escape_regex*3+"$", k)[0]
 
 				if _key not in Jobj.keys():
-					if type(Jloads[k]) not in [list, OrderedDict]:
+					if type(Jloads[k]) not in [list, dict, OrderedDict]:
 						Jobj[_key] = Jloads[k]
 					else:
 						if type(Jloads[k]) == list:
 							Jobj[_key] = list()
+						elif type(Jloads[k]) == dict:
+							Jobj[_key] = dict()
 						else:
 							Jobj[_key] = OrderedDict()
 
 						__convert_Jloads_to_Jobj(Jloads[k], Jobj[_key])
 				else:
 					countObj = len([i for i in Jobj.keys() if _key==re.split(dupSign_start_escape_regex*3+"_\d+_"+dupSign_end_escape_regex*3+"$", i)[0]])
-					if type(Jloads[k]) not in [list, OrderedDict]:
+					if type(Jloads[k]) not in [list, dict, OrderedDict]:
 						Jobj[_key+dupSign_start*3+"_"+str(countObj+1)+"_"+dupSign_end*3] = Jloads[k]
 					else:
 						if type(Jloads[k]) == list:
 							Jobj[_key+dupSign_start*3+"_"+str(countObj+1)+"_"+dupSign_end*3] = list()
+						elif type(Jloads[k]) == dict:
+							Jobj[_key+dupSign_start*3+"_"+str(countObj+1)+"_"+dupSign_end*3] = dict()
 						else:
 							Jobj[_key+dupSign_start*3+"_"+str(countObj+1)+"_"+dupSign_end*3] = OrderedDict()
 
 						__convert_Jloads_to_Jobj(Jloads[k], Jobj[_key+dupSign_start*3+"_"+str(countObj+1)+"_"+dupSign_end*3])
 		elif type(Jloads) == list:
 			for i in range(len(Jloads)):
-				if type(Jloads[i]) not in [list, OrderedDict]:
+				if type(Jloads[i]) not in [list, dict, OrderedDict]:
 					Jobj.append(Jloads[i])
 				else:
 					if type(Jloads[i]) == list:
 						Jobj.append(list())
+					elif type(Jloads[i]) == dict:
+						Jobj.append(dict())
 					else:
 						Jobj.append(OrderedDict())
 
 					__convert_Jloads_to_Jobj(Jloads[i], Jobj[i])
 
 	try:
-		Jloads = json.loads(Jstr, object_pairs_hook=OrderedDict)
+		Jloads = json.loads(Jstr)
+		if ordered_dict:
+			Jloads = json.loads(Jstr, object_pairs_hook=OrderedDict)
 
-		if type(Jloads) in [list, OrderedDict] and len(Jloads) > 0:
+		if type(Jloads) in [list, dict, OrderedDict] and len(Jloads) > 0:
 			try:
 				if type(dupSign_start) not in [str, unicode] or len(dupSign_start) == 0: dupSign_start = "{"
 			except Exception as e:
 				if type(dupSign_start) != str or len(dupSign_start) == 0: dupSign_start = "{"
 
 			dupSign_start_escape = "".join(["\\\\u"+hex(ord(c))[2:].zfill(4) for c in dupSign_start])
 
@@ -88,18 +96,22 @@
 				Jstr = re.sub(r'{dupSign_start}_dupSign_{dupSign_end}"[\s\t\r\n]*:'.format(dupSign_start=dupSign_start_escape*3, dupSign_end=dupSign_end_escape*3), dupSign_start_escape*3+"_"+str(i)+"_"+dupSign_end_escape*3+'":', Jstr, 1)
 				i += 1
 
 			Jstr = re.sub('\x00\x01', r'\\\\', Jstr)
 			Jstr = re.sub('\x02\x03', r'\\"', Jstr)
 			Jstr = re.sub('\x04\x05', r'"', Jstr)
 
-			Jloads = json.loads(Jstr, object_pairs_hook=OrderedDict)
+			Jloads = json.loads(Jstr)
+			if ordered_dict:
+				Jloads = json.loads(Jstr, object_pairs_hook=OrderedDict)
 
 			if type(Jloads) == list:
 				Jobj = list()
+			elif type(Jloads) == dict:
+				Jobj = dict()
 			else:
 				Jobj = OrderedDict()
 
 			__convert_Jloads_to_Jobj(Jloads, Jobj)
 
 			return Jobj
 		else:
@@ -116,26 +128,26 @@
 
 
 # # # # # # # # # # # # # # # # # # # # # # #
 # # # # # # # # # # load  # # # # # # # # # #
 # # # # # # # # # # # # # # # # # # # # # # #
 """
 """
-def load(Jfilepath, dupSign_start="{", dupSign_end="}", _isDebug_=False):
+def load(Jfilepath, dupSign_start="{", dupSign_end="}", ordered_dict=False, _isDebug_=False):
 	import traceback
 
 	try:
 		Jfile = open(Jfilepath)
 		Jstr = Jfile.read()
 		Jfile.close()
 	except:
 		if _isDebug_: traceback.print_exc()
 		return None
 
-	return loads(Jstr, dupSign_start=dupSign_start, dupSign_end=dupSign_end, _isDebug_=_isDebug_)
+	return loads(Jstr, dupSign_start=dupSign_start, dupSign_end=dupSign_end, ordered_dict=ordered_dict, _isDebug_=_isDebug_)
 # # # # # # # # # # # # # # # # # # # # # # #
 # # # # # # # # # # # # # # # # # # # # # # #
 # # # # # # # # # # # # # # # # # # # # # # #
 
 
 
 
@@ -221,24 +233,28 @@
 # # # # # # # # # flatten # # # # # # # # # #
 # # # # # # # # # # # # # # # # # # # # # # #
 """
 >>> INPUT: {'author': 'truocphan', 'version': '22.3.3', 'version{{{_2_}}}': '22.3.14', 'release': [{'version': '22.3.3', 'version{{{_2_}}}': 'latest'}], 'snapshot': {'author': 'truocphan', 'version': '22.3.3', 'release': [{'version': 'latest'}]}}
 
 <<< OUTPUT: {'author': 'truocphan', 'version': '22.3.3', 'version{{{_2_}}}': '22.3.14', 'release||$0$||version': '22.3.3', 'release||$0$||version{{{_2_}}}': 'latest', 'snapshot||author': 'truocphan', 'snapshot||version': '22.3.3', 'snapshot||release||$0$||version': 'latest'}
 """
-def flatten(Jobj, separator="||", parse_index="$", _isDebug_=False):
+def flatten(Jobj, separator="||", parse_index="$", ordered_dict=False, _isDebug_=False):
 	from collections import OrderedDict
 	import traceback
 
-	Jflat = OrderedDict()
+	Jflat = dict()
+	if ordered_dict:
+		Jflat = OrderedDict()
 
 	def __convert_Jobj_to_Jflat(Jobj, key=None):
 		if type(Jobj) in [dict, OrderedDict]:
 			if len(Jobj) == 0:
-				Jflat[key] = OrderedDict()
+				Jflat[key] = dict()
+				if ordered_dict:
+					Jflat[key] = OrderedDict()
 			else:
 				for k,v in Jobj.items():
 					_Jobj = v
 					_key = "{key}{separator}{k}".format(key=key,separator=separator,k=k) if key != None else "{k}".format(k=k)
 
 					__convert_Jobj_to_Jflat(_Jobj, _key)
 		elif type(Jobj) == list:
@@ -293,32 +309,34 @@
 # # # # # # # # # unflatten # # # # # # # # #
 # # # # # # # # # # # # # # # # # # # # # # #
 """
 >>> INPUT: {'author': 'truocphan', 'version': '22.3.3', 'version{{{_2_}}}': '22.3.14', 'release||$0$||version': '22.3.3', 'release||$0$||version{{{_2_}}}': 'latest', 'snapshot||author': 'truocphan', 'snapshot||version': '22.3.3', 'snapshot||release||$0$||version': '22.3.14'}
 
 <<< OUTPUT: {'author': 'truocphan', 'version': '22.3.3', 'version{{{_2_}}}': '22.3.14', 'release': [{'version': '22.3.3', 'version{{{_2_}}}': 'latest'}], 'snapshot': {'author': 'truocphan', 'version': '22.3.3', 'release': [{'version': '22.3.14'}]}}
 """
-def unflatten(Jflat, separator="||", parse_index="$", _isDebug_=False):
+def unflatten(Jflat, separator="||", parse_index="$", ordered_dict=False, _isDebug_=False):
 	import re
 	from collections import OrderedDict
 	import traceback
 
 	try:
 		if type(Jflat) in [dict, OrderedDict]:
 			if len(Jflat) == 0:
-				return OrderedDict()
+				if ordered_dict:
+					return OrderedDict()
+				return dict()
 			else:
-				Jobj = list() if len([k for k in Jflat.keys() if re.compile("^"+re.escape(parse_index)+"\d+"+re.escape(parse_index)+"$").match(str(k).split(separator)[0])]) == len(Jflat.keys()) else OrderedDict()
+				Jobj = list() if len([k for k in Jflat.keys() if re.compile("^"+re.escape(parse_index)+"\d+"+re.escape(parse_index)+"$").match(str(k).split(separator)[0])]) == len(Jflat.keys()) else OrderedDict() if ordered_dict else dict()
 
 				for k, v in Jflat.items():
 					Jtmp = Jobj
 					Jkeys = k.split(separator)
 
 					for count, (Jkey, next_Jkeys) in enumerate(zip(Jkeys, Jkeys[1:] + [v]), 1):
-						v = next_Jkeys if count == len(Jkeys) else list() if re.compile("^"+re.escape(parse_index)+"\d+"+re.escape(parse_index)+"$").match(next_Jkeys) else OrderedDict()
+						v = next_Jkeys if count == len(Jkeys) else list() if re.compile("^"+re.escape(parse_index)+"\d+"+re.escape(parse_index)+"$").match(next_Jkeys) else OrderedDict() if ordered_dict else dict()
 
 						if type(Jtmp) == list:
 							Jkey = int(re.compile(re.escape(parse_index)+"(\d+)"+re.escape(parse_index)).match(Jkey).group(1))
 
 							while Jkey >= len(Jtmp):
 								Jtmp.append(v)
```

### Comparing `json_duplicate_keys-22.5.28/json_duplicate_keys.egg-info/PKG-INFO` & `json_duplicate_keys-23.2.7/json_duplicate_keys.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: json-duplicate-keys
-Version: 22.5.28
-Summary: Flatten / Unflatten and Loads / Dumps JSON object with Duplicate Keys
+Version: 23.2.7
+Summary: Flatten/ Unflatten and Load(s)/ Dump(s) JSON File/ Object with Duplicate Keys
 Home-page: https://github.com/truocphan/json_duplicate_keys
 Author: Truoc Phan
 Author-email: truocphan112017@gmail.com
 License: MIT
 Keywords: json,duplicate keys,json duplicate keys,flatten,unflatten
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: Implementation :: Jython
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 
 # JSON Duplicate Keys
-Flatten / Unflatten and Loads / Dumps JSON object with Duplicate Keys
+Flatten/ Unflatten and Load(s)/ Dump(s) JSON File/ Object with Duplicate Keys
 
 ## Installation
 ```console
 pip install json-duplicate-keys
 ```
 
 ## Usage
```

### Comparing `json_duplicate_keys-22.5.28/setup.py` & `json_duplicate_keys-23.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="json_duplicate_keys",
-	version="22.5.28",
+	version="23.2.7",
 	author="Truoc Phan",
 	license="MIT",
 	author_email="truocphan112017@gmail.com",
-	description="Flatten / Unflatten and Loads / Dumps JSON object with Duplicate Keys",
+	description="Flatten/ Unflatten and Load(s)/ Dump(s) JSON File/ Object with Duplicate Keys",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	install_requires=[],
 	url="https://github.com/truocphan/json_duplicate_keys",
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"Programming Language :: Python :: 2",
```

