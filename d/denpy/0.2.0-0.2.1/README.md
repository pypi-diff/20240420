# Comparing `tmp/denpy-0.2.0.tar.gz` & `tmp/denpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denpy-0.2.0.tar", last modified: Mon Mar 11 15:06:30 2024, max compression
+gzip compressed data, was "denpy-0.2.1.tar", last modified: Sat Apr 20 18:34:32 2024, max compression
```

## Comparing `denpy-0.2.0.tar` & `denpy-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 15:06:30.798072 denpy-0.2.0/
--rw-rw-rw-   0        0        0      123 2024-03-11 15:06:30.798072 denpy-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-11 15:06:30.793086 denpy-0.2.0/denpy/
--rw-rw-rw-   0        0        0      194 2024-03-11 15:04:59.000000 denpy-0.2.0/denpy/__init__.py
--rw-rw-rw-   0        0        0      513 2023-11-16 19:54:53.000000 denpy-0.2.0/denpy/color.py
--rw-rw-rw-   0        0        0     3195 2024-03-11 14:45:35.000000 denpy-0.2.0/denpy/database.py
--rw-rw-rw-   0        0        0     2594 2024-02-18 10:12:48.000000 denpy-0.2.0/denpy/local_database.py
--rw-rw-rw-   0        0        0      398 2024-03-11 15:01:02.000000 denpy-0.2.0/denpy/security.py
--rw-rw-rw-   0        0        0     3072 2024-03-11 14:34:47.000000 denpy-0.2.0/denpy/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-11 15:06:30.797075 denpy-0.2.0/denpy.egg-info/
--rw-rw-rw-   0        0        0      123 2024-03-11 15:06:30.000000 denpy-0.2.0/denpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-03-11 15:06:30.000000 denpy-0.2.0/denpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 15:06:30.000000 denpy-0.2.0/denpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-03-11 15:06:30.000000 denpy-0.2.0/denpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-11 15:06:30.000000 denpy-0.2.0/denpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-11 15:06:30.798072 denpy-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      307 2024-03-11 15:01:02.000000 denpy-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:34:31.998507 denpy-0.2.1/
+-rw-rw-rw-   0        0        0      123 2024-04-20 18:34:31.997510 denpy-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-20 18:34:31.979559 denpy-0.2.1/denpy/
+-rw-rw-rw-   0        0        0      194 2024-03-11 15:04:59.000000 denpy-0.2.1/denpy/__init__.py
+-rw-rw-rw-   0        0        0      513 2023-11-16 19:54:53.000000 denpy-0.2.1/denpy/color.py
+-rw-rw-rw-   0        0        0     3511 2024-04-06 18:18:10.000000 denpy-0.2.1/denpy/database.py
+-rw-rw-rw-   0        0        0     2594 2024-02-18 10:12:48.000000 denpy-0.2.1/denpy/local_database.py
+-rw-rw-rw-   0        0        0      398 2024-03-11 15:01:02.000000 denpy-0.2.1/denpy/security.py
+-rw-rw-rw-   0        0        0     2687 2024-04-20 13:42:43.000000 denpy-0.2.1/denpy/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:34:31.997510 denpy-0.2.1/denpy.egg-info/
+-rw-rw-rw-   0        0        0      123 2024-04-20 18:34:31.000000 denpy-0.2.1/denpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-04-20 18:34:31.000000 denpy-0.2.1/denpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 18:34:31.000000 denpy-0.2.1/denpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-20 18:34:31.000000 denpy-0.2.1/denpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-20 18:34:31.000000 denpy-0.2.1/denpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 18:34:31.998507 denpy-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      307 2024-04-20 13:42:43.000000 denpy-0.2.1/setup.py
```

### Comparing `denpy-0.2.0/denpy/color.py` & `denpy-0.2.1/denpy/color.py`

 * *Files identical despite different names*

### Comparing `denpy-0.2.0/denpy/database.py` & `denpy-0.2.1/denpy/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 import mysql.connector
+import inspect
+import denpy
 
 class Database:
     def __init__(self, endpoint, database_name, username, password):
         self.database = None
         self.cursor = None
         self.data = [endpoint, database_name, username, password]
         self.database_name = database_name
 
     def connect(self):
         self.database = mysql.connector.connect(host=self.data[0], user=self.data[2], password=self.data[3], database=self.data[1])
         self.cursor = self.database.cursor()
 
