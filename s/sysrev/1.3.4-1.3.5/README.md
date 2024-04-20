# Comparing `tmp/sysrev-1.3.4.tar.gz` & `tmp/sysrev-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysrev-1.3.4.tar", last modified: Tue Apr 16 14:19:15 2024, max compression
+gzip compressed data, was "sysrev-1.3.5.tar", last modified: Sat Apr 20 01:04:13 2024, max compression
```

## Comparing `sysrev-1.3.4.tar` & `sysrev-1.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:15.860482 sysrev-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 14:19:15.860482 sysrev-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-16 14:19:08.000000 sysrev-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:19:15.860482 sysrev-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-16 14:19:08.000000 sysrev-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:15.856482 sysrev-1.3.4/sysrev/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 14:19:08.000000 sysrev-1.3.4/sysrev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-04-16 14:19:08.000000 sysrev-1.3.4/sysrev/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:15.860482 sysrev-1.3.4/sysrev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 14:19:15.000000 sysrev-1.3.4/sysrev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 14:19:15.000000 sysrev-1.3.4/sysrev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:19:15.000000 sysrev-1.3.4/sysrev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:19:15.000000 sysrev-1.3.4/sysrev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 14:19:15.000000 sysrev-1.3.4/sysrev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 14:19:15.000000 sysrev-1.3.4/sysrev.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:15.856482 sysrev-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-16 14:19:08.000000 sysrev-1.3.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-16 14:19:08.000000 sysrev-1.3.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:04:13.198064 sysrev-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-20 01:04:13.198064 sysrev-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-20 01:04:07.000000 sysrev-1.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:04:13.198064 sysrev-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-20 01:04:07.000000 sysrev-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:04:13.194064 sysrev-1.3.5/sysrev/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-20 01:04:07.000000 sysrev-1.3.5/sysrev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-04-20 01:04:07.000000 sysrev-1.3.5/sysrev/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:04:13.198064 sysrev-1.3.5/sysrev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-20 01:04:13.000000 sysrev-1.3.5/sysrev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-20 01:04:13.000000 sysrev-1.3.5/sysrev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:04:13.000000 sysrev-1.3.5/sysrev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:04:13.000000 sysrev-1.3.5/sysrev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 01:04:13.000000 sysrev-1.3.5/sysrev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 01:04:13.000000 sysrev-1.3.5/sysrev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:04:13.198064 sysrev-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-20 01:04:07.000000 sysrev-1.3.5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-20 01:04:07.000000 sysrev-1.3.5/tests/test_utils.py
```

### Comparing `sysrev-1.3.4/PKG-INFO` & `sysrev-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.3.4
+Version: 1.3.5
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `sysrev-1.3.4/setup.py` & `sysrev-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Assuming your README file is in Markdown
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='sysrev',
-    version='1.3.4',
+    version='1.3.5',
     description='get sysrev project data and use the sysrev api',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type here
     url='https://github.com/sysrev/PySysrev',
     author='Thomas Luechtefeld',
     author_email='tom@insilica.co',
     packages=['sysrev'],
```

### Comparing `sysrev-1.3.4/sysrev/client.py` & `sysrev-1.3.5/sysrev/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
         # Commit changes and close connection
         conn.commit()
         conn.close()
 
     # TODO - this could be made more efficient by checking sqlite state and updating the sysrev api
     def sync(self, client, project_id):
-        # check that db exists
+        
         if not pathlib.Path('.sr/sr.sqlite').exists():
             self.create_sqlite_db()
             
         project_info = client.get_project_info(project_id)
         
         labels = client.get_labels(project_id)
         labels_df = pd.DataFrame(labels)
@@ -107,19 +107,21 @@
         
         n_articles = project_info['result']['project']['stats']['articles']
         articles = [resp for resp in tqdm.tqdm(client.fetch_all_articles(project_id), total=n_articles)]
         
         article_labels = [a['labels'] for a in articles if a['labels'] is not None]
         article_labels = [lbl for lbls in article_labels for lbl in lbls]
         article_label_df = pd.DataFrame(article_labels)
+        article_label_df['answer'] = article_label_df['answer'].apply(json.dumps)
         
         article_data = [{k: v for k, v in a.items() if k != 'labels'} for a in articles]
         article_data_df = pd.DataFrame(article_data)
+        article_data_df['notes'] = article_data_df['notes'].apply(json.dumps)
         article_data_df['resolve'] = article_data_df['resolve'].apply(json.dumps)
-        
+            
         article_info = []
         for article_id in tqdm.tqdm(article_data_df['article-id'], total=n_articles):
             article_info.append(client.get_article_info(project_id, article_id))
         
         full_texts = pd.DataFrame([{**ft} for a in article_info for ft in a['article'].get('full-texts', []) ])
         full_texts.columns = [col.split('/')[-1] for col in full_texts.columns]
         
@@ -128,25 +130,34 @@
             for label_id, details in a['article'].get('auto-labels', {}).items() ])
         auto_labels['answer'] = auto_labels['answer'].apply(json.dumps)
         
         csl_citations = pd.DataFrame([
             {**{k: json.dumps(v) if isinstance(v, (dict, list)) else v for k, v in item['itemData'].items()}, 
              'article-id': a['article'].get('article-id')} 
             for a in article_info for item in a['article'].get('csl-citation', {}).get('citationItems', [])])
-            
+        csl_citations['issued'] = csl_citations['issued'].apply(json.dumps)
+        csl_citations['author'] = csl_citations['author'].apply(json.dumps)
+        
         # write everything to .sr/sr.sqlite
         conn = sqlite3.connect('.sr/sr.sqlite')
         
+        def write_df(df,name):
+            # replace any - with _ in column names and remove duplicates
+            df.columns = df.columns.str.replace('-', '_')
+            df = df.loc[:,~df.columns.duplicated()]
+            df.to_sql(name, conn, if_exists='replace', index=False) if not df.empty else None
+                
+                
         # Writing data to tables
-        labels_df.to_sql('labels', conn, if_exists='replace', index=False)
-        article_label_df.to_sql('article_label', conn, if_exists='replace', index=False)
-        article_data_df.to_sql('article_data', conn, if_exists='replace', index=False)
-        full_texts.to_sql('full_texts', conn, if_exists='replace', index=False)
-        auto_labels.to_sql('auto_labels', conn, if_exists='replace', index=False)
-        csl_citations.to_sql('csl_citations', conn, if_exists='replace', index=False)
+        write_df(labels_df,'labels')
+        write_df(article_label_df,'article_label')
+        write_df(article_data_df,'article_data')
+        write_df(full_texts,'full_texts')
+        write_df(auto_labels,'auto_labels')
+        write_df(csl_citations,'csl_citations')
         
         conn.close()
 class Client():
     
     def __init__(self, api_key, base_url="https://www.sysrev.com"):
         self.api_key = api_key
         self.base_url = base_url
```

### Comparing `sysrev-1.3.4/sysrev.egg-info/PKG-INFO` & `sysrev-1.3.5/sysrev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.3.4
+Version: 1.3.5
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `sysrev-1.3.4/tests/test_client.py` & `sysrev-1.3.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sysrev-1.3.4/tests/test_utils.py` & `sysrev-1.3.5/tests/test_utils.py`

 * *Files identical despite different names*

