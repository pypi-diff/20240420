# Comparing `tmp/paper2vec-0.2.tar.gz` & `tmp/paper2vec-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper2vec-0.2.tar", last modified: Thu Apr 18 19:54:56 2024, max compression
+gzip compressed data, was "paper2vec-0.3.tar", last modified: Sat Apr 20 02:01:18 2024, max compression
```

## Comparing `paper2vec-0.2.tar` & `paper2vec-0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:54:56.393822 paper2vec-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-18 19:54:49.000000 paper2vec-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-18 19:54:56.393822 paper2vec-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 19:54:49.000000 paper2vec-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:54:56.393822 paper2vec-0.2/paper2vec/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-18 19:54:49.000000 paper2vec-0.2/paper2vec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-18 19:54:49.000000 paper2vec-0.2/paper2vec/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:54:56.393822 paper2vec-0.2/paper2vec/datadestination/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 19:54:49.000000 paper2vec-0.2/paper2vec/datadestination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-18 19:54:49.000000 paper2vec-0.2/paper2vec/datadestination/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:54:56.393822 paper2vec-0.2/paper2vec/datasource/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 19:54:49.000000 paper2vec-0.2/paper2vec/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-18 19:54:49.000000 paper2vec-0.2/paper2vec/datasource/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:54:56.393822 paper2vec-0.2/paper2vec/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-18 19:54:49.000000 paper2vec-0.2/paper2vec/scripts/qdrant_create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:54:56.393822 paper2vec-0.2/paper2vec/vectorizer/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 19:54:49.000000 paper2vec-0.2/paper2vec/vectorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-18 19:54:49.000000 paper2vec-0.2/paper2vec/vectorizer/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:54:56.393822 paper2vec-0.2/paper2vec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-18 19:54:56.000000 paper2vec-0.2/paper2vec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-18 19:54:56.000000 paper2vec-0.2/paper2vec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:54:56.000000 paper2vec-0.2/paper2vec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 19:54:56.000000 paper2vec-0.2/paper2vec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 19:54:56.000000 paper2vec-0.2/paper2vec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:54:56.393822 paper2vec-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-18 19:54:49.000000 paper2vec-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:18.830881 paper2vec-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-20 02:01:13.000000 paper2vec-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-20 02:01:18.830881 paper2vec-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 02:01:13.000000 paper2vec-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:18.830881 paper2vec-0.3/paper2vec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-20 02:01:13.000000 paper2vec-0.3/paper2vec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-20 02:01:13.000000 paper2vec-0.3/paper2vec/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:18.830881 paper2vec-0.3/paper2vec/datadestination/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-20 02:01:13.000000 paper2vec-0.3/paper2vec/datadestination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-20 02:01:13.000000 paper2vec-0.3/paper2vec/datadestination/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:18.830881 paper2vec-0.3/paper2vec/datasource/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-20 02:01:13.000000 paper2vec-0.3/paper2vec/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-20 02:01:13.000000 paper2vec-0.3/paper2vec/datasource/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:18.830881 paper2vec-0.3/paper2vec/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-20 02:01:13.000000 paper2vec-0.3/paper2vec/scripts/qdrant_create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:18.830881 paper2vec-0.3/paper2vec/vectorizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-20 02:01:13.000000 paper2vec-0.3/paper2vec/vectorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-20 02:01:13.000000 paper2vec-0.3/paper2vec/vectorizer/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:18.830881 paper2vec-0.3/paper2vec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-20 02:01:18.000000 paper2vec-0.3/paper2vec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-20 02:01:18.000000 paper2vec-0.3/paper2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:01:18.000000 paper2vec-0.3/paper2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-20 02:01:18.000000 paper2vec-0.3/paper2vec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 02:01:18.000000 paper2vec-0.3/paper2vec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 02:01:18.830881 paper2vec-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-20 02:01:13.000000 paper2vec-0.3/setup.py
```

### Comparing `paper2vec-0.2/LICENSE` & `paper2vec-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paper2vec-0.2/paper2vec/__main__.py` & `paper2vec-0.3/paper2vec/__main__.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.2/paper2vec/abc.py` & `paper2vec-0.3/paper2vec/abc.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.2/paper2vec/datadestination/qdrant.py` & `paper2vec-0.3/paper2vec/datadestination/qdrant.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.2/paper2vec/datasource/neo4j.py` & `paper2vec-0.3/paper2vec/datasource/neo4j.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,44 +3,59 @@
 from argparse import ArgumentParser
 
 
 async def get_papers(tx, query):
     papers = []
     for record in await (await tx.run(query)).values():
         if "title" not in record[0]:
+            papers.append(None)
             continue
         paper = "Title: " + record[0]["title"]
         payload = {"title": record[0]["title"], "title_hash": record[0]["title_hash"]}
         if "abstract" in record[0]:
             paper += " Abstract: " + record[0]["abstract"]
         content = Content(id=record[0]["title_hash"], text=paper, payload=payload)
         papers.append(content)
     return papers
 
 
+async def get_total(tx, query):
+    records = await (await tx.run(query)).values()
+    return records[0][0]
+
+
 class GraphQuery(DataSource):
     @staticmethod
     def add_arguements(parser: ArgumentParser):
         parser.add_argument("--username", type=str, default=None, help=f'Auth username to neo4j database.')
         parser.add_argument("--password", type=str, default=None, help=f'Auth password to neo4j database.')
         parser.add_argument("--uri", type=str, required=True, help=f'URI to neo4j database.')
         parser.add_argument("--query", type=str,
                             default="MATCH (n:Publication)",
-                            help=f'Query to get data. "RETURN n SKIP ... LIMIT <batch_size>" will be added behind ')
+                            help=f'Query to get data. "RETURN n SKIP ... LIMIT <batch_size>" will be added behind.')
+        parser.add_argument("--tail", type=int, default=0,
+                            help=f'If you only want to get last couple of items, use it.')
 
     def __init__(self, args):
         self.uri = args.uri
         self.username = args.username
         self.password = args.password
         self.query = args.query
         self.batch_size = args.batch_size
+        self.tail = args.tail
 
     async def get_contents(self):
         async with AsyncGraphDatabase.driver(self.uri, auth=(self.username, self.password)) as driver:
             async with driver.session() as session:
-                papers = await session.execute_read(get_papers, self.query + (" RETURN n LIMIT %d" % self.batch_size))
-                skip = self.batch_size
+                skip = 0
+                if self.tail > 0:
+                    total = await session.execute_read(get_total, self.query + " RETURN COUNT(n)")
+                    skip = total - self.tail
+                papers = await session.execute_read(get_papers, self.query + (" RETURN n SKIP %d LIMIT %d" % (skip, self.batch_size)))
+                skip += self.batch_size
                 while len(papers) > 0:
                     for paper in papers:
+                        if paper is None:
+                            continue
                         yield paper
                     papers = await session.execute_read(get_papers, self.query + (" RETURN n SKIP %d LIMIT %d" % (skip, self.batch_size)))
                     skip += self.batch_size
```

### Comparing `paper2vec-0.2/paper2vec/vectorizer/openai.py` & `paper2vec-0.3/paper2vec/vectorizer/openai.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.2/setup.py` & `paper2vec-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'paper2vec.datasource': 'paper2vec/datasource',
     'paper2vec.vectorizer': 'paper2vec/vectorizer',
     'paper2vec.scripts': 'paper2vec/scripts',
 }
 
 setup(
     name='paper2vec',
-    version='0.2',
+    version='0.3',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/paper2vec',
     description=u'Turn your collected papers into vectors!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

