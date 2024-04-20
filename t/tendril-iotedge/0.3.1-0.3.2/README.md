# Comparing `tmp/tendril_iotedge-0.3.1.tar.gz` & `tmp/tendril_iotedge-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril_iotedge-0.3.1.tar", last modified: Tue Apr 16 18:44:32 2024, max compression
+gzip compressed data, was "tendril_iotedge-0.3.2.tar", last modified: Sat Apr 20 02:00:08 2024, max compression
```

## Comparing `tendril_iotedge-0.3.1.tar` & `tendril_iotedge-0.3.2.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.567465 tendril_iotedge-0.3.1/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/MANIFEST.in
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5320 2024-04-16 18:44:32.567465 tendril_iotedge-0.3.1/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.535465 tendril_iotedge-0.3.1/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.539465 tendril_iotedge-0.3.1/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-16 18:44:32.567465 tendril_iotedge-0.3.1/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3214 2023-08-29 06:16:15.000000 tendril_iotedge-0.3.1/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.531465 tendril_iotedge-0.3.1/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1879 2024-04-05 13:17:24.000000 tendril_iotedge-0.3.1/src/tendril/apiserver/routers/iotcore.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2909 2023-09-01 12:23:47.000000 tendril_iotedge-0.3.1/src/tendril/apiserver/routers/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.543465 tendril_iotedge-0.3.1/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.547465 tendril_iotedge-0.3.1/src/tendril/common/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-25 05:48:52.000000 tendril_iotedge-0.3.1/src/tendril/common/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      125 2023-07-25 05:51:28.000000 tendril_iotedge-0.3.1/src/tendril/common/iotcore/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril_iotedge-0.3.1/src/tendril/common/iotcore/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.547465 tendril_iotedge-0.3.1/src/tendril/common/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/common/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/common/iotedge/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      734 2023-08-30 15:08:09.000000 tendril_iotedge-0.3.1/src/tendril/common/iotedge/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.547465 tendril_iotedge-0.3.1/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1830 2023-03-28 11:11:29.000000 tendril_iotedge-0.3.1/src/tendril/config/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.551465 tendril_iotedge-0.3.1/src/tendril/core/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril_iotedge-0.3.1/src/tendril/core/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.551465 tendril_iotedge-0.3.1/src/tendril/core/topology/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril_iotedge-0.3.1/src/tendril/core/topology/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      341 2024-04-16 18:36:14.000000 tendril_iotedge-0.3.1/src/tendril/core/topology/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.551465 tendril_iotedge-0.3.1/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.551465 tendril_iotedge-0.3.1/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5595 2024-04-05 13:17:38.000000 tendril_iotedge-0.3.1/src/tendril/db/models/deviceconfig.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.551465 tendril_iotedge-0.3.1/src/tendril/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril_iotedge-0.3.1/src/tendril/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1037 2023-04-08 07:05:40.000000 tendril_iotedge-0.3.1/src/tendril/iotcore/settings.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.559465 tendril_iotedge-0.3.1/src/tendril/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3085 2023-08-14 16:42:02.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/announce.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-08-04 21:50:35.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/config.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      487 2023-08-05 17:25:22.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/heartbeat.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.559465 tendril_iotedge-0.3.1/src/tendril/iotedge/profiles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/profiles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1916 2023-08-12 07:56:01.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/profiles/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4026 2023-07-28 16:44:25.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/profiles/manager.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-08-12 07:26:08.000000 tendril_iotedge-0.3.1/src/tendril/iotedge/registration.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.559465 tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5320 2024-04-16 18:44:32.000000 tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1679 2024-04-16 18:44:32.000000 tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-16 18:44:32.000000 tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2024-04-16 18:44:32.000000 tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-16 18:44:32.000000 tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:44:32.559465 tendril_iotedge-0.3.1/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.1/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.559428 tendril_iotedge-0.3.2/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5320 2024-04-20 02:00:08.559428 tendril_iotedge-0.3.2/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-20 02:00:08.559428 tendril_iotedge-0.3.2/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3214 2023-08-29 06:16:15.000000 tendril_iotedge-0.3.2/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.539428 tendril_iotedge-0.3.2/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.543428 tendril_iotedge-0.3.2/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3114 2024-04-18 22:10:09.000000 tendril_iotedge-0.3.2/src/tendril/apiserver/routers/iotcore.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3424 2024-04-17 22:34:16.000000 tendril_iotedge-0.3.2/src/tendril/apiserver/routers/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/common/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-25 05:48:52.000000 tendril_iotedge-0.3.2/src/tendril/common/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      125 2023-07-25 05:51:28.000000 tendril_iotedge-0.3.2/src/tendril/common/iotcore/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril_iotedge-0.3.2/src/tendril/common/iotcore/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/common/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/common/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/common/iotedge/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      734 2023-08-30 15:08:09.000000 tendril_iotedge-0.3.2/src/tendril/common/iotedge/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1984 2024-04-20 01:19:25.000000 tendril_iotedge-0.3.2/src/tendril/config/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/core/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril_iotedge-0.3.2/src/tendril/core/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.547428 tendril_iotedge-0.3.2/src/tendril/core/topology/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril_iotedge-0.3.2/src/tendril/core/topology/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      339 2024-04-17 13:58:51.000000 tendril_iotedge-0.3.2/src/tendril/core/topology/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.551428 tendril_iotedge-0.3.2/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.551428 tendril_iotedge-0.3.2/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5595 2024-04-05 13:17:38.000000 tendril_iotedge-0.3.2/src/tendril/db/models/deviceconfig.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.551428 tendril_iotedge-0.3.2/src/tendril/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril_iotedge-0.3.2/src/tendril/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1031 2024-04-18 22:10:09.000000 tendril_iotedge-0.3.2/src/tendril/iotcore/logs.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1150 2024-04-17 22:01:55.000000 tendril_iotedge-0.3.2/src/tendril/iotcore/settings.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.551428 tendril_iotedge-0.3.2/src/tendril/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3085 2023-08-14 16:42:02.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/announce.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-08-04 21:50:35.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/config.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      444 2024-04-17 22:10:55.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/heartbeat.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1205 2024-04-20 01:07:13.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/logs.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.551428 tendril_iotedge-0.3.2/src/tendril/iotedge/profiles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/profiles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4253 2024-04-20 01:20:25.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/profiles/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4026 2023-07-28 16:44:25.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/profiles/manager.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-08-12 07:26:08.000000 tendril_iotedge-0.3.2/src/tendril/iotedge/registration.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.555428 tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5320 2024-04-20 02:00:08.000000 tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1735 2024-04-20 02:00:08.000000 tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-20 02:00:08.000000 tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2024-04-20 02:00:08.000000 tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-20 02:00:08.000000 tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 02:00:08.555428 tendril_iotedge-0.3.2/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.2/tox.ini
```

### Comparing `tendril_iotedge-0.3.1/.gitignore` & `tendril_iotedge-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/.readthedocs.yml` & `tendril_iotedge-0.3.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/.travis.yml` & `tendril_iotedge-0.3.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/LICENSE` & `tendril_iotedge-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/PKG-INFO` & `tendril_iotedge-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-iotedge
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tendril IoT Edge Server Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-iotedge
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-iotedge.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-iotedge/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-iotedge
```

### Comparing `tendril_iotedge-0.3.1/README.rst` & `tendril_iotedge-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/docs/Makefile` & `tendril_iotedge-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/docs/_static/custom.css` & `tendril_iotedge-0.3.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/docs/_static/favicon.ico` & `tendril_iotedge-0.3.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/docs/_static/logo.png` & `tendril_iotedge-0.3.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/docs/_static/logo_packed.png` & `tendril_iotedge-0.3.2/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/docs/_templates/about.html` & `tendril_iotedge-0.3.2/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/docs/conf.py` & `tendril_iotedge-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/docs/index.rst` & `tendril_iotedge-0.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/docs/installation.rst` & `tendril_iotedge-0.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/setup.py` & `tendril_iotedge-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/src/tendril/apiserver/routers/iotcore.py` & `tendril_iotedge-0.3.2/src/tendril/apiserver/routers/iotcore.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 
 
 from fastapi import APIRouter
 from fastapi import Depends
