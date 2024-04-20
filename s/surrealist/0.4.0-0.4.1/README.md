# Comparing `tmp/surrealist-0.4.0.tar.gz` & `tmp/surrealist-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surrealist-0.4.0.tar", last modified: Sun Apr 14 06:05:58 2024, max compression
+gzip compressed data, was "surrealist-0.4.1.tar", last modified: Sat Apr 20 09:06:33 2024, max compression
```

## Comparing `surrealist-0.4.0.tar` & `surrealist-0.4.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.290079 surrealist-0.4.0/
--rw-rw-rw-   0        0        0     1091 2024-02-04 05:55:53.000000 surrealist-0.4.0/LICENSE
--rw-rw-rw-   0        0        0    30967 2024-04-14 06:05:58.289079 surrealist-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    28957 2024-04-14 06:04:00.000000 surrealist-0.4.0/README.md
--rw-rw-rw-   0        0        0      905 2024-04-14 06:04:00.000000 surrealist-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 06:05:58.290079 surrealist-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.241079 surrealist-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.251050 surrealist-0.4.0/src/surrealist/
--rw-rw-rw-   0        0        0      757 2024-03-02 11:31:18.000000 surrealist-0.4.0/src/surrealist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.259079 surrealist-0.4.0/src/surrealist/clients/
--rw-rw-rw-   0        0        0      124 2024-02-04 05:55:53.000000 surrealist-0.4.0/src/surrealist/clients/__init__.py
--rw-rw-rw-   0        0        0     5044 2024-02-16 16:27:45.000000 surrealist-0.4.0/src/surrealist/clients/http_client.py
--rw-rw-rw-   0        0        0     8117 2024-02-16 16:26:19.000000 surrealist-0.4.0/src/surrealist/clients/ws_client.py
-drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.264063 surrealist-0.4.0/src/surrealist/connections/
--rw-rw-rw-   0        0        0      198 2024-02-04 05:55:53.000000 surrealist-0.4.0/src/surrealist/connections/__init__.py
--rw-rw-rw-   0        0        0    18589 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/connections/connection.py
--rw-rw-rw-   0        0        0    27023 2024-03-14 16:05:03.000000 surrealist-0.4.0/src/surrealist/connections/http_connection.py
--rw-rw-rw-   0        0        0     8023 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/connections/pool.py
--rw-rw-rw-   0        0        0    29659 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/connections/ws_connection.py
--rw-rw-rw-   0        0        0     2439 2024-03-14 15:59:51.000000 surrealist-0.4.0/src/surrealist/errors.py
-drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.268053 surrealist-0.4.0/src/surrealist/ql/
--rw-rw-rw-   0        0        0      231 2024-03-02 11:31:18.000000 surrealist-0.4.0/src/surrealist/ql/__init__.py
--rw-rw-rw-   0        0        0    15690 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/ql/database.py
--rw-rw-rw-   0        0        0     3135 2024-03-02 11:31:18.000000 surrealist-0.4.0/src/surrealist/ql/pool_database.py
-drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.287079 surrealist-0.4.0/src/surrealist/ql/statements/
--rw-rw-rw-   0        0        0      473 2024-02-11 10:03:17.000000 surrealist-0.4.0/src/surrealist/ql/statements/__init__.py
--rw-rw-rw-   0        0        0     2909 2024-02-11 13:05:41.000000 surrealist-0.4.0/src/surrealist/ql/statements/common_statements.py
--rw-rw-rw-   0        0        0     1518 2024-02-12 10:41:24.000000 surrealist-0.4.0/src/surrealist/ql/statements/create.py
--rw-rw-rw-   0        0        0     1345 2024-02-11 10:03:17.000000 surrealist-0.4.0/src/surrealist/ql/statements/create_statements.py
--rw-rw-rw-   0        0        0    15710 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/ql/statements/define.py
--rw-rw-rw-   0        0        0     1213 2024-02-19 06:12:19.000000 surrealist-0.4.0/src/surrealist/ql/statements/delete.py
--rw-rw-rw-   0        0        0     2409 2024-02-19 06:14:54.000000 surrealist-0.4.0/src/surrealist/ql/statements/insert.py
--rw-rw-rw-   0        0        0      496 2024-02-09 12:21:48.000000 surrealist-0.4.0/src/surrealist/ql/statements/insert_statements.py
--rw-rw-rw-   0        0        0     2967 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/ql/statements/live.py
--rw-rw-rw-   0        0        0     1289 2024-02-12 10:41:24.000000 surrealist-0.4.0/src/surrealist/ql/statements/live_statements.py
--rw-rw-rw-   0        0        0     1749 2024-02-19 06:06:05.000000 surrealist-0.4.0/src/surrealist/ql/statements/permissions.py
--rw-rw-rw-   0        0        0     1377 2024-02-12 10:41:24.000000 surrealist-0.4.0/src/surrealist/ql/statements/relate.py
--rw-rw-rw-   0        0        0     1792 2024-03-13 09:08:42.000000 surrealist-0.4.0/src/surrealist/ql/statements/remove.py
--rw-rw-rw-   0        0        0      825 2024-02-12 10:41:24.000000 surrealist-0.4.0/src/surrealist/ql/statements/returns.py
--rw-rw-rw-   0        0        0     3190 2024-02-19 06:14:54.000000 surrealist-0.4.0/src/surrealist/ql/statements/select.py
--rw-rw-rw-   0        0        0     8006 2024-02-11 12:57:39.000000 surrealist-0.4.0/src/surrealist/ql/statements/select_statements.py
--rw-rw-rw-   0        0        0     1808 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/ql/statements/show.py
--rw-rw-rw-   0        0        0     1510 2024-02-19 06:06:05.000000 surrealist-0.4.0/src/surrealist/ql/statements/simple_statements.py
--rw-rw-rw-   0        0        0     3436 2024-02-16 16:23:17.000000 surrealist-0.4.0/src/surrealist/ql/statements/statement.py
--rw-rw-rw-   0        0        0      924 2024-02-19 06:12:19.000000 surrealist-0.4.0/src/surrealist/ql/statements/transaction.py
--rw-rw-rw-   0        0        0     1273 2024-02-19 06:12:19.000000 surrealist-0.4.0/src/surrealist/ql/statements/update.py
--rw-rw-rw-   0        0        0     2079 2024-02-09 12:21:48.000000 surrealist-0.4.0/src/surrealist/ql/statements/update_statements.py
--rw-rw-rw-   0        0        0     8908 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/ql/table.py
--rw-rw-rw-   0        0        0     8695 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/result.py
--rw-rw-rw-   0        0        0     9831 2024-03-29 07:04:55.000000 surrealist-0.4.0/src/surrealist/surreal.py
--rw-rw-rw-   0        0        0     1578 2024-03-14 16:05:03.000000 surrealist-0.4.0/src/surrealist/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.288079 surrealist-0.4.0/src/surrealist.egg-info/
--rw-rw-rw-   0        0        0    30967 2024-04-14 06:05:58.000000 surrealist-0.4.0/src/surrealist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1729 2024-04-14 06:05:58.000000 surrealist-0.4.0/src/surrealist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 06:05:58.000000 surrealist-0.4.0/src/surrealist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-14 06:05:58.000000 surrealist-0.4.0/src/surrealist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-14 06:05:58.000000 surrealist-0.4.0/src/surrealist.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.703699 surrealist-0.4.1/
+-rw-rw-rw-   0        0        0     1091 2024-02-04 05:55:53.000000 surrealist-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0    31030 2024-04-20 09:06:33.702699 surrealist-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    29020 2024-04-20 09:05:50.000000 surrealist-0.4.1/README.md
+-rw-rw-rw-   0        0        0      905 2024-04-20 09:05:50.000000 surrealist-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-20 09:06:33.703699 surrealist-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.606738 surrealist-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.619746 surrealist-0.4.1/src/surrealist/
+-rw-rw-rw-   0        0        0      849 2024-04-20 09:05:50.000000 surrealist-0.4.1/src/surrealist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.632737 surrealist-0.4.1/src/surrealist/clients/
+-rw-rw-rw-   0        0        0      124 2024-02-04 05:55:53.000000 surrealist-0.4.1/src/surrealist/clients/__init__.py
+-rw-rw-rw-   0        0        0     5044 2024-02-16 16:27:45.000000 surrealist-0.4.1/src/surrealist/clients/http_client.py
+-rw-rw-rw-   0        0        0     8117 2024-02-16 16:26:19.000000 surrealist-0.4.1/src/surrealist/clients/ws_client.py
+drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.650740 surrealist-0.4.1/src/surrealist/connections/
+-rw-rw-rw-   0        0        0      198 2024-02-04 05:55:53.000000 surrealist-0.4.1/src/surrealist/connections/__init__.py
+-rw-rw-rw-   0        0        0    18589 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/connections/connection.py
+-rw-rw-rw-   0        0        0    27023 2024-03-14 16:05:03.000000 surrealist-0.4.1/src/surrealist/connections/http_connection.py
+-rw-rw-rw-   0        0        0     8023 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/connections/pool.py
+-rw-rw-rw-   0        0        0    29659 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/connections/ws_connection.py
+-rw-rw-rw-   0        0        0     2439 2024-03-14 15:59:51.000000 surrealist-0.4.1/src/surrealist/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.657740 surrealist-0.4.1/src/surrealist/ql/
+-rw-rw-rw-   0        0        0      231 2024-03-02 11:31:18.000000 surrealist-0.4.1/src/surrealist/ql/__init__.py
+-rw-rw-rw-   0        0        0    15690 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/ql/database.py
+-rw-rw-rw-   0        0        0     3135 2024-03-02 11:31:18.000000 surrealist-0.4.1/src/surrealist/ql/pool_database.py
+drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.700670 surrealist-0.4.1/src/surrealist/ql/statements/
+-rw-rw-rw-   0        0        0      473 2024-02-11 10:03:17.000000 surrealist-0.4.1/src/surrealist/ql/statements/__init__.py
+-rw-rw-rw-   0        0        0     2909 2024-02-11 13:05:41.000000 surrealist-0.4.1/src/surrealist/ql/statements/common_statements.py
+-rw-rw-rw-   0        0        0     1518 2024-02-12 10:41:24.000000 surrealist-0.4.1/src/surrealist/ql/statements/create.py
+-rw-rw-rw-   0        0        0     1345 2024-02-11 10:03:17.000000 surrealist-0.4.1/src/surrealist/ql/statements/create_statements.py
+-rw-rw-rw-   0        0        0    15710 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/ql/statements/define.py
+-rw-rw-rw-   0        0        0     1213 2024-02-19 06:12:19.000000 surrealist-0.4.1/src/surrealist/ql/statements/delete.py
+-rw-rw-rw-   0        0        0     2409 2024-02-19 06:14:54.000000 surrealist-0.4.1/src/surrealist/ql/statements/insert.py
+-rw-rw-rw-   0        0        0      496 2024-02-09 12:21:48.000000 surrealist-0.4.1/src/surrealist/ql/statements/insert_statements.py
+-rw-rw-rw-   0        0        0     2967 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/ql/statements/live.py
+-rw-rw-rw-   0        0        0     1289 2024-02-12 10:41:24.000000 surrealist-0.4.1/src/surrealist/ql/statements/live_statements.py
+-rw-rw-rw-   0        0        0     1749 2024-02-19 06:06:05.000000 surrealist-0.4.1/src/surrealist/ql/statements/permissions.py
+-rw-rw-rw-   0        0        0     1377 2024-02-12 10:41:24.000000 surrealist-0.4.1/src/surrealist/ql/statements/relate.py
+-rw-rw-rw-   0        0        0     1792 2024-03-13 09:08:42.000000 surrealist-0.4.1/src/surrealist/ql/statements/remove.py
+-rw-rw-rw-   0        0        0      825 2024-02-12 10:41:24.000000 surrealist-0.4.1/src/surrealist/ql/statements/returns.py
+-rw-rw-rw-   0        0        0     3190 2024-02-19 06:14:54.000000 surrealist-0.4.1/src/surrealist/ql/statements/select.py
+-rw-rw-rw-   0        0        0     8006 2024-02-11 12:57:39.000000 surrealist-0.4.1/src/surrealist/ql/statements/select_statements.py
+-rw-rw-rw-   0        0        0     1860 2024-04-20 09:05:50.000000 surrealist-0.4.1/src/surrealist/ql/statements/show.py
+-rw-rw-rw-   0        0        0     1510 2024-02-19 06:06:05.000000 surrealist-0.4.1/src/surrealist/ql/statements/simple_statements.py
+-rw-rw-rw-   0        0        0     3436 2024-02-16 16:23:17.000000 surrealist-0.4.1/src/surrealist/ql/statements/statement.py
+-rw-rw-rw-   0        0        0      924 2024-02-19 06:12:19.000000 surrealist-0.4.1/src/surrealist/ql/statements/transaction.py
+-rw-rw-rw-   0        0        0     1273 2024-02-19 06:12:19.000000 surrealist-0.4.1/src/surrealist/ql/statements/update.py
+-rw-rw-rw-   0        0        0     2079 2024-02-09 12:21:48.000000 surrealist-0.4.1/src/surrealist/ql/statements/update_statements.py
+-rw-rw-rw-   0        0        0     8908 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/ql/table.py
+-rw-rw-rw-   0        0        0     8695 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/result.py
+-rw-rw-rw-   0        0        0     9831 2024-03-29 07:04:55.000000 surrealist-0.4.1/src/surrealist/surreal.py
+-rw-rw-rw-   0        0        0     2221 2024-04-20 09:05:50.000000 surrealist-0.4.1/src/surrealist/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.701699 surrealist-0.4.1/src/surrealist.egg-info/
+-rw-rw-rw-   0        0        0    31030 2024-04-20 09:06:33.000000 surrealist-0.4.1/src/surrealist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1729 2024-04-20 09:06:33.000000 surrealist-0.4.1/src/surrealist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 09:06:33.000000 surrealist-0.4.1/src/surrealist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-20 09:06:33.000000 surrealist-0.4.1/src/surrealist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-20 09:06:33.000000 surrealist-0.4.1/src/surrealist.egg-info/top_level.txt
```

### Comparing `surrealist-0.4.0/LICENSE` & `surrealist-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/PKG-INFO` & `surrealist-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surrealist
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python client for SurrealDB, latest SurrealDB version compatible, all features supported
 Author-email: kotolex <farofwell@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -45,15 +45,15 @@
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
  * only one small dependency (websocket-client), no need to pull a lot of libraries to your project
  * fully documented
  * well tested (on the latest Ubuntu, macOS and Windows 10)
