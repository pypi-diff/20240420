# Comparing `tmp/mingzi-1.2.2.tar.gz` & `tmp/mingzi-1.2.3a0.tar.gz`

## Comparing `mingzi-1.2.2.tar` & `mingzi-1.2.3a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 mingzi-1.2.2/src/mingzi/__init__.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 mingzi-1.2.2/src/mingzi/_mingzi.py
--rw-r--r--   0        0        0    27035 2020-02-02 00:00:00.000000 mingzi-1.2.2/src/mingzi/data.json
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mingzi-1.2.2/LICENSE
--rw-r--r--   0        0        0     9615 2020-02-02 00:00:00.000000 mingzi-1.2.2/README.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 mingzi-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     9930 2020-02-02 00:00:00.000000 mingzi-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 mingzi-1.2.3a0/src/mingzi/__init__.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 mingzi-1.2.3a0/src/mingzi/_mingzi.py
+-rw-r--r--   0        0        0    27035 2020-02-02 00:00:00.000000 mingzi-1.2.3a0/src/mingzi/data.json
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mingzi-1.2.3a0/LICENSE
+-rw-r--r--   0        0        0     9615 2020-02-02 00:00:00.000000 mingzi-1.2.3a0/README.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 mingzi-1.2.3a0/pyproject.toml
+-rw-r--r--   0        0        0     9932 2020-02-02 00:00:00.000000 mingzi-1.2.3a0/PKG-INFO
```

### Comparing `mingzi-1.2.2/src/mingzi/_mingzi.py` & `mingzi-1.2.3a0/src/mingzi/_mingzi.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 
 
 """
 the probability distribution data, and the
 alternative dataset collated from network
 """
 
-with open(os.path.split(os.path.realpath(__file__))[0] + "\\data.json", "r", encoding="UTF-8") as f:
-    data = json.load(f)
+try:
+    with open(os.path.split(os.path.realpath(__file__))[0] + "\\data.json", "r", encoding="UTF-8") as f:
+        data = json.load(f)
+except FileNotFoundError:
+    with open(os.path.split(os.path.realpath(__file__))[0] + "/data.json", "r", encoding="UTF-8") as f:
+        data = json.load(f)
 
 samples = []
 for i in data["surname"].keys():
     samples += [i] * (int(data["surname"][i] * 30000))
 
 
 def gen_surname(com_rate=0.001):
```

### Comparing `mingzi-1.2.2/src/mingzi/data.json` & `mingzi-1.2.3a0/src/mingzi/data.json`

 * *Files identical despite different names*

### Comparing `mingzi-1.2.2/LICENSE` & `mingzi-1.2.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `mingzi-1.2.2/README.md` & `mingzi-1.2.3a0/README.md`

 * *Files identical despite different names*

### Comparing `mingzi-1.2.2/pyproject.toml` & `mingzi-1.2.3a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mingzi"
-version = "1.2.2"
+version = "1.2.3a"
 authors = [
   { name="Aliyacs Souna", email="17818403529@139.com" },
 ]
 description = "这是一个用来生成随机中文姓名的包。This is a library for developers to use to generate random Chinese names."
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `mingzi-1.2.2/PKG-INFO` & `mingzi-1.2.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mingzi
-Version: 1.2.2
+Version: 1.2.3a0
 Summary: 这是一个用来生成随机中文姓名的包。This is a library for developers to use to generate random Chinese names.
 Author-email: Aliyacs Souna <17818403529@139.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
```

