# Comparing `tmp/sphinx-intl-2.1.0.tar.gz` & `tmp/sphinx_intl-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-intl-2.1.0.tar", last modified: Sun Feb  5 05:45:56 2023, max compression
+gzip compressed data, was "sphinx_intl-2.2.0.tar", last modified: Fri Apr 19 21:08:39 2024, max compression
```

## Comparing `sphinx-intl-2.1.0.tar` & `sphinx_intl-2.2.0.tar`

### file list

```diff
@@ -1,45 +1,51 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-02-05 05:45:56.973907 sphinx-intl-2.1.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      297 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/AUTHORS.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7167 2023-02-05 05:44:15.000000 sphinx-intl-2.1.0/CHANGES.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      174 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/CODE_OF_CONDUCT.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      195 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1321 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      121 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2863 2023-02-05 05:45:56.973907 sphinx-intl-2.1.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1616 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/README.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/checklist.rst
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-02-05 05:45:56.965907 sphinx-intl-2.1.0/doc/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      608 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/doc/Makefile
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       29 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/doc/authors.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1107 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/doc/basic.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       29 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/doc/changes.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      800 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/doc/conf.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1448 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/doc/dev.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1569 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/doc/index.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      779 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/doc/make.bat
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7791 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/doc/quickstart.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1097 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/doc/refs.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       24 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/doc/requirements.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       49 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/requirements-dev.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       27 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/requirements-testing.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      234 2023-02-05 05:45:56.981907 sphinx-intl-2.1.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2047 2023-02-05 05:36:17.000000 sphinx-intl-2.1.0/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-02-05 05:45:56.969907 sphinx-intl-2.1.0/sphinx_intl/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       47 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/sphinx_intl/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/sphinx_intl/__main__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4942 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/sphinx_intl/basic.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2072 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/sphinx_intl/catalog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/sphinx_intl/commands.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2024 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/sphinx_intl/pycompat.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      579 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/sphinx_intl/sphinx_util.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5402 2023-02-04 07:21:50.000000 sphinx-intl-2.1.0/sphinx_intl/transifex.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-02-05 05:45:56.973907 sphinx-intl-2.1.0/sphinx_intl.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2863 2023-02-05 05:45:56.000000 sphinx-intl-2.1.0/sphinx_intl.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      823 2023-02-05 05:45:56.000000 sphinx-intl-2.1.0/sphinx_intl.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-05 05:45:56.000000 sphinx-intl-2.1.0/sphinx_intl.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       70 2023-02-05 05:45:56.000000 sphinx-intl-2.1.0/sphinx_intl.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-05 05:45:56.000000 sphinx-intl-2.1.0/sphinx_intl.egg-info/namespace_packages.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-04 07:22:10.000000 sphinx-intl-2.1.0/sphinx_intl.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-02-05 05:45:56.000000 sphinx-intl-2.1.0/sphinx_intl.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       12 2023-02-05 05:45:56.000000 sphinx-intl-2.1.0/sphinx_intl.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      626 2023-02-05 05:36:17.000000 sphinx-intl-2.1.0/tox.ini
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-19 21:08:39.565002 sphinx_intl-2.2.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      297 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/AUTHORS.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8622 2024-04-19 20:54:09.000000 sphinx_intl-2.2.0/CHANGES.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      174 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/CODE_OF_CONDUCT.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      195 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1321 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      121 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/MANIFEST.in
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4680 2024-04-19 21:08:39.565002 sphinx_intl-2.2.0/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1616 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/README.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2024-04-19 20:57:59.000000 sphinx_intl-2.2.0/checklist.rst
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-19 21:08:39.557002 sphinx_intl-2.2.0/doc/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/doc/.gitignore
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      608 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/doc/Makefile
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       29 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/doc/authors.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1108 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/doc/basic.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       29 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/doc/changes.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      820 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/doc/conf.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1448 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/doc/dev.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1569 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/doc/index.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      779 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/doc/make.bat
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7791 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/doc/quickstart.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1177 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/doc/refs.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/doc/requirements.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1738 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       49 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/requirements-dev.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       27 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/requirements-testing.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      131 2024-04-19 21:08:39.565002 sphinx_intl-2.2.0/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-19 21:08:39.561002 sphinx_intl-2.2.0/sphinx_intl/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       47 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/sphinx_intl/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/sphinx_intl/__main__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5176 2024-04-19 20:22:54.000000 sphinx_intl-2.2.0/sphinx_intl/basic.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2615 2024-04-19 20:22:54.000000 sphinx_intl-2.2.0/sphinx_intl/catalog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9622 2024-04-19 20:22:54.000000 sphinx_intl-2.2.0/sphinx_intl/commands.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2024 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/sphinx_intl/pycompat.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      579 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/sphinx_intl/sphinx_util.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5471 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/sphinx_intl/transifex.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-19 21:08:39.565002 sphinx_intl-2.2.0/sphinx_intl.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4680 2024-04-19 21:08:39.000000 sphinx_intl-2.2.0/sphinx_intl.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      916 2024-04-19 21:08:39.000000 sphinx_intl-2.2.0/sphinx_intl.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 21:08:39.000000 sphinx_intl-2.2.0/sphinx_intl.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2024-04-19 21:08:39.000000 sphinx_intl-2.2.0/sphinx_intl.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 20:58:05.000000 sphinx_intl-2.2.0/sphinx_intl.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2024-04-19 21:08:39.000000 sphinx_intl-2.2.0/sphinx_intl.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       12 2024-04-19 21:08:39.000000 sphinx_intl-2.2.0/sphinx_intl.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-19 21:08:39.565002 sphinx_intl-2.2.0/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2782 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/tests/test_basic.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1258 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/tests/test_catalog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5742 2024-04-19 20:22:54.000000 sphinx_intl-2.2.0/tests/test_cmd_pot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7107 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/tests/test_cmd_transifex.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4124 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/tests/test_transifex.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      599 2024-04-19 20:07:15.000000 sphinx_intl-2.2.0/tox.ini
```

### Comparing `sphinx-intl-2.1.0/LICENSE` & `sphinx_intl-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-intl-2.1.0/README.rst` & `sphinx_intl-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx-intl-2.1.0/checklist.rst` & `sphinx_intl-2.2.0/checklist.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. release procedure
 
 Procedure:
 
 1. check GitHub Actions test results: https://github.com/sphinx-doc/sphinx-intl/actions
 2. update release version/date in ``CHANGES.rst``