- * fully compatible with the latest version of SurrealDB (1.4.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
+ * fully compatible with the latest version of SurrealDB (1.4.2), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
  * debug mode to see all that goes in and out if you need
  * iterator to handle big select queries
  * QL-builder to explore, generate and use SurrealDB queries (explain, transaction etc.)
  * connections pool for use at a high load
  * http or websocket transport to use
  * always up to date with SurrealDB features and changes
 
@@ -501,19 +501,20 @@
 `[{'changes': [{'update': {'id': 'reading:w0useg3n9bkne6mei63f', 'story': 'long long time ago'}}], 'versionstamp': 851968}]`
 
 Same example via QL-builder:
 
 **Example 12**
 
 ```python
-from surrealist import Database
+from datetime import datetime, timezone
+from surrealist import Database, to_surreal_datetime_str
 
 
 with Database("http://127.0.0.1:8000", 'test', 'test', credentials=('root', 'root')) as db:
-    tm = "2024-02-06T10:48:08.700483Z" # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER the table was created
+    tm = to_surreal_datetime_str(datetime.now(timezone.utc)) # Again, here is a moment AFTER the table was created
     res = db.table("reading").show_changes().since(tm).run()
     print(res.result) # it will be [] cause no events happen
     # now we add one record
     db.table("reading").create().set(story="long long time ago").run()
     res = db.table("reading").show_changes().since(tm).run()
 ```
```

### Comparing `surrealist-0.4.0/README.md` & `surrealist-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
  * only one small dependency (websocket-client), no need to pull a lot of libraries to your project
  * fully documented
  * well tested (on the latest Ubuntu, macOS and Windows 10)
- * fully compatible with the latest version of SurrealDB (1.4.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
+ * fully compatible with the latest version of SurrealDB (1.4.2), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
  * debug mode to see all that goes in and out if you need
  * iterator to handle big select queries
  * QL-builder to explore, generate and use SurrealDB queries (explain, transaction etc.)
  * connections pool for use at a high load
  * http or websocket transport to use
  * always up to date with SurrealDB features and changes
 
@@ -463,19 +463,20 @@
 `[{'changes': [{'update': {'id': 'reading:w0useg3n9bkne6mei63f', 'story': 'long long time ago'}}], 'versionstamp': 851968}]`
 
 Same example via QL-builder:
 
 **Example 12**
 
 ```python
-from surrealist import Database
+from datetime import datetime, timezone
+from surrealist import Database, to_surreal_datetime_str
 
 
 with Database("http://127.0.0.1:8000", 'test', 'test', credentials=('root', 'root')) as db:
-    tm = "2024-02-06T10:48:08.700483Z" # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER the table was created
+    tm = to_surreal_datetime_str(datetime.now(timezone.utc)) # Again, here is a moment AFTER the table was created
     res = db.table("reading").show_changes().since(tm).run()
     print(res.result) # it will be [] cause no events happen
     # now we add one record
     db.table("reading").create().set(story="long long time ago").run()
     res = db.table("reading").show_changes().since(tm).run()
 ```
```

### Comparing `surrealist-0.4.0/pyproject.toml` & `surrealist-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "surrealist"
-version = "0.4.0"
+version = "0.4.1"
 description = "Python client for SurrealDB, latest SurrealDB version compatible, all features supported"
 readme = "README.md"
 authors = [{ name = "kotolex", email = "farofwell@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
```

### Comparing `surrealist-0.4.0/src/surrealist/__init__.py` & `surrealist-0.4.1/src/surrealist/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .connections import WebSocketConnection, HttpConnection, Connection
 from .errors import *
 from .ql import Database, DatabaseConnectionsPool, Table, Where
 from .result import SurrealResult
 from .surreal import Surreal
-from .utils import DATA_LENGTH_FOR_LOGS, get_uuid
+from .utils import DATA_LENGTH_FOR_LOGS, get_uuid, to_surreal_datetime_str, to_datetime
 
 __all__ = ("Surreal", "SurrealResult", "WebSocketConnection", "HttpConnection", "PySurrealError", "HttpConnectionError",
            "HttpClientError", "SurrealConnectionError", "WebSocketConnectionError", "WebSocketConnectionClosedError",
            "ConnectionParametersError", "CompatibilityError", "OperationOnClosedConnectionError", "WrongCallError",
-           "DATA_LENGTH_FOR_LOGS", "Connection", "get_uuid", "Database", "Table", "Where", "DatabaseConnectionsPool")
+           "DATA_LENGTH_FOR_LOGS", "Connection", "get_uuid", "Database", "Table", "Where", "DatabaseConnectionsPool",
+           "to_surreal_datetime_str", "to_datetime")
```

### Comparing `surrealist-0.4.0/src/surrealist/clients/http_client.py` & `surrealist-0.4.1/src/surrealist/clients/http_client.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/clients/ws_client.py` & `surrealist-0.4.1/src/surrealist/clients/ws_client.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/connections/connection.py` & `surrealist-0.4.1/src/surrealist/connections/connection.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/connections/http_connection.py` & `surrealist-0.4.1/src/surrealist/connections/http_connection.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/connections/pool.py` & `surrealist-0.4.1/src/surrealist/connections/pool.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/connections/ws_connection.py` & `surrealist-0.4.1/src/surrealist/connections/ws_connection.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/errors.py` & `surrealist-0.4.1/src/surrealist/errors.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/database.py` & `surrealist-0.4.1/src/surrealist/ql/database.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/pool_database.py` & `surrealist-0.4.1/src/surrealist/ql/pool_database.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/common_statements.py` & `surrealist-0.4.1/src/surrealist/ql/statements/common_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/create.py` & `surrealist-0.4.1/src/surrealist/ql/statements/create.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/create_statements.py` & `surrealist-0.4.1/src/surrealist/ql/statements/create_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/define.py` & `surrealist-0.4.1/src/surrealist/ql/statements/define.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/delete.py` & `surrealist-0.4.1/src/surrealist/ql/statements/delete.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/insert.py` & `surrealist-0.4.1/src/surrealist/ql/statements/insert.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/live.py` & `surrealist-0.4.1/src/surrealist/ql/statements/live.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/live_statements.py` & `surrealist-0.4.1/src/surrealist/ql/statements/live_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/permissions.py` & `surrealist-0.4.1/src/surrealist/ql/statements/permissions.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/relate.py` & `surrealist-0.4.1/src/surrealist/ql/statements/relate.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/remove.py` & `surrealist-0.4.1/src/surrealist/ql/statements/remove.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/returns.py` & `surrealist-0.4.1/src/surrealist/ql/statements/returns.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/select.py` & `surrealist-0.4.1/src/surrealist/ql/statements/select.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/select_statements.py` & `surrealist-0.4.1/src/surrealist/ql/statements/select_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/show.py` & `surrealist-0.4.1/src/surrealist/ql/statements/show.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import List, Optional
 
 from surrealist.connections import Connection
-from surrealist.utils import OK, DATE_FORMAT, DATE_FORMAT_NS
+from surrealist.utils import OK, DATE_FORMAT, DATE_FORMAT_NS, to_surreal_datetime_str
 from .statement import Statement
 
 
 class Show(Statement):
     """
     Represents SHOW CHANGES statement, it should be able to use any statements from documentation
 
@@ -24,25 +24,25 @@
     def validate(self) -> List[str]:
         result = []
         if self._since:
             try:
                 format_ = DATE_FORMAT if "." not in self._since else DATE_FORMAT_NS
                 datetime.strptime(self._since, format_)
             except ValueError:
-                result.append("Timestamp in wrong format, you need iso-date like 2024-01-01T10:10:10.000001Z")
+                result.append("Timestamp in the wrong format, you need iso-date like 2024-01-01T10:10:10.000001Z")
         if self._limit and self._limit < 1:
             result.append("Limit should not be less than 1")
         return [OK] if not result else result
 
     def limit(self, limit: int) -> "Show":
         self._limit = limit
         return self
 
     def since(self, timestamp: str) -> "Show":
         self._since = timestamp
         return self
 
     def _clean_str(self):
         if not self._since:
-            self._since = f'{datetime.utcnow().isoformat("T")}Z'  # default value
+            self._since = to_surreal_datetime_str(datetime.now(timezone.utc))  # default value
         limit = f" LIMIT {self._limit}" if self._limit else ""
         return f'SHOW CHANGES FOR TABLE {self._table_name} SINCE "{self._since}"{limit}'
```

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/simple_statements.py` & `surrealist-0.4.1/src/surrealist/ql/statements/simple_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/statement.py` & `surrealist-0.4.1/src/surrealist/ql/statements/statement.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/transaction.py` & `surrealist-0.4.1/src/surrealist/ql/statements/transaction.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/update.py` & `surrealist-0.4.1/src/surrealist/ql/statements/update.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/statements/update_statements.py` & `surrealist-0.4.1/src/surrealist/ql/statements/update_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/ql/table.py` & `surrealist-0.4.1/src/surrealist/ql/table.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/result.py` & `surrealist-0.4.1/src/surrealist/result.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist/surreal.py` & `surrealist-0.4.1/src/surrealist/surreal.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.0/src/surrealist.egg-info/PKG-INFO` & `surrealist-0.4.1/src/surrealist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surrealist
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python client for SurrealDB, latest SurrealDB version compatible, all features supported
 Author-email: kotolex <farofwell@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -45,15 +45,15 @@
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
  * only one small dependency (websocket-client), no need to pull a lot of libraries to your project
  * fully documented
  * well tested (on the latest Ubuntu, macOS and Windows 10)
- * fully compatible with the latest version of SurrealDB (1.4.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
+ * fully compatible with the latest version of SurrealDB (1.4.2), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
  * debug mode to see all that goes in and out if you need
  * iterator to handle big select queries
  * QL-builder to explore, generate and use SurrealDB queries (explain, transaction etc.)
  * connections pool for use at a high load
  * http or websocket transport to use
  * always up to date with SurrealDB features and changes
 
@@ -501,19 +501,20 @@
 `[{'changes': [{'update': {'id': 'reading:w0useg3n9bkne6mei63f', 'story': 'long long time ago'}}], 'versionstamp': 851968}]`
 
 Same example via QL-builder:
 
 **Example 12**
 
 ```python
-from surrealist import Database
+from datetime import datetime, timezone
+from surrealist import Database, to_surreal_datetime_str
 
 
 with Database("http://127.0.0.1:8000", 'test', 'test', credentials=('root', 'root')) as db:
-    tm = "2024-02-06T10:48:08.700483Z" # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER the table was created
+    tm = to_surreal_datetime_str(datetime.now(timezone.utc)) # Again, here is a moment AFTER the table was created
     res = db.table("reading").show_changes().since(tm).run()
     print(res.result) # it will be [] cause no events happen
     # now we add one record
     db.table("reading").create().set(story="long long time ago").run()
     res = db.table("reading").show_changes().since(tm).run()
 ```
```

### Comparing `surrealist-0.4.0/src/surrealist.egg-info/SOURCES.txt` & `surrealist-0.4.1/src/surrealist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

