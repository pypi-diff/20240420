# Comparing `tmp/devpi-web-4.2.1.tar.gz` & `tmp/devpi_web-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devpi-web-4.2.1.tar", last modified: Sun Jul  2 12:03:58 2023, max compression
+gzip compressed data, was "devpi_web-4.2.2.tar", last modified: Sat Apr 20 06:42:42 2024, max compression
```

## Comparing `devpi-web-4.2.1.tar` & `devpi_web-4.2.2.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:03:58.274925 devpi-web-4.2.1/
--rw-r--r--   0 fschulze   (501) staff       (20)       80 2023-07-02 12:03:52.000000 devpi-web-4.2.1/AUTHORS
--rw-r--r--   0 fschulze   (501) staff       (20)    15164 2023-07-02 12:03:52.000000 devpi-web-4.2.1/CHANGELOG
--rw-r--r--   0 fschulze   (501) staff       (20)     1061 2023-07-02 12:03:52.000000 devpi-web-4.2.1/LICENSE
--rw-r--r--   0 fschulze   (501) staff       (20)      144 2023-07-02 12:03:52.000000 devpi-web-4.2.1/MANIFEST.in
--rw-r--r--   0 fschulze   (501) staff       (20)     4420 2023-07-02 12:03:58.275063 devpi-web-4.2.1/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)     1122 2023-07-02 12:03:52.000000 devpi-web-4.2.1/README.rst
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:03:58.262475 devpi-web-4.2.1/devpi_web/
--rw-r--r--   0 fschulze   (501) staff       (20)       22 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1575 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/clear_index.py
--rw-r--r--   0 fschulze   (501) staff       (20)      723 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/config.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2921 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/description.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8125 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/doczip.py
--rw-r--r--   0 fschulze   (501) staff       (20)      785 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/hookspecs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3568 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/indexing.py
--rw-r--r--   0 fschulze   (501) staff       (20)    12923 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/main.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1940 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/null_index.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:03:58.266169 devpi-web-4.2.1/devpi_web/static/
--rw-r--r--   0 fschulze   (501) staff       (20)     1580 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/static/common.js
--rw-r--r--   0 fschulze   (501) staff       (20)     3477 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/static/docview.js
--rw-r--r--   0 fschulze   (501) staff       (20)    15086 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/static/favicon.ico
--rw-r--r--   0 fschulze   (501) staff       (20)    89501 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/static/jquery-3.6.0.min.js
--rw-r--r--   0 fschulze   (501) staff       (20)    10274 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/static/style.css
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:03:58.270973 devpi-web-4.2.1/devpi_web/templates/
--rw-r--r--   0 fschulze   (501) staff       (20)     1410 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/doc.pt
--rw-r--r--   0 fschulze   (501) staff       (20)      467 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/error.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     3600 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/index.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     4818 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/macros.pt
--rw-r--r--   0 fschulze   (501) staff       (20)      465 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/notfound.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     1838 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/project.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     1415 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/root.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     2237 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/search.pt
--rw-r--r--   0 fschulze   (501) staff       (20)      462 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/search_help.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     4719 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/status.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     1853 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/toxresult.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     2418 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/toxresults.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     1278 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/user.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     4934 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/version.pt
--rw-r--r--   0 fschulze   (501) staff       (20)    43032 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/views.py
--rw-r--r--   0 fschulze   (501) staff       (20)    36687 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/whoosh_index.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:03:58.264580 devpi-web-4.2.1/devpi_web.egg-info/
--rw-r--r--   0 fschulze   (501) staff       (20)     4420 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)     1376 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/SOURCES.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/dependency_links.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      257 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/entry_points.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/not-zip-safe
--rw-r--r--   0 fschulze   (501) staff       (20)      180 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/requires.txt
--rw-r--r--   0 fschulze   (501) staff       (20)       10 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/top_level.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      546 2023-07-02 12:03:52.000000 devpi-web-4.2.1/pyproject.toml
--rw-r--r--   0 fschulze   (501) staff       (20)       86 2023-07-02 12:03:58.275518 devpi-web-4.2.1/setup.cfg
--rw-r--r--   0 fschulze   (501) staff       (20)     2662 2023-07-02 12:03:52.000000 devpi-web-4.2.1/setup.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:03:58.274627 devpi-web-4.2.1/tests/
--rw-r--r--   0 fschulze   (501) staff       (20)     1732 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/conftest.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4002 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_indexing.py
--rw-r--r--   0 fschulze   (501) staff       (20)     6978 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_main.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1379 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_theme.py
--rw-r--r--   0 fschulze   (501) staff       (20)    30014 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_views.py
--rw-r--r--   0 fschulze   (501) staff       (20)    11471 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_views_docs.py
--rw-r--r--   0 fschulze   (501) staff       (20)    15385 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_views_misc.py
--rw-r--r--   0 fschulze   (501) staff       (20)    14095 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_views_search.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9459 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_views_toxresults.py
--rw-r--r--   0 fschulze   (501) staff       (20)    17960 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_whoosh_index.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1047 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tox.ini
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-04-20 06:42:42.923473 devpi_web-4.2.2/
+-rw-r--r--   0 fschulze   (501) staff       (20)       33 2024-03-04 07:22:59.000000 devpi_web-4.2.2/.flake8
+-rw-r--r--   0 fschulze   (501) staff       (20)       80 2016-09-12 10:26:20.000000 devpi_web-4.2.2/AUTHORS
+-rw-r--r--   0 fschulze   (501) staff       (20)    15570 2024-04-20 06:35:53.000000 devpi_web-4.2.2/CHANGELOG
+-rw-r--r--   0 fschulze   (501) staff       (20)     1061 2021-08-23 10:54:17.000000 devpi_web-4.2.2/LICENSE
+-rw-r--r--   0 fschulze   (501) staff       (20)      152 2024-04-11 06:42:42.000000 devpi_web-4.2.2/MANIFEST.in
+-rw-r--r--   0 fschulze   (501) staff       (20)     5020 2024-04-20 06:42:42.923336 devpi_web-4.2.2/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)     1122 2023-08-09 09:56:19.000000 devpi_web-4.2.2/README.rst
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-04-20 06:42:42.900643 devpi_web-4.2.2/devpi_web/
+-rw-r--r--   0 fschulze   (501) staff       (20)       22 2024-04-20 06:34:56.000000 devpi_web-4.2.2/devpi_web/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1722 2024-04-12 07:54:39.000000 devpi_web-4.2.2/devpi_web/clear_index.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      723 2023-11-20 15:47:49.000000 devpi_web-4.2.2/devpi_web/config.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2921 2023-11-26 07:11:18.000000 devpi_web-4.2.2/devpi_web/description.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8137 2024-04-11 06:42:42.000000 devpi_web-4.2.2/devpi_web/doczip.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      785 2021-08-23 10:54:17.000000 devpi_web-4.2.2/devpi_web/hookspecs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3568 2023-11-26 07:11:18.000000 devpi_web-4.2.2/devpi_web/indexing.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    12923 2023-11-26 07:11:18.000000 devpi_web-4.2.2/devpi_web/main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1940 2023-11-26 07:11:18.000000 devpi_web-4.2.2/devpi_web/null_index.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-04-20 06:42:42.908237 devpi_web-4.2.2/devpi_web/static/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1580 2023-11-20 15:47:49.000000 devpi_web-4.2.2/devpi_web/static/common.js
+-rw-r--r--   0 fschulze   (501) staff       (20)     3675 2024-04-10 10:06:05.000000 devpi_web-4.2.2/devpi_web/static/docview.js
+-rw-r--r--   0 fschulze   (501) staff       (20)    15086 2023-11-20 15:47:49.000000 devpi_web-4.2.2/devpi_web/static/favicon.ico
+-rw-r--r--   0 fschulze   (501) staff       (20)    89501 2023-11-20 15:47:49.000000 devpi_web-4.2.2/devpi_web/static/jquery-3.6.0.min.js
+-rw-r--r--   0 fschulze   (501) staff       (20)    15919 2022-10-16 13:46:35.000000 devpi_web-4.2.2/devpi_web/static/style-old.css
+-rw-r--r--   0 fschulze   (501) staff       (20)    10526 2024-04-10 10:06:05.000000 devpi_web-4.2.2/devpi_web/static/style.css
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-04-20 06:42:42.915347 devpi_web-4.2.2/devpi_web/templates/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1410 2023-11-20 15:47:49.000000 devpi_web-4.2.2/devpi_web/templates/doc.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)      467 2023-08-31 06:24:31.000000 devpi_web-4.2.2/devpi_web/templates/error.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     3600 2023-08-31 06:24:31.000000 devpi_web-4.2.2/devpi_web/templates/index.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     4818 2023-11-20 15:47:49.000000 devpi_web-4.2.2/devpi_web/templates/macros.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)      465 2023-08-31 06:24:31.000000 devpi_web-4.2.2/devpi_web/templates/notfound.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     1838 2023-11-20 15:47:49.000000 devpi_web-4.2.2/devpi_web/templates/project.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     1415 2023-08-31 06:24:31.000000 devpi_web-4.2.2/devpi_web/templates/root.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     2237 2023-08-31 06:24:31.000000 devpi_web-4.2.2/devpi_web/templates/search.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)      462 2023-08-31 06:24:31.000000 devpi_web-4.2.2/devpi_web/templates/search_help.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     4719 2023-08-31 06:24:31.000000 devpi_web-4.2.2/devpi_web/templates/status.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     1853 2023-08-31 06:24:31.000000 devpi_web-4.2.2/devpi_web/templates/toxresult.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     2418 2023-11-20 15:47:49.000000 devpi_web-4.2.2/devpi_web/templates/toxresults.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     1278 2023-08-31 06:24:31.000000 devpi_web-4.2.2/devpi_web/templates/user.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     4934 2023-11-20 15:47:49.000000 devpi_web-4.2.2/devpi_web/templates/version.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)    43001 2023-11-26 07:11:18.000000 devpi_web-4.2.2/devpi_web/views.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    36789 2024-04-16 11:43:32.000000 devpi_web-4.2.2/devpi_web/whoosh_index.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-04-20 06:42:42.922791 devpi_web-4.2.2/devpi_web.egg-info/
+-rw-r--r--   0 fschulze   (501) staff       (20)     5020 2024-04-20 06:42:42.000000 devpi_web-4.2.2/devpi_web.egg-info/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)     1415 2024-04-20 06:42:42.000000 devpi_web-4.2.2/devpi_web.egg-info/SOURCES.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2024-04-20 06:42:42.000000 devpi_web-4.2.2/devpi_web.egg-info/dependency_links.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      257 2024-04-20 06:42:42.000000 devpi_web-4.2.2/devpi_web.egg-info/entry_points.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2014-05-20 10:34:49.000000 devpi_web-4.2.2/devpi_web.egg-info/not-zip-safe
+-rw-r--r--   0 fschulze   (501) staff       (20)      180 2024-04-20 06:42:42.000000 devpi_web-4.2.2/devpi_web.egg-info/requires.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)       10 2024-04-20 06:42:42.000000 devpi_web-4.2.2/devpi_web.egg-info/top_level.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      546 2023-11-20 07:00:20.000000 devpi_web-4.2.2/pyproject.toml
+-rw-r--r--   0 fschulze   (501) staff       (20)       86 2024-04-20 06:42:42.925533 devpi_web-4.2.2/setup.cfg
+-rw-r--r--   0 fschulze   (501) staff       (20)     2667 2024-04-20 06:35:04.000000 devpi_web-4.2.2/setup.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-04-20 06:42:42.921803 devpi_web-4.2.2/tests/
+-rw-r--r--   0 fschulze   (501) staff       (20)     2156 2024-04-11 06:42:42.000000 devpi_web-4.2.2/tests/conftest.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4043 2024-04-16 11:43:32.000000 devpi_web-4.2.2/tests/test_indexing.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     7081 2024-04-16 11:43:32.000000 devpi_web-4.2.2/tests/test_main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1422 2024-03-04 07:22:59.000000 devpi_web-4.2.2/tests/test_theme.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    30055 2024-03-04 07:22:59.000000 devpi_web-4.2.2/tests/test_views.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    11534 2024-03-04 07:22:59.000000 devpi_web-4.2.2/tests/test_views_docs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    15413 2024-04-16 11:43:32.000000 devpi_web-4.2.2/tests/test_views_misc.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    14172 2024-04-16 11:43:32.000000 devpi_web-4.2.2/tests/test_views_search.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9532 2024-04-20 06:38:54.000000 devpi_web-4.2.2/tests/test_views_toxresults.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    18051 2024-04-14 15:50:25.000000 devpi_web-4.2.2/tests/test_whoosh_index.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1238 2024-04-20 06:38:54.000000 devpi_web-4.2.2/tox.ini
```

### Comparing `devpi-web-4.2.1/CHANGELOG` & `devpi_web-4.2.2/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 
 
 .. towncrier release notes start
 
