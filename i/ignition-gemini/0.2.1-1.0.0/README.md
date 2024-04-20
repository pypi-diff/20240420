# Comparing `tmp/ignition_gemini-0.2.1.tar.gz` & `tmp/ignition_gemini-1.0.0.tar.gz`

## Comparing `ignition_gemini-0.2.1.tar` & `ignition_gemini-1.0.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/__init__.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/__main__.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/exceptions.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/globals.py
--rw-r--r--   0        0        0    14119 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/request.py
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/response.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/url.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/util.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/__init__.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_10/LICENSE_NOTICE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_10/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_10/Lib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_10/Lib/urllib/__init__.py
--rw-r--r--   0        0        0    42344 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_10/Lib/urllib/parse.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_11/LICENSE_NOTICE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_11/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_11/Lib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_11/Lib/urllib/__init__.py
--rw-r--r--   0        0        0    42612 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_11/Lib/urllib/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_12/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_12/Lib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_12/Lib/urllib/__init__.py
--rw-r--r--   0        0        0    44947 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_12/Lib/urllib/parse.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_7/LICENSE_NOTICE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_7/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_7/Lib/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_7/Lib/urllib/__init__.py
--rw-r--r--   0        0        0    38818 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_7/Lib/urllib/parse.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_8/LICENSE_NOTICE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_8/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_8/Lib/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_8/Lib/urllib/__init__.py
--rw-r--r--   0        0        0    41750 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_8/Lib/urllib/parse.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_9/LICENSE_NOTICE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_9/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_9/Lib/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_9/Lib/urllib/__init__.py
--rw-r--r--   0        0        0    41749 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/python/python3_9/Lib/urllib/parse.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/ssl/__init__.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/ssl/cert_record.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/ssl/cert_store.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/ignition/ssl/cert_wrapper.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/LICENSE
--rw-r--r--   0        0        0     8534 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/README.md
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 ignition_gemini-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/__init__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/__main__.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/exceptions.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/globals.py
+-rw-r--r--   0        0        0    14119 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/request.py
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/response.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/url.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/util.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_10/LICENSE_NOTICE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_10/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_10/Lib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_10/Lib/urllib/__init__.py
+-rw-r--r--   0        0        0    42344 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_10/Lib/urllib/parse.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_11/LICENSE_NOTICE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_11/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_11/Lib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_11/Lib/urllib/__init__.py
+-rw-r--r--   0        0        0    42612 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_11/Lib/urllib/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_12/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_12/Lib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_12/Lib/urllib/__init__.py
+-rw-r--r--   0        0        0    44947 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_12/Lib/urllib/parse.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_7/LICENSE_NOTICE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_7/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_7/Lib/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_7/Lib/urllib/__init__.py
+-rw-r--r--   0        0        0    38818 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_7/Lib/urllib/parse.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_8/LICENSE_NOTICE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_8/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_8/Lib/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_8/Lib/urllib/__init__.py
+-rw-r--r--   0        0        0    41750 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_8/Lib/urllib/parse.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_9/LICENSE_NOTICE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_9/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_9/Lib/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_9/Lib/urllib/__init__.py
+-rw-r--r--   0        0        0    41749 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/python/python3_9/Lib/urllib/parse.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/ssl/__init__.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/ssl/cert_record.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/ssl/cert_store.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/ignition/ssl/cert_wrapper.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/README.md
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9926 2020-02-02 00:00:00.000000 ignition_gemini-1.0.0/PKG-INFO
```

### Comparing `ignition_gemini-0.2.1/ignition/__init__.py` & `ignition_gemini-1.0.0/ignition/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     RedirectResponse,
     SuccessResponse,
     TempFailureResponse,
 )
 from .ssl.cert_store import CertStore
 from .util import TimeoutManager
 
