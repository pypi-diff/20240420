# Comparing `tmp/snailshell-0.1.0.tar.gz` & `tmp/snailshell-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snailshell-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "snailshell-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `snailshell-0.1.0.tar` & `snailshell-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      240 2024-03-09 09:58:55.973622 snailshell-0.1.0/.env
--rw-r--r--   0        0        0      699 2024-03-09 09:58:55.973859 snailshell-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      827 2024-03-09 12:00:39.632532 snailshell-0.1.0/.github/workflows/notification.yaml
--rw-r--r--   0        0        0     3816 2024-03-30 09:19:52.985535 snailshell-0.1.0/.gitignore
--rw-r--r--   0        0        0      237 2024-02-24 09:06:57.448971 snailshell-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      754 2024-03-30 09:48:00.075267 snailshell-0.1.0/Makefile
--rw-r--r--   0        0        0      549 2024-03-30 09:46:25.726380 snailshell-0.1.0/README.md
--rw-r--r--   0        0        0     1910 2024-03-09 09:58:55.974586 snailshell-0.1.0/cd/client.py
--rw-r--r--   0        0        0     1701 2024-03-30 09:46:25.726560 snailshell-0.1.0/docs/README-dev.md
--rw-r--r--   0        0        0   162240 2024-03-30 09:46:25.726801 snailshell-0.1.0/docs/red-snail.png
--rw-r--r--   0        0        0  9149096 2024-03-30 09:19:53.021221 snailshell-0.1.0/examples/mobilenet-v2.pth
--rw-r--r--   0        0        0    81588 2024-03-09 07:54:30.014457 snailshell-0.1.0/examples/test_image.jpg
--rw-r--r--   0        0        0     1256 2024-03-30 09:46:25.726987 snailshell-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-30 09:46:25.727046 snailshell-0.1.0/snailshell/__init__.py
--rw-r--r--   0        0        0     2642 2024-03-30 09:45:22.949144 snailshell-0.1.0/snailshell/main.py
--rw-r--r--   0        0        0     3231 2024-03-30 09:19:53.021898 snailshell-0.1.0/snailshell/main_test.py
--rw-r--r--   0        0        0      944 2024-03-30 09:19:53.021972 snailshell-0.1.0/snailshell/model_class.py
--rw-r--r--   0        0        0     2719 2024-03-30 09:45:22.949510 snailshell-0.1.0/snailshell/model_loader.py
--rw-r--r--   0        0        0     2029 2024-03-30 09:45:22.949845 snailshell-0.1.0/snailshell/pipeline.py
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 snailshell-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      240 2024-03-09 09:58:55.973622 snailshell-0.2.0/.env
+-rw-r--r--   0        0        0      699 2024-04-20 09:37:12.452620 snailshell-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      827 2024-03-09 12:00:39.632532 snailshell-0.2.0/.github/workflows/notification.yaml
+-rw-r--r--   0        0        0     3816 2024-03-30 09:19:52.985535 snailshell-0.2.0/.gitignore
+-rw-r--r--   0        0        0      237 2024-02-24 09:06:57.448971 snailshell-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      755 2024-04-20 09:46:00.212809 snailshell-0.2.0/Makefile
+-rw-r--r--   0        0        0      549 2024-03-30 09:46:25.726380 snailshell-0.2.0/README.md
+-rw-r--r--   0        0        0     1910 2024-03-09 09:58:55.974586 snailshell-0.2.0/cd/client.py
+-rw-r--r--   0        0        0     1701 2024-03-30 09:52:24.011423 snailshell-0.2.0/docs/README-dev.md
+-rw-r--r--   0        0        0   162240 2024-03-30 09:46:25.726801 snailshell-0.2.0/docs/red-snail.png
+-rw-r--r--   0        0        0  9149096 2024-03-30 09:19:53.021221 snailshell-0.2.0/examples/mobilenet-v2.pth
+-rw-r--r--   0        0        0    81588 2024-03-09 07:54:30.014457 snailshell-0.2.0/examples/test_image.jpg
+-rw-r--r--   0        0        0     1328 2024-04-20 09:45:49.464842 snailshell-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-30 09:46:25.727046 snailshell-0.2.0/snailshell/__init__.py
+-rw-r--r--   0        0        0     2667 2024-04-20 09:45:15.515026 snailshell-0.2.0/snailshell/main.py
+-rw-r--r--   0        0        0     3231 2024-03-30 09:19:53.021898 snailshell-0.2.0/snailshell/main_test.py
+-rw-r--r--   0        0        0      944 2024-03-30 09:19:53.021972 snailshell-0.2.0/snailshell/model_class.py
+-rw-r--r--   0        0        0     2719 2024-03-30 09:45:22.949510 snailshell-0.2.0/snailshell/model_loader.py
+-rw-r--r--   0        0        0     2899 2024-04-20 09:42:23.964946 snailshell-0.2.0/snailshell/pipeline.py
+-rw-r--r--   0        0        0      926 2024-04-20 09:37:12.453571 snailshell-0.2.0/snailshell/utils/port.py
+-rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 snailshell-0.2.0/PKG-INFO
```

### Comparing `snailshell-0.1.0/.github/workflows/ci.yml` & `snailshell-0.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `snailshell-0.1.0/.github/workflows/notification.yaml` & `snailshell-0.2.0/.github/workflows/notification.yaml`

 * *Files identical despite different names*

