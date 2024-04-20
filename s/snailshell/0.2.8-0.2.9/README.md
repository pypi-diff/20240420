# Comparing `tmp/snailshell-0.2.8.tar.gz` & `tmp/snailshell-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snailshell-0.2.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "snailshell-0.2.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `snailshell-0.2.8.tar` & `snailshell-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      240 2024-03-09 09:58:55.973622 snailshell-0.2.8/.env
--rw-r--r--   0        0        0      712 2024-04-20 11:12:34.438449 snailshell-0.2.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0      827 2024-03-09 12:00:39.632532 snailshell-0.2.8/.github/workflows/notification.yaml
--rw-r--r--   0        0        0     3816 2024-03-30 09:19:52.985535 snailshell-0.2.8/.gitignore
--rw-r--r--   0        0        0      237 2024-02-24 09:06:57.448971 snailshell-0.2.8/.vscode/settings.json
--rw-r--r--   0        0        0      754 2024-04-20 11:12:26.279991 snailshell-0.2.8/Makefile
--rw-r--r--   0        0        0      549 2024-03-30 09:46:25.726380 snailshell-0.2.8/README.md
--rw-r--r--   0        0        0     1910 2024-03-09 09:58:55.974586 snailshell-0.2.8/cd/client.py
--rw-r--r--   0        0        0     1701 2024-03-30 09:52:24.011423 snailshell-0.2.8/docs/README-dev.md
--rw-r--r--   0        0        0   162240 2024-03-30 09:46:25.726801 snailshell-0.2.8/docs/red-snail.png
--rw-r--r--   0        0        0  9149096 2024-03-30 09:19:53.021221 snailshell-0.2.8/examples/mobilenet-v2.pth
--rw-r--r--   0        0        0    81588 2024-03-09 07:54:30.014457 snailshell-0.2.8/examples/test_image.jpg
--rw-r--r--   0        0        0     1327 2024-04-20 12:13:29.800805 snailshell-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-30 09:46:25.727046 snailshell-0.2.8/snailshell/__init__.py
--rw-r--r--   0        0        0     2667 2024-04-20 11:38:01.673226 snailshell-0.2.8/snailshell/main.py
--rw-r--r--   0        0        0     3231 2024-03-30 09:19:53.021898 snailshell-0.2.8/snailshell/main_test.py
--rw-r--r--   0        0        0      944 2024-03-30 09:19:53.021972 snailshell-0.2.8/snailshell/model_class.py
--rw-r--r--   0        0        0     2719 2024-04-20 10:06:02.934487 snailshell-0.2.8/snailshell/model_loader.py
--rw-r--r--   0        0        0     2550 2024-04-20 12:13:21.754171 snailshell-0.2.8/snailshell/pipeline.py
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 snailshell-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      240 2024-03-09 09:58:55.973622 snailshell-0.2.9/.env
+-rw-r--r--   0        0        0      712 2024-04-20 11:12:34.438449 snailshell-0.2.9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      827 2024-03-09 12:00:39.632532 snailshell-0.2.9/.github/workflows/notification.yaml
+-rw-r--r--   0        0        0     3816 2024-03-30 09:19:52.985535 snailshell-0.2.9/.gitignore
+-rw-r--r--   0        0        0      237 2024-02-24 09:06:57.448971 snailshell-0.2.9/.vscode/settings.json
+-rw-r--r--   0        0        0      754 2024-04-20 11:12:26.279991 snailshell-0.2.9/Makefile
+-rw-r--r--   0        0        0      549 2024-03-30 09:46:25.726380 snailshell-0.2.9/README.md
+-rw-r--r--   0        0        0     1910 2024-03-09 09:58:55.974586 snailshell-0.2.9/cd/client.py
+-rw-r--r--   0        0        0     1701 2024-03-30 09:52:24.011423 snailshell-0.2.9/docs/README-dev.md
+-rw-r--r--   0        0        0   162240 2024-03-30 09:46:25.726801 snailshell-0.2.9/docs/red-snail.png
+-rw-r--r--   0        0        0  9149096 2024-03-30 09:19:53.021221 snailshell-0.2.9/examples/mobilenet-v2.pth
+-rw-r--r--   0        0        0    81588 2024-03-09 07:54:30.014457 snailshell-0.2.9/examples/test_image.jpg
+-rw-r--r--   0        0        0     1327 2024-04-20 12:15:35.364109 snailshell-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-30 09:46:25.727046 snailshell-0.2.9/snailshell/__init__.py
+-rw-r--r--   0        0        0     2965 2024-04-20 12:15:15.998670 snailshell-0.2.9/snailshell/main.py
+-rw-r--r--   0        0        0     3231 2024-03-30 09:19:53.021898 snailshell-0.2.9/snailshell/main_test.py
+-rw-r--r--   0        0        0      944 2024-03-30 09:19:53.021972 snailshell-0.2.9/snailshell/model_class.py
+-rw-r--r--   0        0        0     2719 2024-04-20 10:06:02.934487 snailshell-0.2.9/snailshell/model_loader.py
+-rw-r--r--   0        0        0     2627 2024-04-20 12:15:19.473253 snailshell-0.2.9/snailshell/pipeline.py
+-rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 snailshell-0.2.9/PKG-INFO
```

### Comparing `snailshell-0.2.8/.github/workflows/ci.yml` & `snailshell-0.2.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.8/.github/workflows/notification.yaml` & `snailshell-0.2.9/.github/workflows/notification.yaml`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.8/.gitignore` & `snailshell-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.8/Makefile` & `snailshell-0.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.8/README.md` & `snailshell-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.8/cd/client.py` & `snailshell-0.2.9/cd/client.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.8/docs/README-dev.md` & `snailshell-0.2.9/docs/README-dev.md`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.8/docs/red-snail.png` & `snailshell-0.2.9/docs/red-snail.png`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.8/examples/mobilenet-v2.pth` & `snailshell-0.2.9/examples/mobilenet-v2.pth`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.8/examples/test_image.jpg` & `snailshell-0.2.9/examples/test_image.jpg`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.8/pyproject.toml` & `snailshell-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "snailshell"
-version = "0.2.8"
+version = "0.2.9"
 description = "싱크대 자동 수전 절수 시스템"
 authors = [
     {name = "Janghoo Lee", email = "dlwkdgn1@naver.com"},
     {name = "Subin Jang", email = "subinaksl@naver.com"},
     {name = "Seokwoo Ahn", email = "patrick0503@naver.com"},
     {name = "Dahyun Kim", email = "builtforlove@naver.com"},
 ]
```

