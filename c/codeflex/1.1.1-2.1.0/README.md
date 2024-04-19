# Comparing `tmp/codeflex-1.1.1.tar.gz` & `tmp/codeflex-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflex-1.1.1.tar", last modified: Thu Apr 18 19:33:13 2024, max compression
+gzip compressed data, was "codeflex-2.1.0.tar", last modified: Fri Apr 19 22:00:41 2024, max compression
```

## Comparing `codeflex-1.1.1.tar` & `codeflex-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 19:33:13.947872 codeflex-1.1.1/
--rw-rw-rw-   0        0        0     1913 2024-04-18 01:41:25.000000 codeflex-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     5197 2024-04-18 19:33:13.932250 codeflex-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4364 2024-04-18 19:27:19.000000 codeflex-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 19:33:13.947872 codeflex-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1021 2024-04-18 19:31:48.000000 codeflex-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:33:13.822901 codeflex-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 19:33:13.854143 codeflex-1.1.1/src/codeflex/
--rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-1.1.1/src/codeflex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:33:13.932250 codeflex-1.1.1/src/codeflex/company/
--rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-1.1.1/src/codeflex/company/__init__.py
--rw-rw-rw-   0        0        0     6303 2024-04-18 19:18:54.000000 codeflex-1.1.1/src/codeflex/company/mysql.py
--rw-rw-rw-   0        0        0     5782 2024-04-18 01:26:43.000000 codeflex-1.1.1/src/codeflex/mysql.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:33:13.932250 codeflex-1.1.1/src/codeflex.egg-info/
--rw-rw-rw-   0        0        0     5197 2024-04-18 19:33:13.000000 codeflex-1.1.1/src/codeflex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-18 19:33:13.000000 codeflex-1.1.1/src/codeflex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 19:33:13.000000 codeflex-1.1.1/src/codeflex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-18 19:33:13.000000 codeflex-1.1.1/src/codeflex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 22:00:41.808132 codeflex-2.1.0/
+-rw-rw-rw-   0        0        0     1913 2024-04-18 01:41:25.000000 codeflex-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     6238 2024-04-19 22:00:41.792514 codeflex-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5362 2024-04-19 21:58:32.000000 codeflex-2.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 22:00:41.808132 codeflex-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2024-04-19 21:48:45.000000 codeflex-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 22:00:41.745647 codeflex-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 22:00:41.761269 codeflex-2.1.0/src/codeflex/
+-rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-2.1.0/src/codeflex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 22:00:41.792514 codeflex-2.1.0/src/codeflex/company/
+-rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-2.1.0/src/codeflex/company/__init__.py
+-rw-rw-rw-   0        0        0     6303 2024-04-18 19:18:54.000000 codeflex-2.1.0/src/codeflex/company/mysql.py
+-rw-rw-rw-   0        0        0     1217 2024-04-19 18:42:33.000000 codeflex-2.1.0/src/codeflex/company/polly.py
+drwxrwxrwx   0        0        0        0 2024-04-19 22:00:41.792514 codeflex-2.1.0/src/codeflex.egg-info/
+-rw-rw-rw-   0        0        0     6238 2024-04-19 22:00:41.000000 codeflex-2.1.0/src/codeflex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-04-19 22:00:41.000000 codeflex-2.1.0/src/codeflex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 22:00:41.000000 codeflex-2.1.0/src/codeflex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-19 22:00:41.000000 codeflex-2.1.0/src/codeflex.egg-info/top_level.txt
```

### Comparing `codeflex-1.1.1/LICENSE` & `codeflex-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflex-1.1.1/PKG-INFO` & `codeflex-2.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: codeflex
-Version: 1.1.1
-Summary: ¡Consulta tus bases de datos MySQL con CodeFlex!
+Version: 2.1.0
+Summary: ¡Conecta a los Microservicios de CodeFlex desde una Sola Librería!
 Home-page: https://codeflex.com.co/
 Author: CODEFLEX S.A.S.
 Author-email: info@codeflex.com.co
 License: This software is owned by CodeFlex S.A.S. and is protected by applicable copyright laws. The distribution and use of this software are subject to the terms and conditions outlined below.
 Project-URL: Bug Tracker, https://docs.codeflex.com.co/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -55,15 +55,15 @@
 ```python
 pip install codeflex
 ```
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
-* Example 1
+* Example 1 | Connection to MySQL
     ```python
     from codeflex.company import mysql
 
     respuesta = mysql.CONNECTOR("your_user", "your_password","your_database", "your_SQL") #Usuario , Contraseña, Base de datos, Cualquier Sql (Actualiza, Elimina, Consulta, Inserta) SOLO TABLAS
     print(respuesta)
 
 
@@ -107,20 +107,44 @@
     print(respuesta)
  
  
     respuesta = mysql.DBQUERY("your_user", "your_password") #Usuario y Contraseña
     print(respuesta)
 
     ```