-3. ``python setup.py release sdist bdist_egg``
+3. ``python -m build``, see details: setup.cfg
 4. ``twine upload dist/<target-package-file>``
 5. check PyPI page: https://pypi.org/p/sphinx-intl
 6. tagging with version name that MUST following semver. e.g.: ``git tag 1.0.1``
 7. ``git push --tags`` to push tag
 8. bump version in ``sphinx_intl/__init__.py`` and ``CHANGES.rst`` then commit/push
    them onto GitHub
```

### Comparing `sphinx-intl-2.1.0/doc/Makefile` & `sphinx_intl-2.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx-intl-2.1.0/doc/basic.rst` & `sphinx_intl-2.2.0/doc/basic.rst`

 * *Files 11% similar despite different names*

```diff
@@ -34,9 +34,9 @@
 =============
 
 It is strongly recommended to use virtualenv/venv for this procedure::
 
    $ pip install sphinx-intl
 
 If you want to use `Optional Features`_, you need install Transifex CLI tool.
-Please refer to `Installation instructions <https://github.com/transifex/cli#installation>`.
+Please refer to `Installation instructions <https://github.com/transifex/cli#installation>`_.
```

### Comparing `sphinx-intl-2.1.0/doc/conf.py` & `sphinx_intl-2.2.0/doc/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 author = 'Sphinx team'
 
 version = release = __version__
 
 # -- General configuration ---------------------------------------------------
 
 extensions = [
+    "sphinx_click",
 ]
 
 source_suffix = '.rst'
 master_doc = 'index'
-language = None
+language = 'en'
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 pygments_style = 'sphinx'
 
 
 # -- Options for HTML output -------------------------------------------------
 
 html_theme = 'sphinx_rtd_theme'
