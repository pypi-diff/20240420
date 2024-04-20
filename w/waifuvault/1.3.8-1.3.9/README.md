# Comparing `tmp/waifuvault-1.3.8.tar.gz` & `tmp/waifuvault-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waifuvault-1.3.8.tar", last modified: Tue Apr  2 18:32:35 2024, max compression
+gzip compressed data, was "waifuvault-1.3.9.tar", last modified: Sat Apr 20 13:54:15 2024, max compression
```

## Comparing `waifuvault-1.3.8.tar` & `waifuvault-1.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:32:35.016278 waifuvault-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 18:32:18.000000 waifuvault-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-04-02 18:32:35.016278 waifuvault-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-02 18:32:18.000000 waifuvault-1.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-02 18:32:18.000000 waifuvault-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:32:35.016278 waifuvault-1.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:32:35.016278 waifuvault-1.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:32:35.016278 waifuvault-1.3.8/src/waifuvault/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 18:32:18.000000 waifuvault-1.3.8/src/waifuvault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-02 18:32:18.000000 waifuvault-1.3.8/src/waifuvault/waifumodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-02 18:32:18.000000 waifuvault-1.3.8/src/waifuvault/waifuvault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:32:35.016278 waifuvault-1.3.8/src/waifuvault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-04-02 18:32:35.000000 waifuvault-1.3.8/src/waifuvault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-02 18:32:35.000000 waifuvault-1.3.8/src/waifuvault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:32:35.000000 waifuvault-1.3.8/src/waifuvault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 18:32:35.000000 waifuvault-1.3.8/src/waifuvault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 18:32:35.000000 waifuvault-1.3.8/src/waifuvault.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:32:35.016278 waifuvault-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-04-02 18:32:18.000000 waifuvault-1.3.8/tests/test_waifuvault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:54:15.405727 waifuvault-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-20 13:54:02.000000 waifuvault-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-20 13:54:15.405727 waifuvault-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-04-20 13:54:02.000000 waifuvault-1.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-20 13:54:02.000000 waifuvault-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:54:15.409727 waifuvault-1.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:54:15.405727 waifuvault-1.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:54:15.405727 waifuvault-1.3.9/src/waifuvault/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-20 13:54:02.000000 waifuvault-1.3.9/src/waifuvault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-20 13:54:02.000000 waifuvault-1.3.9/src/waifuvault/waifumodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-20 13:54:02.000000 waifuvault-1.3.9/src/waifuvault/waifuvault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:54:15.405727 waifuvault-1.3.9/src/waifuvault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-20 13:54:15.000000 waifuvault-1.3.9/src/waifuvault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-20 13:54:15.000000 waifuvault-1.3.9/src/waifuvault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:54:15.000000 waifuvault-1.3.9/src/waifuvault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-20 13:54:15.000000 waifuvault-1.3.9/src/waifuvault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 13:54:15.000000 waifuvault-1.3.9/src/waifuvault.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:54:15.405727 waifuvault-1.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-20 13:54:02.000000 waifuvault-1.3.9/tests/test_waifuvault.py
```

### Comparing `waifuvault-1.3.8/LICENSE` & `waifuvault-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `waifuvault-1.3.8/PKG-INFO` & `waifuvault-1.3.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-Metadata-Version: 2.1
-Name: waifuvault
-Version: 1.3.8
-Summary: waifuVault Python API module
-Author-email: Walker Aldridge <walker@waifuvault.moe>
-Project-URL: Homepage, https://github.com/waifuvault/waifuVault-python-api
-Project-URL: Issues, https://github.com/waifuvault/waifuVault-python-api/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: requests_toolbelt
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-mock; extra == "dev"
-
 # waifuvault-python-api
 
 ![tests](https://github.com/waifuvault/waifuVault-python-api/actions/workflows/deploy.yml/badge.svg)
+[![GitHub issues](https://img.shields.io/github/issues/waifuvault/waifuVault-python-api.png)](https://github.com/waifuvault/waifuVault-python-api/issues)
+[![last-commit](https://img.shields.io/github/last-commit/waifuvault/waifuVault-python-api)](https://github.com/waifuvault/waifuVault-python-api/commits/master)
 
 This contains the official API bindings for uploading, deleting and obtaining files
 with [waifuvault.moe](https://waifuvault.moe/). Contains a full up to date API for interacting with the service
 
 ## Installation
 
 ```sh
