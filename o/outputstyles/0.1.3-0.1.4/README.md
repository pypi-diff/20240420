# Comparing `tmp/outputstyles-0.1.3.tar.gz` & `tmp/outputstyles-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outputstyles-0.1.3.tar", last modified: Fri Apr 19 20:47:23 2024, max compression
+gzip compressed data, was "outputstyles-0.1.4.tar", last modified: Fri Apr 19 20:56:09 2024, max compression
```

## Comparing `outputstyles-0.1.3.tar` & `outputstyles-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 20:47:23.355644 outputstyles-0.1.3/
--rw-rw-rw-   0        0        0     1101 2023-08-26 23:34:28.000000 outputstyles-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     4590 2024-04-19 20:47:23.354645 outputstyles-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4036 2024-04-19 20:46:30.000000 outputstyles-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 20:47:23.340653 outputstyles-0.1.3/outputstyles/
--rw-rw-rw-   0        0        0      527 2024-02-09 01:16:19.000000 outputstyles-0.1.3/outputstyles/__init__.py
--rw-rw-rw-   0        0        0     5263 2024-04-19 19:58:21.000000 outputstyles-0.1.3/outputstyles/apply_styles.py
--rw-rw-rw-   0        0        0     2551 2024-02-09 00:58:05.000000 outputstyles-0.1.3/outputstyles/msg_type.py
--rw-rw-rw-   0        0        0     2107 2024-04-19 19:55:09.000000 outputstyles-0.1.3/outputstyles/variables.py
-drwxrwxrwx   0        0        0        0 2024-04-19 20:47:23.354645 outputstyles-0.1.3/outputstyles.egg-info/
--rw-rw-rw-   0        0        0     4590 2024-04-19 20:47:23.000000 outputstyles-0.1.3/outputstyles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-04-19 20:47:23.000000 outputstyles-0.1.3/outputstyles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 20:47:23.000000 outputstyles-0.1.3/outputstyles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-19 20:47:23.000000 outputstyles-0.1.3/outputstyles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 20:47:23.356644 outputstyles-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      897 2024-04-19 20:31:45.000000 outputstyles-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:56:09.941894 outputstyles-0.1.4/
+-rw-rw-rw-   0        0        0     1101 2023-08-26 23:34:28.000000 outputstyles-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     4584 2024-04-19 20:56:09.940894 outputstyles-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4034 2024-04-19 20:55:42.000000 outputstyles-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 20:56:09.937893 outputstyles-0.1.4/outputstyles/
+-rw-rw-rw-   0        0        0      527 2024-02-09 01:16:19.000000 outputstyles-0.1.4/outputstyles/__init__.py
+-rw-rw-rw-   0        0        0     5263 2024-04-19 19:58:21.000000 outputstyles-0.1.4/outputstyles/apply_styles.py
+-rw-rw-rw-   0        0        0     2551 2024-02-09 00:58:05.000000 outputstyles-0.1.4/outputstyles/msg_type.py
+-rw-rw-rw-   0        0        0     2107 2024-04-19 19:55:09.000000 outputstyles-0.1.4/outputstyles/variables.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:56:09.940894 outputstyles-0.1.4/outputstyles.egg-info/
+-rw-rw-rw-   0        0        0     4584 2024-04-19 20:56:09.000000 outputstyles-0.1.4/outputstyles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-04-19 20:56:09.000000 outputstyles-0.1.4/outputstyles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 20:56:09.000000 outputstyles-0.1.4/outputstyles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-19 20:56:09.000000 outputstyles-0.1.4/outputstyles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 20:56:09.942892 outputstyles-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      897 2024-04-19 20:55:57.000000 outputstyles-0.1.4/setup.py
```

### Comparing `outputstyles-0.1.3/LICENSE` & `outputstyles-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `outputstyles-0.1.3/PKG-INFO` & `outputstyles-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outputstyles
-Version: 0.1.3
+Version: 0.1.4
 Summary: Applying styles to CLI output
 Home-page: https://github.com/dunieskysp/output_styles
 Author: Duniesky Salazar Pérez
 Author-email: <duniesky.salazar@gmail.com>
 Keywords: python,outputstyles,CLI styles,text styles
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Output Styles
 
 Aplicarle estilos al texto de salida por CLI.
 
-## InstalaciÃ³n
+## Instalacion
 
 ```bash
   pip install outputstyles
 ```
 
 ## Uso/Ejemplos
 
@@ -104,15 +104,15 @@
 
 Resultado:
 
 ![output_styles](https://raw.githubusercontent.com/dunieskysp/output_styles/main/docs/img/custom_styles.png)
 
 ### 3 - Crear nuevas funciones
 
-**Definir los datos y la funciÃ³n del nuevo tipo de mensaje:**
+**Definir los datos y la funcion del nuevo tipo de mensaje:**
 
 ```py
 from outputstyles import apply_styles
 
 # Data of the new message.
 msg_data = {
     "ico_code": "\u2726",
```

### Comparing `outputstyles-0.1.3/README.md` & `outputstyles-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Output Styles
 
 Aplicarle estilos al texto de salida por CLI.
 
-## Instalación
+## Instalacion
 
 ```bash
   pip install outputstyles
 ```
 
 ## Uso/Ejemplos
 
@@ -89,15 +89,15 @@
 
 Resultado:
 
 ![output_styles](https://raw.githubusercontent.com/dunieskysp/output_styles/main/docs/img/custom_styles.png)
 
 ### 3 - Crear nuevas funciones
 
-**Definir los datos y la función del nuevo tipo de mensaje:**
+**Definir los datos y la funcion del nuevo tipo de mensaje:**
 
 ```py
 from outputstyles import apply_styles
 
 # Data of the new message.
 msg_data = {
     "ico_code": "\u2726",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `outputstyles-0.1.3/outputstyles/__init__.py` & `outputstyles-0.1.4/outputstyles/__init__.py`

 * *Files identical despite different names*

### Comparing `outputstyles-0.1.3/outputstyles/apply_styles.py` & `outputstyles-0.1.4/outputstyles/apply_styles.py`

 * *Files identical despite different names*

### Comparing `outputstyles-0.1.3/outputstyles/msg_type.py` & `outputstyles-0.1.4/outputstyles/msg_type.py`

 * *Files identical despite different names*

### Comparing `outputstyles-0.1.3/outputstyles/variables.py` & `outputstyles-0.1.4/outputstyles/variables.py`

 * *Files identical despite different names*

### Comparing `outputstyles-0.1.3/outputstyles.egg-info/PKG-INFO` & `outputstyles-0.1.4/outputstyles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outputstyles
-Version: 0.1.3
+Version: 0.1.4
 Summary: Applying styles to CLI output
 Home-page: https://github.com/dunieskysp/output_styles
 Author: Duniesky Salazar Pérez
 Author-email: <duniesky.salazar@gmail.com>
 Keywords: python,outputstyles,CLI styles,text styles
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Output Styles
 
 Aplicarle estilos al texto de salida por CLI.
 
-## InstalaciÃ³n
+## Instalacion
 
 ```bash
   pip install outputstyles
 ```
 
 ## Uso/Ejemplos
 
@@ -104,15 +104,15 @@
 
 Resultado:
 
 ![output_styles](https://raw.githubusercontent.com/dunieskysp/output_styles/main/docs/img/custom_styles.png)
 
 ### 3 - Crear nuevas funciones
 
-**Definir los datos y la funciÃ³n del nuevo tipo de mensaje:**
+**Definir los datos y la funcion del nuevo tipo de mensaje:**
 
 ```py
 from outputstyles import apply_styles
 
 # Data of the new message.
 msg_data = {
     "ico_code": "\u2726",
```

### Comparing `outputstyles-0.1.3/setup.py` & `outputstyles-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # La descripción larga va a ser el mismo fichero README.md
 long_desc = Path("README.md").read_text()
 
 # Datos del paquete
 setup(
     name="outputstyles",
-    version="0.1.3",
+    version="0.1.4",
     author="Duniesky Salazar Pérez",
     author_email="<duniesky.salazar@gmail.com>",
     description="Applying styles to CLI output",
     long_description=long_desc,
     long_description_content_type='text/markdown',
     url='https://github.com/dunieskysp/output_styles',
     packages=find_packages(
```