+4.2.2 (2024-04-20)
+==================
+
+Bug Fixes
+---------
+
+- style.css: Always let content be full browser height. This also gives more height with some documentation themes when content is short.
+
+- style.css: set ``scrollbar-gutter: stable`` on ``body`` to prevent jumping content in documentation iframe.
+
+- Fix #970: overwrite fixed html/body heights like ``100%`` in documentation iframe content.
+
+
+
 4.2.1 (2023-07-02)
 ==================
 
 Bug Fixes
 ---------
 
 - Fix #953: Exception when browsers send ETag for documentation pages.
```

### Comparing `devpi-web-4.2.1/LICENSE` & `devpi_web-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/PKG-INFO` & `devpi_web-4.2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-web
-Version: 4.2.1
+Version: 4.2.2
 Summary: devpi-web: a web view for devpi-server
 Home-page: https://devpi.net
 Maintainer: Florian Schulze
 Maintainer-email: mail@pyfidelity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/devpi/devpi/issues
 Project-URL: Changelog, https://github.com/devpi/devpi/blob/main/web/CHANGELOG
@@ -23,17 +23,28 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.4
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: Whoosh<3
+Requires-Dist: beautifulsoup4!=4.12.1,>=4.3.2
+Requires-Dist: defusedxml
+Requires-Dist: devpi-server>=5.2.0
+Requires-Dist: devpi-common>=3.2.0
+Requires-Dist: docutils>=0.11
+Requires-Dist: pygments>=1.6
+Requires-Dist: pyramid!=1.10a1
+Requires-Dist: pyramid-chameleon
+Requires-Dist: readme-renderer[md]>=23.0
 
 ================================================
 devpi-web: web interface plugin for devpi-server
 ================================================
 
 This plugin adds a web interface with search for `devpi-server`_.
 
