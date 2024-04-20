# Comparing `tmp/kv_sqlite_sync-0.1.4.tar.gz` & `tmp/kv_sqlite_sync-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_sqlite_sync-0.1.4.tar", last modified: Thu Apr 18 07:02:17 2024, max compression
+gzip compressed data, was "kv_sqlite_sync-0.1.5.tar", last modified: Sat Apr 20 18:04:29 2024, max compression
```

## Comparing `kv_sqlite_sync-0.1.4.tar` & `kv_sqlite_sync-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:02:17.316112 kv_sqlite_sync-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      875 2024-04-18 07:02:17.316112 kv_sqlite_sync-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-05 13:15:45.000000 kv_sqlite_sync-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      676 2024-04-18 07:02:11.000000 kv_sqlite_sync-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-18 07:02:17.316112 kv_sqlite_sync-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:02:17.316112 kv_sqlite_sync-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:02:17.306112 kv_sqlite_sync-0.1.4/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:02:17.316112 kv_sqlite_sync-0.1.4/src/kv/sqlite/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-04-05 13:12:45.000000 kv_sqlite_sync-0.1.4/src/kv/sqlite/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:02:17.316112 kv_sqlite_sync-0.1.4/src/kv/sqlite/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-05 13:12:45.000000 kv_sqlite_sync-0.1.4/src/kv/sqlite/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4045 2024-04-18 06:55:32.000000 kv_sqlite_sync-0.1.4/src/kv/sqlite/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:02:17.316112 kv_sqlite_sync-0.1.4/src/kv/sqlite/queries/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       92 2024-04-05 13:12:45.000000 kv_sqlite_sync-0.1.4/src/kv/sqlite/queries/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1546 2024-04-05 13:12:45.000000 kv_sqlite_sync-0.1.4/src/kv/sqlite/queries/queries.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:02:17.316112 kv_sqlite_sync-0.1.4/src/kv_sqlite_sync.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      875 2024-04-18 07:02:17.000000 kv_sqlite_sync-0.1.4/src/kv_sqlite_sync.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      381 2024-04-18 07:02:17.000000 kv_sqlite_sync-0.1.4/src/kv_sqlite_sync.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-18 07:02:17.000000 kv_sqlite_sync-0.1.4/src/kv_sqlite_sync.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-04-18 07:02:17.000000 kv_sqlite_sync-0.1.4/src/kv_sqlite_sync.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-18 07:02:17.000000 kv_sqlite_sync-0.1.4/src/kv_sqlite_sync.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:29.303580 kv_sqlite_sync-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      875 2024-04-20 18:04:29.303580 kv_sqlite_sync-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-05 13:15:45.000000 kv_sqlite_sync-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      676 2024-04-20 18:04:27.000000 kv_sqlite_sync-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-20 18:04:29.303580 kv_sqlite_sync-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:29.293580 kv_sqlite_sync-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:29.293580 kv_sqlite_sync-0.1.5/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:29.293580 kv_sqlite_sync-0.1.5/src/kv/sqlite/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-04-05 13:12:45.000000 kv_sqlite_sync-0.1.5/src/kv/sqlite/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:29.293580 kv_sqlite_sync-0.1.5/src/kv/sqlite/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-05 13:12:45.000000 kv_sqlite_sync-0.1.5/src/kv/sqlite/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4089 2024-04-20 17:28:11.000000 kv_sqlite_sync-0.1.5/src/kv/sqlite/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:29.303580 kv_sqlite_sync-0.1.5/src/kv/sqlite/queries/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       92 2024-04-05 13:12:45.000000 kv_sqlite_sync-0.1.5/src/kv/sqlite/queries/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1546 2024-04-05 13:12:45.000000 kv_sqlite_sync-0.1.5/src/kv/sqlite/queries/queries.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:29.303580 kv_sqlite_sync-0.1.5/src/kv_sqlite_sync.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      875 2024-04-20 18:04:29.000000 kv_sqlite_sync-0.1.5/src/kv_sqlite_sync.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      381 2024-04-20 18:04:29.000000 kv_sqlite_sync-0.1.5/src/kv_sqlite_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-20 18:04:29.000000 kv_sqlite_sync-0.1.5/src/kv_sqlite_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-04-20 18:04:29.000000 kv_sqlite_sync-0.1.5/src/kv_sqlite_sync.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-20 18:04:29.000000 kv_sqlite_sync-0.1.5/src/kv_sqlite_sync.egg-info/top_level.txt
```

### Comparing `kv_sqlite_sync-0.1.4/PKG-INFO` & `kv_sqlite_sync-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-sqlite-sync
-Version: 0.1.4
+Version: 0.1.5
 Summary: Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-sqlite-sync
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

