# Comparing `tmp/jaraco.xonsh-0.5.0.tar.gz` & `tmp/jaraco_xonsh-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.xonsh-0.5.0.tar", last modified: Tue Apr  2 14:38:12 2024, max compression
+gzip compressed data, was "jaraco_xonsh-0.5.1.tar", last modified: Sat Apr 20 13:50:29 2024, max compression
```

## Comparing `jaraco.xonsh-0.5.0.tar` & `jaraco_xonsh-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:38:12.889893 jaraco.xonsh-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:38:12.885893 jaraco.xonsh-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:38:12.885893 jaraco.xonsh-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-02 14:38:12.889893 jaraco.xonsh-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:38:12.885893 jaraco.xonsh-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:38:12.885893 jaraco.xonsh-0.5.0/jaraco/
--rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/jaraco/xonsh.xsh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:38:12.889893 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-02 14:38:12.000000 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-02 14:38:12.000000 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:38:12.000000 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 14:38:12.000000 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-02 14:38:12.000000 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 14:38:12.000000 jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-02 14:38:12.889893 jaraco.xonsh-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-02 14:37:56.000000 jaraco.xonsh-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:50:29.605560 jaraco_xonsh-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:50:29.601560 jaraco_xonsh-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:50:29.601560 jaraco_xonsh-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-20 13:50:29.605560 jaraco_xonsh-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:50:29.601560 jaraco_xonsh-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:50:29.601560 jaraco_xonsh-0.5.1/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/jaraco/xonsh.xsh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:50:29.605560 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-20 13:50:29.000000 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-20 13:50:29.000000 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:50:29.000000 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-20 13:50:29.000000 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-20 13:50:29.000000 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 13:50:29.000000 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:50:29.605560 jaraco_xonsh-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/tox.ini
```

### Comparing `jaraco.xonsh-0.5.0/.github/workflows/main.yml` & `jaraco_xonsh-0.5.1/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
   TOX_OVERRIDE: >-
     testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
+      # https://blog.jaraco.com/efficient-use-of-ci-resources/
       matrix:
         python:
         - "3.8"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
```

### Comparing `jaraco.xonsh-0.5.0/LICENSE` & `jaraco_xonsh-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.xonsh-0.5.0/NEWS.rst` & `jaraco_xonsh-0.5.1/NEWS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v0.5.1
+======
+
+No significant changes.
+
+
 v0.5.0
 ======
 
 Features
 --------
 
 - Use another command to get the whole message.
```

### Comparing `jaraco.xonsh-0.5.0/PKG-INFO` & `jaraco_xonsh-0.5.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: jaraco.xonsh
-Version: 0.5.0
+Version: 0.5.1
 Summary: Xonsh facilities used by jaraco
-Home-page: https://github.com/jaraco/jaraco.xonsh
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/jaraco.xonsh
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: jaraco.clipboard
 Requires-Dist: keyring
 Requires-Dist: xontrib-vox
 Provides-Extra: testing
 Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
```

### Comparing `jaraco.xonsh-0.5.0/README.rst` & `jaraco_xonsh-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.xonsh-0.5.0/docs/conf.py` & `jaraco_xonsh-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.xonsh-0.5.0/jaraco/xonsh.xsh` & `jaraco_xonsh-0.5.1/jaraco/xonsh.xsh`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 aliases['gpj'] = 'git push --set-upstream jaraco @$(git rev-parse --abbrev-ref HEAD)'
 
 aliases['hobgoblins'] = "git commit -a -m '👹 Feed the hobgoblins (delint).'"
 aliases['fade-to-black'] = "git commit -a -m '⚫ Fade to black.'"
 aliases['genuflect'] = "git commit -a -m '🧎‍♀️ Genuflect to the types.'"
 aliases['toil-the-docs'] = "git commit -a -m '🚡 Toil the docs.'"
 
+aliases['check-traps'] = 'pip-run jaraco.home -- -m jaraco.home.check-traps'
+
 try:
 	import jaraco.clipboard
 except ImportError:
 	print("Clipboard support unavailable")
 
 # https://xon.sh/osx.html#path-helper
 if platform.system() == 'Darwin':
```

### Comparing `jaraco.xonsh-0.5.0/jaraco.xonsh.egg-info/PKG-INFO` & `jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: jaraco.xonsh
-Version: 0.5.0
+Version: 0.5.1
 Summary: Xonsh facilities used by jaraco
-Home-page: https://github.com/jaraco/jaraco.xonsh
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/jaraco.xonsh
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: jaraco.clipboard
 Requires-Dist: keyring
 Requires-Dist: xontrib-vox
 Provides-Extra: testing
 Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
```

### Comparing `jaraco.xonsh-0.5.0/pytest.ini` & `jaraco_xonsh-0.5.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.xonsh-0.5.0/tox.ini` & `jaraco_xonsh-0.5.1/tox.ini`

 * *Files identical despite different names*

