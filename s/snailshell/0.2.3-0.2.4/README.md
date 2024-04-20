# Comparing `tmp/snailshell-0.2.3.tar.gz` & `tmp/snailshell-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snailshell-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "snailshell-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `snailshell-0.2.3.tar` & `snailshell-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0      240 2024-03-09 09:58:55.973622 snailshell-0.2.3/.env
--rw-r--r--   0        0        0      699 2024-04-20 10:02:19.474963 snailshell-0.2.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      827 2024-03-09 12:00:39.632532 snailshell-0.2.3/.github/workflows/notification.yaml
--rw-r--r--   0        0        0     3816 2024-03-30 09:19:52.985535 snailshell-0.2.3/.gitignore
--rw-r--r--   0        0        0      237 2024-02-24 09:06:57.448971 snailshell-0.2.3/.vscode/settings.json
--rw-r--r--   0        0        0      755 2024-04-20 10:06:02.933095 snailshell-0.2.3/Makefile
--rw-r--r--   0        0        0      549 2024-03-30 09:46:25.726380 snailshell-0.2.3/README.md
--rw-r--r--   0        0        0     1910 2024-03-09 09:58:55.974586 snailshell-0.2.3/cd/client.py
--rw-r--r--   0        0        0     1701 2024-03-30 09:52:24.011423 snailshell-0.2.3/docs/README-dev.md
--rw-r--r--   0        0        0   162240 2024-03-30 09:46:25.726801 snailshell-0.2.3/docs/red-snail.png
--rw-r--r--   0        0        0  9149096 2024-03-30 09:19:53.021221 snailshell-0.2.3/examples/mobilenet-v2.pth
--rw-r--r--   0        0        0    81588 2024-03-09 07:54:30.014457 snailshell-0.2.3/examples/test_image.jpg
--rw-r--r--   0        0        0     1328 2024-04-20 10:12:21.312770 snailshell-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-30 09:46:25.727046 snailshell-0.2.3/snailshell/__init__.py
--rw-r--r--   0        0        0     2667 2024-04-20 10:06:02.933884 snailshell-0.2.3/snailshell/main.py
--rw-r--r--   0        0        0     3231 2024-03-30 09:19:53.021898 snailshell-0.2.3/snailshell/main_test.py
--rw-r--r--   0        0        0      944 2024-03-30 09:19:53.021972 snailshell-0.2.3/snailshell/model_class.py
--rw-r--r--   0        0        0     2719 2024-04-20 10:06:02.934487 snailshell-0.2.3/snailshell/model_loader.py
--rw-r--r--   0        0        0     2916 2024-04-20 10:12:11.604773 snailshell-0.2.3/snailshell/pipeline.py
--rw-r--r--   0        0        0      926 2024-04-20 10:10:17.532711 snailshell-0.2.3/snailshell/utils/port.py
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 snailshell-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      240 2024-03-09 09:58:55.973622 snailshell-0.2.4/.env
+-rw-r--r--   0        0        0      712 2024-04-20 10:13:33.999800 snailshell-0.2.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      827 2024-03-09 12:00:39.632532 snailshell-0.2.4/.github/workflows/notification.yaml
+-rw-r--r--   0        0        0     3816 2024-03-30 09:19:52.985535 snailshell-0.2.4/.gitignore
+-rw-r--r--   0        0        0      237 2024-02-24 09:06:57.448971 snailshell-0.2.4/.vscode/settings.json
+-rw-r--r--   0        0        0      754 2024-04-20 10:13:34.000192 snailshell-0.2.4/Makefile
+-rw-r--r--   0        0        0      549 2024-03-30 09:46:25.726380 snailshell-0.2.4/README.md
+-rw-r--r--   0        0        0     1910 2024-03-09 09:58:55.974586 snailshell-0.2.4/cd/client.py
+-rw-r--r--   0        0        0     1701 2024-03-30 09:52:24.011423 snailshell-0.2.4/docs/README-dev.md
+-rw-r--r--   0        0        0   162240 2024-03-30 09:46:25.726801 snailshell-0.2.4/docs/red-snail.png
+-rw-r--r--   0        0        0  9149096 2024-03-30 09:19:53.021221 snailshell-0.2.4/examples/mobilenet-v2.pth
+-rw-r--r--   0        0        0    81588 2024-03-09 07:54:30.014457 snailshell-0.2.4/examples/test_image.jpg
+-rw-r--r--   0        0        0     1272 2024-04-20 10:13:44.219816 snailshell-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-30 09:46:25.727046 snailshell-0.2.4/snailshell/__init__.py
+-rw-r--r--   0        0        0     2642 2024-04-20 10:13:34.000814 snailshell-0.2.4/snailshell/main.py
+-rw-r--r--   0        0        0     3231 2024-03-30 09:19:53.021898 snailshell-0.2.4/snailshell/main_test.py
+-rw-r--r--   0        0        0      944 2024-03-30 09:19:53.021972 snailshell-0.2.4/snailshell/model_class.py
+-rw-r--r--   0        0        0     2719 2024-04-20 10:06:02.934487 snailshell-0.2.4/snailshell/model_loader.py
+-rw-r--r--   0        0        0     2029 2024-04-20 10:13:34.001102 snailshell-0.2.4/snailshell/pipeline.py
+-rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 snailshell-0.2.4/PKG-INFO
```

### Comparing `snailshell-0.2.3/.github/workflows/ci.yml` & `snailshell-0.2.4/.github/workflows/ci.yml`

 * *Files 17% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: '3.8'
 
       - name: Install dependencies
-        run: make install
+        run: make install-without-venv
 
   lint:
     needs: setup
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
```

