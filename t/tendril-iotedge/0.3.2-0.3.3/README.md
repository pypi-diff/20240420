# Comparing `tmp/tendril_iotedge-0.3.2.tar.gz` & `tmp/tendril_iotedge-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril_iotedge-0.3.2.tar", last modified: Sat Apr 20 02:00:08 2024, max compression
+gzip compressed data, was "tendril_iotedge-0.3.3.tar", last modified: Sat Apr 20 02:04:21 2024, max compression
```

## Comparing `tendril_iotedge-0.3.2.tar` & `tendril_iotedge-0.3.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.559428 tendril_iotedge-0.3.2/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/MANIFEST.in
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5320 2024-04-20 02:00:08.559428 tendril_iotedge-0.3.2/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-20 02:00:08.559428 tendril_iotedge-0.3.2/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3214 2023-08-29 06:16:15.000000 tendril_iotedge-0.3.2/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.539428 tendril_iotedge-0.3.2/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3114 2024-04-18 22:10:09.000000 tendril_iotedge-0.3.2/src/tendril/apiserver/routers/iotcore.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3424 2024-04-17 22:34:16.000000 tendril_iotedge-0.3.2/src/tendril/apiserver/routers/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/common/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-25 05:48:52.000000 tendril_iotedge-0.3.2/src/tendril/common/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      125 2023-07-25 05:51:28.000000 tendril_iotedge-0.3.2/src/tendril/common/iotcore/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril_iotedge-0.3.2/src/tendril/common/iotcore/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/common/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/common/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/common/iotedge/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      734 2023-08-30 15:08:09.000000 tendril_iotedge-0.3.2/src/tendril/common/iotedge/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1984 2024-04-20 01:19:25.000000 tendril_iotedge-0.3.2/src/tendril/config/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/core/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril_iotedge-0.3.2/src/tendril/core/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/core/topology/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril_iotedge-0.3.2/src/tendril/core/topology/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      339 2024-04-17 13:58:51.000000 tendril_iotedge-0.3.2/src/tendril/core/topology/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.551428 tendril_iotedge-0.3.2/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.551428 tendril_iotedge-0.3.2/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5595 2024-04-05 13:17:38.000000 tendril_iotedge-0.3.2/src/tendril/db/models/deviceconfig.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.551428 tendril_iotedge-0.3.2/src/tendril/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril_iotedge-0.3.2/src/tendril/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1031 2024-04-18 22:10:09.000000 tendril_iotedge-0.3.2/src/tendril/iotcore/logs.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1150 2024-04-17 22:01:55.000000 tendril_iotedge-0.3.2/src/tendril/iotcore/settings.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.551428 tendril_iotedge-0.3.2/src/tendril/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3085 2023-08-14 16:42:02.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/announce.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-08-04 21:50:35.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/config.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      444 2024-04-17 22:10:55.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/heartbeat.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1205 2024-04-20 01:07:13.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/logs.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.551428 tendril_iotedge-0.3.2/src/tendril/iotedge/profiles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/profiles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4253 2024-04-20 01:20:25.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/profiles/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4026 2023-07-28 16:44:25.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/profiles/manager.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-08-12 07:26:08.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/registration.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.555428 tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5320 2024-04-20 02:00:08.000000 tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1735 2024-04-20 02:00:08.000000 tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-20 02:00:08.000000 tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2024-04-20 02:00:08.000000 tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-20 02:00:08.000000 tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.555428 tendril_iotedge-0.3.2/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.369903 tendril_iotedge-0.3.3/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5353 2024-04-20 02:04:21.369903 tendril_iotedge-0.3.3/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.357903 tendril_iotedge-0.3.3/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.357903 tendril_iotedge-0.3.3/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.357903 tendril_iotedge-0.3.3/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.357903 tendril_iotedge-0.3.3/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.357903 tendril_iotedge-0.3.3/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-20 02:04:21.369903 tendril_iotedge-0.3.3/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3239 2024-04-20 02:03:45.000000 tendril_iotedge-0.3.3/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.353903 tendril_iotedge-0.3.3/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.357903 tendril_iotedge-0.3.3/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.357903 tendril_iotedge-0.3.3/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.357903 tendril_iotedge-0.3.3/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3114 2024-04-18 22:10:09.000000 tendril_iotedge-0.3.3/src/tendril/apiserver/routers/iotcore.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3424 2024-04-17 22:34:16.000000 tendril_iotedge-0.3.3/src/tendril/apiserver/routers/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.357903 tendril_iotedge-0.3.3/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.357903 tendril_iotedge-0.3.3/src/tendril/common/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-25 05:48:52.000000 tendril_iotedge-0.3.3/src/tendril/common/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      125 2023-07-25 05:51:28.000000 tendril_iotedge-0.3.3/src/tendril/common/iotcore/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril_iotedge-0.3.3/src/tendril/common/iotcore/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.357903 tendril_iotedge-0.3.3/src/tendril/common/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/src/tendril/common/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/src/tendril/common/iotedge/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      734 2023-08-30 15:08:09.000000 tendril_iotedge-0.3.3/src/tendril/common/iotedge/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.361903 tendril_iotedge-0.3.3/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1984 2024-04-20 01:19:25.000000 tendril_iotedge-0.3.3/src/tendril/config/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.361903 tendril_iotedge-0.3.3/src/tendril/core/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril_iotedge-0.3.3/src/tendril/core/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.361903 tendril_iotedge-0.3.3/src/tendril/core/topology/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril_iotedge-0.3.3/src/tendril/core/topology/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      339 2024-04-17 13:58:51.000000 tendril_iotedge-0.3.3/src/tendril/core/topology/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.361903 tendril_iotedge-0.3.3/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.361903 tendril_iotedge-0.3.3/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5595 2024-04-05 13:17:38.000000 tendril_iotedge-0.3.3/src/tendril/db/models/deviceconfig.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.361903 tendril_iotedge-0.3.3/src/tendril/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril_iotedge-0.3.3/src/tendril/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1031 2024-04-18 22:10:09.000000 tendril_iotedge-0.3.3/src/tendril/iotcore/logs.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1150 2024-04-17 22:01:55.000000 tendril_iotedge-0.3.3/src/tendril/iotcore/settings.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.361903 tendril_iotedge-0.3.3/src/tendril/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/src/tendril/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3085 2023-08-14 16:42:02.000000 tendril_iotedge-0.3.3/src/tendril/iotedge/announce.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-08-04 21:50:35.000000 tendril_iotedge-0.3.3/src/tendril/iotedge/config.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      444 2024-04-17 22:10:55.000000 tendril_iotedge-0.3.3/src/tendril/iotedge/heartbeat.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1205 2024-04-20 01:07:13.000000 tendril_iotedge-0.3.3/src/tendril/iotedge/logs.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.361903 tendril_iotedge-0.3.3/src/tendril/iotedge/profiles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/src/tendril/iotedge/profiles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4253 2024-04-20 01:20:25.000000 tendril_iotedge-0.3.3/src/tendril/iotedge/profiles/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4026 2023-07-28 16:44:25.000000 tendril_iotedge-0.3.3/src/tendril/iotedge/profiles/manager.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-08-12 07:26:08.000000 tendril_iotedge-0.3.3/src/tendril/iotedge/registration.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.365903 tendril_iotedge-0.3.3/src/tendril_iotedge.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5353 2024-04-20 02:04:21.000000 tendril_iotedge-0.3.3/src/tendril_iotedge.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1735 2024-04-20 02:04:21.000000 tendril_iotedge-0.3.3/src/tendril_iotedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-20 02:04:21.000000 tendril_iotedge-0.3.3/src/tendril_iotedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      583 2024-04-20 02:04:21.000000 tendril_iotedge-0.3.3/src/tendril_iotedge.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-20 02:04:21.000000 tendril_iotedge-0.3.3/src/tendril_iotedge.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:04:21.361903 tendril_iotedge-0.3.3/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.3/tox.ini
```

### Comparing `tendril_iotedge-0.3.2/.gitignore` & `tendril_iotedge-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/.readthedocs.yml` & `tendril_iotedge-0.3.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/.travis.yml` & `tendril_iotedge-0.3.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/LICENSE` & `tendril_iotedge-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/PKG-INFO` & `tendril_iotedge-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-iotedge
-Version: 0.3.2
+Version: 0.3.3
 Summary: Tendril IoT Edge Server Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-iotedge
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-iotedge.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-iotedge/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-iotedge
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: tendril-caching>=0.2.2
 Requires-Dist: tendril-auth>=0.3.3
 Requires-Dist: tendril-interests>=0.2.3
