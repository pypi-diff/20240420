# Comparing `tmp/CI-CD-SergiCastillo-0.1.9.tar.gz` & `tmp/CI-CD-SergiCastillo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CI-CD-SergiCastillo-0.1.9.tar", last modified: Thu Apr 18 20:25:19 2024, max compression
+gzip compressed data, was "dist/CI-CD-SergiCastillo-0.2.1.tar", last modified: Sat Apr 20 15:14:37 2024, max compression
```

## Comparing `CI-CD-SergiCastillo-0.1.9.tar` & `CI-CD-SergiCastillo-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:25:19.702783 CI-CD-SergiCastillo-0.1.9/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:25:19.702783 CI-CD-SergiCastillo-0.1.9/CI_CD_SergiCastillo.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 20:25:19.000000 CI-CD-SergiCastillo-0.1.9/CI_CD_SergiCastillo.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      259 2024-04-18 20:25:19.000000 CI-CD-SergiCastillo-0.1.9/CI_CD_SergiCastillo.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-18 20:25:19.000000 CI-CD-SergiCastillo-0.1.9/CI_CD_SergiCastillo.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2024-04-18 20:25:19.000000 CI-CD-SergiCastillo-0.1.9/CI_CD_SergiCastillo.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2024-04-18 20:25:19.000000 CI-CD-SergiCastillo-0.1.9/CI_CD_SergiCastillo.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 20:25:19.702783 CI-CD-SergiCastillo-0.1.9/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-04-18 20:24:08.000000 CI-CD-SergiCastillo-0.1.9/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:25:19.702783 CI-CD-SergiCastillo-0.1.9/app/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:25:07.000000 CI-CD-SergiCastillo-0.1.9/app/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3678 2024-04-18 20:24:08.000000 CI-CD-SergiCastillo-0.1.9/app/app.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-04-18 20:25:19.702783 CI-CD-SergiCastillo-0.1.9/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2024-04-18 20:24:08.000000 CI-CD-SergiCastillo-0.1.9/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 15:14:37.868736 CI-CD-SergiCastillo-0.2.1/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 15:14:37.868736 CI-CD-SergiCastillo-0.2.1/CI_CD_SergiCastillo.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-20 15:14:37.000000 CI-CD-SergiCastillo-0.2.1/CI_CD_SergiCastillo.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      259 2024-04-20 15:14:37.000000 CI-CD-SergiCastillo-0.2.1/CI_CD_SergiCastillo.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-20 15:14:37.000000 CI-CD-SergiCastillo-0.2.1/CI_CD_SergiCastillo.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2024-04-20 15:14:37.000000 CI-CD-SergiCastillo-0.2.1/CI_CD_SergiCastillo.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2024-04-20 15:14:37.000000 CI-CD-SergiCastillo-0.2.1/CI_CD_SergiCastillo.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-20 15:14:37.868736 CI-CD-SergiCastillo-0.2.1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-04-20 15:12:46.000000 CI-CD-SergiCastillo-0.2.1/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 15:14:37.868736 CI-CD-SergiCastillo-0.2.1/app/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-20 15:14:21.000000 CI-CD-SergiCastillo-0.2.1/app/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3233 2024-04-20 15:12:46.000000 CI-CD-SergiCastillo-0.2.1/app/app.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-04-20 15:14:37.868736 CI-CD-SergiCastillo-0.2.1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      704 2024-04-20 15:12:46.000000 CI-CD-SergiCastillo-0.2.1/setup.py
```

### Comparing `CI-CD-SergiCastillo-0.1.9/app/app.py` & `CI-CD-SergiCastillo-0.2.1/app/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,31 +26,18 @@
 
 # Configuración de la base de datos
 configuracion_bd = {
     'host': config['host'],
     'user': config['user'],
     'password': config['password'],
     'database': config['database'],
-    'port': config.get('port', 5432)  # Usar el valor predeterminado 5432 si el puerto no está definido en el archivo JSON
+    'port': config.get('port', 5432),  # Usar el valor predeterminado 5432 si el puerto no está definido en el archivo JSON
+    'sslmode': 'require'  # Establecer SSL mode en require para usar SSL
 }
 
-
-def crear_tabla():
-    try:
-        conexion = psycopg2.connect(**configuracion_bd)
-        cursor = conexion.cursor()
-        cursor.execute("CREATE TABLE IF NOT EXISTS practicas (id SERIAL PRIMARY KEY, nombre VARCHAR(255), correo VARCHAR(255), categoria VARCHAR(255), link VARCHAR(255))")
-        conexion.commit()
-        log.info("Tabla creada correctamente")
-    except Exception as e:
-        log.error({"message": f"Error al crear la tabla: {e}"})
-    finally:
-        if 'conexion' in locals():
-            conexion.close()
-
 def agregar_practica(nombre, correo, categoria, link):
     try:
         conexion = psycopg2.connect(**configuracion_bd)
         cursor = conexion.cursor()
         cursor.execute("INSERT INTO practicas (nombre, correo, categoria, link) VALUES (%s, %s, %s, %s)", (nombre, correo, categoria, link))
         conexion.commit()
         log.info({"message": "Práctica agregada correctamente", "nombre": nombre, "correo": correo, "categoria": categoria, "link": link})
@@ -83,17 +70,14 @@
         log.info({"message": "Práctica eliminada correctamente", "id": practica_id})
     except Exception as e:
         log.error({"message": f"Error al eliminar práctica: {e}"})
     finally:
         if 'conexion' in locals():
             conexion.close()
 
-# Crear la tabla en la base de datos
-crear_tabla()
-
 @app.route('/')
 def index():
     practicas = obtener_practicas()
     return render_template('index.html', practicas=practicas)
 
 @app.route('/agregar', methods=['POST'])
 def agregar():
@@ -104,7 +88,10 @@
     agregar_practica(nombre, correo, categoria, link)
     return redirect('/')
 
 @app.route('/eliminar/<int:practica_id>', methods=['POST'])
 def eliminar(practica_id):
     eliminar_practica(practica_id)
     return redirect('/')
+
+if __name__ == '__main__':
+    app.run(host='0.0.0.0', port=5000)
```

