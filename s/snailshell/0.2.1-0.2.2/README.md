# Comparing `tmp/snailshell-0.2.1.tar.gz` & `tmp/snailshell-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snailshell-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "snailshell-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `snailshell-0.2.1.tar` & `snailshell-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      240 2024-03-09 09:58:55.973622 snailshell-0.2.1/.env
--rw-r--r--   0        0        0      699 2024-04-20 10:02:19.474963 snailshell-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      827 2024-03-09 12:00:39.632532 snailshell-0.2.1/.github/workflows/notification.yaml
--rw-r--r--   0        0        0     3816 2024-03-30 09:19:52.985535 snailshell-0.2.1/.gitignore
--rw-r--r--   0        0        0      237 2024-02-24 09:06:57.448971 snailshell-0.2.1/.vscode/settings.json
--rw-r--r--   0        0        0      755 2024-04-20 10:06:02.933095 snailshell-0.2.1/Makefile
--rw-r--r--   0        0        0      549 2024-03-30 09:46:25.726380 snailshell-0.2.1/README.md
--rw-r--r--   0        0        0     1910 2024-03-09 09:58:55.974586 snailshell-0.2.1/cd/client.py
--rw-r--r--   0        0        0     1701 2024-03-30 09:52:24.011423 snailshell-0.2.1/docs/README-dev.md
--rw-r--r--   0        0        0   162240 2024-03-30 09:46:25.726801 snailshell-0.2.1/docs/red-snail.png
--rw-r--r--   0        0        0  9149096 2024-03-30 09:19:53.021221 snailshell-0.2.1/examples/mobilenet-v2.pth
--rw-r--r--   0        0        0    81588 2024-03-09 07:54:30.014457 snailshell-0.2.1/examples/test_image.jpg
--rw-r--r--   0        0        0     1328 2024-04-20 10:08:10.822573 snailshell-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-30 09:46:25.727046 snailshell-0.2.1/snailshell/__init__.py
--rw-r--r--   0        0        0     2667 2024-04-20 10:06:02.933884 snailshell-0.2.1/snailshell/main.py
--rw-r--r--   0        0        0     3231 2024-03-30 09:19:53.021898 snailshell-0.2.1/snailshell/main_test.py
--rw-r--r--   0        0        0      944 2024-03-30 09:19:53.021972 snailshell-0.2.1/snailshell/model_class.py
--rw-r--r--   0        0        0     2719 2024-04-20 10:06:02.934487 snailshell-0.2.1/snailshell/model_loader.py
--rw-r--r--   0        0        0     2906 2024-04-20 10:07:57.834570 snailshell-0.2.1/snailshell/pipeline.py
--rw-r--r--   0        0        0      926 2024-04-20 10:06:02.935346 snailshell-0.2.1/snailshell/utils/port.py
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 snailshell-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      240 2024-03-09 09:58:55.973622 snailshell-0.2.2/.env
+-rw-r--r--   0        0        0      699 2024-04-20 10:02:19.474963 snailshell-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      827 2024-03-09 12:00:39.632532 snailshell-0.2.2/.github/workflows/notification.yaml
+-rw-r--r--   0        0        0     3816 2024-03-30 09:19:52.985535 snailshell-0.2.2/.gitignore
+-rw-r--r--   0        0        0      237 2024-02-24 09:06:57.448971 snailshell-0.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0      755 2024-04-20 10:06:02.933095 snailshell-0.2.2/Makefile
+-rw-r--r--   0        0        0      549 2024-03-30 09:46:25.726380 snailshell-0.2.2/README.md
+-rw-r--r--   0        0        0     1910 2024-03-09 09:58:55.974586 snailshell-0.2.2/cd/client.py
+-rw-r--r--   0        0        0     1701 2024-03-30 09:52:24.011423 snailshell-0.2.2/docs/README-dev.md
+-rw-r--r--   0        0        0   162240 2024-03-30 09:46:25.726801 snailshell-0.2.2/docs/red-snail.png
+-rw-r--r--   0        0        0  9149096 2024-03-30 09:19:53.021221 snailshell-0.2.2/examples/mobilenet-v2.pth
+-rw-r--r--   0        0        0    81588 2024-03-09 07:54:30.014457 snailshell-0.2.2/examples/test_image.jpg
+-rw-r--r--   0        0        0     1328 2024-04-20 10:10:46.183104 snailshell-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-30 09:46:25.727046 snailshell-0.2.2/snailshell/__init__.py
+-rw-r--r--   0        0        0     2667 2024-04-20 10:06:02.933884 snailshell-0.2.2/snailshell/main.py
+-rw-r--r--   0        0        0     3231 2024-03-30 09:19:53.021898 snailshell-0.2.2/snailshell/main_test.py
+-rw-r--r--   0        0        0      944 2024-03-30 09:19:53.021972 snailshell-0.2.2/snailshell/model_class.py
+-rw-r--r--   0        0        0     2719 2024-04-20 10:06:02.934487 snailshell-0.2.2/snailshell/model_loader.py
+-rw-r--r--   0        0        0     2911 2024-04-20 10:10:34.324285 snailshell-0.2.2/snailshell/pipeline.py
+-rw-r--r--   0        0        0      926 2024-04-20 10:10:17.532711 snailshell-0.2.2/snailshell/utils/port.py
+-rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 snailshell-0.2.2/PKG-INFO
```

### Comparing `snailshell-0.2.1/.github/workflows/ci.yml` & `snailshell-0.2.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/.github/workflows/notification.yaml` & `snailshell-0.2.2/.github/workflows/notification.yaml`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/.gitignore` & `snailshell-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/Makefile` & `snailshell-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/README.md` & `snailshell-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/cd/client.py` & `snailshell-0.2.2/cd/client.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/docs/README-dev.md` & `snailshell-0.2.2/docs/README-dev.md`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/docs/red-snail.png` & `snailshell-0.2.2/docs/red-snail.png`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/examples/mobilenet-v2.pth` & `snailshell-0.2.2/examples/mobilenet-v2.pth`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/examples/test_image.jpg` & `snailshell-0.2.2/examples/test_image.jpg`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/pyproject.toml` & `snailshell-0.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "snailshell"
-version = "0.2.1"
+version = "0.2.2"
 description = "싱크대 자동 수전 절수 시스템"
 authors = [
     {name = "Janghoo Lee", email = "dlwkdgn1@naver.com"},
     {name = "Subin Jang", email = "subinaksl@naver.com"},
     {name = "Seokwoo Ahn", email = "patrick0503@naver.com"},
     {name = "Dahyun Kim", email = "builtforlove@naver.com"},
 ]
```

