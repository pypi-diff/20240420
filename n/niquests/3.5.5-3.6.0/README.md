# Comparing `tmp/niquests-3.5.5.tar.gz` & `tmp/niquests-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Mar 25 05:55:37 2024, max compression
+gzip compressed data, last modified: Sat Apr 20 06:44:55 2024, max compression
```

## Comparing `niquests-3.5.5.tar` & `niquests-3.6.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      718 2024-03-25 05:55:37.000000 niquests-3.5.5/AUTHORS.rst
--rw-r--r--   0        0        0    85279 2024-03-25 05:55:37.000000 niquests-3.5.5/HISTORY.md
--rw-r--r--   0        0        0      377 2024-03-25 05:55:37.000000 niquests-3.5.5/Makefile
--rw-r--r--   0        0        0       38 2024-03-25 05:55:37.000000 niquests-3.5.5/NOTICE
--rw-r--r--   0        0        0        1 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/.nojekyll
--rw-r--r--   0        0        0     7664 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/Makefile
--rw-r--r--   0        0        0     5355 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/api.rst
--rw-r--r--   0        0        0    12305 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/conf.py
--rw-r--r--   0        0        0     4084 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/index.rst
--rw-r--r--   0        0        0     7253 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/make.bat
--rw-r--r--   0        0        0      185 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/requirements.txt
--rw-r--r--   0        0        0     2990 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/_static/custom.css
--rw-r--r--   0        0        0   306086 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/_static/requests-sidebar.png
--rw-r--r--   0        0        0     7379 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/community/faq.rst
--rw-r--r--   0        0        0     2352 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/community/recommended.rst
--rw-r--r--   0        0        0     1782 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/community/release-process.rst
--rw-r--r--   0        0        0      285 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/community/support.rst
--rw-r--r--   0        0        0      324 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/community/updates.rst
--rw-r--r--   0        0        0      945 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/community/vulnerabilities.rst
--rw-r--r--   0        0        0       48 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/dev/authors.rst
--rw-r--r--   0        0        0     5768 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/dev/contributing.rst
--rw-r--r--   0        0        0     1885 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/dev/migrate.rst
--rw-r--r--   0        0        0    52827 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/user/advanced.rst
--rw-r--r--   0        0        0     6315 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/user/authentication.rst
--rw-r--r--   0        0        0     1046 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/user/install.rst
--rw-r--r--   0        0        0    34594 2024-03-25 05:55:37.000000 niquests-3.5.5/docs/user/quickstart.rst
--rw-r--r--   0        0        0     3071 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/__init__.py
--rw-r--r--   0        0        0      534 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/__version__.py
--rw-r--r--   0        0        0    47148 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/_async.py
--rw-r--r--   0        0        0     2189 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/_compat.py
--rw-r--r--   0        0        0      480 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/_constant.py
--rw-r--r--   0        0        0     5942 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/_typing.py
--rw-r--r--   0        0        0    86853 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/adapters.py
--rw-r--r--   0        0        0    27567 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/api.py
--rw-r--r--   0        0        0     9906 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/auth.py
--rw-r--r--   0        0        0    19797 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/cookies.py
--rw-r--r--   0        0        0     4363 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/exceptions.py
--rw-r--r--   0        0        0     5361 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/help.py
--rw-r--r--   0        0        0     2776 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/hooks.py
--rw-r--r--   0        0        0    62438 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/models.py
--rw-r--r--   0        0        0        0 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/py.typed
--rw-r--r--   0        0        0    68404 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/sessions.py
--rw-r--r--   0        0        0     4284 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/status_codes.py
--rw-r--r--   0        0        0     6973 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/structures.py
--rw-r--r--   0        0        0    37300 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/utils.py
--rw-r--r--   0        0        0      119 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/extensions/__init__.py
--rw-r--r--   0        0        0    21173 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/extensions/_async_ocsp.py
--rw-r--r--   0        0        0    20640 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/extensions/_ocsp.py
--rw-r--r--   0        0        0    16942 2024-03-25 05:55:37.000000 niquests-3.5.5/src/niquests/extensions/_picotls.py
--rw-r--r--   0        0        0       80 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/__init__.py
--rw-r--r--   0        0        0     2193 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/conftest.py
--rw-r--r--   0        0        0     7540 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/test_async.py
--rw-r--r--   0        0        0      875 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/test_help.py
--rw-r--r--   0        0        0      893 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/test_hooks.py
--rw-r--r--   0        0        0     4022 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/test_live.py
--rw-r--r--   0        0        0    15985 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/test_lowlevel.py
--rw-r--r--   0        0        0     3722 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/test_multiplexed.py
--rw-r--r--   0        0        0    98955 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/test_requests.py
--rw-r--r--   0        0        0     2593 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/test_structures.py
--rw-r--r--   0        0        0     6213 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/test_testserver.py
--rw-r--r--   0        0        0    26728 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/test_utils.py
--rw-r--r--   0        0        0      613 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/utils.py
--rw-r--r--   0        0        0        0 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/testserver/__init__.py
--rw-r--r--   0        0        0     3882 2024-03-25 05:55:37.000000 niquests-3.5.5/tests/testserver/server.py
--rw-r--r--   0        0        0      362 2024-03-25 05:55:37.000000 niquests-3.5.5/.gitignore
--rw-r--r--   0        0        0    10142 2024-03-25 05:55:37.000000 niquests-3.5.5/LICENSE
--rw-r--r--   0        0        0    10582 2024-03-25 05:55:37.000000 niquests-3.5.5/README.md
--rw-r--r--   0        0        0     3666 2024-03-25 05:55:37.000000 niquests-3.5.5/pyproject.toml
--rw-r--r--   0        0        0    12952 2024-03-25 05:55:37.000000 niquests-3.5.5/PKG-INFO
+-rw-r--r--   0        0        0      718 2024-04-20 06:44:55.000000 niquests-3.6.0/AUTHORS.rst
+-rw-r--r--   0        0        0    85857 2024-04-20 06:44:55.000000 niquests-3.6.0/HISTORY.md
+-rw-r--r--   0        0        0      377 2024-04-20 06:44:55.000000 niquests-3.6.0/Makefile
+-rw-r--r--   0        0        0       38 2024-04-20 06:44:55.000000 niquests-3.6.0/NOTICE
+-rw-r--r--   0        0        0        1 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/.nojekyll
+-rw-r--r--   0        0        0     7664 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/Makefile
+-rw-r--r--   0        0        0     5355 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/api.rst
+-rw-r--r--   0        0        0    12305 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/conf.py
+-rw-r--r--   0        0        0     4084 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/index.rst
+-rw-r--r--   0        0        0     7253 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/make.bat
+-rw-r--r--   0        0        0      185 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/requirements.txt
+-rw-r--r--   0        0        0     2990 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/_static/custom.css
+-rw-r--r--   0        0        0   306086 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/_static/requests-sidebar.png
+-rw-r--r--   0        0        0     7360 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/community/faq.rst
+-rw-r--r--   0        0        0     2720 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/community/recommended.rst
+-rw-r--r--   0        0        0     1782 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/community/release-process.rst
+-rw-r--r--   0        0        0      285 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/community/support.rst
+-rw-r--r--   0        0        0      324 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/community/updates.rst
+-rw-r--r--   0        0        0      945 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/community/vulnerabilities.rst
+-rw-r--r--   0        0        0       48 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/dev/authors.rst
+-rw-r--r--   0        0        0     5768 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/dev/contributing.rst
+-rw-r--r--   0        0        0     1885 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/dev/migrate.rst
+-rw-r--r--   0        0        0    52818 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/user/advanced.rst
+-rw-r--r--   0        0        0     6315 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/user/authentication.rst
+-rw-r--r--   0        0        0     1046 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/user/install.rst
+-rw-r--r--   0        0        0    34594 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/user/quickstart.rst
+-rw-r--r--   0        0        0     3071 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/__init__.py
+-rw-r--r--   0        0        0      534 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/__version__.py
+-rw-r--r--   0        0        0    47149 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/_async.py
+-rw-r--r--   0        0        0     2189 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/_compat.py
+-rw-r--r--   0        0        0      480 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/_constant.py
+-rw-r--r--   0        0        0     5942 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/_typing.py
+-rw-r--r--   0        0        0    86853 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/adapters.py
+-rw-r--r--   0        0        0    27567 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/api.py
+-rw-r--r--   0        0        0     9906 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/auth.py
+-rw-r--r--   0        0        0    19797 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/cookies.py
+-rw-r--r--   0        0        0     4363 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/exceptions.py
+-rw-r--r--   0        0        0     5119 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/help.py
+-rw-r--r--   0        0        0     2776 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/hooks.py
+-rw-r--r--   0        0        0    62438 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/models.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/py.typed
+-rw-r--r--   0        0        0    69113 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/sessions.py
+-rw-r--r--   0        0        0     4284 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/status_codes.py
+-rw-r--r--   0        0        0     6973 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/structures.py
+-rw-r--r--   0        0        0    37300 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/utils.py
+-rw-r--r--   0        0        0      119 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/extensions/__init__.py
+-rw-r--r--   0        0        0    22384 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/extensions/_async_ocsp.py
+-rw-r--r--   0        0        0    21009 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/extensions/_ocsp.py
+-rw-r--r--   0        0        0    16942 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/extensions/_picotls.py
+-rw-r--r--   0        0        0       80 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     2193 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     7540 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_async.py
+-rw-r--r--   0        0        0      875 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_help.py
+-rw-r--r--   0        0        0      893 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_hooks.py
+-rw-r--r--   0        0        0     4022 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_live.py
+-rw-r--r--   0        0        0    15985 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_lowlevel.py
+-rw-r--r--   0        0        0     3722 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_multiplexed.py
+-rw-r--r--   0        0        0    98955 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_requests.py
+-rw-r--r--   0        0        0     2593 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_structures.py
+-rw-r--r--   0        0        0     6213 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_testserver.py
+-rw-r--r--   0        0        0    26728 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_utils.py
+-rw-r--r--   0        0        0      613 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/testserver/__init__.py
+-rw-r--r--   0        0        0     3882 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/testserver/server.py
+-rw-r--r--   0        0        0      362 2024-04-20 06:44:55.000000 niquests-3.6.0/.gitignore
+-rw-r--r--   0        0        0    10142 2024-04-20 06:44:55.000000 niquests-3.6.0/LICENSE
+-rw-r--r--   0        0        0    10931 2024-04-20 06:44:55.000000 niquests-3.6.0/README.md
+-rw-r--r--   0        0        0     3660 2024-04-20 06:44:55.000000 niquests-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0    13292 2024-04-20 06:44:55.000000 niquests-3.6.0/PKG-INFO
```

### Comparing `niquests-3.5.5/AUTHORS.rst` & `niquests-3.6.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/HISTORY.md` & `niquests-3.6.0/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 Release History
 ===============
 