```

### Comparing `sphinx-intl-2.1.0/doc/dev.rst` & `sphinx_intl-2.2.0/doc/dev.rst`

 * *Files identical despite different names*

### Comparing `sphinx-intl-2.1.0/doc/index.rst` & `sphinx_intl-2.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-intl-2.1.0/doc/make.bat` & `sphinx_intl-2.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sphinx-intl-2.1.0/doc/quickstart.rst` & `sphinx_intl-2.2.0/doc/quickstart.rst`

 * *Files identical despite different names*

### Comparing `sphinx-intl-2.1.0/doc/refs.rst` & `sphinx_intl-2.2.0/doc/refs.rst`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,24 @@
    :local:
 
 Commands
 ========
 
 Type `sphinx-intl` without arguments, options to show command help.
 
+.. click:: sphinx_intl.commands:main
+   :prog: sphinx-intl
+   :nested: full
+
 
 Environment Variables
 =====================
 
 All command-line options can be set with environment variables using the
-format SPHINXINTL_<UPPER_LONG_NAME> . Dashes (-) have to be replaced with
+format ``SPHINXINTL_<UPPER_LONG_NAME>``. Dashes (-) have to be replaced with
 underscores (_).
 
 For example, to set the languages::
 
    export SPHINXINTL_LANGUAGE=de,ja
 
 This is the same as passing the option to sphinx-intl directly::
```

### Comparing `sphinx-intl-2.1.0/sphinx_intl/basic.py` & `sphinx_intl-2.2.0/sphinx_intl/basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,23 @@
             if os.path.isdir(d) and not d.endswith('pot')]
     return (tuple(dirs),)
 
 
 # ==================================
 # commands
 
-def update(locale_dir, pot_dir, languages, line_width=76):
+def update(locale_dir, pot_dir, languages, line_width=76, ignore_obsolete=False):
     """
     Update specified language's po files from pot.
 
     :param unicode locale_dir: path for locale directory
     :param unicode pot_dir: path for pot directory
     :param tuple languages: languages to update po files
-    :param number line_width: maximum line wdith of po files
+    :param number line_width: maximum line width of po files
+    :param bool ignore_obsolete: ignore obsolete entries in po files
     :return: {'create': 0, 'update': 0, 'notchanged': 0}
     :rtype: dict
     """
     status = {
         'create': 0,
         'update': 0,
         'notchanged': 0,
@@ -57,23 +58,25 @@
                     new_msgids = set([m.id for m in cat if m.id])
                     if msgids != new_msgids:
                         added = new_msgids - msgids
                         deleted = msgids - new_msgids
                         status['update'] += 1
                         click.echo('Update: {0} +{1}, -{2}'.format(
                             po_file, len(added), len(deleted)))
-                        c.dump_po(po_file, cat, line_width)
+                        c.dump_po(po_file, cat, width=line_width,
+                                  ignore_obsolete=ignore_obsolete)
                     else:
                         status['notchanged'] += 1
                         click.echo('Not Changed: {0}'.format(po_file))
                 else:  # new po file
                     status['create'] += 1
                     click.echo('Create: {0}'.format(po_file))
                     cat_pot.locale = lang
-                    c.dump_po(po_file, cat_pot, line_width)
+                    c.dump_po(po_file, cat_pot, width=line_width,
+                              ignore_obsolete=ignore_obsolete)
 
     return status
 
 
 def build(locale_dir, output_dir, languages):
     """
     Build specified language's po files into mo.
```

### Comparing `sphinx-intl-2.1.0/sphinx_intl/catalog.py` & `sphinx_intl-2.2.0/sphinx_intl/catalog.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,60 +2,70 @@
 
 import os
 import io
 
 from babel.messages import pofile, mofile
 
 
-def load_po(filename):
+def load_po(filename, **kwargs):
     """read po/pot file and return catalog object
 
     :param unicode filename: path to po/pot file
+    :param kwargs: keyword arguments to forward to babel's read_po call
     :return: catalog object
     """
     # pre-read to get charset
     with io.open(filename, 'rb') as f:
         cat = pofile.read_po(f)
     charset = cat.charset or 'utf-8'
 
     # To decode lines by babel, read po file as binary mode and specify charset for
     # read_po function.
     with io.open(filename, 'rb') as f:  # FIXME: encoding VS charset
-        return pofile.read_po(f, charset=charset)
+        return pofile.read_po(f, charset=charset, **kwargs)
 
 
-def dump_po(filename, catalog, line_width=76):
+def dump_po(filename, catalog, **kwargs):
     """write po/pot file from catalog object
 
     :param unicode filename: path to po file
     :param catalog: catalog object
-    :param line_width: maximum line wdith of po files
+    :param kwargs: keyword arguments to forward to babel's write_po call; also
+                    accepts a deprecated `line_width` option to forward to
+                    write_po's `width` option
     :return: None
     """
     dirname = os.path.dirname(filename)
     if not os.path.exists(dirname):
         os.makedirs(dirname)
 
+    # (compatibility) line_width was the original argument used to forward
+    # line width hints into write_po's `width` argument; if provided,
+    # set/override the width value
+    if 'line_width' in kwargs:
+        kwargs['width'] = kwargs['line_width']
+        del kwargs['line_width']
+
     # Because babel automatically encode strings, file should be open as binary mode.
     with io.open(filename, 'wb') as f:
-        pofile.write_po(f, catalog, line_width)
+        pofile.write_po(f, catalog, **kwargs)
 
 
-def write_mo(filename, catalog):
+def write_mo(filename, catalog, **kwargs):
     """write mo file from catalog object
 
     :param unicode filename: path to mo file
     :param catalog: catalog object
     :return: None
     """
     dirname = os.path.dirname(filename)
     if not os.path.exists(dirname):
         os.makedirs(dirname)
     with io.open(filename, 'wb') as f:
-        mofile.write_mo(f, catalog)
+        mofile.write_mo(f, catalog, **kwargs)
 
 
 def translated_entries(catalog):
     return [m for m in catalog if m.id and m.string]
 
 
 def fuzzy_entries(catalog):
```

### Comparing `sphinx-intl-2.1.0/sphinx_intl/commands.py` & `sphinx_intl-2.2.0/sphinx_intl/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Sphinx utility that make it easy to translate and to apply translation.
 
     :copyright: Copyright 2019 by Takayuki SHIMIZUKAWA.
     :license: BSD, see LICENSE for details.
 """
 import re
 import os
+import warnings
 from glob import glob
 
 import click
 from sphinx.util.tags import Tags
 
 from . import basic
 from . import transifex
@@ -107,38 +108,44 @@
     metavar='<DIR>', show_default=True,
     help="mo files directory where files are written. "
          "Default is to match the '--locale-dir' path.")
 
 option_tag = click.option(
     '-t', '--tag',
     envvar=ENVVAR_PREFIX + '_TAG',
-    type=TAGS, default=(), metavar='<TAG>', show_default=True,
+    type=TAGS, metavar='<TAG>', show_default=True,
     multiple=True,
     help="Pass tags to conf.py, as same as passed to sphinx-build -t option.")
 
 option_language = click.option(
     '-l', '--language',
     envvar=ENVVAR_PREFIX + '_LANGUAGE',
-    type=LANGUAGES, default=(), metavar='<LANG>', show_default=True,
+    type=LANGUAGES, metavar='<LANG>', show_default=True,
     multiple=True,
     help="Target language to update po files. Default is ALL.")
 
 option_line_width = click.option(
     '-w', '--line-width',
     envvar=ENVVAR_PREFIX + '_LINE_WIDTH',
     type=int, default=76, metavar='<WIDTH>', show_default=True,
     multiple=False,
     help='The maximum line width for the po files, 0 or a negative number '
          'disable line wrapping')
 