@@ -72,14 +83,28 @@
 Changelog
 =========
 
 
 
 .. towncrier release notes start
 
+4.2.2 (2024-04-20)
+==================
+
+Bug Fixes
+---------
+
+- style.css: Always let content be full browser height. This also gives more height with some documentation themes when content is short.
+
+- style.css: set ``scrollbar-gutter: stable`` on ``body`` to prevent jumping content in documentation iframe.
+
+- Fix #970: overwrite fixed html/body heights like ``100%`` in documentation iframe content.
+
+
+
 4.2.1 (2023-07-02)
 ==================
 
 Bug Fixes
 ---------
 
 - Fix #953: Exception when browsers send ETag for documentation pages.
@@ -140,16 +165,7 @@
 Bug Fixes
 ---------
 
 - Fix #880: explicitly register views for GET method, so there is a 404 on POSTs, like when using twine with wrong upload url.
 
 - Fix #867: AttributeError during ``devpi-import`` and maybe other commands.
 
-
-4.0.8 (2021-08-12)
-==================
-
-Bug Fixes
----------
-
-- On startup loop over mirror indexes last to avoid filling up the indexing queue, which processes non mirror indexes first.
-
```

### Comparing `devpi-web-4.2.1/README.rst` & `devpi_web-4.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/clear_index.py` & `devpi_web-4.2.2/devpi_web/clear_index.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         add_configfile_option(parser, pluginmanager)
         add_storage_options(parser, pluginmanager)
         add_indexer_backend_option(parser, pluginmanager)
         config = parseoptions(pluginmanager, argv, parser=parser)
         configure_cli_logging(config.args)
         xom = xom_from_config(config)
         log = xom.log
-        log.warn("You should stop devpi-server before running this command.")
+        log.warn(  # noqa: PGH002,G010 - this is actually TagLogger from devpi-server, but devpi-web still needs to support older devpi-server versions
+            "You should stop devpi-server before running this command.")
         ix = get_indexer(xom)
         ix.delete_index()
         log.info("Index deleted, start devpi-server again to let the index rebuild automatically.")
     except Fatal as e:
         tw = py.io.TerminalWriter(sys.stderr)
         tw.line("fatal: %s" % e.args[0], red=True)
         return 1