+3.6.0 (2024-04-20)
+------------------
+
+**Added**
+- Support for qh3 version 1.0.0
+  This qh3 release enable a greater flexibility by dropping cryptography. We had to adapt the OCSP code as we
+  relied on cryptography. HTTP/3 experience is greatly improved.
+
+**Changed**
+- urllib3.future lower bound constraint has been raised to version 2.7.904 to ensure support for the last qh3 release.
+
+**Fixed**
+- Improved compatibility with third party mocking tool that are bound to requests.
+- OCSP check did not warn if the HTTP server responded with a non 2xx response in strict mode.
+
 3.5.5 (2024-03-25)
 ------------------
 
 **Added**
 - Support for Happy Eyeballs. This feature is disabled by default, you must pass `happy_eyeballs=True` within your session
   constructor or http adapter in order to leverage this.
```

### Comparing `niquests-3.5.5/docs/Makefile` & `niquests-3.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/docs/api.rst` & `niquests-3.6.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/docs/conf.py` & `niquests-3.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/docs/index.rst` & `niquests-3.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/docs/make.bat` & `niquests-3.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/docs/_static/custom.css` & `niquests-3.6.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/docs/_static/requests-sidebar.png` & `niquests-3.6.0/docs/_static/requests-sidebar.png`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/docs/community/faq.rst` & `niquests-3.6.0/docs/community/faq.rst`

 * *Files 2% similar despite different names*

```diff
@@ -114,23 +114,23 @@
 Can we revert this behavior? Any fallback?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Yes... kind of!
 Niquests ships with a nice alternative to ``CaseInsensitiveDict`` that is ``kiss_headers.Headers``.
 You may access it through the ``oheaders`` property of your usual Response, Request and PreparedRequest.
 
-Am I obligated to install qh3 and dependents?
----------------------------------------------
+Am I obligated to install qh3?
+------------------------------
 
 No. But by default, it could be picked for installation. You may remove it safely at the cost
-of loosing HTTP/3 over QUIC.
+of loosing HTTP/3 over QUIC and OCSP certificate revocation status.
 
 A shortcut would be::
 
-    $ pip uninstall qh3 cryptography cffi pycparser
+    $ pip uninstall qh3
 
 .. warning:: Your site-packages is shared, thus it is possible that other libraries depends on some of the listed programs. Do it with care!
 
 What are "pem lib" errors?
 --------------------------
 
 Ever encountered something along::
```

### Comparing `niquests-3.5.5/docs/community/recommended.rst` & `niquests-3.6.0/docs/community/recommended.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,39 @@
 
 Recommended Packages and Extensions
 ===================================
 
 Niquests is compatible with a great variety of powerful and useful third-party extensions.
 This page provides an overview of some of the best of them.
 
-CacheControl
-------------
+Requests Cache
+--------------
 
-`CacheControl`_ is an extension that adds a full HTTP cache to Niquests. This
-makes your web requests substantially more efficient, and should be used
-whenever you're making a lot of web niquests.
+`requests-cache`_ is a persistent HTTP cache that provides an easy way to get better performance with the python requests library.
 
-.. _CacheControl: https://cachecontrol.readthedocs.io/en/latest/
+.. _requests-cache: https://github.com/requests-cache/requests-cache
+
+.. warning:: There's a catch when trying to use Niquests with `requests-cache`_. You will need a quick patch prior to using it.
+
+Do as follow::
+
+    import requests_cache
+    import niquests
+
+
+    class CacheSession(requests_cache.session.CacheMixin, niquests.Session):
+        ...
+
+
+    if __name__ == "__main__":
+
+        s = CacheSession()
+
+        for i in range(60):
+            r = s.get('https://httpbin.org/delay/1')
 
 Requests-Toolbelt
 -----------------
 
 `Requests-Toolbelt`_ is a collection of utilities that some users of Niquests may desire,
 but do not belong in Niquests proper. This library is actively maintained
 by members of the Requests core team, and reflects the functionality most
```

### Comparing `niquests-3.5.5/docs/community/release-process.rst` & `niquests-3.6.0/docs/community/release-process.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/docs/community/vulnerabilities.rst` & `niquests-3.6.0/docs/community/vulnerabilities.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/docs/dev/contributing.rst` & `niquests-3.6.0/docs/dev/contributing.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/docs/dev/migrate.rst` & `niquests-3.6.0/docs/dev/migrate.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/docs/user/advanced.rst` & `niquests-3.6.0/docs/user/advanced.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1245,15 +1245,15 @@
 e.g. Making a hundred of requests to a hundred of domains, thus consuming resources that should have been
 allocated to browser users. This was made available for users with a limited target of domains to get
 a complementary security measure.
 
 Unless in strict-mode, the proxy configuration will be respected when given, as long as it specify
 a plain ``http`` proxy. This is meant for people who want privacy.
 
