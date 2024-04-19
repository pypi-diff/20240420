# Comparing `tmp/flatpack-3.3.2.tar.gz` & `tmp/flatpack-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.3.2.tar", last modified: Fri Apr 19 09:07:02 2024, max compression
+gzip compressed data, was "flatpack-3.3.3.tar", last modified: Fri Apr 19 23:27:21 2024, max compression
```

## Comparing `flatpack-3.3.2.tar` & `flatpack-3.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 09:07:02.003759 flatpack-3.3.2/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.2/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     5089 2024-04-19 09:07:02.003428 flatpack-3.3.2/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     4456 2024-04-16 19:54:33.000000 flatpack-3.3.2/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 09:07:02.000175 flatpack-3.3.2/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/datasets.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26284 2024-04-19 09:06:10.000000 flatpack-3.3.2/flatpack/main.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/models.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 09:07:02.002647 flatpack-3.3.2/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.2/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.2/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4020 2024-04-19 09:03:52.000000 flatpack-3.3.2/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 09:07:02.003041 flatpack-3.3.2/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     5089 2024-04-19 09:07:01.000000 flatpack-3.3.2/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-19 09:07:01.000000 flatpack-3.3.2/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-19 09:07:01.000000 flatpack-3.3.2/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-19 09:07:01.000000 flatpack-3.3.2/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      206 2024-04-19 09:07:01.000000 flatpack-3.3.2/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-19 09:07:01.000000 flatpack-3.3.2/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-19 09:07:02.003836 flatpack-3.3.2/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)      916 2024-04-19 09:06:34.000000 flatpack-3.3.2/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:27:21.309039 flatpack-3.3.3/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.3/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5243 2024-04-19 23:27:21.308580 flatpack-3.3.3/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4583 2024-04-19 13:23:47.000000 flatpack-3.3.3/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:27:21.305277 flatpack-3.3.3/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.3/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.3/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.3/flatpack/datasets.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.3/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26872 2024-04-19 23:23:50.000000 flatpack-3.3.3/flatpack/main.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.3/flatpack/models.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:27:21.307764 flatpack-3.3.3/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.3/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.3/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.3/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.3/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.3/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6293 2024-04-19 23:25:36.000000 flatpack-3.3.3/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:27:21.308132 flatpack-3.3.3/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5243 2024-04-19 23:27:21.000000 flatpack-3.3.3/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-19 23:27:21.000000 flatpack-3.3.3/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-19 23:27:21.000000 flatpack-3.3.3/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-19 23:27:21.000000 flatpack-3.3.3/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      218 2024-04-19 23:27:21.000000 flatpack-3.3.3/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-19 23:27:21.000000 flatpack-3.3.3/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-19 23:27:21.309156 flatpack-3.3.3/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      939 2024-04-19 13:23:06.000000 flatpack-3.3.3/setup.py
```

### Comparing `flatpack-3.3.2/LICENSE` & `flatpack-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.2/PKG-INFO` & `flatpack-3.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.2
+Version: 3.3.3
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: cryptography==42.0.5
 Requires-Dist: faiss-cpu==1.8.0
 Requires-Dist: fastapi==0.110.1
 Requires-Dist: httpx==0.27.0
 Requires-Dist: ngrok==1.2.0
+Requires-Dist: nltk==3.8.1
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: sentence-transformers==2.6.1
 Requires-Dist: toml==0.10.2
 Requires-Dist: torch==2.2.2
 Requires-Dist: uvicorn==0.29.0
 
