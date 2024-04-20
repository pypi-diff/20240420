# Comparing `tmp/tendril_iotedge-0.3.4.tar.gz` & `tmp/tendril_iotedge-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril_iotedge-0.3.4.tar", last modified: Sat Apr 20 03:07:02 2024, max compression
+gzip compressed data, was "tendril_iotedge-0.3.5.tar", last modified: Sat Apr 20 03:42:30 2024, max compression
```

## Comparing `tendril_iotedge-0.3.4.tar` & `tendril_iotedge-0.3.5.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.715129 tendril_iotedge-0.3.4/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/MANIFEST.in
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5353 2024-04-20 03:07:02.715129 tendril_iotedge-0.3.4/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.703129 tendril_iotedge-0.3.4/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.703129 tendril_iotedge-0.3.4/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-20 03:07:02.719129 tendril_iotedge-0.3.4/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3239 2024-04-20 02:03:45.000000 tendril_iotedge-0.3.4/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.703129 tendril_iotedge-0.3.4/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3075 2024-04-20 03:03:11.000000 tendril_iotedge-0.3.4/src/tendril/apiserver/routers/iotcore.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3424 2024-04-17 22:34:16.000000 tendril_iotedge-0.3.4/src/tendril/apiserver/routers/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/src/tendril/common/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-25 05:48:52.000000 tendril_iotedge-0.3.4/src/tendril/common/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      125 2023-07-25 05:51:28.000000 tendril_iotedge-0.3.4/src/tendril/common/iotcore/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril_iotedge-0.3.4/src/tendril/common/iotcore/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/src/tendril/common/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/src/tendril/common/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/src/tendril/common/iotedge/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      734 2023-08-30 15:08:09.000000 tendril_iotedge-0.3.4/src/tendril/common/iotedge/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1984 2024-04-20 01:19:25.000000 tendril_iotedge-0.3.4/src/tendril/config/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/src/tendril/core/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril_iotedge-0.3.4/src/tendril/core/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/src/tendril/core/topology/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril_iotedge-0.3.4/src/tendril/core/topology/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      339 2024-04-17 13:58:51.000000 tendril_iotedge-0.3.4/src/tendril/core/topology/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5595 2024-04-05 13:17:38.000000 tendril_iotedge-0.3.4/src/tendril/db/models/deviceconfig.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.707130 tendril_iotedge-0.3.4/src/tendril/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril_iotedge-0.3.4/src/tendril/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1031 2024-04-18 22:10:09.000000 tendril_iotedge-0.3.4/src/tendril/iotcore/logs.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1150 2024-04-17 22:01:55.000000 tendril_iotedge-0.3.4/src/tendril/iotcore/settings.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.711130 tendril_iotedge-0.3.4/src/tendril/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/src/tendril/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3085 2023-08-14 16:42:02.000000 tendril_iotedge-0.3.4/src/tendril/iotedge/announce.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-08-04 21:50:35.000000 tendril_iotedge-0.3.4/src/tendril/iotedge/config.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      444 2024-04-17 22:10:55.000000 tendril_iotedge-0.3.4/src/tendril/iotedge/heartbeat.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1205 2024-04-20 01:07:13.000000 tendril_iotedge-0.3.4/src/tendril/iotedge/logs.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.711130 tendril_iotedge-0.3.4/src/tendril/iotedge/profiles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/src/tendril/iotedge/profiles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4253 2024-04-20 01:20:25.000000 tendril_iotedge-0.3.4/src/tendril/iotedge/profiles/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4026 2023-07-28 16:44:25.000000 tendril_iotedge-0.3.4/src/tendril/iotedge/profiles/manager.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-08-12 07:26:08.000000 tendril_iotedge-0.3.4/src/tendril/iotedge/registration.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.711130 tendril_iotedge-0.3.4/src/tendril_iotedge.egg-info/
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5353 2024-04-20 03:07:02.000000 tendril_iotedge-0.3.4/src/tendril_iotedge.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1735 2024-04-20 03:07:02.000000 tendril_iotedge-0.3.4/src/tendril_iotedge.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-20 03:07:02.000000 tendril_iotedge-0.3.4/src/tendril_iotedge.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      583 2024-04-20 03:07:02.000000 tendril_iotedge-0.3.4/src/tendril_iotedge.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-20 03:07:02.000000 tendril_iotedge-0.3.4/src/tendril_iotedge.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:07:02.711130 tendril_iotedge-0.3.4/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.4/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.466407 tendril_iotedge-0.3.5/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5353 2024-04-20 03:42:30.466407 tendril_iotedge-0.3.5/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.446407 tendril_iotedge-0.3.5/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.450407 tendril_iotedge-0.3.5/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.450407 tendril_iotedge-0.3.5/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.450407 tendril_iotedge-0.3.5/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.450407 tendril_iotedge-0.3.5/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-20 03:42:30.466407 tendril_iotedge-0.3.5/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3239 2024-04-20 02:03:45.000000 tendril_iotedge-0.3.5/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.442407 tendril_iotedge-0.3.5/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.450407 tendril_iotedge-0.3.5/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.450407 tendril_iotedge-0.3.5/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.450407 tendril_iotedge-0.3.5/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3075 2024-04-20 03:03:11.000000 tendril_iotedge-0.3.5/src/tendril/apiserver/routers/iotcore.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3496 2024-04-20 03:35:51.000000 tendril_iotedge-0.3.5/src/tendril/apiserver/routers/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.450407 tendril_iotedge-0.3.5/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.454407 tendril_iotedge-0.3.5/src/tendril/common/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-25 05:48:52.000000 tendril_iotedge-0.3.5/src/tendril/common/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      125 2023-07-25 05:51:28.000000 tendril_iotedge-0.3.5/src/tendril/common/iotcore/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril_iotedge-0.3.5/src/tendril/common/iotcore/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.454407 tendril_iotedge-0.3.5/src/tendril/common/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/src/tendril/common/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/src/tendril/common/iotedge/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      734 2023-08-30 15:08:09.000000 tendril_iotedge-0.3.5/src/tendril/common/iotedge/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.454407 tendril_iotedge-0.3.5/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1984 2024-04-20 01:19:25.000000 tendril_iotedge-0.3.5/src/tendril/config/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.454407 tendril_iotedge-0.3.5/src/tendril/core/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril_iotedge-0.3.5/src/tendril/core/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.454407 tendril_iotedge-0.3.5/src/tendril/core/topology/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril_iotedge-0.3.5/src/tendril/core/topology/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      339 2024-04-17 13:58:51.000000 tendril_iotedge-0.3.5/src/tendril/core/topology/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.454407 tendril_iotedge-0.3.5/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.458407 tendril_iotedge-0.3.5/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5595 2024-04-05 13:17:38.000000 tendril_iotedge-0.3.5/src/tendril/db/models/deviceconfig.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.458407 tendril_iotedge-0.3.5/src/tendril/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril_iotedge-0.3.5/src/tendril/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1031 2024-04-18 22:10:09.000000 tendril_iotedge-0.3.5/src/tendril/iotcore/logs.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1150 2024-04-17 22:01:55.000000 tendril_iotedge-0.3.5/src/tendril/iotcore/settings.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.458407 tendril_iotedge-0.3.5/src/tendril/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/src/tendril/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3085 2023-08-14 16:42:02.000000 tendril_iotedge-0.3.5/src/tendril/iotedge/announce.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-08-04 21:50:35.000000 tendril_iotedge-0.3.5/src/tendril/iotedge/config.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      444 2024-04-17 22:10:55.000000 tendril_iotedge-0.3.5/src/tendril/iotedge/heartbeat.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1205 2024-04-20 01:07:13.000000 tendril_iotedge-0.3.5/src/tendril/iotedge/logs.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.462407 tendril_iotedge-0.3.5/src/tendril/iotedge/profiles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/src/tendril/iotedge/profiles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4253 2024-04-20 01:20:25.000000 tendril_iotedge-0.3.5/src/tendril/iotedge/profiles/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4026 2023-07-28 16:44:25.000000 tendril_iotedge-0.3.5/src/tendril/iotedge/profiles/manager.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-08-12 07:26:08.000000 tendril_iotedge-0.3.5/src/tendril/iotedge/registration.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.462407 tendril_iotedge-0.3.5/src/tendril_iotedge.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5353 2024-04-20 03:42:30.000000 tendril_iotedge-0.3.5/src/tendril_iotedge.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1735 2024-04-20 03:42:30.000000 tendril_iotedge-0.3.5/src/tendril_iotedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-20 03:42:30.000000 tendril_iotedge-0.3.5/src/tendril_iotedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      583 2024-04-20 03:42:30.000000 tendril_iotedge-0.3.5/src/tendril_iotedge.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-20 03:42:30.000000 tendril_iotedge-0.3.5/src/tendril_iotedge.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 03:42:30.462407 tendril_iotedge-0.3.5/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril_iotedge-0.3.5/tox.ini
```

### Comparing `tendril_iotedge-0.3.4/.gitignore` & `tendril_iotedge-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/.readthedocs.yml` & `tendril_iotedge-0.3.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/.travis.yml` & `tendril_iotedge-0.3.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/LICENSE` & `tendril_iotedge-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/PKG-INFO` & `tendril_iotedge-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-iotedge
-Version: 0.3.4
+Version: 0.3.5
 Summary: Tendril IoT Edge Server Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-iotedge
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-iotedge.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-iotedge/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-iotedge
```

### Comparing `tendril_iotedge-0.3.4/README.rst` & `tendril_iotedge-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/docs/Makefile` & `tendril_iotedge-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/docs/_static/custom.css` & `tendril_iotedge-0.3.5/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/docs/_static/favicon.ico` & `tendril_iotedge-0.3.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/docs/_static/logo.png` & `tendril_iotedge-0.3.5/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/docs/_static/logo_packed.png` & `tendril_iotedge-0.3.5/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/docs/_templates/about.html` & `tendril_iotedge-0.3.5/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/docs/conf.py` & `tendril_iotedge-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/docs/index.rst` & `tendril_iotedge-0.3.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/docs/installation.rst` & `tendril_iotedge-0.3.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/setup.py` & `tendril_iotedge-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril/apiserver/routers/iotcore.py` & `tendril_iotedge-0.3.5/src/tendril/apiserver/routers/iotcore.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril/apiserver/routers/iotedge.py` & `tendril_iotedge-0.3.5/src/tendril/apiserver/routers/iotedge.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,21 +72,23 @@
 
 
 @iotedge_router.post("/settings", response_model=device_config_unified_model)
 async def iot_device_settings(req: IoTDeviceSettingRequestTModel):
     result = get_config(device_id=req.id, appname=req.appname)
     return result
 