-This feature may not be available if the ``cryptography`` package is missing from your environment.
+This feature may not be available if the ``qh3`` package is missing from your environment.
 Verify the availability by running ``python -m niquests.help``.
 
 .. note:: Access property ``ocsp_verified`` in both ``PreparedRequest``, and ``Response`` to have information about this post handshake verification.
 
 Specify HTTP/3 capable endpoint preemptively
 --------------------------------------------
```

### Comparing `niquests-3.5.5/docs/user/authentication.rst` & `niquests-3.6.0/docs/user/authentication.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/docs/user/install.rst` & `niquests-3.6.0/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/docs/user/quickstart.rst` & `niquests-3.6.0/docs/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/__init__.py` & `niquests-3.6.0/src/niquests/__init__.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/__version__.py` & `niquests-3.6.0/src/niquests/__version__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 __title__: str = "niquests"
 __description__: str = "Python HTTP for Humans."
 __url__: str = "https://niquests.readthedocs.io"
 
 __version__: str
-__version__ = "3.5.5"
+__version__ = "3.6.0"
 
-__build__: int = 0x030505
+__build__: int = 0x030600
 __author__: str = "Kenneth Reitz"
 __author_email__: str = "me@kennethreitz.org"
 __license__: str = "Apache-2.0"
 __copyright__: str = "Copyright Kenneth Reitz"
 __cake__: str = "\u2728 \U0001f370 \u2728"
```

### Comparing `niquests-3.5.5/src/niquests/_async.py` & `niquests-3.6.0/src/niquests/_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,15 +420,15 @@
         r = await adapter.send(request, **kwargs)
 
         # Make sure the timings data are kept as is, conn_info is a reference to
         # urllib3-future conn_info.
         request.conn_info = _deepcopy_ci(request.conn_info)
 
         # We are leveraging a multiplexed connection
-        if r.raw is None:
+        if r.lazy is True:
 
             async def _redirect_method_ref(x, y):
                 try:
                     return await self.resolve_redirects(
                         x, y, yield_requests=True, **kwargs
                     ).__anext__()
                 except StopAsyncIteration:
```

### Comparing `niquests-3.5.5/src/niquests/_compat.py` & `niquests-3.6.0/src/niquests/_compat.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/_typing.py` & `niquests-3.6.0/src/niquests/_typing.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/adapters.py` & `niquests-3.6.0/src/niquests/adapters.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/api.py` & `niquests-3.6.0/src/niquests/api.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/auth.py` & `niquests-3.6.0/src/niquests/auth.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/cookies.py` & `niquests-3.6.0/src/niquests/cookies.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/exceptions.py` & `niquests-3.6.0/src/niquests/exceptions.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/help.py` & `niquests-3.6.0/src/niquests/help.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,19 +35,14 @@
 
 try:
     import certifi  # type: ignore
 except ImportError:
     certifi = None  # type: ignore
 
 try:
-    import cryptography  # type: ignore
-except ImportError:
-    cryptography = None  # type: ignore
-
-try:
     from .extensions._ocsp import verify as ocsp_verify
 except ImportError:
     ocsp_verify = None  # type: ignore
 
 
 def _implementation():
     """Return a dict with the Python implementation and version.
@@ -101,17 +96,14 @@
     urllib3_info = {
         "version": urllib3.__version__,
         "cohabitation_version": __legacy_urllib3_version__,
     }
 
     charset_normalizer_info = {"version": charset_normalizer.__version__}
 
-    cryptography_info = {
-        "version": getattr(cryptography, "__version__", ""),
-    }
     idna_info = {
         "version": getattr(idna, "__version__", ""),
     }
 
     system_ssl = ssl.OPENSSL_VERSION_NUMBER
     system_ssl_info = {
         "version": f"{system_ssl:x}" if system_ssl is not None else "N/A"
@@ -119,15 +111,14 @@
 
     return {
         "platform": platform_info,
         "implementation": implementation_info,
         "system_ssl": system_ssl_info,
         "urllib3.future": urllib3_info,
         "charset_normalizer": charset_normalizer_info,
-        "cryptography": cryptography_info,
         "idna": idna_info,
         "niquests": {
             "version": niquests_version,
         },
         "http3": {
             "enabled": qh3 is not None,
             "qh3": qh3.__version__ if qh3 is not None else None,
```

### Comparing `niquests-3.5.5/src/niquests/hooks.py` & `niquests-3.6.0/src/niquests/hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/models.py` & `niquests-3.6.0/src/niquests/models.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/sessions.py` & `niquests-3.6.0/src/niquests/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1165,22 +1165,34 @@
 
         # Get the appropriate adapter to use
         adapter = self.get_adapter(url=request.url)
 
         # Start time (approximately) of the request
         start = preferred_clock()
 
-        # Send the request
-        r = adapter.send(request, **kwargs)
+        try:
+            # Send the request
+            r = adapter.send(request, **kwargs)
+        except TypeError:
+            # this is required because some people may do an incomplete migration.
+            # this will hint them appropriately.
+            raise TypeError(
+                "You probably tried to add a Requests adapter into a Niquests session. "
+                "Make sure you replaced the 'import requests.adapters' into 'import niquests.adapters' "
+                "and made required adjustment. If you did this to increase pool_maxsize, know that the "
+                "Session constructor support kwargs for it. "
+                "See https://niquests.readthedocs.io/en/latest/user/quickstart.html#scale-your-session-pool to learn more."
+            )
+
         # Make sure the timings data are kept as is, conn_info is a reference to
         # urllib3-future conn_info.
         request.conn_info = _deepcopy_ci(request.conn_info)
 
         # We are leveraging a multiplexed connection
-        if r.raw is None:
+        if r.lazy is True:
             r._resolve_redirect = lambda x, y: next(
                 self.resolve_redirects(x, y, yield_requests=True, **kwargs),  # type: ignore
                 None,
             )
 
             # in multiplexed mode, we are unable to forward this local function for safety reasons.
             kwargs["on_post_connection"] = None
```

### Comparing `niquests-3.5.5/src/niquests/status_codes.py` & `niquests-3.6.0/src/niquests/status_codes.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/structures.py` & `niquests-3.6.0/src/niquests/structures.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/utils.py` & `niquests-3.6.0/src/niquests/utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/src/niquests/extensions/_async_ocsp.py` & `niquests-3.6.0/src/niquests/extensions/_async_ocsp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 import asyncio
 import datetime
 import hmac
 import socket
+import ssl
 import typing
 import warnings
 from contextlib import asynccontextmanager
 from hashlib import sha256
 from random import randint
 from statistics import mean
 
-from cryptography.hazmat.primitives import serialization
-from cryptography.hazmat.primitives.hashes import SHA1
-from cryptography.x509 import (
+from qh3._hazmat import (
+    OCSPRequest,
+    OCSPResponse,
+    OCSPResponseStatus,
+    OCSPCertStatus,
     Certificate,
-    load_der_x509_certificate,
-    load_pem_x509_certificate,
-    ocsp,
 )
 
 from .._compat import HAS_LEGACY_URLLIB3
 
 if HAS_LEGACY_URLLIB3 is False:
     from urllib3 import ConnectionInfo
     from urllib3.exceptions import SecurityWarning
@@ -49,15 +49,15 @@
     handle_server_hello,
     multiply_num_on_ec_point,
     num_to_bytes,
     async_recv_tls,
     async_recv_tls_and_decrypt,
     async_send_tls,
 )
-from ._ocsp import _str_fingerprint_of, _infer_issuer_from
+from ._ocsp import _str_fingerprint_of, readable_revocation_reason
 
 
 async def _ask_nicely_for_issuer(
     hostname: str, dst_address: tuple[str, int], timeout: int | float = 0.2
 ) -> Certificate | None:
     """When encountering a problem in development, one should always say that there is many solutions.
     From dirtiest to the cleanest, not always known but with progressive effort, we'll eventually land at the cleanest.