+option_no_obsolete = click.option(
+    '--no-obsolete',
+    envvar=ENVVAR_PREFIX + '_NO_OBSOLETE',
+    is_flag=True, default=False,
+    help='Remove obsolete #~ messages.')
+
 option_transifex_token = click.option(
     '--transifex-token',
     envvar=ENVVAR_PREFIX + '_TRANSIFEX_TOKEN',
     type=str, metavar='<TOKEN>', required=True,
-    help="Your transifex token.")
+    help="Your transifex token. (DEPRECATED)")
 
 option_transifex_organization_name = click.option(
     '--transifex-organization-name',
     envvar=ENVVAR_PREFIX + '_TRANSIFEX_ORGANIZATION_NAME',
     type=str, metavar='<ORGANIZATION-NAME>', required=True,
     help="Your transifex organization name.")
 
@@ -157,28 +164,14 @@
     '-c', '--config',
     type=click.Path(exists=True, file_okay=True, dir_okay=False),
     default=None, metavar='<FILE>',
     help='Sphinx conf.py file to read a locale directory setting.')
 @option_tag
 @click.pass_context
 def main(ctx, config, tag):
-    """
-    Environment Variables:
-    All command-line options can be set with environment variables using the
-    format SPHINXINTL_<UPPER_LONG_NAME> . Dashes (-) have to replaced with
-        underscores (_).
-
-    For example, to set the languages:
-
-    export SPHINXINTL_LANGUAGE=de,ja
-
-    This is the same as passing the option to txutil directly:
-
-    sphinx-intl update --language=de --language=ja
-    """
     # load conf.py
     ctx.config = config
     if ctx.config is None:
         for c in ('conf.py', 'source/conf.py'):
             if os.path.exists(c):
                 ctx.config = c
                 break
