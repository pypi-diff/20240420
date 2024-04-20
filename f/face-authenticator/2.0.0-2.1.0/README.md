# Comparing `tmp/face_authenticator-2.0.0-py3-none-any.whl.zip` & `tmp/face_authenticator-2.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4660 bytes, number of entries: 5
--rw-rw-r--  2.0 unx     3224 b- defN 24-Apr-20 16:50 face_authenticator-2.0.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6152 b- defN 24-Apr-20 16:50 face_authenticator-2.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-20 16:50 face_authenticator-2.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 24-Apr-20 16:50 face_authenticator-2.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      440 b- defN 24-Apr-20 16:50 face_authenticator-2.0.0.dist-info/RECORD
-5 files, 9909 bytes uncompressed, 3830 bytes compressed:  61.3%
+Zip file size: 4413 bytes, number of entries: 5
+-rw-rw-r--  2.0 unx     3224 b- defN 24-Apr-20 17:02 face_authenticator-2.1.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5465 b- defN 24-Apr-20 17:02 face_authenticator-2.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-20 17:02 face_authenticator-2.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 24-Apr-20 17:02 face_authenticator-2.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      440 b- defN 24-Apr-20 17:02 face_authenticator-2.1.0.dist-info/RECORD
+5 files, 9222 bytes uncompressed, 3583 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: face_authenticator-2.0.0.dist-info/LICENSE
+Filename: face_authenticator-2.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: face_authenticator-2.0.0.dist-info/METADATA
+Filename: face_authenticator-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: face_authenticator-2.0.0.dist-info/WHEEL
+Filename: face_authenticator-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: face_authenticator-2.0.0.dist-info/top_level.txt
+Filename: face_authenticator-2.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: face_authenticator-2.0.0.dist-info/RECORD
+Filename: face_authenticator-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `face_authenticator-2.0.0.dist-info/LICENSE` & `face_authenticator-2.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `face_authenticator-2.0.0.dist-info/METADATA` & `face_authenticator-2.1.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: face-authenticator
-Version: 2.0.0
+Version: 2.1.0
 Summary: FaceAuthenticator package for face recognition and authentication
 Author: Немтырев Алексей Валерьевич
 Author-email: art.net82@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: face-recognition
 Requires-Dist: numpy
@@ -94,18 +94,14 @@
 - Реализация функции распознавания лиц при организации событий или встреч.
 
 ## Зависимости
 
 - face_recognition: библиотека для распознавания и сравнения лиц.
 - numpy: библиотекадля работы с массивами и матрицами.
 - sqlite3: модуль для работы с SQLite базами данных.
-
-## Вклад и обратная связь
-
-Если вы обнаружили ошибку, имеете предложения по улучшению или хотите внести свой вклад в проект, пожалуйста, создайте issue или pull request на [GitHub](https://github.com/your_username/face_authenticator).
-
-Если у вас есть вопросы или требуется помощь в использовании библиотеки, пожалуйста, свяжитесь со мной по электронной почте [your_email@example.com](mailto:your_email@example.com).
+ 
+Если у вас есть вопросы или требуется помощь в использовании библиотеки, пожалуйста, свяжитесь со мной по электронной почте (mailto:art.net82@gmail.com).
 
 ---
 
 **Уведомление об авторских правах:** Face Authenticator является открытым исходным кодом и распространяется под лицензией MIT. См. файл `LICENSE` для получения дополнительной информации.
-Убедитесь, что в инструкции указаны правильные пути и зависимости, и добавьте свой собственный контактный адрес электронной почты в разделе "Вклад и обратная связь".
+
```