```

### Comparing `waifuvault-1.3.8/README.md` & `waifuvault-1.3.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,31 @@
+Metadata-Version: 2.1
+Name: waifuvault
+Version: 1.3.9
+Summary: waifuVault Python API module
+Author-email: Walker Aldridge <walker@waifuvault.moe>
+Project-URL: Homepage, https://github.com/waifuvault/waifuVault-python-api
+Project-URL: Issues, https://github.com/waifuvault/waifuVault-python-api/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: requests_toolbelt
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
+
 # waifuvault-python-api
 
 ![tests](https://github.com/waifuvault/waifuVault-python-api/actions/workflows/deploy.yml/badge.svg)
+[![GitHub issues](https://img.shields.io/github/issues/waifuvault/waifuVault-python-api.png)](https://github.com/waifuvault/waifuVault-python-api/issues)
+[![last-commit](https://img.shields.io/github/last-commit/waifuvault/waifuVault-python-api)](https://github.com/waifuvault/waifuVault-python-api/commits/master)
 
 This contains the official API bindings for uploading, deleting and obtaining files
 with [waifuvault.moe](https://waifuvault.moe/). Contains a full up to date API for interacting with the service
 
 ## Installation
 
 ```sh
```

### Comparing `waifuvault-1.3.8/pyproject.toml` & `waifuvault-1.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waifuvault"
-version = "1.3.8"
+version = "1.3.9"
 authors = [
     { name="Walker Aldridge", email="walker@waifuvault.moe" },
 ]
 description = "waifuVault Python API module"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `waifuvault-1.3.8/src/waifuvault/waifumodels.py` & `waifuvault-1.3.9/src/waifuvault/waifumodels.py`

 * *Files identical despite different names*

### Comparing `waifuvault-1.3.8/src/waifuvault/waifuvault.py` & `waifuvault-1.3.9/src/waifuvault/waifuvault.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         )
         header_data = {'Content-Type': multipart_data.content_type}
     elif file_obj.is_url():
         multipart_data = {'url': file_obj.target}
         header_data = None
     else:
         multipart_data = MultipartEncoder(
-            fields={'file': (os.path.basename(file_obj.target), open(file_obj.target, 'rb'))}
+            fields={'file': (os.path.basename(file_obj.target), open(os.path.expanduser(file_obj.target), 'rb'))}
         )
         header_data = {'Content-Type': multipart_data.content_type}
 
     response = requests.put(
         __base_url__,
         params=file_obj.build_parameters(),
         data=multipart_data,
```

### Comparing `waifuvault-1.3.8/src/waifuvault.egg-info/PKG-INFO` & `waifuvault-1.3.9/src/waifuvault.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waifuvault
-Version: 1.3.8
+Version: 1.3.9
 Summary: waifuVault Python API module
 Author-email: Walker Aldridge <walker@waifuvault.moe>
 Project-URL: Homepage, https://github.com/waifuvault/waifuVault-python-api
 Project-URL: Issues, https://github.com/waifuvault/waifuVault-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,16 @@
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 
 # waifuvault-python-api
 
 ![tests](https://github.com/waifuvault/waifuVault-python-api/actions/workflows/deploy.yml/badge.svg)
+[![GitHub issues](https://img.shields.io/github/issues/waifuvault/waifuVault-python-api.png)](https://github.com/waifuvault/waifuVault-python-api/issues)
+[![last-commit](https://img.shields.io/github/last-commit/waifuvault/waifuVault-python-api)](https://github.com/waifuvault/waifuVault-python-api/commits/master)
 
 This contains the official API bindings for uploading, deleting and obtaining files
 with [waifuvault.moe](https://waifuvault.moe/). Contains a full up to date API for interacting with the service
 
 ## Installation
 
 ```sh
```

### Comparing `waifuvault-1.3.8/tests/test_waifuvault.py` & `waifuvault-1.3.9/tests/test_waifuvault.py`

 * *Files 6% similar despite different names*

```diff
@@ -208,7 +208,21 @@
 def test_download_error(mocker):
     # When
     mock_get = mocker.patch('requests.get', return_value=bad_request)
 
     # Then
     with pytest.raises(Exception, match=re.escape('Error 400 (BAD_REQUEST): Error Test')):
         file_down = waifuvault.get_file(waifuvault.FileResponse(url="https://waifuvault.moe/f/something"), "dangerWaifu")
+
+
+def test_url_args():
+    # Given
+    file_down = waifuvault.FileUpload("https://waifuvault.moe/test", expires="1d", password="testpassword", hidefilename=True, oneTimeDownload=True)
+
+    # When
+    args = file_down.build_parameters()
+
+    # Then
+    assert (args.get("expires") == "1d"), "expires not in arguments"
+    assert (args.get("password") == "testpassword"), "password not in arguments"
+    assert (args.get("hide_filename") == "true"), "hide_filename not in arguments"
+    assert (args.get("one_time_download") == "true"), "one_time_download not in arguments"
```

