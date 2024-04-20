# Comparing `tmp/tendril-filestore-0.4.0.tar.gz` & `tmp/tendril_filestore-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-filestore-0.4.0.tar", last modified: Wed Apr  3 16:34:09 2024, max compression
+gzip compressed data, was "tendril_filestore-0.4.1.tar", last modified: Sat Apr 20 00:03:55 2024, max compression
```

## Comparing `tendril-filestore-0.4.0.tar` & `tendril_filestore-0.4.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.897122 tendril-filestore-0.4.0/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.897122 tendril-filestore-0.4.0/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.897122 tendril-filestore-0.4.0/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      943 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3306 2023-04-20 19:33:00.000000 tendril-filestore-0.4.0/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.893123 tendril-filestore-0.4.0/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.4.0/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.4.0/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7640 2023-07-01 18:41:32.000000 tendril-filestore-0.4.0/src/tendril/apiserver/routers/filestore.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril-filestore-0.4.0/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:03:32.000000 tendril-filestore-0.4.0/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      264 2023-03-27 15:39:22.000000 tendril-filestore-0.4.0/src/tendril/authz/scopes/filestore.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-19 12:09:04.000000 tendril-filestore-0.4.0/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/common/filestore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-19 11:58:32.000000 tendril-filestore-0.4.0/src/tendril/common/filestore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1369 2023-07-22 08:36:30.000000 tendril-filestore-0.4.0/src/tendril/common/filestore/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3744 2023-04-20 12:32:50.000000 tendril-filestore-0.4.0/src/tendril/config/filestore.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3611 2023-07-01 18:41:32.000000 tendril-filestore-0.4.0/src/tendril/config/filestore_core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/src/tendril/filestore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 21:59:13.000000 tendril-filestore-0.4.0/src/tendril/filestore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7922 2024-04-03 11:20:56.000000 tendril-filestore-0.4.0/src/tendril/filestore/actual.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3288 2024-04-03 11:20:56.000000 tendril-filestore-0.4.0/src/tendril/filestore/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2964 2023-09-12 18:19:51.000000 tendril-filestore-0.4.0/src/tendril/filestore/buckets.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/src/tendril/filestore/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 17:57:19.000000 tendril-filestore-0.4.0/src/tendril/filestore/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7178 2024-04-03 11:20:56.000000 tendril-filestore-0.4.0/src/tendril/filestore/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1770 2023-07-01 00:16:52.000000 tendril-filestore-0.4.0/src/tendril/filestore/db/model.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3474 2023-09-12 18:24:26.000000 tendril-filestore-0.4.0/src/tendril/filestore/remote.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/src/tendril_filestore.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2024-04-03 16:34:09.000000 tendril-filestore-0.4.0/src/tendril_filestore.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1362 2024-04-03 16:34:09.000000 tendril-filestore-0.4.0/src/tendril_filestore.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-03 16:34:09.000000 tendril-filestore-0.4.0/src/tendril_filestore.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      603 2024-04-03 16:34:09.000000 tendril-filestore-0.4.0/src/tendril_filestore.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-03 16:34:09.000000 tendril-filestore-0.4.0/src/tendril_filestore.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.820236 tendril_filestore-0.4.1/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5476 2024-04-20 00:03:55.820236 tendril_filestore-0.4.1/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.800236 tendril_filestore-0.4.1/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.804236 tendril_filestore-0.4.1/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.804236 tendril_filestore-0.4.1/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.804236 tendril_filestore-0.4.1/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      943 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.804236 tendril_filestore-0.4.1/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-20 00:03:55.820236 tendril_filestore-0.4.1/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3306 2023-04-20 19:33:00.000000 tendril_filestore-0.4.1/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.796236 tendril_filestore-0.4.1/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.804236 tendril_filestore-0.4.1/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.808236 tendril_filestore-0.4.1/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril_filestore-0.4.1/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.808236 tendril_filestore-0.4.1/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril_filestore-0.4.1/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7690 2024-04-19 23:33:23.000000 tendril_filestore-0.4.1/src/tendril/apiserver/routers/filestore.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.808236 tendril_filestore-0.4.1/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril_filestore-0.4.1/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.808236 tendril_filestore-0.4.1/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:03:32.000000 tendril_filestore-0.4.1/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      264 2023-03-27 15:39:22.000000 tendril_filestore-0.4.1/src/tendril/authz/scopes/filestore.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.808236 tendril_filestore-0.4.1/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-19 12:09:04.000000 tendril_filestore-0.4.1/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.808236 tendril_filestore-0.4.1/src/tendril/common/filestore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-19 11:58:32.000000 tendril_filestore-0.4.1/src/tendril/common/filestore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1369 2023-07-22 08:36:30.000000 tendril_filestore-0.4.1/src/tendril/common/filestore/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.812236 tendril_filestore-0.4.1/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3744 2023-04-20 12:32:50.000000 tendril_filestore-0.4.1/src/tendril/config/filestore.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3611 2023-07-01 18:41:32.000000 tendril_filestore-0.4.1/src/tendril/config/filestore_core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.812236 tendril_filestore-0.4.1/src/tendril/filestore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 21:59:13.000000 tendril_filestore-0.4.1/src/tendril/filestore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7981 2024-04-19 23:33:23.000000 tendril_filestore-0.4.1/src/tendril/filestore/actual.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3315 2024-04-19 23:33:23.000000 tendril_filestore-0.4.1/src/tendril/filestore/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2964 2023-09-12 18:19:51.000000 tendril_filestore-0.4.1/src/tendril/filestore/buckets.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.812236 tendril_filestore-0.4.1/src/tendril/filestore/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 17:57:19.000000 tendril_filestore-0.4.1/src/tendril/filestore/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7240 2024-04-19 23:33:23.000000 tendril_filestore-0.4.1/src/tendril/filestore/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1770 2023-07-01 00:16:52.000000 tendril_filestore-0.4.1/src/tendril/filestore/db/model.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3540 2024-04-19 23:33:23.000000 tendril_filestore-0.4.1/src/tendril/filestore/remote.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.816236 tendril_filestore-0.4.1/src/tendril_filestore.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5476 2024-04-20 00:03:55.000000 tendril_filestore-0.4.1/src/tendril_filestore.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1362 2024-04-20 00:03:55.000000 tendril_filestore-0.4.1/src/tendril_filestore.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-20 00:03:55.000000 tendril_filestore-0.4.1/src/tendril_filestore.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      603 2024-04-20 00:03:55.000000 tendril_filestore-0.4.1/src/tendril_filestore.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-20 00:03:55.000000 tendril_filestore-0.4.1/src/tendril_filestore.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:03:55.816236 tendril_filestore-0.4.1/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-08 18:25:43.000000 tendril_filestore-0.4.1/tox.ini
```

### Comparing `tendril-filestore-0.4.0/.gitignore` & `tendril_filestore-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/.readthedocs.yml` & `tendril_filestore-0.4.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/.travis.yml` & `tendril_filestore-0.4.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/LICENSE` & `tendril_filestore-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/README.rst` & `tendril_filestore-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/docs/Makefile` & `tendril_filestore-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/docs/_static/custom.css` & `tendril_filestore-0.4.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/docs/_static/favicon.ico` & `tendril_filestore-0.4.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/docs/_static/logo.png` & `tendril_filestore-0.4.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/docs/_static/logo_packed.png` & `tendril_filestore-0.4.1/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/docs/_templates/about.html` & `tendril_filestore-0.4.1/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/docs/conf.py` & `tendril_filestore-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/docs/index.rst` & `tendril_filestore-0.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/docs/installation.rst` & `tendril_filestore-0.4.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/setup.py` & `tendril_filestore-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/src/tendril/apiserver/routers/filestore.py` & `tendril_filestore-0.4.1/src/tendril/apiserver/routers/filestore.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 async def upload_file_to_bucket(
         request: Request,
         bucket: BucketName,
         overwrite: bool = False,
         actual_user: Optional[UserReferenceTModel] = None,
         file: UploadFile = File(...),
         interest: Optional[int] = None,
+        label: Optional[str] = None,
         user: AuthUserModel = auth_spec()):
 
     try:
         bucket: FilestoreBucket = get_bucket(bucket)
     except KeyError:
         logger.info(f"Got upload request with bad bucket '{bucket}' ({file.filename})")
         raise HTTPException(
@@ -77,15 +78,15 @@
         raise HTTPException(
             status_code=415,
             detail=f"This bucket does not allow uploads with this extension"
         )
 
     try:
         actual_user = actual_user or user.id
-        sf = bucket.upload(file, actual_user, interest=interest, overwrite=overwrite)
+        sf = bucket.upload(file, actual_user, interest=interest, label=label, overwrite=overwrite)
     except FileExistsError as e:
         logger.info(e)
         raise HTTPException(
             status_code=409,
             detail=str(e)
         )
```

### Comparing `tendril-filestore-0.4.0/src/tendril/common/filestore/formats.py` & `tendril_filestore-0.4.1/src/tendril/common/filestore/formats.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/src/tendril/config/__init__.py` & `tendril_filestore-0.4.1/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/src/tendril/config/filestore.py` & `tendril_filestore-0.4.1/src/tendril/config/filestore.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/src/tendril/config/filestore_core.py` & `tendril_filestore-0.4.1/src/tendril/config/filestore_core.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/src/tendril/filestore/actual.py` & `tendril_filestore-0.4.1/src/tendril/filestore/actual.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                     # Exisiting file is owned by someone else.
                     raise FileExistsError(f'{filename} already exists in the {bucket.name} bucket '
                                       f'and owned by someone else.')
                 logger.warning(f"Overwriting file {filename} in bucket {bucket.name}.")
                 bucket.delete(filename, user, interest, session=session)
 
     @with_db
-    def upload(self, file, user, interest=None, overwrite=False, session=None):
+    def upload(self, file, user, interest=None, label=None, overwrite=False, session=None):
         filename = file.filename
         self._prep_for_upload(self, filename, user, interest, overwrite, session=session)
 
         with self._fs.open(filename, 'wb') as target:
             logger.debug(f"Writing file {filename} to bucket {self.name}")
             target.write(file.file.read())
 
@@ -118,15 +118,16 @@
             if not chunk: break
             sha256hash.update(chunk)
 
         fileinfo = {'props': {'size': info.size, 'created': created, 'modified': modified},
                     'hash': {'sha256': sha256hash.hexdigest()},
                     'ext': ''.join(info.suffixes)}
 
-        sf = register_stored_file(filename, self._id, user, interest, fileinfo, session=session)
+        sf = register_stored_file(filename, self._id, user, interest, fileinfo,
+                                  label=label, session=session)
 
         return sf
 
     @with_db
     def move(self, filename, target_bucket, user, overwrite=False, session=None):
         if not self._fs.exists(filename):
             raise FileNotFoundError(f"Move of nonexisting file {filename} "
```

### Comparing `tendril-filestore-0.4.0/src/tendril/filestore/base.py` & `tendril_filestore-0.4.1/src/tendril/filestore/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def accept_ext(self):
         return self._accept_ext
 
     def check_accepts(self, filename):
         name, ext = os.path.splitext(filename)
         return ext in self._accept_ext
 
-    def upload(self, file, user, overwrite=False):
+    def upload(self, file, user, interest=None, label=None, overwrite=False):
         raise NotImplementedError
 
     def move(self, filename, target_bucket, user, overwrite=False):
         raise NotImplementedError
 
     def list(self, page=None):
         raise NotImplementedError
```

### Comparing `tendril-filestore-0.4.0/src/tendril/filestore/buckets.py` & `tendril_filestore-0.4.1/src/tendril/filestore/buckets.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/src/tendril/filestore/db/controller.py` & `tendril_filestore-0.4.1/src/tendril/filestore/db/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                                             include_owner=include_owner))
     else:
         return _stored_file_transformer(session.execute(stmt).all(),
                                         include_owner=include_owner)
 
 
 @with_db
