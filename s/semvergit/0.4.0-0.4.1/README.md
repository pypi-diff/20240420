# Comparing `tmp/semvergit-0.4.0.tar.gz` & `tmp/semvergit-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semvergit-0.4.0.tar", last modified: Thu Apr 18 15:06:53 2024, max compression
+gzip compressed data, was "semvergit-0.4.1.tar", last modified: Sat Apr 20 11:06:29 2024, max compression
```

## Comparing `semvergit-0.4.0.tar` & `semvergit-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:53.374284 semvergit-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-18 15:06:36.000000 semvergit-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-18 15:06:53.374284 semvergit-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-18 15:06:36.000000 semvergit-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-18 15:06:36.000000 semvergit-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:53.366284 semvergit-0.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-18 15:06:36.000000 semvergit-0.4.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-18 15:06:36.000000 semvergit-0.4.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:06:53.374284 semvergit-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:53.366284 semvergit-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:53.370283 semvergit-0.4.0/src/semvergit/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-18 15:06:36.000000 semvergit-0.4.0/src/semvergit/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:53.370283 semvergit-0.4.0/src/semvergit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-18 15:06:53.000000 semvergit-0.4.0/src/semvergit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-18 15:06:53.000000 semvergit-0.4.0/src/semvergit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:06:53.000000 semvergit-0.4.0/src/semvergit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 15:06:53.000000 semvergit-0.4.0/src/semvergit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-18 15:06:53.000000 semvergit-0.4.0/src/semvergit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 15:06:53.000000 semvergit-0.4.0/src/semvergit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:53.370283 semvergit-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-18 15:06:36.000000 semvergit-0.4.0/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-18 15:06:36.000000 semvergit-0.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-18 15:06:36.000000 semvergit-0.4.0/tests/test_file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-18 15:06:36.000000 semvergit-0.4.0/tests/test_git_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-18 15:06:36.000000 semvergit-0.4.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-18 15:06:36.000000 semvergit-0.4.0/tests/test_log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:06:29.681765 semvergit-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-20 11:06:11.000000 semvergit-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-20 11:06:29.681765 semvergit-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-20 11:06:11.000000 semvergit-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-20 11:06:11.000000 semvergit-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:06:29.673765 semvergit-0.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-20 11:06:11.000000 semvergit-0.4.1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-20 11:06:11.000000 semvergit-0.4.1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 11:06:29.681765 semvergit-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:06:29.673765 semvergit-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:06:29.677765 semvergit-0.4.1/src/semvergit/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 11:06:11.000000 semvergit-0.4.1/src/semvergit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-20 11:06:11.000000 semvergit-0.4.1/src/semvergit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-20 11:06:11.000000 semvergit-0.4.1/src/semvergit/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-20 11:06:11.000000 semvergit-0.4.1/src/semvergit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-20 11:06:11.000000 semvergit-0.4.1/src/semvergit/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-20 11:06:11.000000 semvergit-0.4.1/src/semvergit/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-20 11:06:11.000000 semvergit-0.4.1/src/semvergit/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:06:29.677765 semvergit-0.4.1/src/semvergit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-20 11:06:29.000000 semvergit-0.4.1/src/semvergit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-20 11:06:29.000000 semvergit-0.4.1/src/semvergit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 11:06:29.000000 semvergit-0.4.1/src/semvergit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-20 11:06:29.000000 semvergit-0.4.1/src/semvergit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-20 11:06:29.000000 semvergit-0.4.1/src/semvergit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 11:06:29.000000 semvergit-0.4.1/src/semvergit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:06:29.677765 semvergit-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-20 11:06:11.000000 semvergit-0.4.1/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-20 11:06:11.000000 semvergit-0.4.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-20 11:06:11.000000 semvergit-0.4.1/tests/test_file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-20 11:06:11.000000 semvergit-0.4.1/tests/test_git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-20 11:06:11.000000 semvergit-0.4.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-20 11:06:11.000000 semvergit-0.4.1/tests/test_log_utils.py
```

### Comparing `semvergit-0.4.0/LICENSE` & `semvergit-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `semvergit-0.4.0/PKG-INFO` & `semvergit-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semvergit
-Version: 0.4.0
+Version: 0.4.1
 Summary: Manage your project's version numbers.
 Author-email: Roy Moore <roy@moore.co.il>
 Project-URL: homepage, https://github.com/Tranquility2/semvergit
 Project-URL: repository, https://github.com/Tranquility2/semvergit
 Keywords: packaging,publishing,release,versioning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -90,22 +90,22 @@
 4. Push the tag to the remote
 
 ## Why?
 I created this tool to help me manage my project's version numbers.
 I wanted a simple tool that I could use in my CI/CD pipeline to bump the version number and tag the commit.
 
 ## Features
-❇️ Bump the version number and update the git tag in one command
-❇️ Dry run mode
-❇️ Verbose mode
-❇️ Custom commit message
-❇️ Auto commit message
-🆕 Version 0.4+ introduces the ability to automatically update the version number in a file
+❇️ Bump the version number and update the git tag in one command  
+❇️ Dry run mode  
+❇️ Verbose mode  
+❇️ Custom commit message*  
+❇️ Auto commit message*  
+🆕 Version 0.4+ introduces the ability to automatically update the version number in a file*
 
-Please keep in mind it is designed to be used in a CI/CD pipeline (but not limited to...)
+<sup>*Please see the [limitations](#Limitations) section below</sup>
 
 ## How to use
 
 Simple install using
 ``pip install semvergit``
 
 Then you can use it in your project as simply as:
@@ -130,14 +130,21 @@
   -t, --bump_type TEXT     Bump Type ['major', 'minor', 'patch', 'prerelease']
   -m, --message TEXT       Commit message
   -am, --auto_message      Auto commit message
   -f, --version_file FILE  Version file
   --help                   Show this message and exit.
 ```
 