### Comparing `snailshell-0.2.1/snailshell/main.py` & `snailshell-0.2.2/snailshell/main.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/snailshell/main_test.py` & `snailshell-0.2.2/snailshell/main_test.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/snailshell/model_class.py` & `snailshell-0.2.2/snailshell/model_class.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/snailshell/model_loader.py` & `snailshell-0.2.2/snailshell/model_loader.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/snailshell/pipeline.py` & `snailshell-0.2.2/snailshell/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def run(
     use_pi_camera,
     video_path,
     model_name,
     weight_path,
     visualize,
     target_fps,
-    arduino_port: Union[str, None] = None,
+    arduino_port: Union[str, None] = 'ttyACM0',
 ):
 
     # 모델 로드
     print('모델을 로드합니다.')
     if model_name == "resnet":
         model = ResNetAdapter(weight_path)
     elif model_name == "mobilenet":
```

### Comparing `snailshell-0.2.1/snailshell/utils/port.py` & `snailshell-0.2.2/snailshell/utils/port.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.1/PKG-INFO` & `snailshell-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snailshell
-Version: 0.2.1
+Version: 0.2.2
 Summary: 싱크대 자동 수전 절수 시스템
 Author-email: Janghoo Lee <dlwkdgn1@naver.com>, Subin Jang <subinaksl@naver.com>, Seokwoo Ahn <patrick0503@naver.com>, Dahyun Kim <builtforlove@naver.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: PyYAML
 Requires-Dist: torch
```