```

### Comparing `devpi-web-4.2.1/devpi_web/config.py` & `devpi_web-4.2.2/devpi_web/config.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/description.py` & `devpi_web-4.2.2/devpi_web/description.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/doczip.py` & `devpi_web-4.2.2/devpi_web/doczip.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from devpi_common.archive import Archive
 from devpi_common.types import cached_property
 from devpi_common.validation import normalize_name
 from devpi_server.log import threadlog
 try:
     import fcntl
 except ImportError:
-    fcntl = None  # type: ignore
+    fcntl = None  # type: ignore[assignment]
 import json
 import py
 
 
 def get_unpack_path(stage, name, version):
     path = stage.xom.config.args.documentation_path
     if path is None:
```

### Comparing `devpi-web-4.2.1/devpi_web/hookspecs.py` & `devpi_web-4.2.2/devpi_web/hookspecs.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/indexing.py` & `devpi_web-4.2.2/devpi_web/indexing.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/main.py` & `devpi_web-4.2.2/devpi_web/main.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/null_index.py` & `devpi_web-4.2.2/devpi_web/null_index.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/static/common.js` & `devpi_web-4.2.2/devpi_web/static/common.js`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/static/docview.js` & `devpi_web-4.2.2/devpi_web/static/docview.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -8,14 +8,15 @@
 }
 
 function onIFrameLoad(event) {
     var iframe = this,
         $iframe = $(iframe),
         $doc = $(iframe.contentWindow.document),
         $docHtml = $doc.find('html'),
+        $docBody = $docHtml.find('body'),
         scrolled_to_anchor = false,
         iframeResizeObserver = new ResizeObserver((entries) => {
             for (const entry of entries) {
                 if (entry.contentRect) {
                     const height = Math.ceil(entry.contentRect.height);
                     if (height) {
                         $iframe.height(height);
@@ -24,14 +25,18 @@
                             scrolled_to_anchor = true;
                         }
                     }
                 }
             }
         });
 
+    $docHtml.css('height', 'auto');
+    $docHtml.css('overflow-y', 'hidden');
+    $docBody.css('height', 'auto');
+    $docBody.css('overflow-y', 'hidden');
     // make keyboard actions affect the actual documentation
     // in the iframe by default
     iframe.contentWindow.focus();
     // watch for content size changes to update iframe height
     iframeResizeObserver.observe(iframe.contentWindow.document.body.parentElement);
 
     // fixup link target, so external links are opened outside the window
```

### Comparing `devpi-web-4.2.1/devpi_web/static/favicon.ico` & `devpi_web-4.2.2/devpi_web/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/static/jquery-3.6.0.min.js` & `devpi_web-4.2.2/devpi_web/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/static/style.css` & `devpi_web-4.2.2/devpi_web/static/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,25 @@
     color: black;
     font-family: sans-serif;
     font-size: 16px;
     margin: 0;
     padding: 0;
 }
 
+html {
+    height: 100%;
+}
+
+body {
+    min-height: 100%;
+    display: flex;
+    flex-direction: column;
+    scrollbar-gutter: stable;
+}
+
 pre, table {
     font-size: inherit;
 }
 
 table td {
     line-height: 1.25em;
 }
@@ -19,14 +30,18 @@
     text-decoration: none;
 }
 
 a:hover {
     text-decoration: underline;
 }
 