### Comparing `snailshell-0.2.8/snailshell/main.py` & `snailshell-0.2.9/snailshell/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,19 @@
     # 프레임 수를 처리하기 위한 새로운 인자 추가
     parser.add_argument(
         '--target_fps',
         type=int,
         help='최대 초당 프레임 처리량. 단, 이 값이 높아도 실제 처리량은 하드웨어 성능에 의존적입니다.',
         default=10,
     )
-
+    parser.add_argument(
+        '--without_arduino',
+        action='store_true',
+        help='아두이노 없이도 프로그램을 실행할 수 있습니다. 이 옵션을 사용하면 아두이노 관련 기능이 비활성화됩니다.',
+    )
     args = parser.parse_args()
 
     # 라즈베리파이 카메라를 사용하지 않을 경우 비디오 경로가 필수
     if not args.use_pi_camera:
         if not args.video_path:
             raise ValueError('카메라를 사용하지 않는 경우 `--video_path` 가 필수적입니다.')
         elif not os.path.exists(args.video_path):
@@ -79,12 +83,13 @@
     pipeline.run(
         use_pi_camera=args.use_pi_camera,
         video_path=args.video_path,
         weight_path=args.weight_path,
         model_name=args.model_name,
         visualize=args.visualize,
         target_fps=args.target_fps,
+        use_arduino=(not args.without_arduino)
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `snailshell-0.2.8/snailshell/main_test.py` & `snailshell-0.2.9/snailshell/main_test.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.8/snailshell/model_class.py` & `snailshell-0.2.9/snailshell/model_class.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.8/snailshell/model_loader.py` & `snailshell-0.2.9/snailshell/model_loader.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.8/snailshell/pipeline.py` & `snailshell-0.2.9/snailshell/pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 import cv2
 import serial
 import time
 
 # 프로젝트
 from snailshell.model_loader import MobileNetAdapter, ResNetAdapter
 
-py_serial = serial.Serial('/dev/ttyACM0', 9600)
-
 
 def run(
     use_pi_camera,
     video_path,
     model_name,
     weight_path,
     visualize,
     target_fps,
+    use_arduino,
 ):
+    if use_arduino:
+        py_serial = serial.Serial('/dev/ttyACM0', 9600)
 
     print('모델을 로드합니다.')
     if model_name == "resnet":
         model = ResNetAdapter(weight_path)
     elif model_name == "mobilenet":
         model = MobileNetAdapter(weight_path)
 
@@ -60,15 +61,17 @@
 
         frame_count += 1
         if frame_count == frame_interval:
             frame_count = 0
 
             # 프레임을 모델에 전달하여 클래스 예측
             predicted_class = model.predict(frame)
-            py_serial.write(str(predicted_class).encode())
+
+            if use_arduino:
+                py_serial.write(str(predicted_class).encode())
 
         if visualize:
             # 예측 클래스를 프레임에 표시
             frame = cv2.resize(frame, (500, 500))
             cv2.putText(
                 frame,
                 text=str(predicted_class),
```

### Comparing `snailshell-0.2.8/PKG-INFO` & `snailshell-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snailshell
-Version: 0.2.8
+Version: 0.2.9
 Summary: 싱크대 자동 수전 절수 시스템
 Author-email: Janghoo Lee <dlwkdgn1@naver.com>, Subin Jang <subinaksl@naver.com>, Seokwoo Ahn <patrick0503@naver.com>, Dahyun Kim <builtforlove@naver.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: PyYAML
 Requires-Dist: torch
```

