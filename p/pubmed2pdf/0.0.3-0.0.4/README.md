# Comparing `tmp/pubmed2pdf-0.0.3.tar.gz` & `tmp/pubmed2pdf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pubmed2pdf-0.0.3.tar", last modified: Mon Jul 19 13:00:31 2021, max compression
+gzip compressed data, was "pubmed2pdf-0.0.4.tar", last modified: Sat Apr 20 15:54:50 2024, max compression
```

## Comparing `pubmed2pdf-0.0.3.tar` & `pubmed2pdf-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 danieldomingo   (501) staff       (20)        0 2021-07-19 13:00:31.143530 pubmed2pdf-0.0.3/
--rw-r--r--   0 danieldomingo   (501) staff       (20)     1082 2021-06-18 08:50:10.000000 pubmed2pdf-0.0.3/LICENSE
--rw-r--r--   0 danieldomingo   (501) staff       (20)      116 2021-06-18 08:50:10.000000 pubmed2pdf-0.0.3/MANIFEST.in
--rw-r--r--   0 danieldomingo   (501) staff       (20)     2473 2021-07-19 13:00:31.143708 pubmed2pdf-0.0.3/PKG-INFO
--rw-r--r--   0 danieldomingo   (501) staff       (20)     1321 2021-06-18 08:50:10.000000 pubmed2pdf-0.0.3/README.rst
--rw-r--r--   0 danieldomingo   (501) staff       (20)     1392 2021-07-19 13:00:31.144770 pubmed2pdf-0.0.3/setup.cfg
--rw-r--r--   0 danieldomingo   (501) staff       (20)      115 2021-06-18 08:50:10.000000 pubmed2pdf-0.0.3/setup.py
-drwxr-xr-x   0 danieldomingo   (501) staff       (20)        0 2021-07-19 13:00:31.134502 pubmed2pdf-0.0.3/src/
-drwxr-xr-x   0 danieldomingo   (501) staff       (20)        0 2021-07-19 13:00:31.139225 pubmed2pdf-0.0.3/src/pubmed2pdf/
--rw-r--r--   0 danieldomingo   (501) staff       (20)       41 2021-06-18 08:50:10.000000 pubmed2pdf-0.0.3/src/pubmed2pdf/__init__.py
--rw-r--r--   0 danieldomingo   (501) staff       (20)      110 2021-06-18 08:50:10.000000 pubmed2pdf-0.0.3/src/pubmed2pdf/__main__.py
--rw-r--r--   0 danieldomingo   (501) staff       (20)     4882 2021-07-19 12:41:18.000000 pubmed2pdf-0.0.3/src/pubmed2pdf/cli.py
--rw-r--r--   0 danieldomingo   (501) staff       (20)      551 2021-07-19 11:28:24.000000 pubmed2pdf-0.0.3/src/pubmed2pdf/constants.py
--rw-r--r--   0 danieldomingo   (501) staff       (20)     6190 2021-07-19 13:00:06.000000 pubmed2pdf-0.0.3/src/pubmed2pdf/utils.py
-drwxr-xr-x   0 danieldomingo   (501) staff       (20)        0 2021-07-19 13:00:31.143036 pubmed2pdf-0.0.3/src/pubmed2pdf.egg-info/
--rw-r--r--   0 danieldomingo   (501) staff       (20)     2473 2021-07-19 13:00:30.000000 pubmed2pdf-0.0.3/src/pubmed2pdf.egg-info/PKG-INFO
--rw-r--r--   0 danieldomingo   (501) staff       (20)      444 2021-07-19 13:00:31.000000 pubmed2pdf-0.0.3/src/pubmed2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 danieldomingo   (501) staff       (20)        1 2021-07-19 13:00:30.000000 pubmed2pdf-0.0.3/src/pubmed2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 danieldomingo   (501) staff       (20)       52 2021-07-19 13:00:30.000000 pubmed2pdf-0.0.3/src/pubmed2pdf.egg-info/entry_points.txt
--rw-r--r--   0 danieldomingo   (501) staff       (20)        1 2021-06-18 09:04:29.000000 pubmed2pdf-0.0.3/src/pubmed2pdf.egg-info/not-zip-safe
--rw-r--r--   0 danieldomingo   (501) staff       (20)       65 2021-07-19 13:00:30.000000 pubmed2pdf-0.0.3/src/pubmed2pdf.egg-info/requires.txt
--rw-r--r--   0 danieldomingo   (501) staff       (20)       11 2021-07-19 13:00:30.000000 pubmed2pdf-0.0.3/src/pubmed2pdf.egg-info/top_level.txt
+drwxr-xr-x   0 danieldomingo   (501) staff       (20)        0 2024-04-20 15:54:50.748299 pubmed2pdf-0.0.4/
+-rw-r--r--   0 danieldomingo   (501) staff       (20)     1082 2024-04-20 15:53:52.000000 pubmed2pdf-0.0.4/LICENSE
+-rw-r--r--   0 danieldomingo   (501) staff       (20)      116 2024-04-20 15:53:52.000000 pubmed2pdf-0.0.4/MANIFEST.in
+-rw-r--r--   0 danieldomingo   (501) staff       (20)     2593 2024-04-20 15:54:50.748220 pubmed2pdf-0.0.4/PKG-INFO
+-rw-r--r--   0 danieldomingo   (501) staff       (20)     1321 2024-04-20 15:53:52.000000 pubmed2pdf-0.0.4/README.rst
+-rw-r--r--   0 danieldomingo   (501) staff       (20)     1392 2024-04-20 15:54:50.748664 pubmed2pdf-0.0.4/setup.cfg
+-rw-r--r--   0 danieldomingo   (501) staff       (20)      115 2024-04-20 15:53:52.000000 pubmed2pdf-0.0.4/setup.py
+drwxr-xr-x   0 danieldomingo   (501) staff       (20)        0 2024-04-20 15:54:50.745318 pubmed2pdf-0.0.4/src/
+drwxr-xr-x   0 danieldomingo   (501) staff       (20)        0 2024-04-20 15:54:50.746732 pubmed2pdf-0.0.4/src/pubmed2pdf/
+-rw-r--r--   0 danieldomingo   (501) staff       (20)       41 2024-04-20 15:53:52.000000 pubmed2pdf-0.0.4/src/pubmed2pdf/__init__.py
+-rw-r--r--   0 danieldomingo   (501) staff       (20)      110 2024-04-20 15:53:52.000000 pubmed2pdf-0.0.4/src/pubmed2pdf/__main__.py
+-rw-r--r--   0 danieldomingo   (501) staff       (20)     5176 2024-04-20 15:53:52.000000 pubmed2pdf-0.0.4/src/pubmed2pdf/cli.py
+-rw-r--r--   0 danieldomingo   (501) staff       (20)      551 2024-04-20 15:53:52.000000 pubmed2pdf-0.0.4/src/pubmed2pdf/constants.py
+-rw-r--r--   0 danieldomingo   (501) staff       (20)     6387 2024-04-20 15:53:52.000000 pubmed2pdf-0.0.4/src/pubmed2pdf/utils.py
+drwxr-xr-x   0 danieldomingo   (501) staff       (20)        0 2024-04-20 15:54:50.747970 pubmed2pdf-0.0.4/src/pubmed2pdf.egg-info/
+-rw-r--r--   0 danieldomingo   (501) staff       (20)     2593 2024-04-20 15:54:50.000000 pubmed2pdf-0.0.4/src/pubmed2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 danieldomingo   (501) staff       (20)      444 2024-04-20 15:54:50.000000 pubmed2pdf-0.0.4/src/pubmed2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 danieldomingo   (501) staff       (20)        1 2024-04-20 15:54:50.000000 pubmed2pdf-0.0.4/src/pubmed2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 danieldomingo   (501) staff       (20)       51 2024-04-20 15:54:50.000000 pubmed2pdf-0.0.4/src/pubmed2pdf.egg-info/entry_points.txt
+-rw-r--r--   0 danieldomingo   (501) staff       (20)        1 2024-04-20 15:54:50.000000 pubmed2pdf-0.0.4/src/pubmed2pdf.egg-info/not-zip-safe
+-rw-r--r--   0 danieldomingo   (501) staff       (20)       65 2024-04-20 15:54:50.000000 pubmed2pdf-0.0.4/src/pubmed2pdf.egg-info/requires.txt
+-rw-r--r--   0 danieldomingo   (501) staff       (20)       11 2024-04-20 15:54:50.000000 pubmed2pdf-0.0.4/src/pubmed2pdf.egg-info/top_level.txt
```

### Comparing `pubmed2pdf-0.0.3/LICENSE` & `pubmed2pdf-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pubmed2pdf-0.0.3/PKG-INFO` & `pubmed2pdf-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: pubmed2pdf
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package to download PDFs from OA publications in PubMed
 Home-page: https://github.com/ddomingof/PubMed2PDF