@@ -230,15 +223,16 @@
 
 
 @main.command()
 @option_locale_dir
 @option_pot_dir
 @option_language
 @option_line_width
-def update(locale_dir, pot_dir, language, line_width):
+@option_no_obsolete
+def update(locale_dir, pot_dir, language, line_width, no_obsolete):
     """
     Update specified language's po files from pot.
 
     \b
     For examples:
        sphinx-intl update -l de -l ja
        sphinx-intl update -l de,ja
@@ -256,15 +250,15 @@
     if not languages:
         msg = ("No languages are found. Please specify language with -l "
                "option, or preparing language directories under %(locale_dir)r "
                "directory."
                % locals())
         raise click.BadParameter(msg, param_hint='language')
 
-    basic.update(locale_dir, pot_dir, languages, line_width)
+    basic.update(locale_dir, pot_dir, languages, line_width, ignore_obsolete=no_obsolete)
 
 
 @main.command()
 @option_locale_dir
 @option_output_dir
 @option_language
 def build(locale_dir, output_dir, language):
@@ -296,16 +290,24 @@
     basic.stat(locale_dir, languages)
 
 
 @main.command('create-transifexrc')
 @option_transifex_token
 def create_transifexrc(transifex_token):
     """
-    Create `$HOME/.transifexrc`
+    Create `$HOME/.transifexrc`  (deprecated)
     """
+    warnings.filterwarnings("default", category=DeprecationWarning)
+    warnings.warn(
+        (
+            "create-transifexrc command and SPHINXINTL_TRANSIFEX_TOKEN "
+            "will be deprecated. Please use TX_TOKEN environment variable instead."
+        ),
+        category=DeprecationWarning,
+    )
     transifex.create_transifexrc(transifex_token)
 
 
 @main.command('create-txconfig')
 def create_txconfig():
     """
     Create `./.tx/config`
```

### Comparing `sphinx-intl-2.1.0/sphinx_intl/pycompat.py` & `sphinx_intl-2.2.0/sphinx_intl/pycompat.py`

 * *Files identical despite different names*

### Comparing `sphinx-intl-2.1.0/sphinx_intl/sphinx_util.py` & `sphinx_intl-2.2.0/sphinx_intl/sphinx_util.py`

 * *Files identical despite different names*

### Comparing `sphinx-intl-2.1.0/sphinx_intl/transifex.py` & `sphinx_intl-2.2.0/sphinx_intl/transifex.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 IGNORED_RESOURCE_NAMES = (
     'glossary',
     'settings',
 )
 
 TRANSIFEXRC_TEMPLATE = """\
 [https://www.transifex.com]
-rest_hostname = https://www.transifex.com
+rest_hostname = https://rest.api.transifex.com
 token = %(transifex_token)s
 """
 
 TXCONFIG_TEMPLATE = """\
 [main]
 host = https://www.transifex.com
 """
@@ -149,15 +149,16 @@
     check_transifex_cli_installed()
 
     cmd_tmpl = (
         'tx',
         'add',
         '--organization', '%(transifex_organization_name)s',
         '--project', '%(transifex_project_name)s',
-        '--resource', '%(resource_name)s',
+        '--resource', '%(resource_slug)s',
+        '--resource-name', '%(resource_name)s',
         '--file-filter', '%(locale_dir)s/<lang>/LC_MESSAGES/%(resource_path)s.po',
         '--type', 'PO',
         '%(pot_dir)s/%(resource_path)s.pot',
     )
 
     # convert transifex_project_name to internal name
     transifex_project_name = transifex_project_name.replace(' ', '-')
@@ -170,15 +171,15 @@
         length=len(pot_paths),
         color="green",
         label="adding pots...",
         item_show_func=lambda p: str(p),
     ) as progress_bar:
         for pot_path in progress_bar:
             resource_path = str(pot_path.relative_to(pot_dir).with_suffix(''))
-            resource_name = normalize_resource_name(resource_path)
+            resource_slug = resource_name = normalize_resource_name(resource_path)
             pot = load_po(str(pot_path))
             if len(pot):
                 lv = locals()
                 cmd = [arg % lv for arg in cmd_tmpl]
                 subprocess.check_output(cmd, shell=False)
             else:
                 click.echo('{0} is empty, skipped'.format(pot_path))
```