+from fastapi import BackgroundTasks
 
 from tendril.authn.users import auth_spec
 from tendril.authn.users import authn_dependency
 from tendril.authn.users import AuthUserModel
 
 from tendril.config import INTERESTS_API_ENABLED
 from tendril.iotedge.profiles import device_config_unified_model
 
 from tendril.iotcore.settings import get_device_settings
 from tendril.iotcore.settings import set_device_settings
+from tendril.iotcore.logs import request_device_logs
+from tendril.iotcore.logs import available_device_logs
 
 from tendril.utils.db import get_session
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
 
 
 device_management_router = APIRouter(
@@ -31,21 +34,46 @@
         return get_device_settings(id=id, auth_user=user,
                                    session=session).export(expand=False)
 
 
 @device_management_router.post("/{id}/settings",
                                response_model=device_config_unified_model)
 async def write_device_settings(id: int, settings: device_config_unified_model,
-                                user: AuthUserModel = auth_spec(scopes=['device:write'])):
+                                user: AuthUserModel = auth_spec(scopes=['device:write']),
+                                background_tasks=BackgroundTasks):
     with get_session() as session:
+        # TODO Clean this up.
+        #  We are most probably never using these responses.
+        #  Confirm and remove.
         result = set_device_settings(id=id, settings=settings,
+                                     background_tasks=background_tasks,
                                      auth_user=user, session=session)
         return get_device_settings(id=id, auth_user=user,
                                    session=session).export(expand=False)
 