+ 
+
+* Example 2 | Connection to Polly
+    ```python
+    from codeflex.company import polly
+
+    Text = "Prueba Final"
+    VoiceId = "Lupe" # Para cambiar el VoiceId y LanguageCode, consulta la documentación. | API de Conexión a Polly
+    LanguageCode = "es-US"
+    TokenSub = "Your_TokenSub" # Para acceder a este servicio, utiliza tu TokenSub, que es un identificador único por cuenta y es necesario que pertenezcas al plan premium. | https://codeflex.com.co/drive/index.html#/Polly
+
+    respuesta = polly.AUDIODATA(Text, VoiceId,LanguageCode,TokenSub)
+    print(respuesta)
+    # Respuesta: {"audioData": "SUQzBAAAAAAAI1RTU0UAAAAPAAADTGF2ZjU4Ljc2LjEwMAAAAAAAAAAAAAAA//EzfNsySGqKm/lCw0GpvBJAAwWmuAVDjr+V"} Base64
+
+
+    respuesta = polly.DOWNLOAD(Text, VoiceId,LanguageCode,TokenSub)
+    print(respuesta)
+    # Respuesta: {'audioUrl': 'https://s3.amazonaws.com/hub.codeflex.lat/audioStream_1713562991794.mp3'}
+
+    ```
+
+
+_For more examples, please refer to the [Documentation](https://docs.codeflex.com.co/docs-page.html#section-3)_
 
-_For more examples, please refer to the [Examples packages](https://docs.codeflex.com.co/docs-page.html#section-3)_
+_[CODEFLEX S.A.S.](https://codeflex.com.co/)_
 
-_[Database](http://mysql.codeflex.com.co/)_
+_[Database Mysql](http://mysql.codeflex.com.co/)_
 
-_[Create Account](https://codeflex.com.co/drive/index.html#/phpMyAdmin)_
+_[Create Account Mysql](https://codeflex.com.co/drive/index.html#/phpMyAdmin)_
 
 <!-- LICENSE -->
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <!-- CONTACT -->
```

#### html2text {}

```diff
@@ -1,62 +1,76 @@
-Metadata-Version: 2.1 Name: codeflex Version: 1.1.1 Summary: Â¡Consulta tus
-bases de datos MySQL con CodeFlex! Home-page: https://codeflex.com.co/ Author:
-CODEFLEX S.A.S. Author-email: info@codeflex.com.co License: This software is
-owned by CodeFlex S.A.S. and is protected by applicable copyright laws. The
-distribution and use of this software are subject to the terms and conditions
-outlined below. Project-URL: Bug Tracker, https://docs.codeflex.com.co/
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE [![MIT License][license-shield]](https://s3.amazonaws.com/
-www.codeflex.lat/documentos/c3320017-1937-4353-8881-475e3c89e25e/LICENSE.txt)
+Metadata-Version: 2.1 Name: codeflex Version: 2.1.0 Summary: Â¡Conecta a los
+Microservicios de CodeFlex desde una Sola LibrerÃ­a! Home-page: https://
+codeflex.com.co/ Author: CODEFLEX S.A.S. Author-email: info@codeflex.com.co
+License: This software is owned by CodeFlex S.A.S. and is protected by
+applicable copyright laws. The distribution and use of this software are
+subject to the terms and conditions outlined below. Project-URL: Bug Tracker,
+https://docs.codeflex.com.co/ Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE [![MIT License][license-shield]](https://
+s3.amazonaws.com/www.codeflex.lat/documentos/c3320017-1937-4353-8881-
+475e3c89e25e/LICENSE.txt)
                                     _[_L_o_g_o_]
                            ******** CCOODDEEFFLLEEXX SS..AA..SS.. ********
               CodificaciÃ³n y Almacenamiento Simplificados | IDE
                               _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 ## About The Project [![miniatura][miniatura]](https://codeflex.com.co) ##
 Getting Started ### Prerequisites You need to make sure you have installed the
 following modules. * Requests ```s pip install requests ``` ### Installation
-```python pip install codeflex ``` ## Usage * Example 1 ```python from
-codeflex.company import mysql respuesta = mysql.CONNECTOR("your_user",
-"your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
-datos, Cualquier Sql (Actualiza, Elimina, Consulta, Inserta) SOLO TABLAS print
-(respuesta) respuesta = mysql.UPDATETABLE_CUSTOM("your_user",
-"your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
-datos, Sql print(respuesta) respuesta = mysql.DELETETABLE_CUSTOM("your_user",
-"your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
-datos, Sql print(respuesta) respuesta = mysql.DELETETABLE("your_user",
-"your_password","your_database", "your_tablename") #Usuario , ContraseÃ±a, Base
-de datos, Nombre de la tabla print(respuesta) respuesta =
-mysql.TABLEINSERT_CUSTOM("your_user", "your_password","your_database",
+```python pip install codeflex ``` ## Usage * Example 1 | Connection to MySQL
+```python from codeflex.company import mysql respuesta = mysql.CONNECTOR
+("your_user", "your_password","your_database", "your_SQL") #Usuario ,
+ContraseÃ±a, Base de datos, Cualquier Sql (Actualiza, Elimina, Consulta,
+Inserta) SOLO TABLAS print(respuesta) respuesta = mysql.UPDATETABLE_CUSTOM
+("your_user", "your_password","your_database", "your_SQL") #Usuario ,
+ContraseÃ±a, Base de datos, Sql print(respuesta) respuesta =
+mysql.DELETETABLE_CUSTOM("your_user", "your_password","your_database",
 "your_SQL") #Usuario , ContraseÃ±a, Base de datos, Sql print(respuesta)
-respuesta = mysql.TABLEQUERY_CUSTOM("your_user",
+respuesta = mysql.DELETETABLE("your_user", "your_password","your_database",
+"your_tablename") #Usuario , ContraseÃ±a, Base de datos, Nombre de la tabla
+print(respuesta) respuesta = mysql.TABLEINSERT_CUSTOM("your_user",
+"your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
+datos, Sql print(respuesta) respuesta = mysql.TABLEQUERY_CUSTOM("your_user",
 "your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
 datos, Sql print(respuesta) respuesta = mysql.TABLEQUERY("your_user",
 "your_password","your_database", "your_tablename") #Usuario , ContraseÃ±a, Base
 de datos, Nombre de la tabla print(respuesta) respuesta =
 mysql.CREATETABLE_CUSTOM("your_user", "your_password","your_database",
 "your_SQL") #Usuario , ContraseÃ±a, Base de datos, Sql print(respuesta)
 respuesta = mysql.CREATETABLE("your_user", "your_password","your_database",
 "your_tablename") #Usuario , ContraseÃ±a, Base de datos, Nombre de la tabla
 print(respuesta) respuesta = mysql.DELETEDB("your_user", "your_database")
 #Usuario y Base de datos print(respuesta) respuesta = mysql.CREATEDB
 ("your_user", "your_database") #Usuario y Base de datos print(respuesta)
 respuesta = mysql.DBQUERY("your_user", "your_password") #Usuario y ContraseÃ±a
-print(respuesta) ``` _For more examples, please refer to the [Examples
-packages](https://docs.codeflex.com.co/docs-page.html#section-3)_ _[Database]
-(http://mysql.codeflex.com.co/)_ _[Create Account](https://codeflex.com.co/
-drive/index.html#/phpMyAdmin)_ ## License Distributed under the MIT License.
-See `LICENSE` for more information. ## Contact Telefono: 3008130562 | Email:
-info@codeflex.com.co [contributors-shield]: https://img.shields.io/github/
-contributors/avmmodules/AVMWeather.svg?style=for-the-badge [contributors-url]:
-https://github.com/avmmodules/AVMWeather/graphs/contributors [forks-shield]:
-https://img.shields.io/github/forks/avmmodules/AVMWeather.svg?style=for-the-
-badge [forks-url]: https://github.com/avmmodules/AVMWeather/network/members
-[stars-shield]: https://img.shields.io/github/stars/avmmodules/
+print(respuesta) ``` * Example 2 | Connection to Polly ```python from
+codeflex.company import polly Text = "Prueba Final" VoiceId = "Lupe" # Para
+cambiar el VoiceId y LanguageCode, consulta la documentaciÃ³n. | API de
+ConexiÃ³n a Polly LanguageCode = "es-US" TokenSub = "Your_TokenSub" # Para
+acceder a este servicio, utiliza tu TokenSub, que es un identificador Ãºnico
+por cuenta y es necesario que pertenezcas al plan premium. | https://
+codeflex.com.co/drive/index.html#/Polly respuesta = polly.AUDIODATA(Text,
+VoiceId,LanguageCode,TokenSub) print(respuesta) # Respuesta: {"audioData":
+"SUQzBAAAAAAAI1RTU0UAAAAPAAADTGF2ZjU4Ljc2LjEwMAAAAAAAAAAAAAAA//EzfNsySGqKm/
+lCw0GpvBJAAwWmuAVDjr+V"} Base64 respuesta = polly.DOWNLOAD(Text,
+VoiceId,LanguageCode,TokenSub) print(respuesta) # Respuesta: {'audioUrl':
+'https://s3.amazonaws.com/hub.codeflex.lat/audioStream_1713562991794.mp3'} ```
+_For more examples, please refer to the [Documentation](https://
+docs.codeflex.com.co/docs-page.html#section-3)_ _[CODEFLEX S.A.S.](https://
+codeflex.com.co/)_ _[Database Mysql](http://mysql.codeflex.com.co/)_ _[Create
+Account Mysql](https://codeflex.com.co/drive/index.html#/phpMyAdmin)_ ##
+License Distributed under the MIT License. See `LICENSE` for more information.
+## Contact Telefono: 3008130562 | Email: info@codeflex.com.co [contributors-
+shield]: https://img.shields.io/github/contributors/avmmodules/
+AVMWeather.svg?style=for-the-badge [contributors-url]: https://github.com/
+avmmodules/AVMWeather/graphs/contributors [forks-shield]: https://
+img.shields.io/github/forks/avmmodules/AVMWeather.svg?style=for-the-badge
+[forks-url]: https://github.com/avmmodules/AVMWeather/network/members [stars-
+shield]: https://img.shields.io/github/stars/avmmodules/
 AVMWeather.svg?style=for-the-badge [stars-url]: https://github.com/avmmodules/
 AVMWeather/stargazers [issues-shield]: https://img.shields.io/github/issues/
 avmmodules/AVMWeather.svg?style=for-the-badge [issues-url]: https://github.com/
 avmmodules/AVMWeather/issues [license-shield]: https://img.shields.io/github/
 license/avmmodules/AVMWeather.svg?style=for-the-badge [license-url]: https://
 github.com/avmmodules/AVMWeather/blob/main/LICENSE [miniatura]: https://
 codeflex.com.co/assets/img/ggg.webp
```

### Comparing `codeflex-1.1.1/README.md` & `codeflex-2.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 ```python
 pip install codeflex
 ```
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
-* Example 1
+* Example 1 | Connection to MySQL
     ```python
     from codeflex.company import mysql
 
     respuesta = mysql.CONNECTOR("your_user", "your_password","your_database", "your_SQL") #Usuario , Contraseña, Base de datos, Cualquier Sql (Actualiza, Elimina, Consulta, Inserta) SOLO TABLAS
     print(respuesta)
 
 
@@ -91,20 +91,44 @@
     print(respuesta)
  
  
     respuesta = mysql.DBQUERY("your_user", "your_password") #Usuario y Contraseña
     print(respuesta)
 
     ```
+ 
+
+* Example 2 | Connection to Polly
+    ```python
+    from codeflex.company import polly
+
+    Text = "Prueba Final"
+    VoiceId = "Lupe" # Para cambiar el VoiceId y LanguageCode, consulta la documentación. | API de Conexión a Polly
+    LanguageCode = "es-US"
+    TokenSub = "Your_TokenSub" # Para acceder a este servicio, utiliza tu TokenSub, que es un identificador único por cuenta y es necesario que pertenezcas al plan premium. | https://codeflex.com.co/drive/index.html#/Polly
+
+    respuesta = polly.AUDIODATA(Text, VoiceId,LanguageCode,TokenSub)
+    print(respuesta)
+    # Respuesta: {"audioData": "SUQzBAAAAAAAI1RTU0UAAAAPAAADTGF2ZjU4Ljc2LjEwMAAAAAAAAAAAAAAA//EzfNsySGqKm/lCw0GpvBJAAwWmuAVDjr+V"} Base64
+
+
+    respuesta = polly.DOWNLOAD(Text, VoiceId,LanguageCode,TokenSub)
+    print(respuesta)
+    # Respuesta: {'audioUrl': 'https://s3.amazonaws.com/hub.codeflex.lat/audioStream_1713562991794.mp3'}
+
+    ```
+
+
+_For more examples, please refer to the [Documentation](https://docs.codeflex.com.co/docs-page.html#section-3)_
 
-_For more examples, please refer to the [Examples packages](https://docs.codeflex.com.co/docs-page.html#section-3)_
+_[CODEFLEX S.A.S.](https://codeflex.com.co/)_
 
-_[Database](http://mysql.codeflex.com.co/)_
+_[Database Mysql](http://mysql.codeflex.com.co/)_
 
-_[Create Account](https://codeflex.com.co/drive/index.html#/phpMyAdmin)_
+_[Create Account Mysql](https://codeflex.com.co/drive/index.html#/phpMyAdmin)_
 
 <!-- LICENSE -->
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <!-- CONTACT -->
```

#### html2text {}

```diff
@@ -3,51 +3,64 @@
                                     _[_L_o_g_o_]
                            ******** CCOODDEEFFLLEEXX SS..AA..SS.. ********
               CodificaciÃ³n y Almacenamiento Simplificados | IDE
                               _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 ## About The Project [![miniatura][miniatura]](https://codeflex.com.co) ##
 Getting Started ### Prerequisites You need to make sure you have installed the
 following modules. * Requests ```s pip install requests ``` ### Installation
-```python pip install codeflex ``` ## Usage * Example 1 ```python from
-codeflex.company import mysql respuesta = mysql.CONNECTOR("your_user",
-"your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
-datos, Cualquier Sql (Actualiza, Elimina, Consulta, Inserta) SOLO TABLAS print
-(respuesta) respuesta = mysql.UPDATETABLE_CUSTOM("your_user",
-"your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
-datos, Sql print(respuesta) respuesta = mysql.DELETETABLE_CUSTOM("your_user",
-"your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
-datos, Sql print(respuesta) respuesta = mysql.DELETETABLE("your_user",
-"your_password","your_database", "your_tablename") #Usuario , ContraseÃ±a, Base
-de datos, Nombre de la tabla print(respuesta) respuesta =
-mysql.TABLEINSERT_CUSTOM("your_user", "your_password","your_database",
+```python pip install codeflex ``` ## Usage * Example 1 | Connection to MySQL
+```python from codeflex.company import mysql respuesta = mysql.CONNECTOR
+("your_user", "your_password","your_database", "your_SQL") #Usuario ,
+ContraseÃ±a, Base de datos, Cualquier Sql (Actualiza, Elimina, Consulta,
+Inserta) SOLO TABLAS print(respuesta) respuesta = mysql.UPDATETABLE_CUSTOM
+("your_user", "your_password","your_database", "your_SQL") #Usuario ,
+ContraseÃ±a, Base de datos, Sql print(respuesta) respuesta =
+mysql.DELETETABLE_CUSTOM("your_user", "your_password","your_database",
 "your_SQL") #Usuario , ContraseÃ±a, Base de datos, Sql print(respuesta)
-respuesta = mysql.TABLEQUERY_CUSTOM("your_user",
+respuesta = mysql.DELETETABLE("your_user", "your_password","your_database",
+"your_tablename") #Usuario , ContraseÃ±a, Base de datos, Nombre de la tabla
+print(respuesta) respuesta = mysql.TABLEINSERT_CUSTOM("your_user",
+"your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
+datos, Sql print(respuesta) respuesta = mysql.TABLEQUERY_CUSTOM("your_user",
 "your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
 datos, Sql print(respuesta) respuesta = mysql.TABLEQUERY("your_user",
 "your_password","your_database", "your_tablename") #Usuario , ContraseÃ±a, Base
 de datos, Nombre de la tabla print(respuesta) respuesta =
 mysql.CREATETABLE_CUSTOM("your_user", "your_password","your_database",
 "your_SQL") #Usuario , ContraseÃ±a, Base de datos, Sql print(respuesta)
 respuesta = mysql.CREATETABLE("your_user", "your_password","your_database",
 "your_tablename") #Usuario , ContraseÃ±a, Base de datos, Nombre de la tabla
 print(respuesta) respuesta = mysql.DELETEDB("your_user", "your_database")
 #Usuario y Base de datos print(respuesta) respuesta = mysql.CREATEDB
 ("your_user", "your_database") #Usuario y Base de datos print(respuesta)
 respuesta = mysql.DBQUERY("your_user", "your_password") #Usuario y ContraseÃ±a
-print(respuesta) ``` _For more examples, please refer to the [Examples
-packages](https://docs.codeflex.com.co/docs-page.html#section-3)_ _[Database]
-(http://mysql.codeflex.com.co/)_ _[Create Account](https://codeflex.com.co/
-drive/index.html#/phpMyAdmin)_ ## License Distributed under the MIT License.
-See `LICENSE` for more information. ## Contact Telefono: 3008130562 | Email:
-info@codeflex.com.co [contributors-shield]: https://img.shields.io/github/
-contributors/avmmodules/AVMWeather.svg?style=for-the-badge [contributors-url]:
-https://github.com/avmmodules/AVMWeather/graphs/contributors [forks-shield]:
-https://img.shields.io/github/forks/avmmodules/AVMWeather.svg?style=for-the-
-badge [forks-url]: https://github.com/avmmodules/AVMWeather/network/members
-[stars-shield]: https://img.shields.io/github/stars/avmmodules/
+print(respuesta) ``` * Example 2 | Connection to Polly ```python from
+codeflex.company import polly Text = "Prueba Final" VoiceId = "Lupe" # Para
+cambiar el VoiceId y LanguageCode, consulta la documentaciÃ³n. | API de
+ConexiÃ³n a Polly LanguageCode = "es-US" TokenSub = "Your_TokenSub" # Para
+acceder a este servicio, utiliza tu TokenSub, que es un identificador Ãºnico
+por cuenta y es necesario que pertenezcas al plan premium. | https://
+codeflex.com.co/drive/index.html#/Polly respuesta = polly.AUDIODATA(Text,
+VoiceId,LanguageCode,TokenSub) print(respuesta) # Respuesta: {"audioData":
+"SUQzBAAAAAAAI1RTU0UAAAAPAAADTGF2ZjU4Ljc2LjEwMAAAAAAAAAAAAAAA//EzfNsySGqKm/
+lCw0GpvBJAAwWmuAVDjr+V"} Base64 respuesta = polly.DOWNLOAD(Text,
+VoiceId,LanguageCode,TokenSub) print(respuesta) # Respuesta: {'audioUrl':
+'https://s3.amazonaws.com/hub.codeflex.lat/audioStream_1713562991794.mp3'} ```
+_For more examples, please refer to the [Documentation](https://
+docs.codeflex.com.co/docs-page.html#section-3)_ _[CODEFLEX S.A.S.](https://
+codeflex.com.co/)_ _[Database Mysql](http://mysql.codeflex.com.co/)_ _[Create
+Account Mysql](https://codeflex.com.co/drive/index.html#/phpMyAdmin)_ ##
+License Distributed under the MIT License. See `LICENSE` for more information.
+## Contact Telefono: 3008130562 | Email: info@codeflex.com.co [contributors-
+shield]: https://img.shields.io/github/contributors/avmmodules/
+AVMWeather.svg?style=for-the-badge [contributors-url]: https://github.com/
+avmmodules/AVMWeather/graphs/contributors [forks-shield]: https://
+img.shields.io/github/forks/avmmodules/AVMWeather.svg?style=for-the-badge
+[forks-url]: https://github.com/avmmodules/AVMWeather/network/members [stars-
+shield]: https://img.shields.io/github/stars/avmmodules/
 AVMWeather.svg?style=for-the-badge [stars-url]: https://github.com/avmmodules/
 AVMWeather/stargazers [issues-shield]: https://img.shields.io/github/issues/
 avmmodules/AVMWeather.svg?style=for-the-badge [issues-url]: https://github.com/
 avmmodules/AVMWeather/issues [license-shield]: https://img.shields.io/github/
 license/avmmodules/AVMWeather.svg?style=for-the-badge [license-url]: https://
 github.com/avmmodules/AVMWeather/blob/main/LICENSE [miniatura]: https://
 codeflex.com.co/assets/img/ggg.webp
```

### Comparing `codeflex-1.1.1/setup.py` & `codeflex-2.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="codeflex",
-    version="1.1.1",
+    version="2.1.0",
     author="CODEFLEX S.A.S.", 
     author_email="info@codeflex.com.co",
     license="This software is owned by CodeFlex S.A.S. and is protected by applicable copyright laws. The distribution and use of this software are subject to the terms and conditions outlined below.",
-    description="¡Consulta tus bases de datos MySQL con CodeFlex!",
+    description="¡Conecta a los Microservicios de CodeFlex desde una Sola Librería!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://codeflex.com.co/",
     project_urls={
         "Bug Tracker": "https://docs.codeflex.com.co/",
     },
     classifiers=[
```

### Comparing `codeflex-1.1.1/src/codeflex/company/mysql.py` & `codeflex-2.1.0/src/codeflex/company/mysql.py`

 * *Files identical despite different names*

### Comparing `codeflex-1.1.1/src/codeflex.egg-info/PKG-INFO` & `codeflex-2.1.0/src/codeflex.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: codeflex
-Version: 1.1.1
-Summary: ¡Consulta tus bases de datos MySQL con CodeFlex!
+Version: 2.1.0
+Summary: ¡Conecta a los Microservicios de CodeFlex desde una Sola Librería!
 Home-page: https://codeflex.com.co/
 Author: CODEFLEX S.A.S.
 Author-email: info@codeflex.com.co
 License: This software is owned by CodeFlex S.A.S. and is protected by applicable copyright laws. The distribution and use of this software are subject to the terms and conditions outlined below.
 Project-URL: Bug Tracker, https://docs.codeflex.com.co/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -55,15 +55,15 @@
 ```python
 pip install codeflex
 ```
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
-* Example 1
+* Example 1 | Connection to MySQL
     ```python
     from codeflex.company import mysql
 
     respuesta = mysql.CONNECTOR("your_user", "your_password","your_database", "your_SQL") #Usuario , Contraseña, Base de datos, Cualquier Sql (Actualiza, Elimina, Consulta, Inserta) SOLO TABLAS
     print(respuesta)
 
 
@@ -107,20 +107,44 @@
     print(respuesta)
  
  
     respuesta = mysql.DBQUERY("your_user", "your_password") #Usuario y Contraseña
     print(respuesta)
 
     ```
+ 
+
+* Example 2 | Connection to Polly
+    ```python
+    from codeflex.company import polly
+
+    Text = "Prueba Final"
+    VoiceId = "Lupe" # Para cambiar el VoiceId y LanguageCode, consulta la documentación. | API de Conexión a Polly
+    LanguageCode = "es-US"
+    TokenSub = "Your_TokenSub" # Para acceder a este servicio, utiliza tu TokenSub, que es un identificador único por cuenta y es necesario que pertenezcas al plan premium. | https://codeflex.com.co/drive/index.html#/Polly
+
+    respuesta = polly.AUDIODATA(Text, VoiceId,LanguageCode,TokenSub)
+    print(respuesta)
+    # Respuesta: {"audioData": "SUQzBAAAAAAAI1RTU0UAAAAPAAADTGF2ZjU4Ljc2LjEwMAAAAAAAAAAAAAAA//EzfNsySGqKm/lCw0GpvBJAAwWmuAVDjr+V"} Base64
+
+
+    respuesta = polly.DOWNLOAD(Text, VoiceId,LanguageCode,TokenSub)
+    print(respuesta)
+    # Respuesta: {'audioUrl': 'https://s3.amazonaws.com/hub.codeflex.lat/audioStream_1713562991794.mp3'}
+
+    ```
+
+
+_For more examples, please refer to the [Documentation](https://docs.codeflex.com.co/docs-page.html#section-3)_
 
-_For more examples, please refer to the [Examples packages](https://docs.codeflex.com.co/docs-page.html#section-3)_
+_[CODEFLEX S.A.S.](https://codeflex.com.co/)_
 
-_[Database](http://mysql.codeflex.com.co/)_
+_[Database Mysql](http://mysql.codeflex.com.co/)_
 
-_[Create Account](https://codeflex.com.co/drive/index.html#/phpMyAdmin)_
+_[Create Account Mysql](https://codeflex.com.co/drive/index.html#/phpMyAdmin)_
 
 <!-- LICENSE -->
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <!-- CONTACT -->
```

#### html2text {}

```diff
@@ -1,62 +1,76 @@
-Metadata-Version: 2.1 Name: codeflex Version: 1.1.1 Summary: Â¡Consulta tus
-bases de datos MySQL con CodeFlex! Home-page: https://codeflex.com.co/ Author:
-CODEFLEX S.A.S. Author-email: info@codeflex.com.co License: This software is
-owned by CodeFlex S.A.S. and is protected by applicable copyright laws. The
-distribution and use of this software are subject to the terms and conditions
-outlined below. Project-URL: Bug Tracker, https://docs.codeflex.com.co/
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE [![MIT License][license-shield]](https://s3.amazonaws.com/
-www.codeflex.lat/documentos/c3320017-1937-4353-8881-475e3c89e25e/LICENSE.txt)
+Metadata-Version: 2.1 Name: codeflex Version: 2.1.0 Summary: Â¡Conecta a los
+Microservicios de CodeFlex desde una Sola LibrerÃ­a! Home-page: https://
+codeflex.com.co/ Author: CODEFLEX S.A.S. Author-email: info@codeflex.com.co
+License: This software is owned by CodeFlex S.A.S. and is protected by
+applicable copyright laws. The distribution and use of this software are
+subject to the terms and conditions outlined below. Project-URL: Bug Tracker,
+https://docs.codeflex.com.co/ Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE [![MIT License][license-shield]](https://
+s3.amazonaws.com/www.codeflex.lat/documentos/c3320017-1937-4353-8881-
+475e3c89e25e/LICENSE.txt)
                                     _[_L_o_g_o_]
                            ******** CCOODDEEFFLLEEXX SS..AA..SS.. ********
               CodificaciÃ³n y Almacenamiento Simplificados | IDE
                               _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 ## About The Project [![miniatura][miniatura]](https://codeflex.com.co) ##
 Getting Started ### Prerequisites You need to make sure you have installed the
 following modules. * Requests ```s pip install requests ``` ### Installation
-```python pip install codeflex ``` ## Usage * Example 1 ```python from
-codeflex.company import mysql respuesta = mysql.CONNECTOR("your_user",
-"your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
-datos, Cualquier Sql (Actualiza, Elimina, Consulta, Inserta) SOLO TABLAS print
-(respuesta) respuesta = mysql.UPDATETABLE_CUSTOM("your_user",
-"your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
-datos, Sql print(respuesta) respuesta = mysql.DELETETABLE_CUSTOM("your_user",
-"your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
-datos, Sql print(respuesta) respuesta = mysql.DELETETABLE("your_user",
-"your_password","your_database", "your_tablename") #Usuario , ContraseÃ±a, Base
-de datos, Nombre de la tabla print(respuesta) respuesta =
-mysql.TABLEINSERT_CUSTOM("your_user", "your_password","your_database",
+```python pip install codeflex ``` ## Usage * Example 1 | Connection to MySQL
+```python from codeflex.company import mysql respuesta = mysql.CONNECTOR
+("your_user", "your_password","your_database", "your_SQL") #Usuario ,
+ContraseÃ±a, Base de datos, Cualquier Sql (Actualiza, Elimina, Consulta,
+Inserta) SOLO TABLAS print(respuesta) respuesta = mysql.UPDATETABLE_CUSTOM
+("your_user", "your_password","your_database", "your_SQL") #Usuario ,
+ContraseÃ±a, Base de datos, Sql print(respuesta) respuesta =
+mysql.DELETETABLE_CUSTOM("your_user", "your_password","your_database",
 "your_SQL") #Usuario , ContraseÃ±a, Base de datos, Sql print(respuesta)
-respuesta = mysql.TABLEQUERY_CUSTOM("your_user",
+respuesta = mysql.DELETETABLE("your_user", "your_password","your_database",
+"your_tablename") #Usuario , ContraseÃ±a, Base de datos, Nombre de la tabla
+print(respuesta) respuesta = mysql.TABLEINSERT_CUSTOM("your_user",
+"your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
+datos, Sql print(respuesta) respuesta = mysql.TABLEQUERY_CUSTOM("your_user",
 "your_password","your_database", "your_SQL") #Usuario , ContraseÃ±a, Base de
 datos, Sql print(respuesta) respuesta = mysql.TABLEQUERY("your_user",
 "your_password","your_database", "your_tablename") #Usuario , ContraseÃ±a, Base
 de datos, Nombre de la tabla print(respuesta) respuesta =
 mysql.CREATETABLE_CUSTOM("your_user", "your_password","your_database",
 "your_SQL") #Usuario , ContraseÃ±a, Base de datos, Sql print(respuesta)
 respuesta = mysql.CREATETABLE("your_user", "your_password","your_database",
 "your_tablename") #Usuario , ContraseÃ±a, Base de datos, Nombre de la tabla
 print(respuesta) respuesta = mysql.DELETEDB("your_user", "your_database")
 #Usuario y Base de datos print(respuesta) respuesta = mysql.CREATEDB
 ("your_user", "your_database") #Usuario y Base de datos print(respuesta)
 respuesta = mysql.DBQUERY("your_user", "your_password") #Usuario y ContraseÃ±a
-print(respuesta) ``` _For more examples, please refer to the [Examples
-packages](https://docs.codeflex.com.co/docs-page.html#section-3)_ _[Database]
-(http://mysql.codeflex.com.co/)_ _[Create Account](https://codeflex.com.co/
-drive/index.html#/phpMyAdmin)_ ## License Distributed under the MIT License.
-See `LICENSE` for more information. ## Contact Telefono: 3008130562 | Email:
-info@codeflex.com.co [contributors-shield]: https://img.shields.io/github/
-contributors/avmmodules/AVMWeather.svg?style=for-the-badge [contributors-url]:
-https://github.com/avmmodules/AVMWeather/graphs/contributors [forks-shield]:
-https://img.shields.io/github/forks/avmmodules/AVMWeather.svg?style=for-the-
-badge [forks-url]: https://github.com/avmmodules/AVMWeather/network/members
-[stars-shield]: https://img.shields.io/github/stars/avmmodules/
+print(respuesta) ``` * Example 2 | Connection to Polly ```python from
+codeflex.company import polly Text = "Prueba Final" VoiceId = "Lupe" # Para
+cambiar el VoiceId y LanguageCode, consulta la documentaciÃ³n. | API de
+ConexiÃ³n a Polly LanguageCode = "es-US" TokenSub = "Your_TokenSub" # Para
+acceder a este servicio, utiliza tu TokenSub, que es un identificador Ãºnico
+por cuenta y es necesario que pertenezcas al plan premium. | https://
+codeflex.com.co/drive/index.html#/Polly respuesta = polly.AUDIODATA(Text,
+VoiceId,LanguageCode,TokenSub) print(respuesta) # Respuesta: {"audioData":
+"SUQzBAAAAAAAI1RTU0UAAAAPAAADTGF2ZjU4Ljc2LjEwMAAAAAAAAAAAAAAA//EzfNsySGqKm/
+lCw0GpvBJAAwWmuAVDjr+V"} Base64 respuesta = polly.DOWNLOAD(Text,
+VoiceId,LanguageCode,TokenSub) print(respuesta) # Respuesta: {'audioUrl':
+'https://s3.amazonaws.com/hub.codeflex.lat/audioStream_1713562991794.mp3'} ```
+_For more examples, please refer to the [Documentation](https://
+docs.codeflex.com.co/docs-page.html#section-3)_ _[CODEFLEX S.A.S.](https://
+codeflex.com.co/)_ _[Database Mysql](http://mysql.codeflex.com.co/)_ _[Create
+Account Mysql](https://codeflex.com.co/drive/index.html#/phpMyAdmin)_ ##
+License Distributed under the MIT License. See `LICENSE` for more information.
+## Contact Telefono: 3008130562 | Email: info@codeflex.com.co [contributors-
+shield]: https://img.shields.io/github/contributors/avmmodules/
+AVMWeather.svg?style=for-the-badge [contributors-url]: https://github.com/
+avmmodules/AVMWeather/graphs/contributors [forks-shield]: https://
+img.shields.io/github/forks/avmmodules/AVMWeather.svg?style=for-the-badge
+[forks-url]: https://github.com/avmmodules/AVMWeather/network/members [stars-
+shield]: https://img.shields.io/github/stars/avmmodules/
 AVMWeather.svg?style=for-the-badge [stars-url]: https://github.com/avmmodules/
 AVMWeather/stargazers [issues-shield]: https://img.shields.io/github/issues/
 avmmodules/AVMWeather.svg?style=for-the-badge [issues-url]: https://github.com/
 avmmodules/AVMWeather/issues [license-shield]: https://img.shields.io/github/
 license/avmmodules/AVMWeather.svg?style=for-the-badge [license-url]: https://
 github.com/avmmodules/AVMWeather/blob/main/LICENSE [miniatura]: https://
 codeflex.com.co/assets/img/ggg.webp
```

