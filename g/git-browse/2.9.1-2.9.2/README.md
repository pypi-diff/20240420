# Comparing `tmp/git-browse-2.9.1.tar.gz` & `tmp/git-browse-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/git-browse-2.9.1.tar", last modified: Wed Jan 13 08:00:43 2021, max compression
+gzip compressed data, was "git-browse-2.9.2.tar", last modified: Tue Feb 23 07:50:00 2021, max compression
```

## Comparing `git-browse-2.9.1.tar` & `git-browse-2.9.2.tar`

### file list

```diff
@@ -1,23 +1,17 @@
-drwxrwxr-x   0 albertyw  (1000) albertyw  (1004)        0 2021-01-13 08:00:43.379109 git-browse-2.9.1/
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)     3777 2021-01-13 07:55:53.000000 git-browse-2.9.1/CHANGELOG.md
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)       56 2021-01-12 07:44:55.000000 git-browse-2.9.1/MANIFEST.in
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)     5979 2021-01-13 08:00:43.379109 git-browse-2.9.1/PKG-INFO
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)     4216 2020-10-19 05:01:52.000000 git-browse-2.9.1/README.md
-drwxrwxr-x   0 albertyw  (1000) albertyw  (1004)        0 2021-01-13 08:00:43.279106 git-browse-2.9.1/git_browse/
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)        0 2019-02-03 02:15:46.000000 git-browse-2.9.1/git_browse/__init__.py
--rwxrwxr-x   0 albertyw  (1000) albertyw  (1004)    16655 2021-01-13 07:56:03.000000 git-browse-2.9.1/git_browse/browse.py
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)        0 2020-07-07 05:43:57.000000 git-browse-2.9.1/git_browse/py.typed
-drwxrwxr-x   0 albertyw  (1000) albertyw  (1004)        0 2021-01-13 08:00:43.375109 git-browse-2.9.1/git_browse/tests/
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)        0 2018-07-04 05:47:21.000000 git-browse-2.9.1/git_browse/tests/__init__.py
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)    17582 2021-01-13 07:52:49.000000 git-browse-2.9.1/git_browse/tests/test.py
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)     4684 2021-01-13 07:53:17.000000 git-browse-2.9.1/git_browse/tests/test_git_urls.py
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)      234 2020-07-12 06:52:06.000000 git-browse-2.9.1/git_browse/tests/test_util.py
-drwxrwxr-x   0 albertyw  (1000) albertyw  (1004)        0 2021-01-13 08:00:43.315107 git-browse-2.9.1/git_browse.egg-info/
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)     5979 2021-01-13 08:00:41.000000 git-browse-2.9.1/git_browse.egg-info/PKG-INFO
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)      431 2021-01-13 08:00:42.000000 git-browse-2.9.1/git_browse.egg-info/SOURCES.txt
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)        1 2021-01-13 08:00:41.000000 git-browse-2.9.1/git_browse.egg-info/dependency_links.txt
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)       55 2021-01-13 08:00:41.000000 git-browse-2.9.1/git_browse.egg-info/entry_points.txt
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)       15 2021-01-13 08:00:41.000000 git-browse-2.9.1/git_browse.egg-info/requires.txt
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)       11 2021-01-13 08:00:41.000000 git-browse-2.9.1/git_browse.egg-info/top_level.txt
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)       38 2021-01-13 08:00:43.379109 git-browse-2.9.1/setup.cfg
--rw-rw-r--   0 albertyw  (1000) albertyw  (1004)     1833 2021-01-12 08:32:23.000000 git-browse-2.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-23 07:50:00.120070 git-browse-2.9.2/
+-rw-r--r--   0 root         (0) root         (0)     3879 2021-02-23 07:49:37.000000 git-browse-2.9.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)       56 2021-02-23 07:49:37.000000 git-browse-2.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5936 2021-02-23 07:50:00.120070 git-browse-2.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4205 2021-02-23 07:49:37.000000 git-browse-2.9.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-23 07:50:00.120070 git-browse-2.9.2/git_browse/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-02-23 07:49:37.000000 git-browse-2.9.2/git_browse/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    16655 2021-02-23 07:49:37.000000 git-browse-2.9.2/git_browse/browse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-23 07:50:00.120070 git-browse-2.9.2/git_browse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5936 2021-02-23 07:50:00.000000 git-browse-2.9.2/git_browse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      293 2021-02-23 07:50:00.000000 git-browse-2.9.2/git_browse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-02-23 07:50:00.000000 git-browse-2.9.2/git_browse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2021-02-23 07:50:00.000000 git-browse-2.9.2/git_browse.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2021-02-23 07:50:00.000000 git-browse-2.9.2/git_browse.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2021-02-23 07:50:00.000000 git-browse-2.9.2/git_browse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-02-23 07:50:00.120070 git-browse-2.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1833 2021-02-23 07:49:37.000000 git-browse-2.9.2/setup.py
```

### Comparing `git-browse-2.9.1/CHANGELOG.md` & `git-browse-2.9.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+v2.9.2 (2021-02-22)
+-------------------
+
+ - Switch CI from codeship to Drone
+ - Update dependencies
+
+
 v2.9.1 (2021-01-13)
 -------------------
 
  - Change how browsing phabricator urls works.  Instead of entirely offloading the work to arcanist, read arcanist's output.
  - Significant refactors to simplify code and update to more modern python