-    def disconnect(self, commit=False):
+    def disconnect(self, commit: bool = False):
         if commit is True:
             self.database.commit()
         self.cursor.close()
         self.database.close()
 
-    def add(self, table_name, columns, values: list):
+    def add(self, table_name: str, columns: list, values: list):
         self.connect()
         values = ", ".join(f'"{value}"' for value in values)
         self.cursor.execute(f'INSERT INTO {self.database_name}.{table_name} ({", ".join(columns)}) VALUES ({values});')
         self.disconnect(commit=True)
 
-    def get(self, table_name, columns, where=None, fetchall=False):
+    def get(self, table_name: str, columns: list, where: str = None, fetchall: bool = False):
         self.connect()
         if where is None:
             self.cursor.execute(f'SELECT {", ".join(columns)} FROM {self.database_name}.{table_name};')
         else:
             self.cursor.execute(f'SELECT {", ".join(columns)} FROM {self.database_name}.{table_name} WHERE {where.split(" = ")[0]} = "{where.split(" = ")[1]}";')
-        result = self.cursor.fetchall()
-        self.disconnect()
         if fetchall is False:
-            if not result:
-                return None
-            else:
-                return result[0]
+            result = self.cursor.fetchone()
         else:
-            return result
+            result = self.cursor.fetchall()
+        if result is not None and len(result) == 1:
+            result = result[0]
+        self.disconnect()
+        return result
 
-    def delete(self, table_name, colum=None, where=None):
+    def delete(self, table_name: str, colum: str = None, where: str = None):
         self.connect()
         if where is None:
             if colum is None:
                 self.cursor.execute(f'DELETE FROM {self.database_name}.{table_name};')
             else:
                 self.cursor.execute(f'DELETE {colum} FROM {self.database_name}.{table_name};')
         else:
             if colum is None:
                 self.cursor.execute(f'DELETE FROM {self.database_name}.{table_name} WHERE {where.split(" = ")[0]} = "{where.split(" = ")[1]}";')
             else:
                 self.cursor.execute(f'DELETE {colum} FROM {self.database_name}.{table_name} WHERE {where.split(" = ")[0]} = "{where.split(" = ")[1]}";')
         self.disconnect(commit=True)
 
-    def edit(self, table_name, column, value, where=None):
+    def edit(self, table_name: str, column: list, value: list, where: str = None):
         self.connect()
         if where is None:
-            self.cursor.execute(f'UPDATE {self.database_name}.{table_name} SET {column} = "{value}";')
+            for i in range(len(column)):
+                self.cursor.execute(f'UPDATE {self.database_name}.{table_name} SET {column[i]} = "{value[i]}";')
         else:
-            self.cursor.execute(f'UPDATE {self.database_name}.{table_name} SET {column} = "{value}" WHERE {where.split(" = ")[0]} = "{where.split(" = ")[1]}";')
+            for i in range(len(column)):
+                self.cursor.execute(f'UPDATE {self.database_name}.{table_name} SET {column[i]} = "{value[i]}" WHERE {where.split(" = ")[0]} = "{where.split(" = ")[1]}";')
         self.disconnect(commit=True)
 
-    def default(self, table_name, columns: list = None, delete=False):
+    def table(self, table_name: str, columns: list, values: list, delete: bool = False):
         self.connect()
         if delete is True:
             self.cursor.execute(f'DROP TABLE IF EXISTS `{self.database_name}`.`{table_name}`;')
         else:
-            self.cursor.execute(f'CREATE TABLE IF NOT EXISTS `{self.database_name}`.`{table_name}` ({", ".join(columns)});')
+            self.cursor.execute(f'CREATE TABLE IF NOT EXISTS `{self.database_name}`.`{table_name}` ({", ".join([f"{column} {value}" for column, value in zip(columns, values)])});')
         self.disconnect(commit=True)