### Comparing `snailshell-0.1.0/.gitignore` & `snailshell-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `snailshell-0.1.0/Makefile` & `snailshell-0.2.0/Makefile`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 format:
 	python3 -m yapf -ir .
 
 cd-client:
 	python3 -m cd.client
 
 publish:
-	python3 -m flit publish
+	python3 -m flit publish
```

### Comparing `snailshell-0.1.0/README.md` & `snailshell-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `snailshell-0.1.0/cd/client.py` & `snailshell-0.2.0/cd/client.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.1.0/docs/README-dev.md` & `snailshell-0.2.0/docs/README-dev.md`

 * *Files identical despite different names*

### Comparing `snailshell-0.1.0/docs/red-snail.png` & `snailshell-0.2.0/docs/red-snail.png`

 * *Files identical despite different names*

### Comparing `snailshell-0.1.0/examples/mobilenet-v2.pth` & `snailshell-0.2.0/examples/mobilenet-v2.pth`

 * *Files identical despite different names*

### Comparing `snailshell-0.1.0/examples/test_image.jpg` & `snailshell-0.2.0/examples/test_image.jpg`

 * *Files identical despite different names*

### Comparing `snailshell-0.1.0/pyproject.toml` & `snailshell-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "snailshell"
-version = "0.1.0"
+version = "0.2.0"
 description = "싱크대 자동 수전 절수 시스템"
 authors = [
     {name = "Janghoo Lee", email = "dlwkdgn1@naver.com"},
     {name = "Subin Jang", email = "subinaksl@naver.com"},
     {name = "Seokwoo Ahn", email = "patrick0503@naver.com"},
     {name = "Dahyun Kim", email = "builtforlove@naver.com"},
 ]