+## Limitations
+Please keep in mind that when using features like `commit message` / `auto commit message` and `version file` the tool will try and commit the changes to the git repo.
+
+Even though this is quite handy, it should be used mannually as it **cannot be used directly in a CI/CD pipeline directed at `master` or `main` branches** as it will likly fail due to the commit not being allowed without a PR.
+
+💡 Only git tags can be pushed to the remote without a PR *(and this is the main use case for this tool)*.
+
 ## Development
 
 Please see [CONTRIBUTING.md](CONTRIBUTING.md)
 
 ## License
 
 This project is published under the MIT license.
```

### Comparing `semvergit-0.4.0/README.md` & `semvergit-0.4.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 4. Push the tag to the remote
 
 ## Why?
 I created this tool to help me manage my project's version numbers.
 I wanted a simple tool that I could use in my CI/CD pipeline to bump the version number and tag the commit.
 
 ## Features
-❇️ Bump the version number and update the git tag in one command
-❇️ Dry run mode
-❇️ Verbose mode
-❇️ Custom commit message
-❇️ Auto commit message
-🆕 Version 0.4+ introduces the ability to automatically update the version number in a file
+❇️ Bump the version number and update the git tag in one command  
+❇️ Dry run mode  
+❇️ Verbose mode  
+❇️ Custom commit message*  
+❇️ Auto commit message*  
+🆕 Version 0.4+ introduces the ability to automatically update the version number in a file*
 
