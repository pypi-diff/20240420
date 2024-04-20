# Comparing `tmp/processwebpage-0.0.1.tar.gz` & `tmp/processwebpage-0.0.2.tar.gz`

## Comparing `processwebpage-0.0.1.tar` & `processwebpage-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 processwebpage-0.0.1/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 processwebpage-0.0.1/src/processwebpage/__init__.py
--rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 processwebpage-0.0.1/src/processwebpage/processwebpage.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 processwebpage-0.0.1/LICENSE
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 processwebpage-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 processwebpage-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 processwebpage-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 processwebpage-0.0.2/src/processwebpagepkg/__init__.py
+-rw-r--r--   0        0        0    10878 2020-02-02 00:00:00.000000 processwebpage-0.0.2/src/processwebpagepkg/processwebpage.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 processwebpage-0.0.2/LICENSE
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 processwebpage-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 processwebpage-0.0.2/PKG-INFO
```

### Comparing `processwebpage-0.0.1/README.md` & `processwebpage-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `processwebpage-0.0.1/src/processwebpage/processwebpage.py` & `processwebpage-0.0.2/src/processwebpagepkg/processwebpage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 '''Created By: Lalit Jagotra'''
-from databasev2 import database
+#from databasev2 import database
 from urllib import request
 import string
 import re
 import fileinput
 import json
 
 
 class ProcessWebpage:
     def __init__(self, HTMLContent):
         self.HTMLContent= HTMLContent
         self.indexedhtml=dict()
 
     def SearchHTML(self):
         #print("SearchHTML code...HTMLCOntent:{}".format(self.HTMLContent))
-        db2=database(filename= "C:/Python_Files\Password_Management/Application/HTMLindexing", table="Indexpage")
-        db2.connect_database()
-        query = 'drop table if exists Indexpage'
-        db2.sql_noparam(query)
+        #db2=database(filename= "C:/Python_Files\Password_Management/Application/HTMLindexing", table="Indexpage")
+        #db2.connect_database()
+        #query = 'drop table if exists Indexpage'
+        #db2.sql_noparam(query)
         Tagsname= "(?P<tagname>(?<=\<)\w+)"
         Tagsboundary="(<\tagname.*?[(\>)|(</\tagname>)])"
         testhtml= "<html><head><link rel='shortcut icon' href='#' /></head><body><div id=1234><p style='bold'>This is default response from server</p></div><div></div></body></html>"
         tagparams={}
         indexedhtml={}
         try:
             Tagsnamere =re.finditer(Tagsname,str(self.HTMLContent["Default"]),re.DOTALL)
```

### Comparing `processwebpage-0.0.1/LICENSE` & `processwebpage-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `processwebpage-0.0.1/pyproject.toml` & `processwebpage-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires=["hatchling"]
 build-backend="hatchling.build"
 [project]
 name= "processwebpage"
-version = "0.0.1"
+version = "0.0.2"
 authors= [
 {"name"= "Lalit Jagotra", "email"= "lalit.jagotra@gmail.com"},
 ]
 description= "ProcessWebpage is python module used for indexing HTML code and make changes to the HTML page dynamically while updating HTML attributes, HTML tag content etc. Support of Javascript processing is currenly under development."
 requires-python= ">=3.8"
 classifiers=[
 "Programming Language :: Python :: 3",
```

### Comparing `processwebpage-0.0.1/PKG-INFO` & `processwebpage-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: processwebpage
-Version: 0.0.1
+Version: 0.0.2
 Summary: ProcessWebpage is python module used for indexing HTML code and make changes to the HTML page dynamically while updating HTML attributes, HTML tag content etc. Support of Javascript processing is currenly under development.
 Project-URL: Homepage, https://github.com/lalit1029/applications
 Project-URL: Issues, https://github.com/lalit1029/applications/issues
 Author-email: Lalit Jagotra <lalit.jagotra@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

