# Comparing `tmp/php_ast-1.1.tar.gz` & `tmp/php_ast-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/php_ast-1.1.tar", last modified: Sat Apr 20 09:22:56 2024, max compression
+gzip compressed data, was "dist/php_ast-1.2.tar", last modified: Sat Apr 20 09:36:16 2024, max compression
```

## Comparing `php_ast-1.1.tar` & `php_ast-1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 09:22:56.000000 php_ast-1.1/
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-20 07:29:24.000000 php_ast-1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1248 2024-04-20 09:22:56.000000 php_ast-1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      926 2024-04-20 08:41:23.000000 php_ast-1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 09:22:56.000000 php_ast-1.1/php_ast/
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-20 08:35:57.000000 php_ast-1.1/php_ast/__init__.py
--rw-r--r--   0 root         (0) root         (0) 12946080 2024-04-19 02:22:47.000000 php_ast-1.1/php_ast/libphp7.so
--rw-r--r--   0 root         (0) root         (0)     3003 2024-04-20 09:22:45.000000 php_ast-1.1/php_ast/php_ast.py
--rw-r--r--   0 root         (0) root         (0)      166 2024-04-20 08:38:13.000000 php_ast-1.1/php_ast/php_ast_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 09:22:56.000000 php_ast-1.1/php_ast.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1248 2024-04-20 09:22:56.000000 php_ast-1.1/php_ast.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      249 2024-04-20 09:22:56.000000 php_ast-1.1/php_ast.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 09:22:56.000000 php_ast-1.1/php_ast.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-20 09:22:56.000000 php_ast-1.1/php_ast.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 09:22:56.000000 php_ast-1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      589 2024-04-20 09:22:15.000000 php_ast-1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 09:22:56.000000 php_ast-1.1/test/
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-20 08:01:47.000000 php_ast-1.1/test/test_ast.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 09:36:16.000000 php_ast-1.2/
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-20 07:29:24.000000 php_ast-1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1294 2024-04-20 09:36:16.000000 php_ast-1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      972 2024-04-20 09:33:35.000000 php_ast-1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 09:36:16.000000 php_ast-1.2/php_ast/
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-20 08:35:57.000000 php_ast-1.2/php_ast/__init__.py
+-rw-r--r--   0 root         (0) root         (0) 12946080 2024-04-19 02:22:47.000000 php_ast-1.2/php_ast/libphp7.so
+-rw-r--r--   0 root         (0) root         (0)     3003 2024-04-20 09:22:45.000000 php_ast-1.2/php_ast/php_ast.py
+-rw-r--r--   0 root         (0) root         (0)      166 2024-04-20 08:38:13.000000 php_ast-1.2/php_ast/php_ast_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 09:36:16.000000 php_ast-1.2/php_ast.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1294 2024-04-20 09:36:16.000000 php_ast-1.2/php_ast.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      249 2024-04-20 09:36:16.000000 php_ast-1.2/php_ast.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 09:36:16.000000 php_ast-1.2/php_ast.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-20 09:36:16.000000 php_ast-1.2/php_ast.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 09:36:16.000000 php_ast-1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      589 2024-04-20 09:36:05.000000 php_ast-1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 09:36:16.000000 php_ast-1.2/test/
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-20 08:01:47.000000 php_ast-1.2/test/test_ast.py
```

### Comparing `php_ast-1.1/LICENSE` & `php_ast-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `php_ast-1.1/PKG-INFO` & `php_ast-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: php_ast
-Version: 1.1
+Version: 1.2
 Summary: A Python package for php_ast
 Home-page: https://github.com/php-ast/php_ast
 Author: php_ast
 Author-email: 20200120614@nxmu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #A Python Get PHP AST 
 
 
 #install 
 ```bash
-    pip install php_ast
+    btpip install -i https://pypi.tuna.tsinghua.edu.cn/simple php-ast
 ```
 
 
 #exapme 
 ```Python
 # get phpinfo ast
 from php_ast import get_ast
```

### Comparing `php_ast-1.1/README.md` & `php_ast-1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #A Python Get PHP AST 
 
 
 #install 
 ```bash
-    pip install php_ast
+    btpip install -i https://pypi.tuna.tsinghua.edu.cn/simple php-ast
 ```
 
 
 #exapme 
 ```Python
 # get phpinfo ast
 from php_ast import get_ast
```

### Comparing `php_ast-1.1/php_ast/libphp7.so` & `php_ast-1.2/php_ast/libphp7.so`

 * *Files identical despite different names*

### Comparing `php_ast-1.1/php_ast/php_ast.py` & `php_ast-1.2/php_ast/php_ast.py`

 * *Files identical despite different names*

### Comparing `php_ast-1.1/php_ast.egg-info/PKG-INFO` & `php_ast-1.2/php_ast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: php-ast
-Version: 1.1
+Version: 1.2
 Summary: A Python package for php_ast
 Home-page: https://github.com/php-ast/php_ast
 Author: php_ast
 Author-email: 20200120614@nxmu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #A Python Get PHP AST 
 
 
 #install 
 ```bash
-    pip install php_ast
+    btpip install -i https://pypi.tuna.tsinghua.edu.cn/simple php-ast
 ```
 
 
 #exapme 
 ```Python
 # get phpinfo ast
 from php_ast import get_ast
```

### Comparing `php_ast-1.1/setup.py` & `php_ast-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name="php_ast",
-    version="1.1",
+    version="1.2",
     packages=find_packages(),
     package_data={
         'php_ast': ['*.so'],
     },
     author="php_ast",
     author_email="20200120614@nxmu.edu.cn",
     description="A Python package for php_ast",
```