-Please keep in mind it is designed to be used in a CI/CD pipeline (but not limited to...)
+<sup>*Please see the [limitations](#Limitations) section below</sup>
 
 ## How to use
 
 Simple install using
 ``pip install semvergit``
 
 Then you can use it in your project as simply as:
@@ -65,14 +65,21 @@
   -t, --bump_type TEXT     Bump Type ['major', 'minor', 'patch', 'prerelease']
   -m, --message TEXT       Commit message
   -am, --auto_message      Auto commit message
   -f, --version_file FILE  Version file
   --help                   Show this message and exit.
 ```
 
+## Limitations
+Please keep in mind that when using features like `commit message` / `auto commit message` and `version file` the tool will try and commit the changes to the git repo.
+
+Even though this is quite handy, it should be used mannually as it **cannot be used directly in a CI/CD pipeline directed at `master` or `main` branches** as it will likly fail due to the commit not being allowed without a PR.
+
+💡 Only git tags can be pushed to the remote without a PR *(and this is the main use case for this tool)*.
+
 ## Development
 
 Please see [CONTRIBUTING.md](CONTRIBUTING.md)
 
 ## License
 
 This project is published under the MIT license.
```

### Comparing `semvergit-0.4.0/pyproject.toml` & `semvergit-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `semvergit-0.4.0/requirements/requirements-dev.txt` & `semvergit-0.4.1/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `semvergit-0.4.0/requirements/requirements-test.txt` & `semvergit-0.4.1/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `semvergit-0.4.0/src/semvergit/app.py` & `semvergit-0.4.1/src/semvergit/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import List, Optional
 
 from loguru import logger
 from semver import VersionInfo
 
 from semvergit.file_utils import update_verion_file
 from semvergit.git_utils import (
+    add_file,
     get_active_branch,
     get_repo,
     get_tags_with_prefix,
     new_commit,
     pull_remote,
     push_remote,
     set_tag,
@@ -84,14 +85,15 @@
 
         if dry_run:
             logger.warning("⚠️ Dry run (no tag set or pushed)")
 
         if version_file:
             logger.info(f"📝 Writing version to {version_file}...")
             update_verion_file(version_file, new_version, dry_run)
+            add_file(repo=self.current_repo, file_path=version_file, dry_run=dry_run)
 
             if not commit_message:
                 # Upading the version file requires a commit message
                 auto_message = True
 
         if auto_message:
             commit_message = f"New version: {str(new_version)}"
```

### Comparing `semvergit-0.4.0/src/semvergit/cli.py` & `semvergit-0.4.1/src/semvergit/cli.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.4.0/src/semvergit/file_utils.py` & `semvergit-0.4.1/src/semvergit/file_utils.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.4.0/src/semvergit/git_utils.py` & `semvergit-0.4.1/src/semvergit/git_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,21 @@
     new_commit_id = repo.index.commit(message=message)
     short_commit_id = new_commit_id.hexsha[:7]
     logger.debug(f"Created commit [{short_commit_id}] {message}")
     return short_commit_id
 
 
 @drywrap
+def add_file(repo: Repo, file_path: str) -> None:
+    """Add file."""
+    repo.index.add([file_path])
+    logger.debug(f"Added file {file_path}")
+
+
+@drywrap
 def set_tag(repo: Repo, tag: str) -> VersionInfo:
     """Set tag."""
     new_tag = repo.create_tag(tag)
     logger.debug(f"Created {str(new_tag)}")
     return new_tag
```

### Comparing `semvergit-0.4.0/src/semvergit/log_utils.py` & `semvergit-0.4.1/src/semvergit/log_utils.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.4.0/src/semvergit.egg-info/PKG-INFO` & `semvergit-0.4.1/src/semvergit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semvergit
-Version: 0.4.0
+Version: 0.4.1
 Summary: Manage your project's version numbers.
 Author-email: Roy Moore <roy@moore.co.il>
 Project-URL: homepage, https://github.com/Tranquility2/semvergit
 Project-URL: repository, https://github.com/Tranquility2/semvergit
 Keywords: packaging,publishing,release,versioning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -90,22 +90,22 @@
 4. Push the tag to the remote
 
 ## Why?
 I created this tool to help me manage my project's version numbers.
 I wanted a simple tool that I could use in my CI/CD pipeline to bump the version number and tag the commit.
 
 ## Features
-❇️ Bump the version number and update the git tag in one command
-❇️ Dry run mode
-❇️ Verbose mode
-❇️ Custom commit message
-❇️ Auto commit message
-🆕 Version 0.4+ introduces the ability to automatically update the version number in a file
+❇️ Bump the version number and update the git tag in one command  
+❇️ Dry run mode  
+❇️ Verbose mode  
+❇️ Custom commit message*  
+❇️ Auto commit message*  
+🆕 Version 0.4+ introduces the ability to automatically update the version number in a file*
 
-Please keep in mind it is designed to be used in a CI/CD pipeline (but not limited to...)
+<sup>*Please see the [limitations](#Limitations) section below</sup>
 
 ## How to use
 
 Simple install using
 ``pip install semvergit``
 
 Then you can use it in your project as simply as:
@@ -130,14 +130,21 @@
   -t, --bump_type TEXT     Bump Type ['major', 'minor', 'patch', 'prerelease']
   -m, --message TEXT       Commit message
   -am, --auto_message      Auto commit message
   -f, --version_file FILE  Version file
   --help                   Show this message and exit.
 ```
 
+## Limitations
+Please keep in mind that when using features like `commit message` / `auto commit message` and `version file` the tool will try and commit the changes to the git repo.
+
+Even though this is quite handy, it should be used mannually as it **cannot be used directly in a CI/CD pipeline directed at `master` or `main` branches** as it will likly fail due to the commit not being allowed without a PR.
+
+💡 Only git tags can be pushed to the remote without a PR *(and this is the main use case for this tool)*.
+
 ## Development
 
 Please see [CONTRIBUTING.md](CONTRIBUTING.md)
 
 ## License
 
 This project is published under the MIT license.
```

### Comparing `semvergit-0.4.0/src/semvergit.egg-info/SOURCES.txt` & `semvergit-0.4.1/src/semvergit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `semvergit-0.4.0/src/semvergit.egg-info/requires.txt` & `semvergit-0.4.1/src/semvergit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `semvergit-0.4.0/tests/test_app.py` & `semvergit-0.4.1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.4.0/tests/test_cli.py` & `semvergit-0.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.4.0/tests/test_file_utils.py` & `semvergit-0.4.1/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.4.0/tests/test_git_utils.py` & `semvergit-0.4.1/tests/test_git_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from typing import Dict, List, Tuple, TypeVar
 
 from git import Repo
 from pytest import MonkeyPatch, mark
 
 from semvergit.git_utils import (
+    add_file,
     drywrap,
     get_active_branch,
     get_repo,
     get_tags_with_prefix,
     new_commit,
     pull_remote,
     push_remote,
@@ -143,14 +144,31 @@
     test_repo = Repo()
 
     MonkeyPatch().setattr("semvergit.git_utils.Repo.index", MockIndex)
     result = new_commit(test_repo, "testmessage")
     assert result == "112233"
 
 
+def test_add_file() -> None:
+    """Test add_file."""
+
+    class MockIndex:  # pylint: disable=too-few-public-methods
+        """Mock index."""
+
+        @staticmethod
+        def add(files: List[str]) -> None:  # pylint: disable=unused-argument
+            """Add."""
+            pass  # pylint: disable=unnecessary-pass
+
+    test_repo = Repo()
+
+    MonkeyPatch().setattr("semvergit.git_utils.Repo.index", MockIndex)
+    add_file(test_repo, "testfile")
+
+
 def test_set_tag() -> None:
     """Test set_tag."""
 
     def mock_create_tag(repo: Repo, tag: str) -> str:  # pylint: disable=unused-argument
         """Mock create_tag."""
         return tag
```

### Comparing `semvergit-0.4.0/tests/test_integration.py` & `semvergit-0.4.1/tests/test_integration.py`

 * *Files identical despite different names*