### Comparing `snailshell-0.2.3/.github/workflows/notification.yaml` & `snailshell-0.2.4/.github/workflows/notification.yaml`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.3/.gitignore` & `snailshell-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.3/Makefile` & `snailshell-0.2.4/Makefile`

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

### Comparing `snailshell-0.2.3/README.md` & `snailshell-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.3/cd/client.py` & `snailshell-0.2.4/cd/client.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.3/docs/README-dev.md` & `snailshell-0.2.4/docs/README-dev.md`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.3/docs/red-snail.png` & `snailshell-0.2.4/docs/red-snail.png`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.3/examples/mobilenet-v2.pth` & `snailshell-0.2.4/examples/mobilenet-v2.pth`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.3/examples/test_image.jpg` & `snailshell-0.2.4/examples/test_image.jpg`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.3/pyproject.toml` & `snailshell-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "snailshell"
-version = "0.2.3"
+version = "0.2.4"
 description = "싱크대 자동 수전 절수 시스템"
 authors = [
     {name = "Janghoo Lee", email = "dlwkdgn1@naver.com"},
     {name = "Subin Jang", email = "subinaksl@naver.com"},
     {name = "Seokwoo Ahn", email = "patrick0503@naver.com"},
     {name = "Dahyun Kim", email = "builtforlove@naver.com"},
 ]
@@ -23,17 +23,14 @@
     "numpy",
     "torchvision",
     "transformers",
     "opencv-python",
     "pyserial",
 ]
 