+Download-URL: https://github.com/ddomingof/PubMed2PDF
 Author: Daniel Domingo-Fernández
 Author-email: ddomingof@gmail.com
 Maintainer: Daniel Domingo-Fernández
 Maintainer-email: ddomingof@gmail.com
 License: MIT License
-Download-URL: https://github.com/ddomingof/PubMed2PDF
 Project-URL: Bug Tracker, https://github.com/ddomingof/PubMed2PDF/issues
 Project-URL: Source Code, https://github.com/ddomingof/PubMed2PDF
 Project-URL: Documentation, https://github.com/ddomingof/PubMed2PDF
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 License-File: LICENSE
+Requires-Dist: click==7.0
+Requires-Dist: requests==2.22.0
+Requires-Dist: requests3
+Requires-Dist: beautifulsoup4==4.7.1
+Requires-Dist: lxml
 
 PubMed2PDF
 ==========
 
 A Python package to download PDFs from OA publications in PubMed. The underlying code is forked from
 https://github.com/billgreenwald/Pubmed-Batch-Download. Downloaded files are located  by default in your personal folder under the 'pubmed2pdf' directory.
 
@@ -74,9 +78,7 @@
     $ python3 -m pubmed2pdf pdf --pmids="123, 1234, 12345"
 
 Run the help command to see all functionalities
 
 .. code-block:: sh
 
     $ python3 -m pubmed2pdf pdf --help
