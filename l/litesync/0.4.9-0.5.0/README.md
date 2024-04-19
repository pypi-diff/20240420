# Comparing `tmp/litesync-0.4.9.tar.gz` & `tmp/litesync-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesync-0.4.9.tar", last modified: Sun Feb 11 22:12:45 2024, max compression
+gzip compressed data, was "litesync-0.5.0.tar", last modified: Fri Apr 19 23:49:31 2024, max compression
```

## Comparing `litesync-0.4.9.tar` & `litesync-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-02-11 22:12:45.517808 litesync-0.4.9/
--rw-r--r--   0 bernardo   (501) staff       (20)      889 2021-06-02 22:30:16.000000 litesync-0.4.9/LICENSE
--rw-r--r--   0 bernardo   (501) staff       (20)      128 2021-06-02 22:30:16.000000 litesync-0.4.9/MANIFEST.in
--rw-r--r--   0 bernardo   (501) staff       (20)     2370 2024-02-11 22:12:45.517666 litesync-0.4.9/PKG-INFO
--rw-r--r--   0 bernardo   (501) staff       (20)     1566 2021-06-03 06:16:33.000000 litesync-0.4.9/README.md
-drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-02-11 22:12:45.484473 litesync-0.4.9/litesync/
--rw-r--r--   0 bernardo   (501) staff       (20)     1018 2021-06-03 01:51:18.000000 litesync-0.4.9/litesync/__init__.py
--rw-r--r--   0 bernardo   (501) staff       (20)     2723 2021-06-03 01:51:18.000000 litesync-0.4.9/litesync/dbapi2.py
-drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-02-11 22:12:45.517113 litesync-0.4.9/litesync.egg-info/
--rw-r--r--   0 bernardo   (501) staff       (20)     2370 2024-02-11 22:12:45.000000 litesync-0.4.9/litesync.egg-info/PKG-INFO
--rw-r--r--   0 bernardo   (501) staff       (20)      510 2024-02-11 22:12:45.000000 litesync-0.4.9/litesync.egg-info/SOURCES.txt
--rw-r--r--   0 bernardo   (501) staff       (20)        1 2024-02-11 22:12:45.000000 litesync-0.4.9/litesync.egg-info/dependency_links.txt
--rw-r--r--   0 bernardo   (501) staff       (20)        9 2024-02-11 22:12:45.000000 litesync-0.4.9/litesync.egg-info/top_level.txt
--rw-r--r--   0 bernardo   (501) staff       (20)      115 2024-02-11 22:12:45.518344 litesync-0.4.9/setup.cfg
--rw-r--r--   0 bernardo   (501) staff       (20)     2934 2024-02-11 22:11:45.000000 litesync-0.4.9/setup.py
-drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-02-11 22:12:45.515821 litesync-0.4.9/src/
--rw-r--r--   0 bernardo   (501) staff       (20)    17810 2021-06-02 22:30:16.000000 litesync-0.4.9/src/blob.c
--rw-r--r--   0 bernardo   (501) staff       (20)      580 2021-06-03 00:06:41.000000 litesync-0.4.9/src/blob.h
--rw-r--r--   0 bernardo   (501) staff       (20)    12679 2021-06-02 22:30:16.000000 litesync-0.4.9/src/cache.c
--rw-r--r--   0 bernardo   (501) staff       (20)     2357 2021-06-02 22:30:16.000000 litesync-0.4.9/src/cache.h
--rw-r--r--   0 bernardo   (501) staff       (20)    61808 2024-02-11 22:11:45.000000 litesync-0.4.9/src/connection.c
--rw-r--r--   0 bernardo   (501) staff       (20)     4713 2021-06-03 00:06:57.000000 litesync-0.4.9/src/connection.h
--rw-r--r--   0 bernardo   (501) staff       (20)    29823 2021-06-02 22:30:16.000000 litesync-0.4.9/src/cursor.c
--rw-r--r--   0 bernardo   (501) staff       (20)     2441 2021-06-02 22:30:16.000000 litesync-0.4.9/src/cursor.h
--rw-r--r--   0 bernardo   (501) staff       (20)     4551 2021-06-02 22:30:16.000000 litesync-0.4.9/src/microprotocols.c
--rw-r--r--   0 bernardo   (501) staff       (20)     2079 2021-06-02 22:30:16.000000 litesync-0.4.9/src/microprotocols.h
--rw-r--r--   0 bernardo   (501) staff       (20)    18422 2021-06-02 22:30:16.000000 litesync-0.4.9/src/module.c
--rw-r--r--   0 bernardo   (501) staff       (20)     1956 2021-06-02 22:30:16.000000 litesync-0.4.9/src/module.h
--rw-r--r--   0 bernardo   (501) staff       (20)     4396 2021-06-02 22:30:16.000000 litesync-0.4.9/src/prepare_protocol.c
--rw-r--r--   0 bernardo   (501) staff       (20)     1525 2021-06-02 22:30:16.000000 litesync-0.4.9/src/prepare_protocol.h
--rw-r--r--   0 bernardo   (501) staff       (20)     9515 2021-06-02 22:30:16.000000 litesync-0.4.9/src/row.c
--rw-r--r--   0 bernardo   (501) staff       (20)     1296 2021-06-02 22:30:16.000000 litesync-0.4.9/src/row.h
--rw-r--r--   0 bernardo   (501) staff       (20)    17339 2021-06-02 22:30:16.000000 litesync-0.4.9/src/statement.c
--rw-r--r--   0 bernardo   (501) staff       (20)     2080 2021-06-03 00:07:23.000000 litesync-0.4.9/src/statement.h
--rw-r--r--   0 bernardo   (501) staff       (20)     4812 2021-06-02 22:30:16.000000 litesync-0.4.9/src/util.c
--rw-r--r--   0 bernardo   (501) staff       (20)     1487 2021-06-03 00:07:35.000000 litesync-0.4.9/src/util.h
+drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-19 23:49:31.518882 litesync-0.5.0/
+-rw-r--r--   0 bernardo   (501) staff       (20)      889 2021-06-02 22:30:16.000000 litesync-0.5.0/LICENSE
+-rw-r--r--   0 bernardo   (501) staff       (20)      128 2021-06-02 22:30:16.000000 litesync-0.5.0/MANIFEST.in
+-rw-r--r--   0 bernardo   (501) staff       (20)     1804 2024-04-19 23:49:31.518750 litesync-0.5.0/PKG-INFO
+-rw-r--r--   0 bernardo   (501) staff       (20)     1000 2024-04-19 23:00:13.000000 litesync-0.5.0/README.md
+drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-19 23:49:31.492875 litesync-0.5.0/litesync/
+-rw-r--r--   0 bernardo   (501) staff       (20)     1018 2021-06-03 01:51:18.000000 litesync-0.5.0/litesync/__init__.py
+-rw-r--r--   0 bernardo   (501) staff       (20)     2723 2021-06-03 01:51:18.000000 litesync-0.5.0/litesync/dbapi2.py
+drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-19 23:49:31.518240 litesync-0.5.0/litesync.egg-info/
+-rw-r--r--   0 bernardo   (501) staff       (20)     1804 2024-04-19 23:49:31.000000 litesync-0.5.0/litesync.egg-info/PKG-INFO
+-rw-r--r--   0 bernardo   (501) staff       (20)      525 2024-04-19 23:49:31.000000 litesync-0.5.0/litesync.egg-info/SOURCES.txt
+-rw-r--r--   0 bernardo   (501) staff       (20)        1 2024-04-19 23:49:31.000000 litesync-0.5.0/litesync.egg-info/dependency_links.txt
+-rw-r--r--   0 bernardo   (501) staff       (20)        9 2024-04-19 23:49:31.000000 litesync-0.5.0/litesync.egg-info/top_level.txt
+-rw-r--r--   0 bernardo   (501) staff       (20)     1040 2024-04-19 23:42:57.000000 litesync-0.5.0/pyproject.toml
+-rw-r--r--   0 bernardo   (501) staff       (20)      115 2024-04-19 23:49:31.519492 litesync-0.5.0/setup.cfg
+-rw-r--r--   0 bernardo   (501) staff       (20)     2916 2024-04-19 23:46:20.000000 litesync-0.5.0/setup.py
+drwxr-xr-x   0 bernardo   (501) staff       (20)        0 2024-04-19 23:49:31.517085 litesync-0.5.0/src/
+-rw-r--r--   0 bernardo   (501) staff       (20)    17810 2021-06-02 22:30:16.000000 litesync-0.5.0/src/blob.c
+-rw-r--r--   0 bernardo   (501) staff       (20)      580 2021-06-03 00:06:41.000000 litesync-0.5.0/src/blob.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    12679 2021-06-02 22:30:16.000000 litesync-0.5.0/src/cache.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     2357 2021-06-02 22:30:16.000000 litesync-0.5.0/src/cache.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    63003 2024-04-19 22:06:56.000000 litesync-0.5.0/src/connection.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     4713 2024-02-13 01:52:40.000000 litesync-0.5.0/src/connection.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    29823 2021-06-02 22:30:16.000000 litesync-0.5.0/src/cursor.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     2441 2021-06-02 22:30:16.000000 litesync-0.5.0/src/cursor.h
+-rw-r--r--   0 bernardo   (501) staff       (20)     4551 2021-06-02 22:30:16.000000 litesync-0.5.0/src/microprotocols.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     2079 2021-06-02 22:30:16.000000 litesync-0.5.0/src/microprotocols.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    20182 2024-02-16 00:48:36.000000 litesync-0.5.0/src/module.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     1956 2021-06-02 22:30:16.000000 litesync-0.5.0/src/module.h
+-rw-r--r--   0 bernardo   (501) staff       (20)     4338 2024-04-19 22:07:29.000000 litesync-0.5.0/src/prepare_protocol.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     1525 2021-06-02 22:30:16.000000 litesync-0.5.0/src/prepare_protocol.h
+-rw-r--r--   0 bernardo   (501) staff       (20)     9515 2021-06-02 22:30:16.000000 litesync-0.5.0/src/row.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     1296 2021-06-02 22:30:16.000000 litesync-0.5.0/src/row.h
+-rw-r--r--   0 bernardo   (501) staff       (20)    17339 2021-06-02 22:30:16.000000 litesync-0.5.0/src/statement.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     2080 2021-06-03 00:07:23.000000 litesync-0.5.0/src/statement.h
+-rw-r--r--   0 bernardo   (501) staff       (20)     4812 2021-06-02 22:30:16.000000 litesync-0.5.0/src/util.c
+-rw-r--r--   0 bernardo   (501) staff       (20)     1487 2021-06-03 00:07:35.000000 litesync-0.5.0/src/util.h
```

### Comparing `litesync-0.4.9/LICENSE` & `litesync-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/PKG-INFO` & `litesync-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesync
-Version: 0.4.9
+Version: 0.5.0
 Summary: DB-API 2.0 interface for LiteSync
 Home-page: https://gitlab.com/litesync/litesync-python3
 Author: Bernardo Ramos
 Author-email: contact@litesync.io
 License: zlib/libpng
 Platform: ALL
 Classifier: Development Status :: 4 - Beta