+Requires-Dist: tendril-filestore
 Requires-Dist: wheel
 Provides-Extra: docs
 Requires-Dist: setuptools_scm; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-argparse; extra == "docs"
 Requires-Dist: alabaster; extra == "docs"
 Provides-Extra: tests
```

### Comparing `tendril_iotedge-0.3.2/README.rst` & `tendril_iotedge-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/docs/Makefile` & `tendril_iotedge-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/docs/_static/custom.css` & `tendril_iotedge-0.3.3/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/docs/_static/favicon.ico` & `tendril_iotedge-0.3.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/docs/_static/logo.png` & `tendril_iotedge-0.3.3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/docs/_static/logo_packed.png` & `tendril_iotedge-0.3.3/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/docs/_templates/about.html` & `tendril_iotedge-0.3.3/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/docs/conf.py` & `tendril_iotedge-0.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/docs/index.rst` & `tendril_iotedge-0.3.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/docs/installation.rst` & `tendril_iotedge-0.3.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/setup.py` & `tendril_iotedge-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     return content
 
 
 core_dependencies = [
     'tendril-caching>=0.2.2',
     'tendril-auth>=0.3.3',
     'tendril-interests>=0.2.3',
+    'tendril-filestore',
 ]
 
 install_requires = core_dependencies + ['wheel']
 
 setup_requires = ['setuptools_scm']
 
 doc_requires = setup_requires + ['sphinx', 'sphinx-argparse', 'alabaster']