-
-
```

### Comparing `pubmed2pdf-0.0.3/README.rst` & `pubmed2pdf-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `pubmed2pdf-0.0.3/setup.cfg` & `pubmed2pdf-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pubmed2pdf
-version = 0.0.3
+version = 0.0.4
 description = A Python package to download PDFs from OA publications in PubMed
 long_description = file: README.rst
 url = https://github.com/ddomingof/PubMed2PDF
 download_url = https://github.com/ddomingof/PubMed2PDF
 project_urls = 
 	Bug Tracker = https://github.com/ddomingof/PubMed2PDF/issues
 	Source Code = https://github.com/ddomingof/PubMed2PDF
```

### Comparing `pubmed2pdf-0.0.3/src/pubmed2pdf/cli.py` & `pubmed2pdf-0.0.4/src/pubmed2pdf/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,26 +27,27 @@
     '--exported',
     help='Output file path for pmids which were succesfully downloaded', default=SUCCESSFULLY_DOWN_FILES,
     type=click.Path(),
     show_default=True,
 )
 @click.option('--maxtries', help='Max number of tries per article', default=3, type=int, show_default=True)
 @click.option('-v', '--verbose', help='Log everything', is_flag=True)
-def pdf(pmids, pmidsfile, out, errors, exported, maxtries, verbose):
+@click.option('--search', help='Search terms for use in PubMed', type=str)
+def pdf(pmids, pmidsfile, out, errors, exported, maxtries, verbose, search):
     """Get PDFs from PubMed idenfiers."""
 
     if verbose:
         logger.setLevel(logging.DEBUG)
         logger.debug('Full log mode activated')
     else:
         logger.setLevel(logging.INFO)
 
     # Checking arguments
-    if not pmids and not pmidsfile:
-        click.echo("Error: One of the two arguments '--pmids' or '--pmidsfile' must be used. Exiting...")
+    if not pmids and not pmidsfile and not search:
+        click.echo("Error: One of the arguments '--pmids' or '--pmidsfile' or '--search' must be used. Exiting...")
         exit(1)
     if pmids and pmidsfile:
         click.echo("Error: --pmids and --pmidsfile cannot be used together. Please select only one. Exiting...")
         exit(1)
 
     if not os.path.exists(out):
         click.echo(f"Output directory of {out} did not exist.  Created the directory.")
