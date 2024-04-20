# Comparing `tmp/flatpack-3.3.6.tar.gz` & `tmp/flatpack-3.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.3.6.tar", last modified: Fri Apr 19 23:45:37 2024, max compression
+gzip compressed data, was "flatpack-3.3.7.tar", last modified: Sat Apr 20 00:33:13 2024, max compression
```

## Comparing `flatpack-3.3.6.tar` & `flatpack-3.3.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:45:37.754659 flatpack-3.3.6/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.6/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     5243 2024-04-19 23:45:37.754373 flatpack-3.3.6/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     4583 2024-04-19 13:23:47.000000 flatpack-3.3.6/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:45:37.751879 flatpack-3.3.6/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/datasets.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26884 2024-04-19 23:45:08.000000 flatpack-3.3.6/flatpack/main.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/models.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:45:37.753600 flatpack-3.3.6/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.6/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.6/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6394 2024-04-19 23:44:50.000000 flatpack-3.3.6/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-19 23:45:37.754047 flatpack-3.3.6/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     5243 2024-04-19 23:45:37.000000 flatpack-3.3.6/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-19 23:45:37.000000 flatpack-3.3.6/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-19 23:45:37.000000 flatpack-3.3.6/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-19 23:45:37.000000 flatpack-3.3.6/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      218 2024-04-19 23:45:37.000000 flatpack-3.3.6/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-19 23:45:37.000000 flatpack-3.3.6/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-19 23:45:37.754733 flatpack-3.3.6/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)      939 2024-04-19 23:45:29.000000 flatpack-3.3.6/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:33:13.252400 flatpack-3.3.7/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.7/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6049 2024-04-20 00:33:13.252092 flatpack-3.3.7/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5360 2024-04-20 00:32:11.000000 flatpack-3.3.7/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:33:13.247801 flatpack-3.3.7/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.7/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.7/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.7/flatpack/datasets.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.7/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26884 2024-04-19 23:45:08.000000 flatpack-3.3.7/flatpack/main.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.7/flatpack/models.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:33:13.251406 flatpack-3.3.7/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.7/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.7/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.7/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.7/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.7/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6394 2024-04-19 23:44:50.000000 flatpack-3.3.7/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:33:13.251751 flatpack-3.3.7/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6049 2024-04-20 00:33:13.000000 flatpack-3.3.7/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-20 00:33:13.000000 flatpack-3.3.7/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-20 00:33:13.000000 flatpack-3.3.7/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-20 00:33:13.000000 flatpack-3.3.7/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      232 2024-04-20 00:33:13.000000 flatpack-3.3.7/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-20 00:33:13.000000 flatpack-3.3.7/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-20 00:33:13.252459 flatpack-3.3.7/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      964 2024-04-20 00:33:08.000000 flatpack-3.3.7/setup.py
```

### Comparing `flatpack-3.3.6/LICENSE` & `flatpack-3.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.6/PKG-INFO` & `flatpack-3.3.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.6
+Version: 3.3.7
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
 Requires-Dist: nltk==3.8.1
+Requires-Dist: olefile==0.47
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: sentence-transformers==2.6.1
 Requires-Dist: toml==0.10.2
 Requires-Dist: torch==2.2.2
 Requires-Dist: uvicorn==0.29.0
 
