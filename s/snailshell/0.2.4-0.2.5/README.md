# Comparing `tmp/snailshell-0.2.4.tar.gz` & `tmp/snailshell-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snailshell-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "snailshell-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `snailshell-0.2.4.tar` & `snailshell-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      240 2024-03-09 09:58:55.973622 snailshell-0.2.4/.env
--rw-r--r--   0        0        0      712 2024-04-20 10:13:33.999800 snailshell-0.2.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      827 2024-03-09 12:00:39.632532 snailshell-0.2.4/.github/workflows/notification.yaml
--rw-r--r--   0        0        0     3816 2024-03-30 09:19:52.985535 snailshell-0.2.4/.gitignore
--rw-r--r--   0        0        0      237 2024-02-24 09:06:57.448971 snailshell-0.2.4/.vscode/settings.json
--rw-r--r--   0        0        0      754 2024-04-20 10:13:34.000192 snailshell-0.2.4/Makefile
--rw-r--r--   0        0        0      549 2024-03-30 09:46:25.726380 snailshell-0.2.4/README.md
--rw-r--r--   0        0        0     1910 2024-03-09 09:58:55.974586 snailshell-0.2.4/cd/client.py
--rw-r--r--   0        0        0     1701 2024-03-30 09:52:24.011423 snailshell-0.2.4/docs/README-dev.md
--rw-r--r--   0        0        0   162240 2024-03-30 09:46:25.726801 snailshell-0.2.4/docs/red-snail.png
--rw-r--r--   0        0        0  9149096 2024-03-30 09:19:53.021221 snailshell-0.2.4/examples/mobilenet-v2.pth
--rw-r--r--   0        0        0    81588 2024-03-09 07:54:30.014457 snailshell-0.2.4/examples/test_image.jpg
--rw-r--r--   0        0        0     1272 2024-04-20 10:13:44.219816 snailshell-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-30 09:46:25.727046 snailshell-0.2.4/snailshell/__init__.py
--rw-r--r--   0        0        0     2642 2024-04-20 10:13:34.000814 snailshell-0.2.4/snailshell/main.py
--rw-r--r--   0        0        0     3231 2024-03-30 09:19:53.021898 snailshell-0.2.4/snailshell/main_test.py
--rw-r--r--   0        0        0      944 2024-03-30 09:19:53.021972 snailshell-0.2.4/snailshell/model_class.py
--rw-r--r--   0        0        0     2719 2024-04-20 10:06:02.934487 snailshell-0.2.4/snailshell/model_loader.py
--rw-r--r--   0        0        0     2029 2024-04-20 10:13:34.001102 snailshell-0.2.4/snailshell/pipeline.py
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 snailshell-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      240 2024-03-09 09:58:55.973622 snailshell-0.2.5/.env
+-rw-r--r--   0        0        0      712 2024-04-20 10:13:33.999800 snailshell-0.2.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      827 2024-03-09 12:00:39.632532 snailshell-0.2.5/.github/workflows/notification.yaml
+-rw-r--r--   0        0        0     3816 2024-03-30 09:19:52.985535 snailshell-0.2.5/.gitignore
+-rw-r--r--   0        0        0      237 2024-02-24 09:06:57.448971 snailshell-0.2.5/.vscode/settings.json
+-rw-r--r--   0        0        0      754 2024-04-20 10:13:34.000192 snailshell-0.2.5/Makefile
+-rw-r--r--   0        0        0      549 2024-03-30 09:46:25.726380 snailshell-0.2.5/README.md
+-rw-r--r--   0        0        0     1910 2024-03-09 09:58:55.974586 snailshell-0.2.5/cd/client.py
+-rw-r--r--   0        0        0     1701 2024-03-30 09:52:24.011423 snailshell-0.2.5/docs/README-dev.md
+-rw-r--r--   0        0        0   162240 2024-03-30 09:46:25.726801 snailshell-0.2.5/docs/red-snail.png
+-rw-r--r--   0        0        0  9149096 2024-03-30 09:19:53.021221 snailshell-0.2.5/examples/mobilenet-v2.pth
+-rw-r--r--   0        0        0    81588 2024-03-09 07:54:30.014457 snailshell-0.2.5/examples/test_image.jpg
+-rw-r--r--   0        0        0     1327 2024-04-20 10:15:07.292848 snailshell-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-30 09:46:25.727046 snailshell-0.2.5/snailshell/__init__.py
+-rw-r--r--   0        0        0     2667 2024-04-20 10:14:55.499249 snailshell-0.2.5/snailshell/main.py
+-rw-r--r--   0        0        0     3231 2024-03-30 09:19:53.021898 snailshell-0.2.5/snailshell/main_test.py
+-rw-r--r--   0        0        0      944 2024-03-30 09:19:53.021972 snailshell-0.2.5/snailshell/model_class.py
+-rw-r--r--   0        0        0     2719 2024-04-20 10:06:02.934487 snailshell-0.2.5/snailshell/model_loader.py
+-rw-r--r--   0        0        0     2029 2024-04-20 10:13:34.001102 snailshell-0.2.5/snailshell/pipeline.py
+-rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 snailshell-0.2.5/PKG-INFO
```

### Comparing `snailshell-0.2.4/.github/workflows/ci.yml` & `snailshell-0.2.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/.github/workflows/notification.yaml` & `snailshell-0.2.5/.github/workflows/notification.yaml`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/.gitignore` & `snailshell-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/Makefile` & `snailshell-0.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/README.md` & `snailshell-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/cd/client.py` & `snailshell-0.2.5/cd/client.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/docs/README-dev.md` & `snailshell-0.2.5/docs/README-dev.md`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/docs/red-snail.png` & `snailshell-0.2.5/docs/red-snail.png`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/examples/mobilenet-v2.pth` & `snailshell-0.2.5/examples/mobilenet-v2.pth`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/examples/test_image.jpg` & `snailshell-0.2.5/examples/test_image.jpg`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/pyproject.toml` & `snailshell-0.2.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "snailshell"
-version = "0.2.4"
+version = "0.2.5"
 description = "싱크대 자동 수전 절수 시스템"
 authors = [
     {name = "Janghoo Lee", email = "dlwkdgn1@naver.com"},
     {name = "Subin Jang", email = "subinaksl@naver.com"},
     {name = "Seokwoo Ahn", email = "patrick0503@naver.com"},
     {name = "Dahyun Kim", email = "builtforlove@naver.com"},
 ]
@@ -23,14 +23,17 @@
     "numpy",
     "torchvision",
     "transformers",
     "opencv-python",
     "pyserial",
 ]
 
+[project.scripts]
+snailshell = "snailshell.main:main"
+
 [project.optional-dependencies]
 dev = [
     "flit",
     "pylint",
     "yapf",
     "python-dotenv",
     "requests",
```