@@ -24,63 +24,51 @@
 ====================
 
 This is a wrapper library to use [LiteSync](http://litesync.io) on Python 3
 
 It is based on [pysqlite3](https://github.com/coleifer/pysqlite3)
 
 
-### Additional features:  (compared to Python's sqlite3 module)
-
-* User-defined window functions (requires SQLite >= 3.25)
-* Flags and VFS an be specified when opening connection
-* Incremental BLOB I/O, [bpo-24905](https://github.com/python/cpython/pull/271)
-* Improved error messages, [bpo-16379](https://github.com/python/cpython/pull/1108)
-* Simplified detection of DML statements via `sqlite3_stmt_readonly`.
-* Sqlite native backup API (also present in standard library 3.7 and newer).
-
-
 Installation
 ------------
 
-You must install some LiteSync library for this one to work. It can be either
-pre-compiled binaries or you can compile it by yourself. You can start with
-the [free version](http://litesync.io/en/download.html).
+### 1. Install the Native Library
 
+You must install the native LiteSync library for this wrapper to work.
+It can be either pre-compiled binaries or you can compile it by yourself.
+You can start with the [free version](http://litesync.io/en/download.html)
 
-### Installing with pip
+### 2. Install the Wrapper
+
+#### With pip
 
 ```
 pip install litesync
 ```
 
+#### Cloning and Building
 
-### Cloning and Building
-
-Optionally you can clone the repo and build it:
+Optionally you can clone this repo and build it:
 
 ```
 git clone --depth=1 https://gitlab.com/litesync/litesync-python3
 cd litesync-python3
 python3 setup.py build install
 ```
 
 
 Usage
 -----
 
 ```python
 import litesync
-import json
 import time
 
 conn = litesync.connect('file:app.db?node=secondary&connect=tcp://server:port')
 
 # check if the db is ready
-while True:
-    result = conn.cursor().execute("PRAGMA sync_status").fetchone()
-    status = json.loads(result[0])
-    if status["db_is_ready"]: break
+while not conn.is_ready():
     time.sleep(0.250)
 
 # now we can use the db connection
 ...
 ```
```

### Comparing `litesync-0.4.9/litesync/__init__.py` & `litesync-0.5.0/litesync/__init__.py`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/litesync/dbapi2.py` & `litesync-0.5.0/litesync/dbapi2.py`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/litesync.egg-info/PKG-INFO` & `litesync-0.5.0/litesync.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesync
-Version: 0.4.9
+Version: 0.5.0
 Summary: DB-API 2.0 interface for LiteSync
 Home-page: https://gitlab.com/litesync/litesync-python3
 Author: Bernardo Ramos
 Author-email: contact@litesync.io
 License: zlib/libpng
 Platform: ALL
 Classifier: Development Status :: 4 - Beta
@@ -24,63 +24,51 @@
 ====================
 
 This is a wrapper library to use [LiteSync](http://litesync.io) on Python 3
 
 It is based on [pysqlite3](https://github.com/coleifer/pysqlite3)
 
 
-### Additional features:  (compared to Python's sqlite3 module)
-
-* User-defined window functions (requires SQLite >= 3.25)
-* Flags and VFS an be specified when opening connection
-* Incremental BLOB I/O, [bpo-24905](https://github.com/python/cpython/pull/271)
-* Improved error messages, [bpo-16379](https://github.com/python/cpython/pull/1108)
-* Simplified detection of DML statements via `sqlite3_stmt_readonly`.
-* Sqlite native backup API (also present in standard library 3.7 and newer).
-
-
 Installation
 ------------
 
-You must install some LiteSync library for this one to work. It can be either
-pre-compiled binaries or you can compile it by yourself. You can start with
-the [free version](http://litesync.io/en/download.html).
+### 1. Install the Native Library
 
+You must install the native LiteSync library for this wrapper to work.
+It can be either pre-compiled binaries or you can compile it by yourself.
+You can start with the [free version](http://litesync.io/en/download.html)
 
-### Installing with pip
+### 2. Install the Wrapper
+
+#### With pip
 
 ```
 pip install litesync
 ```
 
+#### Cloning and Building
 
-### Cloning and Building
-
-Optionally you can clone the repo and build it:
+Optionally you can clone this repo and build it:
 
 ```
 git clone --depth=1 https://gitlab.com/litesync/litesync-python3
 cd litesync-python3
 python3 setup.py build install
 ```
 
 
 Usage
 -----
 
 ```python
 import litesync
-import json
 import time
 
 conn = litesync.connect('file:app.db?node=secondary&connect=tcp://server:port')
 
 # check if the db is ready
-while True:
-    result = conn.cursor().execute("PRAGMA sync_status").fetchone()
-    status = json.loads(result[0])
-    if status["db_is_ready"]: break
+while not conn.is_ready():
     time.sleep(0.250)
 
 # now we can use the db connection
 ...
 ```
```

### Comparing `litesync-0.4.9/setup.py` & `litesync-0.5.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from distutils import log
 from distutils.command.build_ext import build_ext
 from setuptools import Extension
 
 # If you need to change anything, it should be enough to change setup.cfg.
 
 PACKAGE_NAME = 'litesync'
-VERSION = '0.4.9'
+VERSION = '0.5.0'
 
 # define sqlite sources
 sources = [os.path.join('src', source)
            for source in ["module.c", "connection.c", "cursor.c", "cache.c",
                           "microprotocols.c", "prepare_protocol.c",
                           "statement.c", "util.c", "row.c", "blob.c"]]
 
@@ -26,17 +26,16 @@
 EXTENSION_MODULE_NAME = "._sqlite3"
 
 # Work around clang raising hard error for unused arguments
 if sys.platform == "darwin":
     os.environ['CFLAGS'] = "-Qunused-arguments"
     log.info("CFLAGS: " + os.environ['CFLAGS'])
 
-
 def quote_argument(arg):
-    q = '\\"' if sys.platform == 'win32' and sys.version_info < (3, 9) else '"'
+    q = '"'   #if sys.platform == 'win32' and sys.version_info < (3, 8) else '"'
     return q + arg + q
 
 define_macros = [('MODULE_NAME', quote_argument(PACKAGE_NAME + '.dbapi2'))]
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
@@ -44,14 +43,16 @@
 
 class SystemLibSqliteBuilder(build_ext):
     description = "Builds a C extension linking against the litesync library"
 
     def build_extension(self, ext):
         log.info(self.description)
         ext.libraries.append('litesync')
+        if sys.platform == "win32":
+            ext.include_dirs.append(".")
         build_ext.build_extension(self, ext)
 
 
 def get_setup_args():
     return dict(
         name=PACKAGE_NAME,
         version=VERSION,
@@ -83,15 +84,9 @@
             "Topic :: Software Development :: Libraries :: Python Modules"],
         cmdclass={
             "build_ext": SystemLibSqliteBuilder
         }
     )
 
 
-def main():
-    try:
-        setuptools.setup(**get_setup_args())
-    except BaseException as ex:
-        log.info(str(ex))
-
 if __name__ == "__main__":
-    main()
+    setuptools.setup(**get_setup_args())
```

### Comparing `litesync-0.4.9/src/blob.c` & `litesync-0.5.0/src/blob.c`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/blob.h` & `litesync-0.5.0/src/blob.h`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/cache.c` & `litesync-0.5.0/src/cache.c`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/cache.h` & `litesync-0.5.0/src/cache.h`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/connection.c` & `litesync-0.5.0/src/connection.c`

 * *Files 1% similar despite different names*

```diff
@@ -461,14 +461,59 @@
         PyErr_SetString(pysqlite_ProgrammingError, "Cannot operate on a closed database.");
         return 0;
     } else {
         return 1;
     }
 }
 
+PyObject* pysqlite_connection_is_ready(pysqlite_Connection* self)
+{
+    int rc;
+    sqlite3_stmt* statement;
+    const char *sync_status;
+    int is_ready = 0;
+
+    Py_BEGIN_ALLOW_THREADS
+    rc = sqlite3_prepare_v2(self->db, "pragma sync_status", -1, &statement, NULL);
+    Py_END_ALLOW_THREADS
+
+    if (rc != SQLITE_OK) {
+        _pysqlite_seterror(self->db);
+        goto error;
+    }
+
+    rc = pysqlite_step(statement, self);
+    if (rc != SQLITE_ROW) {
+        _pysqlite_seterror(self->db);
+    }
+
+    // retrieve the result (string)
+    sync_status = (const char *)sqlite3_column_text(statement, 0);
+    if (sync_status) {
+        if (strstr(sync_status, "\"db_is_ready\": true") != NULL) {
+            is_ready = 1;
+        }
+    }
+
+    Py_BEGIN_ALLOW_THREADS
+    rc = sqlite3_finalize(statement);
+    Py_END_ALLOW_THREADS
+
+    if (rc != SQLITE_OK && !PyErr_Occurred()) {
+        _pysqlite_seterror(self->db);
+    }
+
+error:
+    if (PyErr_Occurred()) {
+        return NULL;
+    } else {
+        return PyBool_FromLong(is_ready);
+    }
+}
+
 PyObject* _pysqlite_connection_begin(pysqlite_Connection* self)
 {
     int rc;
     sqlite3_stmt* statement;
 
     Py_BEGIN_ALLOW_THREADS
     rc = sqlite3_prepare_v2(self->db, self->begin_statement, -1, &statement, NULL);
@@ -726,15 +771,15 @@
     threadstate = PyGILState_Ensure();
 
     aggregate_class = (PyObject*)sqlite3_user_data(context);
 
     aggregate_instance = (PyObject**)sqlite3_aggregate_context(context, sizeof(PyObject*));
 
     if (*aggregate_instance == NULL) {
-        *aggregate_instance = _PyObject_CallNoArg(aggregate_class);
+        *aggregate_instance = PyObject_CallObject(aggregate_class, NULL);
 
         if (PyErr_Occurred()) {
             *aggregate_instance = 0;
             if (_pysqlite_enable_callback_tracebacks) {
                 PyErr_Print();
             } else {
                 PyErr_Clear();
@@ -1176,15 +1221,15 @@
 static int _progress_handler(void* user_arg)
 {
     int rc;
     PyObject *ret;
     PyGILState_STATE gilstate;
 
     gilstate = PyGILState_Ensure();
-    ret = _PyObject_CallNoArg((PyObject*)user_arg);
+    ret = PyObject_CallObject((PyObject*)user_arg, NULL);
 
     if (!ret) {
         if (_pysqlite_enable_callback_tracebacks) {
             PyErr_Print();
         } else {
             PyErr_Clear();
         }
@@ -1934,14 +1979,16 @@
     {"isolation_level",  (getter)pysqlite_connection_get_isolation_level, (setter)pysqlite_connection_set_isolation_level},
     {"total_changes",  (getter)pysqlite_connection_get_total_changes, (setter)0},
     {"in_transaction",  (getter)pysqlite_connection_get_in_transaction, (setter)0},
     {NULL}
 };
 
 static PyMethodDef connection_methods[] = {
+    {"is_ready", (PyCFunction)pysqlite_connection_is_ready, METH_NOARGS,
+        PyDoc_STR("Check if the database is ready for access.")},
     {"cursor", (PyCFunction)(void(*)(void))pysqlite_connection_cursor, METH_VARARGS|METH_KEYWORDS,
         PyDoc_STR("Return a cursor for the connection.")},
     {"open_blob", (PyCFunction)pysqlite_connection_blob, METH_VARARGS|METH_KEYWORDS,
         PyDoc_STR("return a blob object")},
     {"close", (PyCFunction)pysqlite_connection_close, METH_NOARGS,
         PyDoc_STR("Closes the connection.")},
     {"commit", (PyCFunction)pysqlite_connection_commit, METH_NOARGS,
```

### Comparing `litesync-0.4.9/src/connection.h` & `litesync-0.5.0/src/connection.h`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/cursor.c` & `litesync-0.5.0/src/cursor.c`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/cursor.h` & `litesync-0.5.0/src/cursor.h`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/microprotocols.c` & `litesync-0.5.0/src/microprotocols.c`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/microprotocols.h` & `litesync-0.5.0/src/microprotocols.h`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/module.c` & `litesync-0.5.0/src/module.c`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,18 @@
 PyObject *pysqlite_InternalError = NULL;
 PyObject *pysqlite_OperationalError = NULL;
 PyObject *pysqlite_ProgrammingError = NULL;
 PyObject *pysqlite_IntegrityError = NULL;
 PyObject *pysqlite_DataError = NULL;
 PyObject *pysqlite_NotSupportedError = NULL;
 
+PyObject *pysqlite_error_callback = NULL;
+
 PyObject* _pysqlite_converters = NULL;
-int _pysqlite_enable_callback_tracebacks = 0;
+int _pysqlite_enable_callback_tracebacks = 1;
 int pysqlite_BaseTypeAdapted = 0;
 
 static PyObject* module_connect(PyObject* self, PyObject* args, PyObject*
         kwargs)
 {
     /* Python seems to have no way of extracting a single keyword-arg at
      * C-level, so this code is redundant with the one in connection_init in
@@ -216,14 +218,71 @@
 }
 
 PyDoc_STRVAR(module_register_converter_doc,
 "register_converter(typename, callable)\n\
 \n\
 Registers a converter with pysqlite. Non-standard.");
 
+static void _error_callback(void* user_arg, int error_code, const char* error_message)
+{
+    PyObject *ret = NULL;
+
+    PyGILState_STATE gilstate;
+    gilstate = PyGILState_Ensure();
+
+    if (error_message == NULL) error_message = "";
+
+    ret = PyObject_CallFunction(pysqlite_error_callback, "is", error_code, error_message);
+
+    if (ret) {
+        Py_DECREF(ret);
+    } else {
+        if (_pysqlite_enable_callback_tracebacks) {
+            PyErr_Print();
+        } else {
+            PyErr_Clear();
+        }
+    }
+
+    PyGILState_Release(gilstate);
+}
+
+static PyObject* module_set_error_callback(PyObject* self, PyObject* args, PyObject* kwargs)
+{
+    PyObject* error_callback = NULL;
+
+    static char *kwlist[] = { "error_callback", NULL };
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O:set_error_callback",
+                                     kwlist, &error_callback)) {
+        return NULL;
+    }
+
+    if (pysqlite_error_callback != NULL) {
+        Py_DECREF(pysqlite_error_callback);
+        pysqlite_error_callback = NULL;
+    }
+
+    if (error_callback == Py_None) {
+        /* None clears the error callback previously set */
+        sqlite3_config(SQLITE_CONFIG_LOG, NULL, NULL);
+    } else {
+        sqlite3_config(SQLITE_CONFIG_LOG, _error_callback, NULL);
+        pysqlite_error_callback = error_callback;
+        Py_INCREF(pysqlite_error_callback);
+    }
+
+    Py_RETURN_NONE;
+}
+
+PyDoc_STRVAR(set_error_callback_doc,
+"set_error_callback(error_callback)\n\
+\n\
+Sets an error log callback called for each error on all open connections. Non-standard.");
+
 static PyObject* enable_callback_tracebacks(PyObject* self, PyObject* args)
 {
     if (!PyArg_ParseTuple(args, "i", &_pysqlite_enable_callback_tracebacks)) {
         return NULL;
     }
 
     Py_RETURN_NONE;
@@ -257,14 +316,16 @@
      METH_VARARGS, module_register_adapter_doc},
     {"register_converter", (PyCFunction)module_register_converter,
      METH_VARARGS, module_register_converter_doc},
     {"adapt",  (PyCFunction)pysqlite_adapt, METH_VARARGS,
      pysqlite_adapt_doc},
     {"enable_callback_tracebacks",  (PyCFunction)enable_callback_tracebacks,
      METH_VARARGS, enable_callback_tracebacks_doc},
+    {"set_error_callback", (PyCFunction)(void(*)(void))module_set_error_callback,
+    METH_VARARGS | METH_KEYWORDS, set_error_callback_doc},
     {NULL, NULL}
 };
 
 struct _IntConstantPair {
     const char *constant_name;
     int constant_value;
 };
```

### Comparing `litesync-0.4.9/src/module.h` & `litesync-0.5.0/src/module.h`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/prepare_protocol.c` & `litesync-0.5.0/src/prepare_protocol.c`

 * *Files 2% similar despite different names*

```diff
@@ -74,10 +74,9 @@
         0,                                              /* tp_new */
         0                                               /* tp_free */
 };
 
 extern int pysqlite_prepare_protocol_setup_types(void)
 {
     pysqlite_PrepareProtocolType.tp_new = PyType_GenericNew;
-    Py_TYPE(&pysqlite_PrepareProtocolType)= &PyType_Type;
     return PyType_Ready(&pysqlite_PrepareProtocolType);
 }
```

### Comparing `litesync-0.4.9/src/prepare_protocol.h` & `litesync-0.5.0/src/prepare_protocol.h`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/row.c` & `litesync-0.5.0/src/row.c`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/row.h` & `litesync-0.5.0/src/row.h`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/statement.c` & `litesync-0.5.0/src/statement.c`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/statement.h` & `litesync-0.5.0/src/statement.h`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/util.c` & `litesync-0.5.0/src/util.c`

 * *Files identical despite different names*

### Comparing `litesync-0.4.9/src/util.h` & `litesync-0.5.0/src/util.h`

 * *Files identical despite different names*