@@ -66,57 +67,58 @@
 
 ## License
 
 This project is released under [Apache-2.0](https://github.com/romlingroup/flatpack-ai/blob/main/LICENSE).
 
 ## install_requires
 
-BSD-3-Clause (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of
-the original BSD-licensed component when distributed
-separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-3-Clause/Apache-2.0)).
-
-MIT (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the
-original MIT-licensed component when distributed
-separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/MIT/Apache-2.0)).
-
-*Check out
-the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (
-European Commission 2023).*
+**DISCLAIMER:** The license compatibility information provided herein serves solely as a technical reference. It does not imply endorsement or legal advice. Users are encouraged to perform compatibility checks and consult with legal experts before commercially utilising any software. The user is responsible for ensuring compliance with applicable licensing requirements.
+
+BSD 2-Clause "Simplified" License (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-2-Clause/Apache-2.0)).
+
+BSD-3-Clause (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-3-Clause/Apache-2.0)).
+
+MIT (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original MIT-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/MIT/Apache-2.0)).
+
+*Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).*
 
 - **[beautifulsoup4](https://pypi.org/project/beautifulsoup4/)**\
   MIT ([LICENSE](https://pypi.org/project/beautifulsoup4/))
 
 - **[cryptography](https://pypi.org/project/cryptography/)**\
   Apache-2.0 OR BSD-3-Clause ([LICENSE](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
 
 - **[faiss-cpu](https://pypi.org/project/faiss-cpu/)**\
   MIT ([LICENSE](https://github.com/kyamagu/faiss-wheels/blob/main/LICENSE))
 
 - **[fastapi](https://pypi.org/project/fastapi/)**\
   MIT ([LICENSE](https://github.com/tiangolo/fastapi/blob/master/LICENSE))
 
 - **[httpx](https://pypi.org/project/httpx/)**\
-  BSD-3-Clause ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
+  BSD ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
 - **[ngrok](https://pypi.org/project/ngrok/)**\
   Apache-2.0 OR MIT ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
 - **[nltk](https://pypi.org/project/nltk/)**\
   Apache-2.0 ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
 
+- **[olefile](https://pypi.org/project/olefile/)**\
+  BSD ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt)
+
 - **[pypdf](https://pypi.org/project/pypdf/)**\
-  BSD-3-Clause ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE)
+  BSD ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE)
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache-2.0 ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
   Apache-2.0 ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
 
 - **[toml](https://pypi.org/project/toml/)**\
   MIT ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
 - **[torch](https://pypi.org/project/torch/)**\
   BSD-3-Clause ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
 
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
-  BSD-3-Clause ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
+  BSD ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
```

### Comparing `flatpack-3.3.6/README.md` & `flatpack-3.3.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -43,57 +43,58 @@
 
 ## License
 
 This project is released under [Apache-2.0](https://github.com/romlingroup/flatpack-ai/blob/main/LICENSE).
 
 ## install_requires
 
-BSD-3-Clause (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of
-the original BSD-licensed component when distributed
-separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-3-Clause/Apache-2.0)).
-
-MIT (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the
-original MIT-licensed component when distributed
-separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/MIT/Apache-2.0)).
-
-*Check out
-the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (
-European Commission 2023).*
+**DISCLAIMER:** The license compatibility information provided herein serves solely as a technical reference. It does not imply endorsement or legal advice. Users are encouraged to perform compatibility checks and consult with legal experts before commercially utilising any software. The user is responsible for ensuring compliance with applicable licensing requirements.
+
+BSD 2-Clause "Simplified" License (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-2-Clause/Apache-2.0)).
+
+BSD-3-Clause (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-3-Clause/Apache-2.0)).
+
+MIT (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original MIT-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/MIT/Apache-2.0)).
+
+*Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).*
 
 - **[beautifulsoup4](https://pypi.org/project/beautifulsoup4/)**\
   MIT ([LICENSE](https://pypi.org/project/beautifulsoup4/))
 
 - **[cryptography](https://pypi.org/project/cryptography/)**\
   Apache-2.0 OR BSD-3-Clause ([LICENSE](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
 
 - **[faiss-cpu](https://pypi.org/project/faiss-cpu/)**\
   MIT ([LICENSE](https://github.com/kyamagu/faiss-wheels/blob/main/LICENSE))
 
 - **[fastapi](https://pypi.org/project/fastapi/)**\
   MIT ([LICENSE](https://github.com/tiangolo/fastapi/blob/master/LICENSE))
 
 - **[httpx](https://pypi.org/project/httpx/)**\
-  BSD-3-Clause ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
+  BSD ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
 - **[ngrok](https://pypi.org/project/ngrok/)**\
   Apache-2.0 OR MIT ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
 - **[nltk](https://pypi.org/project/nltk/)**\
   Apache-2.0 ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
 
+- **[olefile](https://pypi.org/project/olefile/)**\
+  BSD ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt)
+
 - **[pypdf](https://pypi.org/project/pypdf/)**\
-  BSD-3-Clause ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE)
+  BSD ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE)
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache-2.0 ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
   Apache-2.0 ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
 
 - **[toml](https://pypi.org/project/toml/)**\
   MIT ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
 - **[torch](https://pypi.org/project/torch/)**\
   BSD-3-Clause ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
 
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
-  BSD-3-Clause ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
+  BSD ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
```

### Comparing `flatpack-3.3.6/flatpack/datasets.py` & `flatpack-3.3.7/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.6/flatpack/instructions.py` & `flatpack-3.3.7/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.6/flatpack/main.py` & `flatpack-3.3.7/flatpack/main.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.6/flatpack/modules/lstm.py` & `flatpack-3.3.7/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.6/flatpack/modules/rnn.py` & `flatpack-3.3.7/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.6/flatpack/parsers.py` & `flatpack-3.3.7/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.6/flatpack/vector_manager.py` & `flatpack-3.3.7/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.6/flatpack.egg-info/PKG-INFO` & `flatpack-3.3.7/flatpack.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.6
+Version: 3.3.7
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
 Requires-Dist: nltk==3.8.1
+Requires-Dist: olefile==0.47
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: sentence-transformers==2.6.1
 Requires-Dist: toml==0.10.2
 Requires-Dist: torch==2.2.2
 Requires-Dist: uvicorn==0.29.0
 
@@ -66,57 +67,58 @@
 
 ## License
 
 This project is released under [Apache-2.0](https://github.com/romlingroup/flatpack-ai/blob/main/LICENSE).
 
 ## install_requires
 
-BSD-3-Clause (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of
-the original BSD-licensed component when distributed
-separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-3-Clause/Apache-2.0)).
-
-MIT (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the
-original MIT-licensed component when distributed
-separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/MIT/Apache-2.0)).
-
-*Check out
-the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (
-European Commission 2023).*
+**DISCLAIMER:** The license compatibility information provided herein serves solely as a technical reference. It does not imply endorsement or legal advice. Users are encouraged to perform compatibility checks and consult with legal experts before commercially utilising any software. The user is responsible for ensuring compliance with applicable licensing requirements.
+
+BSD 2-Clause "Simplified" License (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-2-Clause/Apache-2.0)).
+
+BSD-3-Clause (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-3-Clause/Apache-2.0)).
+
+MIT (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original MIT-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/MIT/Apache-2.0)).
+
+*Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).*
 
 - **[beautifulsoup4](https://pypi.org/project/beautifulsoup4/)**\
   MIT ([LICENSE](https://pypi.org/project/beautifulsoup4/))
 
 - **[cryptography](https://pypi.org/project/cryptography/)**\
   Apache-2.0 OR BSD-3-Clause ([LICENSE](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
 
 - **[faiss-cpu](https://pypi.org/project/faiss-cpu/)**\
   MIT ([LICENSE](https://github.com/kyamagu/faiss-wheels/blob/main/LICENSE))
 
 - **[fastapi](https://pypi.org/project/fastapi/)**\
   MIT ([LICENSE](https://github.com/tiangolo/fastapi/blob/master/LICENSE))
 
 - **[httpx](https://pypi.org/project/httpx/)**\
-  BSD-3-Clause ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
+  BSD ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
 - **[ngrok](https://pypi.org/project/ngrok/)**\
   Apache-2.0 OR MIT ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
 - **[nltk](https://pypi.org/project/nltk/)**\
   Apache-2.0 ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
 
+- **[olefile](https://pypi.org/project/olefile/)**\
+  BSD ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt)
+
 - **[pypdf](https://pypi.org/project/pypdf/)**\
-  BSD-3-Clause ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE)
+  BSD ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE)
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache-2.0 ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
   Apache-2.0 ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
 
 - **[toml](https://pypi.org/project/toml/)**\
   MIT ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
 - **[torch](https://pypi.org/project/torch/)**\
   BSD-3-Clause ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
 
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
-  BSD-3-Clause ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
+  BSD ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
```

### Comparing `flatpack-3.3.6/setup.py` & `flatpack-3.3.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.3.6",
+    version="3.3.7",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.1",
         "httpx==0.27.0",
         "ngrok==1.2.0",
         "nltk==3.8.1",
+        "olefile==0.47",
         "pypdf==4.2.0",
         "requests==2.31.0",
         "sentence-transformers==2.6.1",
         "toml==0.10.2",
         "torch==2.2.2",
         "uvicorn==0.29.0"
     ],
```