-def register_stored_file(filename, bucket, user, interest=None, fileinfo=None, overwrite=True, session=None):
+def register_stored_file(filename, bucket, user, interest=None, fileinfo=None, overwrite=True, label=None, session=None):
     if not config.FILESTORE_ENABLED:
         raise EnvironmentError("Filestore not enabled on this component. "
                                "Use the filestore API on the filestore component instead.")
 
     if filename is None:
         raise AttributeError("name cannot be None")
 
@@ -153,15 +153,16 @@
         existing = get_stored_file(filename=filename, bucket=bucket_id, session=session)
     except NoResultFound:
         storedfile = StoredFileModel(filename=filename,
                                      bucket_id=bucket_id,
                                      fileinfo=fileinfo,
                                      user_id=user_id,
                                      interest_id=interest_id,
-                                     type='stored_file')
+                                     type='stored_file',
+                                     label=label)
         # TODO Create Log Entry?
     else:
         if not overwrite:
             raise ValueError(f"File {filename} seems to already exist in bucket "
                              f"{bucket_id}. For now, you might have to manually "
                              f"delete it from the database if this is something "
                              f"you really want to do.")
```

### Comparing `tendril-filestore-0.4.0/src/tendril/filestore/db/model.py` & `tendril_filestore-0.4.1/src/tendril/filestore/db/model.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/src/tendril/filestore/remote.py` & `tendril_filestore-0.4.1/src/tendril/filestore/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,20 +40,22 @@
     def _async_http_client_args(self):
         return {
             'base_url': self.uri,
             'auth': _authenticator
         }
 
     @with_async_client_cl()
-    async def upload(self, file, actual_user=None, interest=None, overwrite=False, client=None):
+    async def upload(self, file, actual_user=None, interest=None, label=None, overwrite=False, client=None):
         params = {}
         if actual_user:
             params['actual_user'] = actual_user
         if interest:
             params['interest'] = interest
+        if label:
+            params['label'] = label
         response = await client.post(f'/v1/filestore/{self.name}/upload',
                                      files={'file': file}, params=params)
         response.raise_for_status()
         return response.json()
 
     @with_async_client_cl()
     async def move(self, filename, target_bucket, actual_user=None, overwrite=False, client=None):
```

### Comparing `tendril-filestore-0.4.0/src/tendril_filestore.egg-info/SOURCES.txt` & `tendril_filestore-0.4.1/src/tendril_filestore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/src/tendril_filestore.egg-info/requires.txt` & `tendril_filestore-0.4.1/src/tendril_filestore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/tests/coveralls.py` & `tendril_filestore-0.4.1/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.4.0/tox.ini` & `tendril_filestore-0.4.1/tox.ini`

 * *Files identical despite different names*