-[project.scripts]
-snailshell = "snailshell.main:main"
-
 [project.optional-dependencies]
 dev = [
     "flit",
     "pylint",
     "yapf",
     "python-dotenv",
     "requests",
@@ -48,8 +45,8 @@
 [tool.yapf]
 indent_width = 4
 based_on_style = 'google'
 COLUMN_LIMIT = 100
 DEDENT_CLOSING_BRACKETS = true
 
 [tool.pylint.FORMAT]
-max-line-length = 100
+max-line-length = 100
```

### Comparing `snailshell-0.2.3/snailshell/main.py` & `snailshell-0.2.4/snailshell/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,21 +70,17 @@
 
     if not os.path.exists(args.weight_path):
         raise FileNotFoundError(f"{args.weight_path} 파일이나 디렉토리를 찾을 수 없습니다.")
 
     return args
 
 
-def main():
+if __name__ == '__main__':
     args = parse()
     pipeline.run(
         use_pi_camera=args.use_pi_camera,
         video_path=args.video_path,
         weight_path=args.weight_path,
         model_name=args.model_name,
         visualize=args.visualize,
         target_fps=args.target_fps,
     )
-
-
-if __name__ == '__main__':
-    main()
```

### Comparing `snailshell-0.2.3/snailshell/main_test.py` & `snailshell-0.2.4/snailshell/main_test.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.3/snailshell/model_class.py` & `snailshell-0.2.4/snailshell/model_class.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.3/snailshell/model_loader.py` & `snailshell-0.2.4/snailshell/model_loader.py`

 * *Files identical despite different names*

### Comparing `snailshell-0.2.3/snailshell/pipeline.py` & `snailshell-0.2.4/snailshell/pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,40 @@
-# 내장
-import time
-from typing import Union
-
 # 서드파티
 import cv2
 import serial
+import time
 
 # 프로젝트
-from snailshell.utils.port import get_arduino_serial_ports
 from snailshell.model_loader import MobileNetAdapter, ResNetAdapter
 
+py_serial = serial.Serial(
+    '/dev/ttyACM0',
+    9600,
+)
+
 
 def run(
     use_pi_camera,
     video_path,
     model_name,
     weight_path,
     visualize,
     target_fps,
-    arduino_port: Union[str, None] = '/dev/ttyACM0',
 ):
 
     # 모델 로드
-    print('모델을 로드합니다.')
     if model_name == "resnet":
         model = ResNetAdapter(weight_path)
     elif model_name == "mobilenet":
         model = MobileNetAdapter(weight_path)
-    print('✅ 모델을 로드했습니다.')
 
     # 비디오 캡처
     if use_pi_camera:
-        print('카메라를 준비합니다.')
         cap = cv2.VideoCapture(0)
     else:
-        print('비디오를 준비합니다.')
         cap = cv2.VideoCapture(video_path)
 
     cap.set(cv2.CAP_PROP_FPS, 50)
 
     # 비디오의 프레임 수, 너비 및 높이 가져오기
     fps = int(cap.get(cv2.CAP_PROP_FPS))
     frame_width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
@@ -46,27 +42,14 @@
 
     print(f'FPS:{fps}')
     print(f'FRAME_Height:{frame_height}')
     print(f'FRAME_Width:{frame_width}')
     frame_interval = int(fps / target_fps)
     frame_count = 0
     predicted_class = -1
-    print('✅ 준비를 마쳤습니다.')
-
-    # 포트 번호를 명시적으로 지정하지 않아도 모르는 기기에서 돌 수 있음
-    print('아두이노 연결을 확인합니다.')
-    while (port := get_arduino_serial_ports(arduino_port)) is None:
-        if port:
-            py_serial = serial.Serial(port, baudrate=9600)
-            print('✅ 아두이노와 연결합니다.')
-            break
-        _t = 1
-        print(f'{_t}초 뒤에 다시 시도합니다...')
-        time.sleep(_t)
-
     while cap.isOpened():
         # 비디오로부터 프레임 읽기
         ret, frame = cap.read()
         if not ret:
             break
 
         frame_count += 1
@@ -76,23 +59,16 @@
             # 프레임을 모델에 전달하여 클래스 예측
             predicted_class = model.predict(frame)
             py_serial.write(str(predicted_class).encode())
 
         if visualize:
             # 예측 클래스를 프레임에 표시
             frame = cv2.resize(frame, (500, 500))
-            cv2.putText(
-                frame,
-                str(predicted_class),
-                (50, 100),
-                cv2.FONT_HERSHEY_SIMPLEX,
-                3,
-                (0, 0, 0),
-                2,
-            )
+            cv2.putText(frame, str(predicted_class), (50, 100),
+                        cv2.FONT_HERSHEY_SIMPLEX, 3, (0, 0, 0), 2)
 
             # 화면에 프레임 표시
             cv2.imshow('Frame', frame)
 
         # 'q'를 누르면 종료
         if cv2.waitKey(1) & 0xFF == ord('q'):
             break
```

### Comparing `snailshell-0.2.3/PKG-INFO` & `snailshell-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snailshell
-Version: 0.2.3
+Version: 0.2.4
 Summary: 싱크대 자동 수전 절수 시스템
 Author-email: Janghoo Lee <dlwkdgn1@naver.com>, Subin Jang <subinaksl@naver.com>, Seokwoo Ahn <patrick0503@naver.com>, Dahyun Kim <builtforlove@naver.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: PyYAML
 Requires-Dist: torch
```