+
+@device_management_router.post("/{id}/logs")
+async def request_logs_from_device(id: int,
+                       user: AuthUserModel = auth_spec(scopes=['device:write']),
+                       background_tasks=BackgroundTasks):
+    with get_session() as session:
+        return request_device_logs(id=id, background_tasks=background_tasks,
+                                   auth_user=user, session=session)
+
+
+@device_management_router.get("/{id}/logs")
+async def get_available_logs(id: int,
+                             user: AuthUserModel = auth_spec(scopes=['device:write']),
+                             background_tasks=BackgroundTasks):
+    with get_session() as session:
+        return available_device_logs(id=id, background_tasks=background_tasks,
+                                     auth_user=user, session=session)
+
+
+
 if INTERESTS_API_ENABLED:
     routers = [
         device_management_router
     ]
 else:
     logger.info("Not creating Device Management API routers.")
     routers = []
```

### Comparing `tendril_iotedge-0.3.1/src/tendril/common/iotedge/exceptions.py` & `tendril_iotedge-0.3.2/src/tendril/common/iotedge/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/src/tendril/common/iotedge/formats.py` & `tendril_iotedge-0.3.2/src/tendril/common/iotedge/formats.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/src/tendril/config/__init__.py` & `tendril_iotedge-0.3.2/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/src/tendril/config/iotedge.py` & `tendril_iotedge-0.3.2/src/tendril/config/iotedge.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,19 @@
     ConfigOption(
         'IOTEDGE_ANNOUNCE_ENDPOINT_OPEN',
         "True",
         "Whether the /announce endpoint is open (unauthenticated). This is required for the "
         "integrated device registration flow.",
         parser=bool
     ),
+    ConfigOption(
+        'IOTEDGE_DEVICE_LOGS_UPLOAD_FILESTORE_BUCKET',
+        '"incoming"',
+        "Filestore bucket to upload device logs to."
+    )
 ]
 
 
 def load(manager):
     logger.debug("Loading {0}".format(__name__))
     manager.load_elements(config_elements_iotedge,
                           doc="Tendril IOT Edge Configuration")