```

### Comparing `tendril_iotedge-0.3.2/src/tendril/apiserver/routers/iotcore.py` & `tendril_iotedge-0.3.3/src/tendril/apiserver/routers/iotcore.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril/apiserver/routers/iotedge.py` & `tendril_iotedge-0.3.3/src/tendril/apiserver/routers/iotedge.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril/common/iotedge/exceptions.py` & `tendril_iotedge-0.3.3/src/tendril/common/iotedge/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril/common/iotedge/formats.py` & `tendril_iotedge-0.3.3/src/tendril/common/iotedge/formats.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril/config/__init__.py` & `tendril_iotedge-0.3.3/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril/config/iotedge.py` & `tendril_iotedge-0.3.3/src/tendril/config/iotedge.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril/db/models/deviceconfig.py` & `tendril_iotedge-0.3.3/src/tendril/db/models/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril/iotcore/logs.py` & `tendril_iotedge-0.3.3/src/tendril/iotcore/logs.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril/iotcore/settings.py` & `tendril_iotedge-0.3.3/src/tendril/iotcore/settings.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril/iotedge/announce.py` & `tendril_iotedge-0.3.3/src/tendril/iotedge/announce.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril/iotedge/logs.py` & `tendril_iotedge-0.3.3/src/tendril/iotedge/logs.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril/iotedge/profiles/base.py` & `tendril_iotedge-0.3.3/src/tendril/iotedge/profiles/base.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril/iotedge/profiles/manager.py` & `tendril_iotedge-0.3.3/src/tendril/iotedge/profiles/manager.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril/iotedge/registration.py` & `tendril_iotedge-0.3.3/src/tendril/iotedge/registration.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/PKG-INFO` & `tendril_iotedge-0.3.3/src/tendril_iotedge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-iotedge
-Version: 0.3.2
+Version: 0.3.3
 Summary: Tendril IoT Edge Server Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-iotedge
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-iotedge.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-iotedge/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-iotedge
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: tendril-caching>=0.2.2
 Requires-Dist: tendril-auth>=0.3.3
 Requires-Dist: tendril-interests>=0.2.3
+Requires-Dist: tendril-filestore
 Requires-Dist: wheel
 Provides-Extra: docs
 Requires-Dist: setuptools_scm; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-argparse; extra == "docs"
 Requires-Dist: alabaster; extra == "docs"
 Provides-Extra: tests
```

### Comparing `tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/SOURCES.txt` & `tendril_iotedge-0.3.3/src/tendril_iotedge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/requires.txt` & `tendril_iotedge-0.3.3/src/tendril_iotedge.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 tendril-caching>=0.2.2
 tendril-auth>=0.3.3
 tendril-interests>=0.2.3
+tendril-filestore
 wheel
 
 [build]
 setuptools_scm
 sphinx
 sphinx-argparse
 alabaster
```

### Comparing `tendril_iotedge-0.3.2/tests/coveralls.py` & `tendril_iotedge-0.3.3/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.2/tox.ini` & `tendril_iotedge-0.3.3/tox.ini`

 * *Files identical despite different names*