-__version__ = "0.2.1"
+__version__ = "1.0.0"
 
 __timeout = TimeoutManager(DEFAULT_REQUEST_TIMEOUT)
 __cert_store = CertStore(DEFAULT_HOSTS_FILE)
 
 
 def set_default_hosts_file(hosts_file):
     """
```

### Comparing `ignition_gemini-0.2.1/ignition/exceptions.py` & `ignition_gemini-1.0.0/ignition/exceptions.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/globals.py` & `ignition_gemini-1.0.0/ignition/globals.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/request.py` & `ignition_gemini-1.0.0/ignition/request.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/response.py` & `ignition_gemini-1.0.0/ignition/response.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/url.py` & `ignition_gemini-1.0.0/ignition/url.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/util.py` & `ignition_gemini-1.0.0/ignition/util.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/python/__init__.py` & `ignition_gemini-1.0.0/ignition/python/__init__.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/python/python3_10/Lib/urllib/parse.py` & `ignition_gemini-1.0.0/ignition/python/python3_10/Lib/urllib/parse.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/python/python3_11/Lib/urllib/parse.py` & `ignition_gemini-1.0.0/ignition/python/python3_11/Lib/urllib/parse.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/python/python3_12/Lib/urllib/parse.py` & `ignition_gemini-1.0.0/ignition/python/python3_12/Lib/urllib/parse.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/python/python3_7/Lib/urllib/parse.py` & `ignition_gemini-1.0.0/ignition/python/python3_7/Lib/urllib/parse.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/python/python3_8/Lib/urllib/parse.py` & `ignition_gemini-1.0.0/ignition/python/python3_8/Lib/urllib/parse.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/python/python3_9/Lib/urllib/parse.py` & `ignition_gemini-1.0.0/ignition/python/python3_9/Lib/urllib/parse.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/ssl/cert_record.py` & `ignition_gemini-1.0.0/ignition/ssl/cert_record.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/ssl/cert_store.py` & `ignition_gemini-1.0.0/ignition/ssl/cert_store.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/ignition/ssl/cert_wrapper.py` & `ignition_gemini-1.0.0/ignition/ssl/cert_wrapper.py`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/LICENSE` & `ignition_gemini-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ignition_gemini-0.2.1/README.md` & `ignition_gemini-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,18 @@
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/cbrews/ignition?label=ignition)
 [![CI v2](https://github.com/cbrews/ignition/actions/workflows/ci-v2.yml/badge.svg)](https://github.com/cbrews/ignition/actions/workflows/ci-v2.yml)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ignition-gemini)
 ![PyPI - License](https://img.shields.io/pypi/l/ignition-gemini)
 
 ![The status is good to go.  This is Gemini Control.](docs/img/transcript-2.png)
 
-Ignition is currently in prerelease.  You can use Ignition today at your own risk, please monitor this repository for changes until version 1.0 is released.  Please be advised that there may be breaking changes in the API until that time.
-
-You can see ignition in action at [gemini.cbrews.xyz](https://gemini.cbrews.xyz).
+Ignition is no longer being updated.
 
 ## Installation
-⚠ Ignition currently supports Python versions 3.7 - 3.11.
+⚠ Ignition supports Python versions 3.7 - 3.12.
 
 Ignition can be installed via [PIP](https://pypi.org/project/ignition-gemini/).  You should install it in alignment with your current development process; if you do not have a build process yet, I recommend you install within a [virtual environment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/)
 
 ```bash
 pip install ignition-gemini
 ```
 
@@ -57,15 +55,15 @@
 
 In **all** cases, Ignition assumes that the specified endpoint and protocol will respond over the Gemini protocol, so even if you provide a different protocol or port, it will assume that the endpoint is a Gemini capsule.
 
 ## Key Features
 
 ![This is Gemini Control.  The conversation between pilot and ground so far in this filght has largely been confined to the normal type of test pilot talk that you would expect.](docs/img/transcript-3.png)
 
-✅ Ignition currently supports the following features:
+✅ Ignition supports the following features:
 * Basic request/response connectivity to a Gemini-enabled server.
 * Basic URL parsing mechanics to allow for specifying protocol, host, port, path, and query params, as per [RFC-3986](https://tools.ietf.org/html/rfc3986)
 * Optional referer URL handling.  Ignition allows the user to pass a path & referer URL and can construct the new path, to simplifying the resolution of links on a Gemini capsule page.
 * Basic decoding of body responses on successful (20) response from Gemini servers.
 * Trust-on-first-use certificate verification handling scheme using key signatures.
 * Fully-featured response objects for each response type.
 * Standardized & robust, human-readable error management.
@@ -75,16 +73,14 @@
 * Behavioral processing/handling of specific response types from Gemini capsules, including:
   * Generation of client certificates & automatic resubmission.
   * Automatic redirection following on 3x responses.
 * Advanced body response rendering and/or display of text/gemini mime types.
 * Command line or GUI interface.
 * Advanced session & history management.
 * Support for other protocols.
-
-⚠ These features are not currently supported but may be supported in the future:
 * Non-verified certificate scheme
 * Improved TOFU scenarios
 
 ## Advanced Usage
 More advanced request usage:
 
 ```python
@@ -153,22 +149,20 @@
 ## API Documentation
 Full API documentation for Ignition is available [here](./docs/api.md).
 
 ## Developers
 
 ![There are a few reports from the pilots.  They are simply identifying their flight plan very carefully.  Four minutes into the flight, Gordon Cooper just told Grissom that he is looking mighty good.  Gus gave him a reasuring laugh.  A very calm pilot in command of that spacecraft.](docs/img/transcript-4.png)
 
-Want to help contribute to Ignition?  See the [developer documentation](./docs/developer.md) for contribution guidelines, build processes, and testing.
-
-The developer documentation is still being completed, if you have specific questions, please open tickets within this project.
+Ignition is no longer accepting contributions.  Please feel free to fork this repository.
 
 ## License
 Ignition is licensed under [Mozilla Public License 2.0](https://www.mozilla.org/en-US/MPL/).
 
-Copyright 2020-2022 by [Chris Brousseau](https://github.com/cbrews).
+Copyright 2020-2024 by [Chris Brousseau](https://github.com/cbrews).
 
 ## Thank you
 * *solderpunk* for leading the design of the [Gemini protocol](https://geminiprotocol.net/docs/specification.html), without which this project would not have been possible.
 * *Sean Conman* for writing the [Gemini torture tests](gemini://gemini.conman.org/test/torture), which were instrumental in initial client testing.
 * *Michael Lazar* for his work on [Jetforce](https://github.com/michael-lazar/jetforce), which helped testing along the way.
 
 🔭 Happy exploring!
```

### Comparing `ignition_gemini-0.2.1/pyproject.toml` & `ignition_gemini-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   { name="Chris Brousseau", email="cbrews@users.noreply.github.com" },
 ]
 description = "ignition - Gemini Protocol Client Transport Library"
 readme = "README.md"
 license = { text = "MPL 2.0" }
 requires-python = ">=3.7"
 classifiers = [
-  "Development Status :: 3 - Alpha",
+  "Development Status :: 7 - Inactive",
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Libraries",
   "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -31,32 +31,32 @@
 dynamic = ["version"]
 dependencies = [
   "cryptography>=36.0.0",
 ]
 
 [project.optional-dependencies]
 dev = [
-  "cryptography==41.0.4",
+  "cryptography==42.0.5",
   "mock==5.1.0",
-  "pytest==7.4.2",
+  "pytest==7.4.4",
   "pytest-cov==4.1.0",
   "pytest-mock==3.11.1",
-  "black==23.10.1",
-  "pre-commit==3.5.0",
-  "ruff==0.1.3",
+  "black==24.4.0",
+  "pre-commit==3.7.0",
+  "ruff==0.4.0",
 ]
 lint = [
-  "ruff==0.1.3",
-  "black==23.10.1",
+  "ruff==0.4.0",
+  "black==24.4.0",
   "mock==5.1.0",
-  "pytest==7.4.2",
+  "pytest==7.4.4",
 ]
 test = [
   "mock==5.1.0",
-  "pytest==7.4.2",
+  "pytest==7.4.4",
   "pytest-cov==4.1.0",
   "pytest-mock==3.11.1",
 ]
 build = [
   "build",
   "twine",
 ]
@@ -74,14 +74,17 @@
 [tool.hatch.build.targets.sdist]
 include = [
     '/README.md',
     '/LICENSE',
     '/ignition',
 ]
 
+[tool.hatch.build.targets.wheel]
+packages = ["ignition"]
+
 [tool.black]
 exclude = "ignition/python"
 
 [tool.ruff]
 select = [
   "I", # isort
   "PLC", # pylint conventions
```

### Comparing `ignition_gemini-0.2.1/PKG-INFO` & `ignition_gemini-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ignition-gemini
-Version: 0.2.1
+Version: 1.0.0
 Summary: ignition - Gemini Protocol Client Transport Library
 Project-URL: Homepage, https://github.com/cbrews/ignition
 Author-email: Chris Brousseau <cbrews@users.noreply.github.com>
 License: MPL 2.0
 License-File: LICENSE
 Keywords: client,gemini,networking,request,socket
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 7 - Inactive
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,32 +21,32 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Requires-Dist: cryptography>=36.0.0
 Provides-Extra: build
 Requires-Dist: build; extra == 'build'
 Requires-Dist: twine; extra == 'build'
 Provides-Extra: dev
-Requires-Dist: black==23.10.1; extra == 'dev'
-Requires-Dist: cryptography==41.0.4; extra == 'dev'
+Requires-Dist: black==24.4.0; extra == 'dev'
+Requires-Dist: cryptography==42.0.5; extra == 'dev'
 Requires-Dist: mock==5.1.0; extra == 'dev'
-Requires-Dist: pre-commit==3.5.0; extra == 'dev'
+Requires-Dist: pre-commit==3.7.0; extra == 'dev'
 Requires-Dist: pytest-cov==4.1.0; extra == 'dev'
 Requires-Dist: pytest-mock==3.11.1; extra == 'dev'
-Requires-Dist: pytest==7.4.2; extra == 'dev'
-Requires-Dist: ruff==0.1.3; extra == 'dev'
+Requires-Dist: pytest==7.4.4; extra == 'dev'
+Requires-Dist: ruff==0.4.0; extra == 'dev'
 Provides-Extra: lint
-Requires-Dist: black==23.10.1; extra == 'lint'
+Requires-Dist: black==24.4.0; extra == 'lint'
 Requires-Dist: mock==5.1.0; extra == 'lint'
-Requires-Dist: pytest==7.4.2; extra == 'lint'
-Requires-Dist: ruff==0.1.3; extra == 'lint'
+Requires-Dist: pytest==7.4.4; extra == 'lint'
+Requires-Dist: ruff==0.4.0; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: mock==5.1.0; extra == 'test'
 Requires-Dist: pytest-cov==4.1.0; extra == 'test'
 Requires-Dist: pytest-mock==3.11.1; extra == 'test'
-Requires-Dist: pytest==7.4.2; extra == 'test'
+Requires-Dist: pytest==7.4.4; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Ignition: Python3 Gemini Protocol Client Transport Library
 
 ![This is Gemini Control.  We're at T-1 minute, T-60 seconds and counting.  T-45 seconds and counting.  The range holding a final status check.  T-30 seconds.  Recorders have gone to fast speed.  Twenty seconds.  Fifteen seconds.  Ten, nine, eight, seven, six, five, four, three, two, one zero.  Ignition.](docs/img/transcript-1.png)
 
 Ignition is a simple but powerful transport library for Python3 clients using the recently designed [Gemini protocol](https://geminiprotocol.net/). This project intends to implement all of the [transport specifications](https://geminiprotocol.net/docs/specification.gmi) (sections 1-4) of the Gemini protocol and provide an easy-to-use interface, so as to act as a building block in a larger application.
@@ -61,20 +61,18 @@
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/cbrews/ignition?label=ignition)
 [![CI v2](https://github.com/cbrews/ignition/actions/workflows/ci-v2.yml/badge.svg)](https://github.com/cbrews/ignition/actions/workflows/ci-v2.yml)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ignition-gemini)
 ![PyPI - License](https://img.shields.io/pypi/l/ignition-gemini)
 
 ![The status is good to go.  This is Gemini Control.](docs/img/transcript-2.png)
 
-Ignition is currently in prerelease.  You can use Ignition today at your own risk, please monitor this repository for changes until version 1.0 is released.  Please be advised that there may be breaking changes in the API until that time.
-
-You can see ignition in action at [gemini.cbrews.xyz](https://gemini.cbrews.xyz).
+Ignition is no longer being updated.
 
 ## Installation
-⚠ Ignition currently supports Python versions 3.7 - 3.11.
+⚠ Ignition supports Python versions 3.7 - 3.12.
 
 Ignition can be installed via [PIP](https://pypi.org/project/ignition-gemini/).  You should install it in alignment with your current development process; if you do not have a build process yet, I recommend you install within a [virtual environment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/)
 
 ```bash
 pip install ignition-gemini
 ```
 
@@ -104,15 +102,15 @@
 
 In **all** cases, Ignition assumes that the specified endpoint and protocol will respond over the Gemini protocol, so even if you provide a different protocol or port, it will assume that the endpoint is a Gemini capsule.
 
 ## Key Features
 
 ![This is Gemini Control.  The conversation between pilot and ground so far in this filght has largely been confined to the normal type of test pilot talk that you would expect.](docs/img/transcript-3.png)
 
-✅ Ignition currently supports the following features:
+✅ Ignition supports the following features:
 * Basic request/response connectivity to a Gemini-enabled server.
 * Basic URL parsing mechanics to allow for specifying protocol, host, port, path, and query params, as per [RFC-3986](https://tools.ietf.org/html/rfc3986)
 * Optional referer URL handling.  Ignition allows the user to pass a path & referer URL and can construct the new path, to simplifying the resolution of links on a Gemini capsule page.
 * Basic decoding of body responses on successful (20) response from Gemini servers.
 * Trust-on-first-use certificate verification handling scheme using key signatures.
 * Fully-featured response objects for each response type.
 * Standardized & robust, human-readable error management.
@@ -122,16 +120,14 @@
 * Behavioral processing/handling of specific response types from Gemini capsules, including:
   * Generation of client certificates & automatic resubmission.
   * Automatic redirection following on 3x responses.
 * Advanced body response rendering and/or display of text/gemini mime types.
 * Command line or GUI interface.
 * Advanced session & history management.
 * Support for other protocols.
-
-⚠ These features are not currently supported but may be supported in the future:
 * Non-verified certificate scheme
 * Improved TOFU scenarios
 
 ## Advanced Usage
 More advanced request usage:
 
 ```python
@@ -200,22 +196,20 @@
 ## API Documentation
 Full API documentation for Ignition is available [here](./docs/api.md).
 
 ## Developers
 
 ![There are a few reports from the pilots.  They are simply identifying their flight plan very carefully.  Four minutes into the flight, Gordon Cooper just told Grissom that he is looking mighty good.  Gus gave him a reasuring laugh.  A very calm pilot in command of that spacecraft.](docs/img/transcript-4.png)
 
-Want to help contribute to Ignition?  See the [developer documentation](./docs/developer.md) for contribution guidelines, build processes, and testing.
-
-The developer documentation is still being completed, if you have specific questions, please open tickets within this project.
+Ignition is no longer accepting contributions.  Please feel free to fork this repository.
 
 ## License
 Ignition is licensed under [Mozilla Public License 2.0](https://www.mozilla.org/en-US/MPL/).
 
-Copyright 2020-2022 by [Chris Brousseau](https://github.com/cbrews).
+Copyright 2020-2024 by [Chris Brousseau](https://github.com/cbrews).
 
 ## Thank you
 * *solderpunk* for leading the design of the [Gemini protocol](https://geminiprotocol.net/docs/specification.html), without which this project would not have been possible.
 * *Sean Conman* for writing the [Gemini torture tests](gemini://gemini.conman.org/test/torture), which were instrumental in initial client testing.
 * *Michael Lazar* for his work on [Jetforce](https://github.com/michael-lazar/jetforce), which helped testing along the way.
 
 🔭 Happy exploring!
```