```

### Comparing `denpy-0.2.0/denpy/local_database.py` & `denpy-0.2.1/denpy/local_database.py`

 * *Files identical despite different names*

### Comparing `denpy-0.2.0/denpy/utils.py` & `denpy-0.2.1/denpy/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,61 @@
 import discord
 from rich.table import Table
 from rich.console import Console
 from json import load
 import inspect
 import psutil
 
+
 def create_table(params, values):
     table = Table()
     for param, value in zip(params, values):
         table.add_column(param)
     table.add_row(*values)
     console = Console()
     console.print(table)
 
+
 def get_ram_usage():
     return f'{round(psutil.virtual_memory().used / 10000000)} MB'
 
-async def send_custom_message(id, channel: discord.TextChannel, view=None, variables=None, edit: discord.Message or discord.Interaction = False):
+
+async def send_custom_message(id, channel: discord.TextChannel or discord.DMChannel, view=None, variables=None, edit: discord.Message or discord.Interaction = False):
     if variables is None:
         variables = {}
     path = inspect.stack()[1].filename.replace('\\', '/').split('/')
     path.pop(-1)
+    path.pop(-1)
     with open(f'{"/".join(path)}/embeds/{id}.json', 'r', encoding='utf-8') as file:
         config = load(file)
 
     embeds = []
-    for embed2 in config['embeds']:
-        try:
-            embed2['title']
-        except KeyError:
-            embed2['title'] = None
-        try:
-            embed2['description']
-        except KeyError:
-            embed2['description'] = None
-        try:
-            embed2['image']['url']
-        except KeyError:
-            embed = discord.Embed(
-                title=embed2['title'],
-                description=embed2['description'],
-                color=embed2['color']
-            )
-        else:
-            embed = discord.Embed(
-                title=embed2['title'],
-                description=embed2['description'],
-                color=embed2['color']
-            ).set_image(url=embed2['image']['url'])
-        try:
-            embed2['thumbnail']['url']
-        except KeyError:
-            pass
-        else:
-            embed.set_thumbnail(url=embed2['thumbnail']['url'])
-        try:
-            embed2['fields']
-        except KeyError:
-            pass
-        else:
-            for field in embed2['fields']:
+    for embed_ in config['embeds']:
+        embed = discord.Embed(
+            title=embed_.get('title'),
+            description=embed_.get('description'),
+            color=embed_['color']
+        )
+        if 'image' in embed_:
+            embed.set_image(url=embed_['image']['url'])
+        if 'thumbnail' in embed_:
+            embed.set_thumbnail(url=embed_['thumbnail']['url'])
+        if 'fields' in embed_:
+            for field in embed_['fields']:
                 embed.add_field(name=field['name'], value=field['value'], inline=field['inline'])
         embeds.append(embed)
+
     for variable in variables:
-        if config['content'] is not None:
-            config['content'] = config['content'].replace(f'{variable}', variables[variable])
+        config['content'] = config['content'].replace(f'{variable}', str(variables[variable])) if config['content'] is not None else None
         for embed in embeds:
-            embed.title = embed.title.replace(f'{variable}', variables[variable])
-            embed.description = embed.description.replace(f'{variable}', variables[variable])
+            embed.title = embed.title.replace(f'{variable}', str(variables[variable])) if embed.title is not None else None
+            embed.description = embed.description.replace(f'{variable}', str(variables[variable])) if embed.description is not None else None
             for field in embed.fields:
-                field.name = field.name.replace(f'{variable}', variables[variable])
-                field.value = field.value.replace(f'{variable}', variables[variable])
+                field.name = field.name.replace(f'{variable}', str(variables[variable])) if field.name is not None else None
+                field.value = field.value.replace(f'{variable}', str(variables[variable])) if field.value is not None else None
 
     if edit is False:
         message = await channel.send(content=config['content'], embeds=embeds, view=view)
     else:
         if discord.message.Message == type(edit):
             message = await edit.edit(content=config['content'], embeds=embeds, view=view)
         else:
```