```

### Comparing `tendril_iotedge-0.3.1/src/tendril/db/models/deviceconfig.py` & `tendril_iotedge-0.3.2/src/tendril/db/models/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/src/tendril/iotcore/settings.py` & `tendril_iotedge-0.3.2/src/tendril/iotcore/settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 
 
 from tendril.libraries import interests
 from tendril.common.interests.exceptions import InterestTypeUnsupported
 
 from tendril.utils.db import with_db
 from tendril.utils import log
-logger = log.get_logger(__name__, log.DEFAULT)
+logger = log.get_logger(__name__)
 
 
 @with_db
 def get_device_settings(id: int, auth_user=None, session=None):
     library = interests.find_library(id)
     interest = library.item(id=id, session=session)
     if not hasattr(interest, 'appname'):
         raise InterestTypeUnsupported("'appname' attribute", id=id, name=interest.name)
     profile = interest.profile(auth_user=auth_user, session=session)
     return profile.config(session=session)
 
 
 @with_db
-def set_device_settings(id: int, settings=None, auth_user=None, session=None):
+def set_device_settings(id: int, settings=None, background_tasks=None, auth_user=None, session=None):
     library = interests.find_library(id)
     interest = library.item(id=id, session=session)
     if not hasattr(interest, 'appname'):
         raise InterestTypeUnsupported("'appname' attribute", id=id, name=interest.name)
-    return interest.configure(settings=settings, auth_user=auth_user, session=session)
+    response = interest.configure(settings=settings, auth_user=auth_user, session=session)
+    interest.trigger_device_settings_update(background_tasks=background_tasks)
+    return response
```

### Comparing `tendril_iotedge-0.3.1/src/tendril/iotedge/announce.py` & `tendril_iotedge-0.3.2/src/tendril/iotedge/announce.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/src/tendril/iotedge/profiles/manager.py` & `tendril_iotedge-0.3.2/src/tendril/iotedge/profiles/manager.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/src/tendril/iotedge/registration.py` & `tendril_iotedge-0.3.2/src/tendril/iotedge/registration.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/PKG-INFO` & `tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-iotedge
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tendril IoT Edge Server Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-iotedge
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-iotedge.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-iotedge/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-iotedge
```

### Comparing `tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/SOURCES.txt` & `tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -37,19 +37,21 @@
 src/tendril/core/__init__.py
 src/tendril/core/topology/__init__.py
 src/tendril/core/topology/iotedge.py
 src/tendril/db/__init__.py
 src/tendril/db/models/__init__.py
 src/tendril/db/models/deviceconfig.py
 src/tendril/iotcore/__init__.py
+src/tendril/iotcore/logs.py
 src/tendril/iotcore/settings.py
 src/tendril/iotedge/__init__.py
 src/tendril/iotedge/announce.py
 src/tendril/iotedge/config.py
 src/tendril/iotedge/heartbeat.py
+src/tendril/iotedge/logs.py
 src/tendril/iotedge/registration.py
 src/tendril/iotedge/profiles/__init__.py
 src/tendril/iotedge/profiles/base.py
 src/tendril/iotedge/profiles/manager.py
 src/tendril_iotedge.egg-info/PKG-INFO
 src/tendril_iotedge.egg-info/SOURCES.txt
 src/tendril_iotedge.egg-info/dependency_links.txt
```

### Comparing `tendril_iotedge-0.3.1/src/tendril_iotedge.egg-info/requires.txt` & `tendril_iotedge-0.3.2/src/tendril_iotedge.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/tests/coveralls.py` & `tendril_iotedge-0.3.2/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.1/tox.ini` & `tendril_iotedge-0.3.2/tox.ini`

 * *Files identical despite different names*