@@ -161,38 +161,42 @@
 
     server_seq_num += 1
 
     der_certificates = handle_server_cert(server_cert)
     certificates = []
 
     for der in der_certificates:
-        certificates.append(load_der_x509_certificate(der))
+        certificates.append(Certificate(der))
 
     await async_send_tls(sock, ALERT, b"\x01\x00")
     sock.close()
 
     if len(certificates) <= 1:
         return None
 
     # kept in order, the immediate issuer come just after the leaf one.
     return certificates[1]
 
 
 class InMemoryRevocationStatus:
     def __init__(self, max_size: int = 2048):
         self._max_size: int = max_size
-        self._store: dict[str, ocsp.OCSPResponse] = {}
+        self._store: dict[str, OCSPResponse] = {}
         self._semaphores: dict[str, asyncio.Semaphore] = {}
-        self._issuers: list[Certificate] = []
+        self._issuers_map: dict[str, Certificate] = {}
         self._timings: list[datetime.datetime] = []
         self.hold: bool = False
 
-    @property
-    def issuers(self) -> list[Certificate]:
-        return self._issuers
+    def get_issuer_of(self, peer_certificate: Certificate) -> Certificate | None:
+        fingerprint: str = _str_fingerprint_of(peer_certificate)
+
+        if fingerprint not in self._issuers_map:
+            return None
+
+        return self._issuers_map[fingerprint]
 
     def __len__(self) -> int:
         return len(self._store)
 
     @asynccontextmanager
     async def lock(
         self, peer_certificate: Certificate
@@ -218,72 +222,69 @@
                 previous_dt = dt
                 continue
             delays.append((dt - previous_dt).total_seconds())
             previous_dt = dt
 
         return mean(delays) if delays else 0.0
 
-    def check(self, peer_certificate: Certificate) -> ocsp.OCSPResponse | None:
+    def check(self, peer_certificate: Certificate) -> OCSPResponse | None:
         fingerprint: str = _str_fingerprint_of(peer_certificate)
 
         if fingerprint not in self._store:
             return None
 
         cached_response = self._store[fingerprint]
 
-        if cached_response.certificate_status == ocsp.OCSPCertStatus.GOOD:
+        if cached_response.certificate_status == OCSPCertStatus.GOOD:
             if (
                 cached_response.next_update
-                and datetime.datetime.now().timestamp()
-                >= cached_response.next_update.timestamp()
+                and datetime.datetime.now().timestamp() >= cached_response.next_update
             ):
                 del self._store[fingerprint]
                 return None
             return cached_response
 
         return cached_response
 
     def save(
         self,
         peer_certificate: Certificate,
         issuer_certificate: Certificate,
-        ocsp_response: ocsp.OCSPResponse,
+        ocsp_response: OCSPResponse,
     ) -> None:
         if len(self._store) >= self._max_size:
             tbd_key: str | None = None
-            closest_next_update: datetime.datetime | None = None
+            closest_next_update: int | None = None
 
             for k in self._store:
-                if self._store[k].response_status != ocsp.OCSPResponseStatus.SUCCESSFUL:
+                if self._store[k].response_status != OCSPResponseStatus.SUCCESSFUL:
                     tbd_key = k
                     break
 
-                if self._store[k].certificate_status != ocsp.OCSPCertStatus.REVOKED:
+                if self._store[k].certificate_status != OCSPCertStatus.REVOKED:
                     if closest_next_update is None:
                         closest_next_update = self._store[k].next_update
                         tbd_key = k
                         continue
                     if self._store[k].next_update > closest_next_update:  # type: ignore
                         closest_next_update = self._store[k].next_update
                         tbd_key = k
 
             if tbd_key:
                 del self._store[tbd_key]
+                del self._issuers_map[tbd_key]
             else:
-                del self._store[list(self._store.keys())[0]]
-
-        self._store[_str_fingerprint_of(peer_certificate)] = ocsp_response
+                first_key = list(self._store.keys())[0]
+                del self._store[first_key]
+                del self._issuers_map[first_key]
 
-        issuer_fingerprint = _str_fingerprint_of(issuer_certificate)
+        peer_fingerprint: str = _str_fingerprint_of(peer_certificate)
 
-        if not any(_str_fingerprint_of(c) == issuer_fingerprint for c in self._issuers):
-            self._issuers.append(issuer_certificate)
-
-        if len(self._issuers) >= self._max_size:
-            self._issuers.pop(0)
+        self._store[peer_fingerprint] = ocsp_response
+        self._issuers_map[peer_fingerprint] = issuer_certificate
 
         self._timings.append(datetime.datetime.now())
 
         if len(self._timings) >= self._max_size:
             self._timings.pop(0)
 
 
@@ -304,15 +305,15 @@
     if (
         conn_info is None
         or conn_info.certificate_der is None
         or conn_info.certificate_dict is None
     ):
         return
 
-    peer_certificate = load_der_x509_certificate(conn_info.certificate_der)
+    peer_certificate = Certificate(conn_info.certificate_der)
 
     async with _SharedRevocationStatusCache.lock(peer_certificate):
         endpoints: list[str] = [  # type: ignore
             # exclude non-HTTP endpoint. like ldap.
             ep  # type: ignore
             for ep in list(conn_info.certificate_dict.get("OCSP", []))  # type: ignore
             if ep.startswith("http://")  # type: ignore
@@ -332,31 +333,31 @@
 
             if _SharedRevocationStatusCache.hold:
                 return
 
         cached_response = _SharedRevocationStatusCache.check(peer_certificate)
 
         if cached_response is not None:
-            issuer_certificate = _infer_issuer_from(peer_certificate)
+            issuer_certificate = _SharedRevocationStatusCache.get_issuer_of(
+                peer_certificate
+            )
 
             if issuer_certificate:
-                conn_info.issuer_certificate_der = issuer_certificate.public_bytes(
-                    serialization.Encoding.DER
-                )
+                conn_info.issuer_certificate_der = issuer_certificate.public_bytes()
 
-            if cached_response.response_status == ocsp.OCSPResponseStatus.SUCCESSFUL:
-                if cached_response.certificate_status == ocsp.OCSPCertStatus.REVOKED:
+            if cached_response.response_status == OCSPResponseStatus.SUCCESSFUL:
+                if cached_response.certificate_status == OCSPCertStatus.REVOKED:
                     r.ocsp_verified = False
                     raise SSLError(
                         f"""Unable to establish a secure connection to {r.url} because the certificate has been revoked
-                        by issuer ({cached_response.revocation_reason or "unspecified"}).
+                        by issuer ({readable_revocation_reason(cached_response.revocation_reason) or "unspecified"}).
                         You should avoid trying to request anything from it as the remote has been compromised.
                         See https://en.wikipedia.org/wiki/OCSP_stapling for more information."""
                     )
-                elif cached_response.certificate_status == ocsp.OCSPCertStatus.UNKNOWN:
+                elif cached_response.certificate_status == OCSPCertStatus.UNKNOWN:
                     r.ocsp_verified = False
                     if strict is True:
                         raise SSLError(
                             f"""Unable to establish a secure connection to {r.url} because the issuer does not know whether
                             certificate is valid or not. This error occurred because you enabled strict mode for
                             the OCSP / Revocation check."""
                         )
@@ -377,15 +378,17 @@
             # Unfortunately! But no worries, we can circumvent it! (Python 3.10+ is not concerned anymore)
             # Three ways are valid to fetch it (in order of preference, safest to riskiest):
             #   - The issuer can be (but unlikely) a root CA.
             #   - Retrieve it by asking it from the TLS layer.
             #   - Downloading it using specified caIssuers from the peer certificate.
             if conn_info.issuer_certificate_der is None:
                 # It could be a root (self-signed) certificate. Or a previously seen issuer.
-                issuer_certificate = _infer_issuer_from(peer_certificate)
+                issuer_certificate = _SharedRevocationStatusCache.get_issuer_of(
+                    peer_certificate
+                )
 
                 # If not, try to ask nicely the remote to give us the certificate chain, and extract
                 # from it the immediate issuer.
                 if issuer_certificate is None:
                     try:
                         if r.url is None:
                             raise ValueError
@@ -403,19 +406,14 @@
                                 url_parsed.hostname,
                                 conn_info.destination_address,
                                 timeout,
                             )
                         else:
                             issuer_certificate = None
 
-                        if issuer_certificate is not None:
-                            peer_certificate.verify_directly_issued_by(
-                                issuer_certificate
-                            )
-
                     except (
                         socket.gaierror,
                         TimeoutError,
                         ConnectionError,
                         AttributeError,
                     ):
                         pass
@@ -444,56 +442,61 @@
 
                             if raw_intermediary_content is not None:
                                 # binary DER
                                 if (
                                     b"-----BEGIN CERTIFICATE-----"
                                     not in raw_intermediary_content
                                 ):
-                                    issuer_certificate = load_der_x509_certificate(
+                                    issuer_certificate = Certificate(
                                         raw_intermediary_content
                                     )
                                 # b64 PEM
                                 elif (
                                     b"-----BEGIN CERTIFICATE-----"
                                     in raw_intermediary_content
                                 ):
-                                    issuer_certificate = load_pem_x509_certificate(
-                                        raw_intermediary_content
+                                    issuer_certificate = Certificate(
+                                        ssl.PEM_cert_to_DER_cert(
+                                            raw_intermediary_content.decode()
+                                        )
                                     )
 
                 # Well! We're out of luck. No further should we go.
                 if issuer_certificate is None:
                     if strict:
                         warnings.warn(
                             f"""Unable to insure that the remote peer ({r.url}) has a currently valid certificate via OCSP.
                             You are seeing this warning due to enabling strict mode for OCSP / Revocation check.
                             Reason: Remote did not provide any intermediaries certificate.""",
                             SecurityWarning,
                         )
                     return
 
-                conn_info.issuer_certificate_der = issuer_certificate.public_bytes(
-                    serialization.Encoding.DER
-                )
+                conn_info.issuer_certificate_der = issuer_certificate.public_bytes()
             else:
-                issuer_certificate = load_der_x509_certificate(
-                    conn_info.issuer_certificate_der
-                )
-
-            builder = ocsp.OCSPRequestBuilder()
-            builder = builder.add_certificate(
-                peer_certificate, issuer_certificate, SHA1()
-            )
+                issuer_certificate = Certificate(conn_info.issuer_certificate_der)
 
-            req = builder.build()
+            try:
+                req = OCSPRequest(
+                    peer_certificate.public_bytes(), issuer_certificate.public_bytes()
+                )
+            except ValueError:
+                if strict:
+                    warnings.warn(
+                        f"""Unable to insure that the remote peer ({r.url}) has a currently valid certificate via OCSP.
+                        You are seeing this warning due to enabling strict mode for OCSP / Revocation check.
+                        Reason: The X509 OCSP generator failed to assemble the request""",
+                        SecurityWarning,
+                    )
+                return
 
             try:
                 ocsp_http_response = await session.post(
                     endpoints[randint(0, len(endpoints) - 1)],
-                    data=req.public_bytes(serialization.Encoding.DER),
+                    data=req.public_bytes(),
                     headers={"Content-Type": "application/ocsp-request"},
                     timeout=timeout,
                 )
             except RequestException as e:
                 if strict:
                     warnings.warn(
                         f"""Unable to insure that the remote peer ({r.url}) has a currently valid certificate via OCSP.
@@ -506,30 +509,40 @@
             if (
                 ocsp_http_response.status_code
                 and 300 > ocsp_http_response.status_code >= 200
             ):
                 if ocsp_http_response.content is None:
                     return
 
-                ocsp_resp = ocsp.load_der_ocsp_response(ocsp_http_response.content)
+                try:
+                    ocsp_resp = OCSPResponse(ocsp_http_response.content)
+                except ValueError:
+                    if strict:
+                        warnings.warn(
+                            f"""Unable to insure that the remote peer ({r.url}) has a currently valid certificate via OCSP.
+                            You are seeing this warning due to enabling strict mode for OCSP / Revocation check.
+                            Reason: The X509 OCSP parser failed to read the response""",
+                            SecurityWarning,
+                        )
+                    return
 
                 _SharedRevocationStatusCache.save(
                     peer_certificate, issuer_certificate, ocsp_resp
                 )
 
-                if ocsp_resp.response_status == ocsp.OCSPResponseStatus.SUCCESSFUL:
-                    if ocsp_resp.certificate_status == ocsp.OCSPCertStatus.REVOKED:
+                if ocsp_resp.response_status == OCSPResponseStatus.SUCCESSFUL:
+                    if ocsp_resp.certificate_status == OCSPCertStatus.REVOKED:
                         r.ocsp_verified = False
                         raise SSLError(
                             f"""Unable to establish a secure connection to {r.url} because the certificate has been revoked
-                            by issuer ({ocsp_resp.revocation_reason or "unspecified"}).
+                            by issuer ({readable_revocation_reason(ocsp_resp.revocation_reason) or "unspecified"}).
                             You should avoid trying to request anything from it as the remote has been compromised.
                             See https://en.wikipedia.org/wiki/OCSP_stapling for more information."""
                         )
-                    if ocsp_resp.certificate_status == ocsp.OCSPCertStatus.UNKNOWN:
+                    if ocsp_resp.certificate_status == OCSPCertStatus.UNKNOWN:
                         r.ocsp_verified = False
                         if strict is True:
                             raise SSLError(
                                 f"""Unable to establish a secure connection to {r.url} because the issuer does not know whether
                                 certificate is valid or not. This error occurred because you enabled strict mode for
                                 the OCSP / Revocation check."""
                             )
@@ -539,10 +552,18 @@
                     if strict:
                         warnings.warn(
                             f"""Unable to insure that the remote peer ({r.url}) has a currently valid certificate via OCSP.
                             You are seeing this warning due to enabling strict mode for OCSP / Revocation check.
                             OCSP Server Status: {ocsp_resp.response_status}""",
                             SecurityWarning,
                         )
+            else:
+                if strict:
+                    warnings.warn(
+                        f"""Unable to insure that the remote peer ({r.url}) has a currently valid certificate via OCSP.
+                            You are seeing this warning due to enabling strict mode for OCSP / Revocation check.
+                            OCSP Server Status: {str(ocsp_http_response)}""",
+                        SecurityWarning,
+                    )
 
 
 __all__ = ("verify",)
```

### Comparing `niquests-3.5.5/src/niquests/extensions/_ocsp.py` & `niquests-3.6.0/src/niquests/extensions/_ocsp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import datetime
 import hmac
 import socket
+import ssl
 import threading
 import warnings
 from hashlib import sha256
 from random import randint
 from statistics import mean
 
-import wassima
-from cryptography.hazmat.primitives import serialization
-from cryptography.hazmat.primitives.hashes import SHA1
-from cryptography.x509 import (
+from qh3._hazmat import (
+    OCSPRequest,
+    OCSPResponse,
+    OCSPResponseStatus,
+    OCSPCertStatus,
     Certificate,
-    load_der_x509_certificate,
-    load_pem_x509_certificate,
-    ocsp,
+    ReasonFlags,
 )
 
 from .._compat import HAS_LEGACY_URLLIB3
 
 if HAS_LEGACY_URLLIB3 is False:
     from urllib3 import ConnectionInfo
     from urllib3.exceptions import SecurityWarning
@@ -49,46 +49,21 @@
     recv_tls,
     recv_tls_and_decrypt,
     send_tls,
 )
 
 
 def _str_fingerprint_of(certificate: Certificate) -> str:
-    return ":".join([format(i, "02x") for i in certificate.fingerprint(SHA1())])
+    return ":".join(
+        [format(i, "02x") for i in sha256(certificate.public_bytes()).digest()]
+    )
 
 
-def _infer_issuer_from(certificate: Certificate) -> Certificate | None:
-    issuer: Certificate | None = None
-
-    for der_cert in (
-        wassima.root_der_certificates() + _SharedRevocationStatusCache.issuers
-    ):
-        if isinstance(der_cert, Certificate):
-            possible_issuer = der_cert
-        else:
-            try:
-                possible_issuer = load_der_x509_certificate(der_cert)
-            except (
-                ValueError
-            ):  # Defensive: mitigation against future Cryptography evolutions
-                continue
-
-        # detect cryptography old build
-        if not hasattr(certificate, "verify_directly_issued_by"):
-            break
-
-        try:
-            certificate.verify_directly_issued_by(possible_issuer)
-        except ValueError:
-            continue
-        else:
-            issuer = possible_issuer
-            break
-
-    return issuer
+def readable_revocation_reason(flag: ReasonFlags | None) -> str | None:
+    return flag.name.lower() if flag is not None else None
 
 
 def _ask_nicely_for_issuer(
     hostname: str, dst_address: tuple[str, int], timeout: int | float = 0.2
 ) -> Certificate | None:
     """When encountering a problem in development, one should always say that there is many solutions.
     From dirtiest to the cleanest, not always known but with progressive effort, we'll eventually land at the cleanest.
@@ -192,39 +167,43 @@
 
     server_seq_num += 1
 
     der_certificates = handle_server_cert(server_cert)
     certificates = []
 
     for der in der_certificates:
-        certificates.append(load_der_x509_certificate(der))
+        certificates.append(Certificate(der))
 
     send_tls(sock, ALERT, b"\x01\x00")
     sock.close()
 
     if len(certificates) <= 1:
         return None
 
     # kept in order, the immediate issuer come just after the leaf one.
     return certificates[1]
 
 
 class InMemoryRevocationStatus:
     def __init__(self, max_size: int = 2048):
         self._max_size: int = max_size
-        self._store: dict[str, ocsp.OCSPResponse] = {}
-        self._issuers: list[Certificate] = []
+        self._store: dict[str, OCSPResponse] = {}
+        self._issuers_map: dict[str, Certificate] = {}
         self._timings: list[datetime.datetime] = []
         self._access_lock = threading.RLock()
         self.hold: bool = False
 
-    @property
-    def issuers(self) -> list[Certificate]:
+    def get_issuer_of(self, peer_certificate: Certificate) -> Certificate | None:
         with self._access_lock:
-            return self._issuers
+            fingerprint: str = _str_fingerprint_of(peer_certificate)
+
+            if fingerprint not in self._issuers_map:
+                return None
+
+            return self._issuers_map[fingerprint]
 
     def __len__(self) -> int:
         with self._access_lock:
             return len(self._store)
 
     def rate(self):
         with self._access_lock:
@@ -236,79 +215,72 @@
                     previous_dt = dt
                     continue
                 delays.append((dt - previous_dt).total_seconds())
                 previous_dt = dt
 
             return mean(delays) if delays else 0.0
 
-    def check(self, peer_certificate: Certificate) -> ocsp.OCSPResponse | None:
+    def check(self, peer_certificate: Certificate) -> OCSPResponse | None:
         with self._access_lock:
             fingerprint: str = _str_fingerprint_of(peer_certificate)
 
             if fingerprint not in self._store:
                 return None
 
             cached_response = self._store[fingerprint]
 
-            if cached_response.certificate_status == ocsp.OCSPCertStatus.GOOD:
+            if cached_response.certificate_status == OCSPCertStatus.GOOD:
                 if (
                     cached_response.next_update
                     and datetime.datetime.now().timestamp()
-                    >= cached_response.next_update.timestamp()
+                    >= cached_response.next_update
                 ):
                     del self._store[fingerprint]
                     return None
                 return cached_response
 
             return cached_response
 
     def save(
         self,
         peer_certificate: Certificate,
         issuer_certificate: Certificate,
-        ocsp_response: ocsp.OCSPResponse,
+        ocsp_response: OCSPResponse,
     ) -> None:
         with self._access_lock:
             if len(self._store) >= self._max_size:
                 tbd_key: str | None = None
-                closest_next_update: datetime.datetime | None = None
+                closest_next_update: int | None = None
 
                 for k in self._store:
-                    if (
-                        self._store[k].response_status
-                        != ocsp.OCSPResponseStatus.SUCCESSFUL
-                    ):
+                    if self._store[k].response_status != OCSPResponseStatus.SUCCESSFUL:
                         tbd_key = k
                         break
 
-                    if self._store[k].certificate_status != ocsp.OCSPCertStatus.REVOKED:
+                    if self._store[k].certificate_status != OCSPCertStatus.REVOKED:
                         if closest_next_update is None:
                             closest_next_update = self._store[k].next_update
                             tbd_key = k
                             continue
                         if self._store[k].next_update > closest_next_update:  # type: ignore
                             closest_next_update = self._store[k].next_update
                             tbd_key = k
 
                 if tbd_key:
                     del self._store[tbd_key]
+                    del self._issuers_map[tbd_key]
                 else:
-                    del self._store[list(self._store.keys())[0]]
-
-            self._store[_str_fingerprint_of(peer_certificate)] = ocsp_response
+                    first_key = list(self._store.keys())[0]
+                    del self._store[first_key]
+                    del self._issuers_map[first_key]
 
-            issuer_fingerprint = _str_fingerprint_of(issuer_certificate)
+            peer_fingerprint: str = _str_fingerprint_of(peer_certificate)
 
-            if not any(
-                _str_fingerprint_of(c) == issuer_fingerprint for c in self._issuers
-            ):
-                self._issuers.append(issuer_certificate)
-
-            if len(self._issuers) >= self._max_size:
-                self._issuers.pop(0)
+            self._store[peer_fingerprint] = ocsp_response
+            self._issuers_map[peer_fingerprint] = issuer_certificate
 
             self._timings.append(datetime.datetime.now())
 
             if len(self._timings) >= self._max_size:
                 self._timings.pop(0)
 
 
@@ -351,35 +323,35 @@
 
         if cache_count >= 10 and mean_rate_sec <= 1.0:
             _SharedRevocationStatusCache.hold = True
 
         if _SharedRevocationStatusCache.hold:
             return
 
-    peer_certificate = load_der_x509_certificate(conn_info.certificate_der)
+    peer_certificate = Certificate(conn_info.certificate_der)
     cached_response = _SharedRevocationStatusCache.check(peer_certificate)
 
     if cached_response is not None:
-        issuer_certificate = _infer_issuer_from(peer_certificate)
+        issuer_certificate = _SharedRevocationStatusCache.get_issuer_of(
+            peer_certificate
+        )
 
         if issuer_certificate:
-            conn_info.issuer_certificate_der = issuer_certificate.public_bytes(
-                serialization.Encoding.DER
-            )
+            conn_info.issuer_certificate_der = issuer_certificate.public_bytes()
 
-        if cached_response.response_status == ocsp.OCSPResponseStatus.SUCCESSFUL:
-            if cached_response.certificate_status == ocsp.OCSPCertStatus.REVOKED:
+        if cached_response.response_status == OCSPResponseStatus.SUCCESSFUL:
+            if cached_response.certificate_status == OCSPCertStatus.REVOKED:
                 r.ocsp_verified = False
                 raise SSLError(
                     f"""Unable to establish a secure connection to {r.url} because the certificate has been revoked
-                    by issuer ({cached_response.revocation_reason or "unspecified"}).
+                    by issuer ({readable_revocation_reason(cached_response.revocation_reason) or "unspecified"}).
                     You should avoid trying to request anything from it as the remote has been compromised.
                     See https://en.wikipedia.org/wiki/OCSP_stapling for more information."""
                 )
-            elif cached_response.certificate_status == ocsp.OCSPCertStatus.UNKNOWN:
+            elif cached_response.certificate_status == OCSPCertStatus.UNKNOWN:
                 r.ocsp_verified = False
                 if strict is True:
                     raise SSLError(
                         f"""Unable to establish a secure connection to {r.url} because the issuer does not know whether
                         certificate is valid or not. This error occurred because you enabled strict mode for
                         the OCSP / Revocation check."""
                     )
@@ -398,15 +370,17 @@
         # Unfortunately! But no worries, we can circumvent it!
         # Three ways are valid to fetch it (in order of preference, safest to riskiest):
         #   - The issuer can be (but unlikely) a root CA.
         #   - Retrieve it by asking it from the TLS layer.
         #   - Downloading it using specified caIssuers from the peer certificate.
         if conn_info.issuer_certificate_der is None:
             # It could be a root (self-signed) certificate. Or a previously seen issuer.
-            issuer_certificate = _infer_issuer_from(peer_certificate)
+            issuer_certificate = _SharedRevocationStatusCache.get_issuer_of(
+                peer_certificate
+            )
 
             # If not, try to ask nicely the remote to give us the certificate chain, and extract
             # from it the immediate issuer.
             if issuer_certificate is None:
                 try:
                     if r.url is None:
                         raise ValueError
@@ -424,17 +398,14 @@
                             url_parsed.hostname,
                             conn_info.destination_address,
                             timeout,
                         )
                     else:
                         issuer_certificate = None
 
-                    if issuer_certificate is not None:
-                        peer_certificate.verify_directly_issued_by(issuer_certificate)
-
                 except (socket.gaierror, TimeoutError, ConnectionError, AttributeError):
                     pass
                 except ValueError:
                     issuer_certificate = None
 
             hint_ca_issuers: list[str] = [
                 ep  # type: ignore
@@ -456,54 +427,61 @@
 
                         if raw_intermediary_content is not None:
                             # binary DER
                             if (
                                 b"-----BEGIN CERTIFICATE-----"
                                 not in raw_intermediary_content
                             ):
-                                issuer_certificate = load_der_x509_certificate(
+                                issuer_certificate = Certificate(
                                     raw_intermediary_content
                                 )
                             # b64 PEM
                             elif (
                                 b"-----BEGIN CERTIFICATE-----"
                                 in raw_intermediary_content
                             ):
-                                issuer_certificate = load_pem_x509_certificate(
-                                    raw_intermediary_content
+                                issuer_certificate = Certificate(
+                                    ssl.PEM_cert_to_DER_cert(
+                                        raw_intermediary_content.decode()
+                                    )
                                 )
 
             # Well! We're out of luck. No further should we go.
             if issuer_certificate is None:
                 if strict:
                     warnings.warn(
                         f"""Unable to insure that the remote peer ({r.url}) has a currently valid certificate via OCSP.
                         You are seeing this warning due to enabling strict mode for OCSP / Revocation check.
                         Reason: Remote did not provide any intermediaries certificate.""",
                         SecurityWarning,
                     )
                 return
 
-            conn_info.issuer_certificate_der = issuer_certificate.public_bytes(
-                serialization.Encoding.DER
-            )
+            conn_info.issuer_certificate_der = issuer_certificate.public_bytes()
         else:
-            issuer_certificate = load_der_x509_certificate(
-                conn_info.issuer_certificate_der
-            )
-
-        builder = ocsp.OCSPRequestBuilder()
-        builder = builder.add_certificate(peer_certificate, issuer_certificate, SHA1())
+            issuer_certificate = Certificate(conn_info.issuer_certificate_der)
 
-        req = builder.build()
+        try:
+            req = OCSPRequest(
+                peer_certificate.public_bytes(), issuer_certificate.public_bytes()
+            )
+        except ValueError:
+            if strict:
+                warnings.warn(
+                    f"""Unable to insure that the remote peer ({r.url}) has a currently valid certificate via OCSP.
+                    You are seeing this warning due to enabling strict mode for OCSP / Revocation check.
+                    Reason: The X509 OCSP generator failed to assemble the request""",
+                    SecurityWarning,
+                )
+            return
 
         try:
             ocsp_http_response = session.post(
                 endpoints[randint(0, len(endpoints) - 1)],
-                data=req.public_bytes(serialization.Encoding.DER),
+                data=req.public_bytes(),
                 headers={"Content-Type": "application/ocsp-request"},
                 timeout=timeout,
             )
         except RequestException as e:
             if strict:
                 warnings.warn(
                     f"""Unable to insure that the remote peer ({r.url}) has a currently valid certificate via OCSP.
@@ -516,30 +494,40 @@
         if (
             ocsp_http_response.status_code
             and 300 > ocsp_http_response.status_code >= 200
         ):
             if ocsp_http_response.content is None:
                 return
 
-            ocsp_resp = ocsp.load_der_ocsp_response(ocsp_http_response.content)
+            try:
+                ocsp_resp = OCSPResponse(ocsp_http_response.content)
+            except ValueError:
+                if strict:
+                    warnings.warn(
+                        f"""Unable to insure that the remote peer ({r.url}) has a currently valid certificate via OCSP.
+                        You are seeing this warning due to enabling strict mode for OCSP / Revocation check.
+                        Reason: The X509 OCSP parser failed to read the response""",
+                        SecurityWarning,
+                    )
+                return
 
             _SharedRevocationStatusCache.save(
                 peer_certificate, issuer_certificate, ocsp_resp
             )
 
-            if ocsp_resp.response_status == ocsp.OCSPResponseStatus.SUCCESSFUL:
-                if ocsp_resp.certificate_status == ocsp.OCSPCertStatus.REVOKED:
+            if ocsp_resp.response_status == OCSPResponseStatus.SUCCESSFUL:
+                if ocsp_resp.certificate_status == OCSPCertStatus.REVOKED:
                     r.ocsp_verified = False
                     raise SSLError(
                         f"""Unable to establish a secure connection to {r.url} because the certificate has been revoked
-                        by issuer ({ocsp_resp.revocation_reason or "unspecified"}).
+                        by issuer ({readable_revocation_reason(ocsp_resp.revocation_reason) or "unspecified"}).
                         You should avoid trying to request anything from it as the remote has been compromised.
                         See https://en.wikipedia.org/wiki/OCSP_stapling for more information."""
                     )
-                if ocsp_resp.certificate_status == ocsp.OCSPCertStatus.UNKNOWN:
+                if ocsp_resp.certificate_status == OCSPCertStatus.UNKNOWN:
                     r.ocsp_verified = False
                     if strict is True:
                         raise SSLError(
                             f"""Unable to establish a secure connection to {r.url} because the issuer does not know whether
                             certificate is valid or not. This error occurred because you enabled strict mode for
                             the OCSP / Revocation check."""
                         )
@@ -549,10 +537,18 @@
                 if strict:
                     warnings.warn(
                         f"""Unable to insure that the remote peer ({r.url}) has a currently valid certificate via OCSP.
                         You are seeing this warning due to enabling strict mode for OCSP / Revocation check.
                         OCSP Server Status: {ocsp_resp.response_status}""",
                         SecurityWarning,
                     )
+        else:
+            if strict:
+                warnings.warn(
+                    f"""Unable to insure that the remote peer ({r.url}) has a currently valid certificate via OCSP.
+                    You are seeing this warning due to enabling strict mode for OCSP / Revocation check.
+                    OCSP Server Status: {str(ocsp_http_response)}""",
+                    SecurityWarning,
+                )
 
 
 __all__ = ("verify",)
```

### Comparing `niquests-3.5.5/src/niquests/extensions/_picotls.py` & `niquests-3.6.0/src/niquests/extensions/_picotls.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/tests/conftest.py` & `niquests-3.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/tests/test_async.py` & `niquests-3.6.0/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/tests/test_help.py` & `niquests-3.6.0/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/tests/test_hooks.py` & `niquests-3.6.0/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/tests/test_live.py` & `niquests-3.6.0/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/tests/test_lowlevel.py` & `niquests-3.6.0/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/tests/test_multiplexed.py` & `niquests-3.6.0/tests/test_multiplexed.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/tests/test_requests.py` & `niquests-3.6.0/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/tests/test_structures.py` & `niquests-3.6.0/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/tests/test_testserver.py` & `niquests-3.6.0/tests/test_testserver.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/tests/test_utils.py` & `niquests-3.6.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/tests/utils.py` & `niquests-3.6.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/tests/testserver/server.py` & `niquests-3.6.0/tests/testserver/server.py`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/LICENSE` & `niquests-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `niquests-3.5.5/README.md` & `niquests-3.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 </div>
 
 **Niquests** is a simple, yet elegant, HTTP library. It is a drop-in replacement for **Requests**, which is under feature freeze.
 
 Niquests, is the “**Safest**, **Fastest[^10]**, **Easiest**, and **Most advanced**” Python HTTP Client. Production Ready!
 
 ✔️ **Try before you switch:** [See Multiplexed in Action](https://replit.com/@ahmedtahri4/Python#main.py)<br>
-📖 **See why you should switch:** [Read about 10 reasons why](https://medium.com/dev-genius/10-reasons-you-should-quit-your-http-client-98fd4c94bef3)
+📖 **See why you should switch:** [Read about 10 reasons why](https://medium.com/dev-genius/10-reasons-you-should-quit-your-http-client-98fd4c94bef3), and ["_Revived the promise made six years ago for Requests 3_"](https://medium.com/@ahmed.tahri/revived-the-promise-made-six-years-ago-for-requests-3-37b440e6a064)
 
 <details>
   <summary>👆 <b>Look at the feature table comparison</b> against <i>requests, httpx and aiohttp</i>!</summary>
 
 | Feature                             | niquests | requests  |     httpx     | aiohttp       |
 |-------------------------------------|:--------:|:---------:|:-------------:|---------------|
 | `HTTP/1.1`                          |    ✅     |     ✅     |       ✅       | ✅             |
@@ -110,14 +110,16 @@
 ```
 
 Niquests allows you to send HTTP requests extremely easily. There’s no need to manually add query strings to your URLs, or to form-encode your `PUT` & `POST` data — just use the `json` method!
 
 [![Downloads](https://static.pepy.tech/badge/niquests/month)](https://pepy.tech/project/niquests)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/niquests.svg)](https://pypi.org/project/niquests)
 
+This project does not require any compilation toolchain. The HTTP/3 support is not enforced and installed if your platform can support it natively _(e.g. pre-built wheel available)_.
+
 ## ✨ Installing Niquests and Supported Versions
 
 Niquests is available on PyPI:
 
 ```console
 $ python -m pip install niquests
 ```
```

### Comparing `niquests-3.5.5/pyproject.toml` & `niquests-3.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,32 +37,32 @@
     "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">=3.7"
 dynamic = ["version"]
 dependencies = [
     "charset_normalizer>=2,<4",
     "idna>=2.5,<4",
-    "urllib3.future>=2.7.900,<3",
+    "urllib3.future>=2.7.904,<3",
     "wassima>=1.0.1,<2",
     "kiss_headers>=2,<4",
 ]
 
 [project.optional-dependencies]
 socks = [
     "urllib3.future[socks]",
 ]
 http3 = [
-    "urllib3.future[qh3]"
+    "urllib3.future[qh3]",
 ]
 ocsp = [
-    "cryptography<43.0.0,>=41.0.0"
+    "urllib3.future[qh3]",
 ]
 speedups = [
     "orjson>=3,<4",
-    "urllib3.future[zstd,brotli]"
+    "urllib3.future[zstd,brotli]",
 ]
 
 [project.urls]
 "Changelog" = "https://github.com/jawah/niquests/blob/main/HISTORY.md"
 "Documentation" = "https://niquests.readthedocs.io"
 "Code" = "https://github.com/jawah/niquests"
 "Issue tracker" = "https://github.com/jawah/niquests/issues"
```

### Comparing `niquests-3.5.5/PKG-INFO` & `niquests-3.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: niquests
-Version: 3.5.5
+Version: 3.6.0
 Summary: Niquests is a simple, yet elegant, HTTP library. It is a drop-in replacement for Requests, which is under feature freeze.
 Project-URL: Changelog, https://github.com/jawah/niquests/blob/main/HISTORY.md
 Project-URL: Documentation, https://niquests.readthedocs.io
 Project-URL: Code, https://github.com/jawah/niquests
 Project-URL: Issue tracker, https://github.com/jawah/niquests/issues
 Author-email: Kenneth Reitz <me@kennethreitz.org>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
@@ -30,20 +30,20 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Requires-Dist: charset-normalizer<4,>=2
 Requires-Dist: idna<4,>=2.5
 Requires-Dist: kiss-headers<4,>=2
-Requires-Dist: urllib3-future<3,>=2.7.900
+Requires-Dist: urllib3-future<3,>=2.7.904
 Requires-Dist: wassima<2,>=1.0.1
 Provides-Extra: http3
 Requires-Dist: urllib3-future[qh3]; extra == 'http3'
 Provides-Extra: ocsp
-Requires-Dist: cryptography<43.0.0,>=41.0.0; extra == 'ocsp'
+Requires-Dist: urllib3-future[qh3]; extra == 'ocsp'
 Provides-Extra: socks
 Requires-Dist: urllib3-future[socks]; extra == 'socks'
 Provides-Extra: speedups
 Requires-Dist: orjson<4,>=3; extra == 'speedups'
 Requires-Dist: urllib3-future[brotli,zstd]; extra == 'speedups'
 Description-Content-Type: text/markdown
 
@@ -52,15 +52,15 @@
 </div>
 
 **Niquests** is a simple, yet elegant, HTTP library. It is a drop-in replacement for **Requests**, which is under feature freeze.
 
 Niquests, is the “**Safest**, **Fastest[^10]**, **Easiest**, and **Most advanced**” Python HTTP Client. Production Ready!
 
 ✔️ **Try before you switch:** [See Multiplexed in Action](https://replit.com/@ahmedtahri4/Python#main.py)<br>
-📖 **See why you should switch:** [Read about 10 reasons why](https://medium.com/dev-genius/10-reasons-you-should-quit-your-http-client-98fd4c94bef3)
+📖 **See why you should switch:** [Read about 10 reasons why](https://medium.com/dev-genius/10-reasons-you-should-quit-your-http-client-98fd4c94bef3), and ["_Revived the promise made six years ago for Requests 3_"](https://medium.com/@ahmed.tahri/revived-the-promise-made-six-years-ago-for-requests-3-37b440e6a064)
 
 <details>
   <summary>👆 <b>Look at the feature table comparison</b> against <i>requests, httpx and aiohttp</i>!</summary>
 
 | Feature                             | niquests | requests  |     httpx     | aiohttp       |
 |-------------------------------------|:--------:|:---------:|:-------------:|---------------|
 | `HTTP/1.1`                          |    ✅     |     ✅     |       ✅       | ✅             |
@@ -159,14 +159,16 @@
 ```
 
 Niquests allows you to send HTTP requests extremely easily. There’s no need to manually add query strings to your URLs, or to form-encode your `PUT` & `POST` data — just use the `json` method!
 
 [![Downloads](https://static.pepy.tech/badge/niquests/month)](https://pepy.tech/project/niquests)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/niquests.svg)](https://pypi.org/project/niquests)
 
+This project does not require any compilation toolchain. The HTTP/3 support is not enforced and installed if your platform can support it natively _(e.g. pre-built wheel available)_.
+
 ## ✨ Installing Niquests and Supported Versions
 
 Niquests is available on PyPI:
 
 ```console
 $ python -m pip install niquests
 ```
```