+
 @iotedge_router.post("/logs")
 async def iot_device_publish_logs(background_tasks: BackgroundTasks,
                                   file: UploadFile = File(...),
                                   user: AuthUserModel = auth_spec()):
     device_id = user.email.split('@')[0]
-    response = await publish_logs(device_id=device_id, logs_archive=file)
-    return "TODO"
+    response = await publish_logs(device_id=device_id, logs_archive=file,
+                                  background_tasks=background_tasks)
+    return response
 
 
 routers = []
 
 
 if IOTEDGE_API_ENABLED:
     routers.extend([
```

### Comparing `tendril_iotedge-0.3.4/src/tendril/common/iotedge/exceptions.py` & `tendril_iotedge-0.3.5/src/tendril/common/iotedge/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril/common/iotedge/formats.py` & `tendril_iotedge-0.3.5/src/tendril/common/iotedge/formats.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril/config/__init__.py` & `tendril_iotedge-0.3.5/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril/config/iotedge.py` & `tendril_iotedge-0.3.5/src/tendril/config/iotedge.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril/db/models/deviceconfig.py` & `tendril_iotedge-0.3.5/src/tendril/db/models/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril/iotcore/logs.py` & `tendril_iotedge-0.3.5/src/tendril/iotcore/logs.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril/iotcore/settings.py` & `tendril_iotedge-0.3.5/src/tendril/iotcore/settings.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril/iotedge/announce.py` & `tendril_iotedge-0.3.5/src/tendril/iotedge/announce.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril/iotedge/logs.py` & `tendril_iotedge-0.3.5/src/tendril/iotedge/logs.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril/iotedge/profiles/base.py` & `tendril_iotedge-0.3.5/src/tendril/iotedge/profiles/base.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril/iotedge/profiles/manager.py` & `tendril_iotedge-0.3.5/src/tendril/iotedge/profiles/manager.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril/iotedge/registration.py` & `tendril_iotedge-0.3.5/src/tendril/iotedge/registration.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril_iotedge.egg-info/PKG-INFO` & `tendril_iotedge-0.3.5/src/tendril_iotedge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-iotedge
-Version: 0.3.4
+Version: 0.3.5
 Summary: Tendril IoT Edge Server Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-iotedge
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-iotedge.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-iotedge/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-iotedge
```

### Comparing `tendril_iotedge-0.3.4/src/tendril_iotedge.egg-info/SOURCES.txt` & `tendril_iotedge-0.3.5/src/tendril_iotedge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/src/tendril_iotedge.egg-info/requires.txt` & `tendril_iotedge-0.3.5/src/tendril_iotedge.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/tests/coveralls.py` & `tendril_iotedge-0.3.5/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril_iotedge-0.3.4/tox.ini` & `tendril_iotedge-0.3.5/tox.ini`

 * *Files identical despite different names*