```

### Comparing `git-browse-2.9.1/PKG-INFO` & `git-browse-2.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: git-browse
-Version: 2.9.1
+Version: 2.9.2
 Summary: Open repositories, directories, and files in the browser
 Home-page: https://github.com/albertyw/git-browse
 Author: Albert Wang
 Author-email: git@albertyw.com
 License: MIT
 Description: Git Browse
         ==========
         
         [![PyPI](https://img.shields.io/pypi/v/git-browse)](https://pypi.org/project/git-browse/)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/git-browse)
         ![PyPI - License](https://img.shields.io/pypi/l/git-browse)
         
-        [![Codeship Status for albertyw/git-browse](https://app.codeship.com/projects/fbd67810-b952-0134-2c2e-166255a25182/status?branch=master)](https://app.codeship.com/projects/194945)
+        [![Build Status](https://drone.albertyw.com/api/badges/albertyw/git-browse/status.svg)](https://drone.albertyw.com/albertyw/git-browse)
         [![Dependency Status](https://pyup.io/repos/github/albertyw/git-browse/shield.svg)](https://pyup.io/repos/github/albertyw/git-browse/)
         [![Code Climate](https://codeclimate.com/github/albertyw/git-browse/badges/gpa.svg)](https://codeclimate.com/github/albertyw/git-browse)
         [![Test Coverage](https://codeclimate.com/github/albertyw/git-browse/badges/coverage.svg)](https://codeclimate.com/github/albertyw/git-browse/coverage)
         
         
         Open repositories, directories, and files in the browser. See also,
         [git-reviewers](https://github.com/albertyw/git-reviewer).
@@ -100,21 +100,17 @@
         flake8
         mypy git_browse/browse.py
         ```
         
         Publishing
         ----------
         
-        ```bash
-        pip install twine
-        python setup.py sdist bdist_wheel
-        twine upload dist/*
-        ```
-        
-        Need to also update [albertyw/homebrew-albertyw](https://github.com/albertyw/homebrew-albertyw).
+        1.  Update changelog and `__version__` variable with a semantic version
+        2.  Commit changes, create a version tag, and push both
+        3.  Update [albertyw/homebrew-albertyw](https://github.com/albertyw/homebrew-albertyw)
         
 Keywords: github phabricator repository browser
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Version Control
```

### Comparing `git-browse-2.9.1/README.md` & `git-browse-2.9.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Git Browse
 ==========
 
 [![PyPI](https://img.shields.io/pypi/v/git-browse)](https://pypi.org/project/git-browse/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/git-browse)
 ![PyPI - License](https://img.shields.io/pypi/l/git-browse)
 
-[![Codeship Status for albertyw/git-browse](https://app.codeship.com/projects/fbd67810-b952-0134-2c2e-166255a25182/status?branch=master)](https://app.codeship.com/projects/194945)
+[![Build Status](https://drone.albertyw.com/api/badges/albertyw/git-browse/status.svg)](https://drone.albertyw.com/albertyw/git-browse)
 [![Dependency Status](https://pyup.io/repos/github/albertyw/git-browse/shield.svg)](https://pyup.io/repos/github/albertyw/git-browse/)
 [![Code Climate](https://codeclimate.com/github/albertyw/git-browse/badges/gpa.svg)](https://codeclimate.com/github/albertyw/git-browse)
 [![Test Coverage](https://codeclimate.com/github/albertyw/git-browse/badges/coverage.svg)](https://codeclimate.com/github/albertyw/git-browse/coverage)
 
 
 Open repositories, directories, and files in the browser. See also,
 [git-reviewers](https://github.com/albertyw/git-reviewer).
@@ -92,14 +92,10 @@
 flake8
 mypy git_browse/browse.py
 ```
 
 Publishing
 ----------
 
-```bash
-pip install twine
-python setup.py sdist bdist_wheel
-twine upload dist/*
-```
-
-Need to also update [albertyw/homebrew-albertyw](https://github.com/albertyw/homebrew-albertyw).
+1.  Update changelog and `__version__` variable with a semantic version
+2.  Commit changes, create a version tag, and push both
+3.  Update [albertyw/homebrew-albertyw](https://github.com/albertyw/homebrew-albertyw)
```

### Comparing `git-browse-2.9.1/git_browse/browse.py` & `git-browse-2.9.2/git_browse/browse.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import re
 import subprocess
 from typing import Dict, Match, Optional, Type
 import webbrowser
 
 
-__version__ = '2.9.1'
+__version__ = '2.9.2'
 GITHUB_HOST = '(?P<host>github\\.com)'
 UBER_HOST = '(?P<host>code\\.uber\\.internal)'
 UBER_CONFIG_HOST = '(?P<host>config\\.uber\\.internal)'
 USER_REGEX = '(?P<user>[\\w\\.@:\\/~_-]+)'
 REPOSITORY_REGEX = '(?P<repository>[\\w\\.@:\\/~_-]+)'
 GITHUB_SSH_URL = 'git@%s:%s/%s' % (GITHUB_HOST, USER_REGEX, REPOSITORY_REGEX)
 GITHUB_HTTPS_URL = 'https://%s/%s/%s' % \
```

### Comparing `git-browse-2.9.1/git_browse.egg-info/PKG-INFO` & `git-browse-2.9.2/git_browse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: git-browse
-Version: 2.9.1
+Version: 2.9.2
 Summary: Open repositories, directories, and files in the browser
 Home-page: https://github.com/albertyw/git-browse
 Author: Albert Wang
 Author-email: git@albertyw.com
 License: MIT
 Description: Git Browse
         ==========
         
         [![PyPI](https://img.shields.io/pypi/v/git-browse)](https://pypi.org/project/git-browse/)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/git-browse)
         ![PyPI - License](https://img.shields.io/pypi/l/git-browse)
         
-        [![Codeship Status for albertyw/git-browse](https://app.codeship.com/projects/fbd67810-b952-0134-2c2e-166255a25182/status?branch=master)](https://app.codeship.com/projects/194945)
+        [![Build Status](https://drone.albertyw.com/api/badges/albertyw/git-browse/status.svg)](https://drone.albertyw.com/albertyw/git-browse)
         [![Dependency Status](https://pyup.io/repos/github/albertyw/git-browse/shield.svg)](https://pyup.io/repos/github/albertyw/git-browse/)
         [![Code Climate](https://codeclimate.com/github/albertyw/git-browse/badges/gpa.svg)](https://codeclimate.com/github/albertyw/git-browse)
         [![Test Coverage](https://codeclimate.com/github/albertyw/git-browse/badges/coverage.svg)](https://codeclimate.com/github/albertyw/git-browse/coverage)
         
         
         Open repositories, directories, and files in the browser. See also,
         [git-reviewers](https://github.com/albertyw/git-reviewer).
@@ -100,21 +100,17 @@
         flake8
         mypy git_browse/browse.py
         ```
         
         Publishing
         ----------
         
-        ```bash
-        pip install twine
-        python setup.py sdist bdist_wheel
-        twine upload dist/*
-        ```
-        
-        Need to also update [albertyw/homebrew-albertyw](https://github.com/albertyw/homebrew-albertyw).
+        1.  Update changelog and `__version__` variable with a semantic version
+        2.  Commit changes, create a version tag, and push both
+        3.  Update [albertyw/homebrew-albertyw](https://github.com/albertyw/homebrew-albertyw)
         
 Keywords: github phabricator repository browser
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Version Control
```

### Comparing `git-browse-2.9.1/setup.py` & `git-browse-2.9.2/setup.py`

 * *Files identical despite different names*