+#content {
+    flex: auto;
+}
+
 form, #content, #navigation, .searchresults {
     position: relative;
     margin: 0 1em;
 }
 
 .header {
     position: relative;
@@ -541,18 +556,24 @@
 .toxresult pre {
     margin-left: 1.5em;
     white-space: pre-wrap;
     overflow: scroll;
 }
 
 div.iframe {
+    flex: auto;
     margin: 0;
+    display: flex;
+}
+
+div.iframe iframe {
+    flex: auto;
 }
 
-div.iframe, iframe {
+div.iframe, div.iframe iframe {
     width: 100%;
     border: 0;
 }
 
 table .file_history {
     list-style: none;
     margin: 0;
```

### Comparing `devpi-web-4.2.1/devpi_web/templates/doc.pt` & `devpi_web-4.2.2/devpi_web/templates/doc.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/templates/index.pt` & `devpi_web-4.2.2/devpi_web/templates/index.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/templates/macros.pt` & `devpi_web-4.2.2/devpi_web/templates/macros.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/templates/project.pt` & `devpi_web-4.2.2/devpi_web/templates/project.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/templates/root.pt` & `devpi_web-4.2.2/devpi_web/templates/root.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/templates/search.pt` & `devpi_web-4.2.2/devpi_web/templates/search.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/templates/status.pt` & `devpi_web-4.2.2/devpi_web/templates/status.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/templates/toxresult.pt` & `devpi_web-4.2.2/devpi_web/templates/toxresult.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/templates/toxresults.pt` & `devpi_web-4.2.2/devpi_web/templates/toxresults.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/templates/user.pt` & `devpi_web-4.2.2/devpi_web/templates/user.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/templates/version.pt` & `devpi_web-4.2.2/devpi_web/templates/version.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/devpi_web/views.py` & `devpi_web-4.2.2/devpi_web/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         version_links.append(dict(
             title="Latest documentation",
             url=request.route_url(
                 "docviewroot", user=stage.user.name, index=stage.index,
                 project=name, version='latest', relpath="index.html")))
     try:
         stable_doc_info = get_doc_info(context, request, version='stable', check_content=False)
-        if stable_doc_info['doc_version'] != doc_info['doc_version'] and stable_doc_info['doc_version'] != latest_doc_info['doc_version']:
+        if stable_doc_info['doc_version'] not in (doc_info['doc_version'], latest_doc_info['doc_version']):
             version_links.append(dict(
                 title="Stable documentation",
                 url=request.route_url(
                     "docviewroot", user=stage.user.name, index=stage.index,
                     project=name, version='stable', relpath="index.html")))
     except (HTTPFound, HTTPNotFound):
         pass
```

### Comparing `devpi-web-4.2.1/devpi_web/whoosh_index.py` & `devpi_web-4.2.2/devpi_web/whoosh_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,15 +510,19 @@
     def runtime_setup(self, xom):
         self.xom = xom
         self.indexer_thread = setup_thread(xom)
         self.shared_data = self.indexer_thread.shared_data
 
     def ix(self, name):
         schema = getattr(self, '%s_schema' % name)
-        if not exists_in(self.index_path, indexname=name):
+        try:
+            exists = exists_in(self.index_path, indexname=name)
+        except FileNotFoundError:
+            exists = False
+        if not exists:
             return create_in(self.index_path, schema, indexname=name)
         ix = open_dir(self.index_path, indexname=name)
         update_schema(ix, schema)
         return ix
 
     def delete_index(self):
         shutil.rmtree(self.index_path)
```

### Comparing `devpi-web-4.2.1/devpi_web.egg-info/PKG-INFO` & `devpi_web-4.2.2/devpi_web.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-web
-Version: 4.2.1
+Version: 4.2.2
 Summary: devpi-web: a web view for devpi-server
 Home-page: https://devpi.net
 Maintainer: Florian Schulze
 Maintainer-email: mail@pyfidelity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/devpi/devpi/issues
 Project-URL: Changelog, https://github.com/devpi/devpi/blob/main/web/CHANGELOG
@@ -23,17 +23,28 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.4
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: Whoosh<3
+Requires-Dist: beautifulsoup4!=4.12.1,>=4.3.2
+Requires-Dist: defusedxml
+Requires-Dist: devpi-server>=5.2.0
+Requires-Dist: devpi-common>=3.2.0
+Requires-Dist: docutils>=0.11
+Requires-Dist: pygments>=1.6
+Requires-Dist: pyramid!=1.10a1
+Requires-Dist: pyramid-chameleon
+Requires-Dist: readme-renderer[md]>=23.0
 
 ================================================
 devpi-web: web interface plugin for devpi-server
 ================================================
 
 This plugin adds a web interface with search for `devpi-server`_.
 
@@ -72,14 +83,28 @@
 Changelog
 =========
 
 
 
 .. towncrier release notes start
 
+4.2.2 (2024-04-20)
+==================
+
+Bug Fixes
+---------
+
+- style.css: Always let content be full browser height. This also gives more height with some documentation themes when content is short.
+
+- style.css: set ``scrollbar-gutter: stable`` on ``body`` to prevent jumping content in documentation iframe.
+
+- Fix #970: overwrite fixed html/body heights like ``100%`` in documentation iframe content.
+
+
+
 4.2.1 (2023-07-02)
 ==================
 
 Bug Fixes
 ---------
 
 - Fix #953: Exception when browsers send ETag for documentation pages.
@@ -140,16 +165,7 @@
 Bug Fixes
 ---------
 
 - Fix #880: explicitly register views for GET method, so there is a 404 on POSTs, like when using twine with wrong upload url.
 
 - Fix #867: AttributeError during ``devpi-import`` and maybe other commands.
 
-
-4.0.8 (2021-08-12)
-==================
-
-Bug Fixes
----------
-
-- On startup loop over mirror indexes last to avoid filling up the indexing queue, which processes non mirror indexes first.
-
```

### Comparing `devpi-web-4.2.1/devpi_web.egg-info/SOURCES.txt` & `devpi_web-4.2.2/devpi_web.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.flake8
 AUTHORS
 CHANGELOG
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
@@ -25,14 +26,15 @@
 devpi_web.egg-info/not-zip-safe
 devpi_web.egg-info/requires.txt
 devpi_web.egg-info/top_level.txt
 devpi_web/static/common.js
 devpi_web/static/docview.js
 devpi_web/static/favicon.ico
 devpi_web/static/jquery-3.6.0.min.js
+devpi_web/static/style-old.css
 devpi_web/static/style.css
 devpi_web/templates/doc.pt
 devpi_web/templates/error.pt
 devpi_web/templates/index.pt
 devpi_web/templates/macros.pt
 devpi_web/templates/notfound.pt
 devpi_web/templates/project.pt
```

### Comparing `devpi-web-4.2.1/pyproject.toml` & `devpi_web-4.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.1/setup.py` & `devpi_web-4.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,30 +30,30 @@
     url="https://devpi.net",
     project_urls={
         'Bug Tracker': 'https://github.com/devpi/devpi/issues',
         'Changelog': 'https://github.com/devpi/devpi/blob/main/web/CHANGELOG',
         'Documentation': 'https://doc.devpi.net',
         'Source Code': 'https://github.com/devpi/devpi'
     },
-    version='4.2.1',
+    version='4.2.2',
     maintainer="Florian Schulze",
     maintainer_email="mail@pyfidelity.com",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Topic :: Internet :: WWW/HTTP",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Application"] + [
             "Programming Language :: Python :: %s" % x
-            for x in "3.4 3.5 3.6 3.7 3.8 3.9 3.10 3.11".split()],
+            for x in "3.4 3.5 3.6 3.7 3.8 3.9 3.10 3.11 3.12".split()],
     entry_points={
         'console_scripts': [
             "devpi-clear-search-index = devpi_web.clear_index:clear_index"],
         'devpi_server': [
             "devpi-web = devpi_web.main",
             "devpi-web-whoosh = devpi_web.whoosh_index"],
         'devpi_web': [
```

### Comparing `devpi-web-4.2.1/tests/conftest.py` & `devpi_web-4.2.2/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-from test_devpi_server.conftest import gentmp, httpget, makemapp  # noqa
-from test_devpi_server.conftest import maketestapp, makexom, mapp  # noqa
-from test_devpi_server.conftest import pypiurls, testapp, pypistage  # noqa
-from test_devpi_server.conftest import dummyrequest, pypiurls, testapp  # noqa
-from test_devpi_server.conftest import simpypi, simpypiserver  # noqa
-from test_devpi_server.conftest import storage_info  # noqa
-from test_devpi_server.conftest import mock, pyramidconfig  # noqa
-from test_devpi_server.conftest import speed_up_sqlite  # noqa
-from test_devpi_server.conftest import speed_up_sqlite_fs  # noqa
-try:
-    from test_devpi_server.conftest import lower_argon2_parameters  # noqa
-except ImportError:
-    pass
+from devpi_common.metadata import parse_version
+from devpi_server import __version__ as _devpi_server_version
 import pytest
 
 
-(makexom,)  # shut up pyflakes
+devpi_server_version = parse_version(_devpi_server_version)
+
+
+if devpi_server_version < parse_version("6.9.3dev"):
+    from test_devpi_server.conftest import gentmp, httpget, makemapp  # noqa: F401
+    from test_devpi_server.conftest import maketestapp, makexom, mapp  # noqa: F401
+    from test_devpi_server.conftest import pypiurls, testapp, pypistage  # noqa: F401
+    from test_devpi_server.conftest import dummyrequest  # noqa: F401
+    from test_devpi_server.conftest import simpypi, simpypiserver  # noqa: F401
+    from test_devpi_server.conftest import storage_info  # noqa: F401
+    from test_devpi_server.conftest import mock, pyramidconfig  # noqa: F401
+    from test_devpi_server.conftest import speed_up_sqlite  # noqa: F401
+    from test_devpi_server.conftest import speed_up_sqlite_fs  # noqa: F401
+    if devpi_server_version >= parse_version("6.0.0dev"):
+        from test_devpi_server.conftest import lower_argon2_parameters  # noqa: F401
+    (makexom,)  # noqa: B018 shut up pyflakes
+else:
+    pytest_plugins = ["pytest_devpi_server", "test_devpi_server.plugin"]
 
 
 def pytest_addoption(parser):
     parser.addoption("--fast", help="skip functional/slow tests", default=False,
                      action="store_true")
```

### Comparing `devpi-web-4.2.1/tests/test_indexing.py` & `devpi_web-4.2.2/tests/test_indexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from devpi_web.indexing import iter_projects
 from devpi_web.indexing import preprocess_project
 from devpi_server import __version__ as _devpi_server_version
 import pytest
 
 
 devpi_server_version = parse_version(_devpi_server_version)
+pytestmark = [pytest.mark.notransaction]
 
 
 @pytest.mark.skipif(
     devpi_server_version < parse_version("6.6.0dev"),
     reason="Needs un-normalized project names from list_projects_perstage on mirrors")
 def test_original_project_name(pypistage):
     xom = pypistage.xom
```

### Comparing `devpi-web-4.2.1/tests/test_main.py` & `devpi_web-4.2.2/tests/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from devpi_common.metadata import parse_version
 from devpi_server import __version__ as _devpi_server_version
 import pytest
 import textwrap
 
 
 devpi_server_version = parse_version(_devpi_server_version)
+pytestmark = [pytest.mark.notransaction]
 
 
 def test_importable():
     import devpi_web
     assert devpi_web
 
 
@@ -86,25 +87,25 @@
     xom_container = []
 
     class MyXOM(XOM):
         def __init__(self, config):
             xom_container.append(self)
             XOM.__init__(self, config)
 
-        def httpget(self, url, allow_redirects=True, extra_headers=None):
+        def httpget(self, url, allow_redirects=True, extra_headers=None):  # noqa: ARG002
             class Response:
                 def __init__(self):
                     self.status_code = 200
                     self.text = """<a href='foo'>foo</a>"""
                     self.url = url
             return Response()
 
         def create_app(self):
             # if the webserver is started, we fail
-            0 / 0
+            0 / 0  # noqa: B018
 
     calls = []
 
     monkeypatch.setattr(devpi_server.main, "XOM", MyXOM)
     monkeypatch.setattr(
         NullIndex, "delete_index",
         lambda s: calls.append("delete_index"))
@@ -142,15 +143,15 @@
 
     def test_indexer_backend_options(self):
         from devpi_web import main
         from pluggy import HookimplMarker
         hookimpl = HookimplMarker("devpiweb")
 
         class Index(object):
-            def __init__(self, config, settings):
+            def __init__(self, config, settings):  # noqa: ARG002
                 self.settings = settings
 
         class Plugin:
             @hookimpl
             def devpiweb_indexer_backend(self):
                 return dict(
                     indexer=Index,
@@ -168,15 +169,15 @@
     @pytest.mark.skipif(devpi_server_version < parse_version("4.7dev"), reason="Needs config file support")
     def test_indexer_backend_yaml_options(self, make_yaml_config):
         from devpi_web import main
         from pluggy import HookimplMarker
         hookimpl = HookimplMarker("devpiweb")
 
         class Index(object):
-            def __init__(self, config, settings):
+            def __init__(self, config, settings):  # noqa: ARG002
                 self.settings = settings
 
         class Plugin:
             @hookimpl
             def devpiweb_indexer_backend(self):
                 return dict(
                     indexer=Index,
```

### Comparing `devpi-web-4.2.1/tests/test_theme.py` & `devpi_web-4.2.2/tests/test_theme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import pytest
 
 
+pytestmark = [pytest.mark.notransaction]
+
+
 @pytest.fixture
 def themedir(tmpdir):
     path = tmpdir.join('theme')
     path.ensure_dir()
     path.join('static').ensure_dir()
     path.join('templates').ensure_dir()
     return path
```

### Comparing `devpi-web-4.2.1/tests/test_views.py` & `devpi_web-4.2.2/tests/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from devpi_server import __version__ as _devpi_server_version
 from time import struct_time
 import pytest
 import re
 
 
 devpi_server_version = parse_version(_devpi_server_version)
+pytestmark = [pytest.mark.notransaction]
 
 
 def compareable_text(text):
     return re.sub(r'\s+', ' ', text.strip())
 
 
 def test_root_view(testapp):
```

### Comparing `devpi-web-4.2.1/tests/test_views_docs.py` & `devpi_web-4.2.2/tests/test_views_docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from devpi_common.archive import zip_dict
 from hashlib import sha256
 import pytest
 import re
 import sys
 
 
-pytestmark = pytest.mark.xfail(sys.platform.startswith("win"), run=False, reason="flaky test on windows")
+pytestmark = [
+    pytest.mark.notransaction,
+    pytest.mark.xfail(
+        sys.platform.startswith("win"),
+        run=False,
+        reason="flaky test on windows")]
 
 
 def compareable_text(text):
     return re.sub(r'\s+', ' ', text.strip())
 
 
 @pytest.fixture(autouse=True)
```

### Comparing `devpi-web-4.2.1/tests/test_views_misc.py` & `devpi_web-4.2.2/tests/test_views_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from devpi_web.main import hookimpl
 from test_devpi_server.conftest import make_file_url
 import pytest
 import re
 
 
 devpi_server_version = parse_version(_devpi_server_version)
+pytestmark = [pytest.mark.notransaction]
 
 
 def compareable_text(text):
     return re.sub(r'\s+', ' ', text.strip())
 
 
 @pytest.mark.parametrize("input, expected", [
@@ -251,15 +252,15 @@
             (IViewClassifier, request_iface, Interface), IView, name=name,
             default=None)
 
     @pytest.fixture
     def plugin(self):
         class Plugin:
             @hookimpl
-            def devpiweb_get_status_info(self, request):
+            def devpiweb_get_status_info(self, request):  # noqa: ARG002
                 result = self.results.pop()
                 if isinstance(result, Exception):
                     raise result
                 return result
         return Plugin()
 
     @pytest.fixture
@@ -365,15 +366,15 @@
 
     @pytest.mark.parametrize("msgs", [
         [dict(status="warn", msg="Bar"), dict(status="fatal", msg="Foo")],
         [dict(status="fatal", msg="Foo"), dict(status="warn", msg="Bar")]])
     def test_status_macros_mixed(self, dummyrequest, plugin, statusview, msgs):
         from bs4 import BeautifulSoup
         from devpi_web.main import status_info
-        plugin.results = [[dict(status="fatal", msg="Foo")]]
+        plugin.results = [msgs]
         dummyrequest.status_info = status_info(dummyrequest)
         result = statusview(None, dummyrequest)
         html = BeautifulSoup(result.body, 'html.parser')
         assert html.select('.statusbadge')[0].text.strip() == 'fatal'
         assert 'fatal' in html.select('.statusbadge')[0].attrs['class']
         assert 'Bar' not in html.select('#serverstatus')[0].text
         assert 'Foo' in html.select('#serverstatus')[0].text
```

### Comparing `devpi-web-4.2.1/tests/test_views_search.py` & `devpi_web-4.2.2/tests/test_views_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from devpi_common.archive import zip_dict
 from devpi_web.indexing import ProjectIndexingInfo
 from devpi_web.main import get_indexer
 import pytest
 import re
 
 
+pytestmark = [pytest.mark.notransaction]
+
+
 @pytest.fixture
 def makexom(request, makexom):
     orig_makexom = makexom
 
     def makexom(*args, **kw):
         xom = orig_makexom(*args, **kw)
         if request.node.get_closest_marker("with_indexer"):
@@ -279,14 +282,15 @@
     api = mapp.create_and_use(indexconfig=dict(bases=[pypistage.name]))
     pypistage.mock_simple("pkg1", '<a href="/pkg1-2.6.zip" /a>')
     pypistage.mock_simple("pkg2", '')
     # we need to set dummy data, so we can use waithooks
     mapp.set_versiondata({"name": "pkg2", "version": "2.7"}, waithooks=True)
     # now we can access the indexer directly without causing locking issues
     indexer = get_indexer(mapp.xom)
+    indexer.indexer_thread.wait()
     with mapp.xom.keyfs.transaction(write=False):
         stage = mapp.xom.model.getstage(pypistage.name)
         indexer.update_projects([
             ProjectIndexingInfo(stage=stage, name=u'pkg1'),
             ProjectIndexingInfo(stage=stage, name=u'pkg2')], clear=True)
     mapp.set_versiondata({
         "name": "pkg2",
```

### Comparing `devpi-web-4.2.1/tests/test_views_toxresults.py` & `devpi_web-4.2.2/tests/test_views_toxresults.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import hashlib
 import json
 import pytest
 import re
 
 
+pytestmark = [pytest.mark.notransaction]
+
+
 def compareable_text(text):
     return re.sub(r'\s+', ' ', text.strip())
 
 
 @pytest.mark.with_notifier
 def test_testdata(mapp, testapp, tox_result_data):
     api = mapp.create_and_use()
@@ -115,15 +118,15 @@
 
 def test_toxresults_state():
     from devpi_web.views import get_toxresults_info
     from devpi_web.views import get_toxresults_state
     from io import BytesIO
 
     class LinkStore(list):
-        def get_links(self, rel, for_entrypath):
+        def get_links(self, rel, for_entrypath):  # noqa: ARG002
             return self[for_entrypath]
 
     class Link(object):
         def __init__(self, testenvs):
             self.testenvs = testenvs
             self.basename = "pytest-1.7.zip.toxresult"
 
@@ -138,15 +141,15 @@
             result = {
                 "reportversion": "1",
                 "toxversion": "1.6",
                 "platform": "linux2",
                 "host": "foo",
                 "installpkg": {
                     "basename": "pytest-1.7.zip",
-                    "md5": hashlib.md5(b"123").hexdigest(),
+                    "md5": hashlib.md5(b"123").hexdigest(),  # noqa: S324
                     "sha256": hashlib.sha256(b"123").hexdigest(),
                 },
                 "testenvs": self.testenvs}
             return json.dumps(result).encode('utf-8')
 
     linkstore = LinkStore([[Link({})]])
     assert get_toxresults_state(get_toxresults_info(linkstore, 0)) is None
```

### Comparing `devpi-web-4.2.1/tests/test_whoosh_index.py` & `devpi_web-4.2.2/tests/test_whoosh_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from devpi_web.indexing import ProjectIndexingInfo
 import pytest
 
 
+pytestmark = [pytest.mark.notransaction]
+
+
 @pytest.mark.parametrize("input, expected", [
     ("Foo", [(0, 0, 3, "Foo")]),
     ("Foo Bar", [(0, 0, 3, "Foo"), (1, 4, 7, "Bar")]),
     ("Foo-Bar", [(0, 0, 3, "Foo"), (1, 4, 7, "Bar")]),
     ("Foo_Bar", [(0, 0, 3, "Foo"), (1, 4, 7, "Bar")]),
     ("1Foo Bar", [(0, 0, 4, "1Foo"), (1, 5, 8, "Bar")]),
     ("1Foo-Bar", [(0, 0, 4, "1Foo"), (1, 5, 8, "Bar")]),
@@ -167,15 +170,15 @@
 class FakeStage(object):
     def __init__(self, index_type):
         self.ixconfig = dict(type=index_type)
         self.name = index_type
         self.serials = {}
         self.serial = -1
 
-    def get_last_project_change_serial_perstage(self, project, at_serial=None):
+    def get_last_project_change_serial_perstage(self, project, at_serial=None):  # noqa: ARG002
         return self.serials.get(project, self.serial)
 
 
 class TestIndexingSharedData:
     @pytest.fixture
     def shared_data(self):
         from devpi_web.whoosh_index import IndexingSharedData
@@ -344,19 +347,19 @@
         mirror.serial = 0
         prjs = []
         for i in range(10):
             prjs.append(ProjectIndexingInfo(stage=mirror, name='prj%d' % i))
 
         result = []
 
-        def handler(is_from_mirror, serial, indexname, names):
+        def handler(is_from_mirror, serial, indexname, names):  # noqa: ARG001
             result.append(names)
 
         class FakeSearcher:
-            def document_number(self, path):
+            def document_number(self, path):  # noqa: ARG002
                 return None
 
         shared_data.queue_projects(prjs, 0, FakeSearcher())
         assert shared_data.queue.qsize() == 4
 
         shared_data.process_next(handler)
         assert shared_data.queue.qsize() == 3
```

### Comparing `devpi-web-4.2.1/tox.ini` & `devpi_web-4.2.2/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 [tox]
-envlist = py35-server520,py37{,-keyfs},py310,pypy3
+envlist = py35-server520,py37{,-keyfs},py310,pypy3,flake8
+# for Python 3.5 we need older virtualenv
+requires = virtualenv<20.22.0
 
 
 [testenv]
 commands =
     !keyfs: py.test --cov {envsitepackagesdir}/devpi_web {posargs}
-    keyfs: py.test --backend=devpi_server.keyfs_sqlite {posargs}
+    keyfs: py.test --devpi-server-storage-backend=devpi_server.keyfs_sqlite {posargs}
 
 passenv = GITHUB_ACTIONS, LANG
 setenv =
     CHAMELEON_CACHE = {envtmpdir}
 
 deps =
     webtest
     mock
     pytest
     pytest-cov
-    pytest-flake8
-    flake8<5
     pytest-github-actions-annotate-failures
     server520: devpi-server==5.2.0
     server520: ruamel.yaml<0.17.22;python_version<"3.6"
     pyparsing<3;python_version<"3.6"
     importlib.metadata;python_version<"3.8"
 
 
+[testenv:flake8]
+commands = flake8 --config .flake8
+deps = flake8
+skip_install = true
+
+
 [pytest]
-addopts = -r a --flake8 --cov-report=term --cov-report=html -W once::DeprecationWarning -W ignore::DeprecationWarning:webob.acceptparse -W ignore::DeprecationWarning:docutils.io -W once::pytest.PytestDeprecationWarning -W once::ResourceWarning
-flake8-ignore =
-    * E501 E741 W503
-norecursedirs = .tox ja
+addopts =
+    -r a
+    --cov-report=term
+    --cov-report=html
+    -W once::DeprecationWarning
+    -W ignore::DeprecationWarning:webob.acceptparse
+    -W ignore::DeprecationWarning:docutils.io
+    -W once::pytest.PytestDeprecationWarning
+    -W once::ResourceWarning
+norecursedirs = .tox build
 markers =
     nomocking: do not mock anything in fixtures
+    notransaction: do not open a transaction
     with_indexer: use the indexer thread
     with_notifier: use the notifier thread
```