### Comparing `kv_sqlite_sync-0.1.4/pyproject.toml` & `kv_sqlite_sync-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-sqlite-sync"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB"
 dependencies = [
   "kv-api", "haskellian", "ramda"
 ]
```

### Comparing `kv_sqlite_sync-0.1.4/src/kv/sqlite/api/api.py` & `kv_sqlite_sync-0.1.5/src/kv/sqlite/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,17 @@
   @classmethod
   def at(
     cls, db_path: str, table: str = 'kv',
     parse: Callable[[str], E.Either[InvalidData, T]] = lambda x: E.Right(cast(T, x)),
     dump: Callable[[T], str] = lambda x: str(x),
     dtype: str = 'TEXT'
   ) -> 'SQLiteKV[T]':
-    os.makedirs(os.path.dirname(db_path), exist_ok=True)
+    dir = os.path.dirname(db_path)
+    if dir != '':
+      os.makedirs(dir, exist_ok=True)
     return SQLiteKV(sqlite3.connect(db_path), table, parse, dump, dtype)
 
   @classmethod
   def validated(cls, Type: type[M], db_path: str, table: str = 'kv') -> 'SQLiteKV[M]':
     Model = RootModel[Type]
     return cls.at(
       db_path=db_path, table=table, dtype='JSON',
@@ -49,19 +51,19 @@
     try:
       cur = self.conn.execute(*query)
       self.conn.commit()
       return E.Right(cur)
     except sqlite3.Error as err:
       return E.Left(DBError(str(err)))
 
-  @P.lift
-  async def update(self, key: str, value: T) -> E.Either[DBError|InexistentItem, None]:
-    return self.execute(queries.update(key, self.dump(value), table=self.table)).bind(
-      lambda cur: E.Left(InexistentItem(key)) if cur.rowcount == 0 else E.Right(None)
-    )
+  # @P.lift
+  # async def update(self, key: str, value: T) -> E.Either[DBError|InexistentItem, None]:
+  #   return self.execute(queries.update(key, self.dump(value), table=self.table)).bind(
+  #     lambda cur: E.Left(InexistentItem(key)) if cur.rowcount == 0 else E.Right(None)
+  #   )
   
   @P.lift
   async def insert(self, key: str, value: T, *, replace = False) -> E.Either[DBError, None]:
     make_query = queries.upsert if replace else queries.insert
     return self.execute(make_query(key, self.dump(value), table=self.table)) | (lambda _: None)
   
   @P.lift
```

### Comparing `kv_sqlite_sync-0.1.4/src/kv/sqlite/queries/queries.py` & `kv_sqlite_sync-0.1.5/src/kv/sqlite/queries/queries.py`

 * *Files identical despite different names*

### Comparing `kv_sqlite_sync-0.1.4/src/kv_sqlite_sync.egg-info/PKG-INFO` & `kv_sqlite_sync-0.1.5/src/kv_sqlite_sync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-sqlite-sync
-Version: 0.1.4
+Version: 0.1.5
 Summary: Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-sqlite-sync
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