@@ -20,16 +20,20 @@
 dependencies = [
     "PyYAML",
     "torch",
     "numpy",
     "torchvision",
     "transformers",
     "opencv-python",
+    "pyserial",
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
@@ -44,8 +48,8 @@
 [tool.yapf]
 indent_width = 4
 based_on_style = 'google'
 COLUMN_LIMIT = 100
 DEDENT_CLOSING_BRACKETS = true
 
 [tool.pylint.FORMAT]
-max-line-length = 100
+max-line-length = 100
```

### Comparing `snailshell-0.1.0/snailshell/main.py` & `snailshell-0.2.0/snailshell/main.py`

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

### Comparing `snailshell-0.1.0/snailshell/main_test.py` & `snailshell-0.2.0/snailshell/main_test.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.1.0/snailshell/model_class.py` & `snailshell-0.2.0/snailshell/model_class.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.1.0/snailshell/model_loader.py` & `snailshell-0.2.0/snailshell/model_loader.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.1.0/snailshell/pipeline.py` & `snailshell-0.2.0/snailshell/pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,44 @@
+# 내장
+import time
+from typing import Union
+
 # 서드파티
 import cv2
 import serial
-import time
 
 # 프로젝트
+from snailshell.utils.port import get_arduino_serial_ports
 from snailshell.model_loader import MobileNetAdapter, ResNetAdapter
 
-py_serial = serial.Serial(
-    '/dev/ttyACM0',
-    9600,
-)
-
 
 def run(
     use_pi_camera,
     video_path,
     model_name,
     weight_path,
     visualize,
     target_fps,
+    arduino_port: Union[str, None],
 ):
 
     # 모델 로드
+    print('모델을 로드합니다.')
     if model_name == "resnet":
         model = ResNetAdapter(weight_path)
     elif model_name == "mobilenet":
         model = MobileNetAdapter(weight_path)
+    print('✅ 모델을 로드했습니다.')
 
     # 비디오 캡처
     if use_pi_camera:
+        print('카메라를 준비합니다.')
         cap = cv2.VideoCapture(0)
     else:
+        print('비디오를 준비합니다.')
         cap = cv2.VideoCapture(video_path)
 
     cap.set(cv2.CAP_PROP_FPS, 50)
 
     # 비디오의 프레임 수, 너비 및 높이 가져오기
     fps = int(cap.get(cv2.CAP_PROP_FPS))
     frame_width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
@@ -42,14 +46,27 @@
 
     print(f'FPS:{fps}')
     print(f'FRAME_Height:{frame_height}')
     print(f'FRAME_Width:{frame_width}')
     frame_interval = int(fps / target_fps)
     frame_count = 0
     predicted_class = -1
+    print('✅ 준비를 마쳤습니다.')
+
+    # 포트 번호를 명시적으로 지정하지 않아도 모르는 기기에서 돌 수 있음
+    print('아두이노 연결을 확인합니다.')
+    while (port := get_arduino_serial_ports(arduino_port)) is None:
+        if port:
+            py_serial = serial.Serial(port, baudrate=9600)
+            print('✅ 아두이노와 연결합니다.')
+            break
+        _t = 1
+        print(f'{_t}초 뒤에 다시 시도합니다...')
+        time.sleep(_t)
+
     while cap.isOpened():
         # 비디오로부터 프레임 읽기
         ret, frame = cap.read()
         if not ret:
             break
 
         frame_count += 1
@@ -59,16 +76,23 @@
             # 프레임을 모델에 전달하여 클래스 예측
             predicted_class = model.predict(frame)
             py_serial.write(str(predicted_class).encode())
 
         if visualize:
             # 예측 클래스를 프레임에 표시
             frame = cv2.resize(frame, (500, 500))
-            cv2.putText(frame, str(predicted_class), (50, 100),
-                        cv2.FONT_HERSHEY_SIMPLEX, 3, (0, 0, 0), 2)
+            cv2.putText(
+                frame,
+                str(predicted_class),
+                (50, 100),
+                cv2.FONT_HERSHEY_SIMPLEX,
+                3,
+                (0, 0, 0),
+                2,
+            )
 
             # 화면에 프레임 표시
             cv2.imshow('Frame', frame)
 
         # 'q'를 누르면 종료
         if cv2.waitKey(1) & 0xFF == ord('q'):
             break
```

### Comparing `snailshell-0.1.0/PKG-INFO` & `snailshell-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: snailshell
-Version: 0.1.0
+Version: 0.2.0
 Summary: 싱크대 자동 수전 절수 시스템
 Author-email: Janghoo Lee <dlwkdgn1@naver.com>, Subin Jang <subinaksl@naver.com>, Seokwoo Ahn <patrick0503@naver.com>, Dahyun Kim <builtforlove@naver.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: PyYAML
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: torchvision
 Requires-Dist: transformers
 Requires-Dist: opencv-python
+Requires-Dist: pyserial
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: pylint ; extra == "dev"
 Requires-Dist: yapf ; extra == "dev"
 Requires-Dist: python-dotenv ; extra == "dev"
 Requires-Dist: requests ; extra == "dev"
 Provides-Extra: dev
```

