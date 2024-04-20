# Comparing `tmp/across_burstcube-0.0.4.tar.gz` & `tmp/across_burstcube-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "across_burstcube-0.0.4.tar", last modified: Fri Apr 19 19:38:01 2024, max compression
+gzip compressed data, was "across_burstcube-0.4.tar", last modified: Fri Apr 19 18:58:37 2024, max compression
```

## Comparing `across_burstcube-0.0.4.tar` & `across_burstcube-0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:38:01.150447 across_burstcube-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:38:01.142447 across_burstcube-0.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:38:01.142447 across_burstcube-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-19 19:38:01.150447 across_burstcube-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:38:01.150447 across_burstcube-0.0.4/across_burstcube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-19 19:38:01.000000 across_burstcube-0.0.4/across_burstcube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-19 19:38:01.000000 across_burstcube-0.0.4/across_burstcube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:38:01.000000 across_burstcube-0.0.4/across_burstcube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 19:38:01.000000 across_burstcube-0.0.4/across_burstcube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 19:38:01.000000 across_burstcube-0.0.4/across_burstcube.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:38:01.146447 across_burstcube-0.0.4/across_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:38:01.146447 across_burstcube-0.0.4/across_client/across/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/across/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/across/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/across/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:38:01.146447 across_burstcube-0.0.4/across_client/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/base/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/base/coords.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/base/daterange.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/base/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/base/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:38:01.150447 across_burstcube-0.0.4/across_client/burstcube/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/burstcube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/burstcube/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/burstcube/fov.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/burstcube/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/burstcube/toorequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/across_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-19 19:37:54.000000 across_burstcube-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:38:01.150447 across_burstcube-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.469876 across_burstcube-0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.461876 across_burstcube-0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.461876 across_burstcube-0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 18:58:32.000000 across_burstcube-0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-19 18:58:32.000000 across_burstcube-0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 18:58:37.469876 across_burstcube-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-19 18:58:32.000000 across_burstcube-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_burstcube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/across/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/daterange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/burstcube/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/fov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/toorequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-19 18:58:32.000000 across_burstcube-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:58:37.469876 across_burstcube-0.4/setup.cfg
```

### Comparing `across_burstcube-0.0.4/.github/ISSUE_TEMPLATE.md` & `across_burstcube-0.4/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/.github/PULL_REQUEST_TEMPLATE.md` & `across_burstcube-0.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/.github/workflows/deploy.yml` & `across_burstcube-0.4/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/.github/workflows/pylint.yml` & `across_burstcube-0.4/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/PKG-INFO` & `across_burstcube-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: across-burstcube
-Version: 0.0.4
+Version: 0.4
 Summary: ACROSS API Python client
 Author-email: "Jamie A. Kennea" <jak51@psu.edu>
 Maintainer-email: "Jamie A. Kennea" <jak51@psu.edu>
 Project-URL: Homepage, https://github.com/jak574/across-api-client
 Project-URL: Bug Reports, https://github.com/jak574/across-api-client/issues
 Project-URL: Source, https://github.com/jak574/across-api-client/
 Keywords: astronomy,api,across
```

### Comparing `across_burstcube-0.0.4/across_burstcube.egg-info/PKG-INFO` & `across_burstcube-0.4/across_burstcube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: across-burstcube
-Version: 0.0.4
+Version: 0.4
 Summary: ACROSS API Python client
 Author-email: "Jamie A. Kennea" <jak51@psu.edu>
 Maintainer-email: "Jamie A. Kennea" <jak51@psu.edu>
 Project-URL: Homepage, https://github.com/jak574/across-api-client
 Project-URL: Bug Reports, https://github.com/jak574/across-api-client/issues
 Project-URL: Source, https://github.com/jak574/across-api-client/
 Keywords: astronomy,api,across
```

### Comparing `across_burstcube-0.0.4/across_burstcube.egg-info/SOURCES.txt` & `across_burstcube-0.4/across_burstcube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/across_client/across/resolve.py` & `across_burstcube-0.4/across_client/across/resolve.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/across_client/across/schema.py` & `across_burstcube-0.4/across_client/across/schema.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/across_client/base/common.py` & `across_burstcube-0.4/across_client/base/common.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/across_client/base/coords.py` & `across_burstcube-0.4/across_client/base/coords.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/across_client/base/daterange.py` & `across_burstcube-0.4/across_client/base/daterange.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/across_client/base/schema.py` & `across_burstcube-0.4/across_client/base/schema.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/across_client/burstcube/schema.py` & `across_burstcube-0.4/across_client/burstcube/schema.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/across_client/burstcube/toorequest.py` & `across_burstcube-0.4/across_client/burstcube/toorequest.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/across_client/functions.py` & `across_burstcube-0.4/across_client/functions.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.4/pyproject.toml` & `across_burstcube-0.4/pyproject.toml`

 * *Files identical despite different names*