@@ -95,14 +96,17 @@
 
 - **[httpx](https://pypi.org/project/httpx/)**\
   BSD-3-Clause ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
 - **[ngrok](https://pypi.org/project/ngrok/)**\
   Apache-2.0 OR MIT ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
+- **[nltk](https://pypi.org/project/nltk/)**\
+  Apache-2.0 ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
+
 - **[pypdf](https://pypi.org/project/pypdf/)**\
   BSD-3-Clause ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE)
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache-2.0 ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
```

### Comparing `flatpack-3.3.2/README.md` & `flatpack-3.3.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -73,14 +73,17 @@
 
 - **[httpx](https://pypi.org/project/httpx/)**\
   BSD-3-Clause ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
 - **[ngrok](https://pypi.org/project/ngrok/)**\
   Apache-2.0 OR MIT ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
+- **[nltk](https://pypi.org/project/nltk/)**\
+  Apache-2.0 ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
+
 - **[pypdf](https://pypi.org/project/pypdf/)**\
   BSD-3-Clause ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE)
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache-2.0 ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
```

### Comparing `flatpack-3.3.2/flatpack/datasets.py` & `flatpack-3.3.3/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.2/flatpack/instructions.py` & `flatpack-3.3.3/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.2/flatpack/main.py` & `flatpack-3.3.3/flatpack/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -562,14 +562,18 @@
             parser_add_pdf = subparsers.add_parser('vector-add-pdf',
                                                    help='Add text from a PDF file to the vector database.')
             parser_add_pdf.add_argument('pdf_path', help='Path to the PDF file to add.')
 
             parser_add_url = subparsers.add_parser('vector-add-url', help='Add text from a URL to the vector database.')
             parser_add_url.add_argument('url', help='URL to add.')
 
+            parser_add_wikipedia_page = subparsers.add_parser('vector-add-wikipedia-page',
+                                                              help='Add text from a Wikipedia page to the vector database.')
+            parser_add_wikipedia_page.add_argument('page_title', help='The title of the Wikipedia page to add.')
+
             args = parser.parse_args()
 
             fpk_get_api_key()
 
             if args.command == 'vector-add-texts':
                 vm.add_texts(args.texts)
                 print(f"Added {len(args.texts)} texts to the database.")
@@ -607,14 +611,18 @@
                     if response.status_code >= 200 and response.status_code < 400:
                         vm.add_url(url)
                         print(f"✅ Added text from URL: '{url}' to the vector database.")
                     else:
                         print(f"❌ URL is not accessible: '{url}'. HTTP Status Code: {response.status_code}")
                 except requests.RequestException as e:
                     print(f"❌ Failed to access URL: '{url}'. Error: {e}")
+            elif args.command == 'vector-add-wikipedia-page':
+                page_title = args.page_title
+                vm.add_wikipedia_page(page_title)
+                print(f"✅ Added text from Wikipedia page: '{page_title}' to the vector database.")
             elif args.command == "find":
                 print(fpk_find_models())
             elif args.command == "help":
                 print("[HELP]")
             elif args.command == "get-api-key":
                 print(fpk_get_api_key())
             elif args.command == "unbox":
```

### Comparing `flatpack-3.3.2/flatpack/modules/lstm.py` & `flatpack-3.3.3/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.2/flatpack/modules/rnn.py` & `flatpack-3.3.3/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.2/flatpack/parsers.py` & `flatpack-3.3.3/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.2/flatpack.egg-info/PKG-INFO` & `flatpack-3.3.3/flatpack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.2
+Version: 3.3.3
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: cryptography==42.0.5
 Requires-Dist: faiss-cpu==1.8.0
 Requires-Dist: fastapi==0.110.1
 Requires-Dist: httpx==0.27.0
 Requires-Dist: ngrok==1.2.0
+Requires-Dist: nltk==3.8.1
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: sentence-transformers==2.6.1
 Requires-Dist: toml==0.10.2
 Requires-Dist: torch==2.2.2
 Requires-Dist: uvicorn==0.29.0
 
@@ -95,14 +96,17 @@
 
 - **[httpx](https://pypi.org/project/httpx/)**\
   BSD-3-Clause ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
 - **[ngrok](https://pypi.org/project/ngrok/)**\
   Apache-2.0 OR MIT ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
+- **[nltk](https://pypi.org/project/nltk/)**\
+  Apache-2.0 ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
+
 - **[pypdf](https://pypi.org/project/pypdf/)**\
   BSD-3-Clause ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE)
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache-2.0 ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
```

### Comparing `flatpack-3.3.2/setup.py` & `flatpack-3.3.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.3.2",
+    version="3.3.3",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.1",
         "httpx==0.27.0",
         "ngrok==1.2.0",
+        "nltk==3.8.1",
         "pypdf==4.2.0",
         "requests==2.31.0",
         "sentence-transformers==2.6.1",
         "toml==0.10.2",
         "torch==2.2.2",
         "uvicorn==0.29.0"
     ],
```