@@ -66,22 +67,29 @@
     # Add headers
     headers = requests.utils.default_headers()
     headers['User-Agent'] = 'Mozilla/5.0 (X11; Linux x86_64) ' \
                             'AppleWebKit/537.36 (KHTML, like Gecko) ' \
                             'Chrome/56.0.2924.87 ' \
                             'Safari/537.36'
 
+
     if pmids:
         # Split by comma the pubmeds
         pmids = [i.strip() for i in pmids.split(",")]
         names = pmids
+    elif search:
+    	# Get list of  pubmeds from search
+        pmids = search_pubmed(search)
+        print(pmids)
+        #pmids = [i.strip() for i in pmids.split(",")]
+        names = pmids
     else:
         # Read file and get the pubmeds
         pmids = [
-            line.strip().split().strip()
+            line.strip().split()
             for line in open(pmidsfile)
         ]
         # Get names if there are two columns
         if len(pmids[0]) == 1:
             pmids = [
                 x[0]
                 for x in pmids
```

### Comparing `pubmed2pdf-0.0.3/src/pubmed2pdf/constants.py` & `pubmed2pdf-0.0.4/src/pubmed2pdf/constants.py`

 * *Files identical despite different names*

### Comparing `pubmed2pdf-0.0.3/src/pubmed2pdf/utils.py` & `pubmed2pdf-0.0.4/src/pubmed2pdf/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import os
 import re
 import urllib
 
 import requests
 from bs4 import BeautifulSoup
 
+from Bio import Entrez
+
 logger = logging.getLogger(__name__)
 
 
 def getMainUrl(url):
     return "/".join(url.split("/")[:3])
 
 
@@ -66,14 +68,21 @@
                 break
 
     if not success:
         logger.debug("** Reprint {0} could not be fetched with the current finders.".format(pmid))
         errorPmids.write("{}\t{}\n".format(pmid, name))
 
 
+def search_pubmed(query):
+    handle = Entrez.esearch(db="pubmed", term=query, retmax=100)
+    record = Entrez.read(handle)
+    handle.close()
+    return record["IdList"]
+
+
 def acsPublications(req, soup, headers):
     possibleLinks = [
         x
         for x in soup.find_all('a')
         if type(x.get('title')) == str and (
             'high-res pdf' in x.get('title').lower()
             or 'low-res pdf' in x.get('title').lower())
```

### Comparing `pubmed2pdf-0.0.3/src/pubmed2pdf.egg-info/PKG-INFO` & `pubmed2pdf-0.0.4/src/pubmed2pdf.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: pubmed2pdf
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package to download PDFs from OA publications in PubMed
 Home-page: https://github.com/ddomingof/PubMed2PDF
+Download-URL: https://github.com/ddomingof/PubMed2PDF
 Author: Daniel Domingo-Fernández
 Author-email: ddomingof@gmail.com
 Maintainer: Daniel Domingo-Fernández
 Maintainer-email: ddomingof@gmail.com
 License: MIT License
-Download-URL: https://github.com/ddomingof/PubMed2PDF
 Project-URL: Bug Tracker, https://github.com/ddomingof/PubMed2PDF/issues
 Project-URL: Source Code, https://github.com/ddomingof/PubMed2PDF
 Project-URL: Documentation, https://github.com/ddomingof/PubMed2PDF
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 License-File: LICENSE
+Requires-Dist: click==7.0
+Requires-Dist: requests==2.22.0
+Requires-Dist: requests3
+Requires-Dist: beautifulsoup4==4.7.1
+Requires-Dist: lxml
 
 PubMed2PDF
 ==========
 
 A Python package to download PDFs from OA publications in PubMed. The underlying code is forked from
 https://github.com/billgreenwald/Pubmed-Batch-Download. Downloaded files are located  by default in your personal folder under the 'pubmed2pdf' directory.
 
@@ -74,9 +78,7 @@
     $ python3 -m pubmed2pdf pdf --pmids="123, 1234, 12345"
 
 Run the help command to see all functionalities
 
 .. code-block:: sh
 
     $ python3 -m pubmed2pdf pdf --help
-
-
```