### Comparing `snailshell-0.2.4/snailshell/main.py` & `snailshell-0.2.5/snailshell/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,17 +70,21 @@
 
     if not os.path.exists(args.weight_path):
         raise FileNotFoundError(f"{args.weight_path} 파일이나 디렉토리를 찾을 수 없습니다.")
 
     return args
 
 
-if __name__ == '__main__':
+def main():
     args = parse()
     pipeline.run(
         use_pi_camera=args.use_pi_camera,
         video_path=args.video_path,
         weight_path=args.weight_path,
         model_name=args.model_name,
         visualize=args.visualize,
         target_fps=args.target_fps,
     )
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `snailshell-0.2.4/snailshell/main_test.py` & `snailshell-0.2.5/snailshell/main_test.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/snailshell/model_class.py` & `snailshell-0.2.5/snailshell/model_class.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/snailshell/model_loader.py` & `snailshell-0.2.5/snailshell/model_loader.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/snailshell/pipeline.py` & `snailshell-0.2.5/snailshell/pipeline.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.4/PKG-INFO` & `snailshell-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snailshell
-Version: 0.2.4
+Version: 0.2.5
 Summary: 싱크대 자동 수전 절수 시스템
 Author-email: Janghoo Lee <dlwkdgn1@naver.com>, Subin Jang <subinaksl@naver.com>, Seokwoo Ahn <patrick0503@naver.com>, Dahyun Kim <builtforlove@naver.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: PyYAML
 Requires-Dist: torch
```

