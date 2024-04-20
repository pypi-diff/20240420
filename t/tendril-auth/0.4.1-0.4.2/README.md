# Comparing `tmp/tendril_auth-0.4.1.tar.gz` & `tmp/tendril_auth-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril_auth-0.4.1.tar", last modified: Mon Apr 15 06:50:05 2024, max compression
+gzip compressed data, was "tendril_auth-0.4.2.tar", last modified: Sat Apr 20 00:25:32 2024, max compression
```

## Comparing `tendril_auth-0.4.1.tar` & `tendril_auth-0.4.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.991567 tendril_auth-0.4.1/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/MANIFEST.in
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5384 2024-04-15 06:50:05.987568 tendril_auth-0.4.1/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2144 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.971567 tendril_auth-0.4.1/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril_auth-0.4.1/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13454 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1518 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-15 06:50:05.991567 tendril_auth-0.4.1/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3286 2024-04-15 02:28:03.000000 tendril_auth-0.4.1/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.971567 tendril_auth-0.4.1/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril_auth-0.4.1/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril_auth-0.4.1/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1198 2024-04-08 19:39:52.000000 tendril_auth-0.4.1/src/tendril/apiserver/routers/authn.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2024-04-15 05:40:52.000000 tendril_auth-0.4.1/src/tendril/apiserver/routers/jwt.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.979567 tendril_auth-0.4.1/src/tendril/authn/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-16 14:15:27.000000 tendril_auth-0.4.1/src/tendril/authn/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6159 2024-04-09 12:57:03.000000 tendril_auth-0.4.1/src/tendril/authn/auth0.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1836 2023-04-21 09:10:22.000000 tendril_auth-0.4.1/src/tendril/authn/client.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.979567 tendril_auth-0.4.1/src/tendril/authn/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril_auth-0.4.1/src/tendril/authn/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2890 2023-02-28 04:21:34.000000 tendril_auth-0.4.1/src/tendril/authn/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      405 2022-12-10 17:21:52.000000 tendril_auth-0.4.1/src/tendril/authn/db/mixins.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1486 2022-12-09 17:58:03.000000 tendril_auth-0.4.1/src/tendril/authn/db/model.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1393 2023-04-21 12:28:51.000000 tendril_auth-0.4.1/src/tendril/authn/pydantic.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2945 2024-04-09 12:57:04.000000 tendril_auth-0.4.1/src/tendril/authn/users.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.979567 tendril_auth-0.4.1/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:30:01.000000 tendril_auth-0.4.1/src/tendril/authz/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1926 2023-09-12 04:42:42.000000 tendril_auth-0.4.1/src/tendril/authz/auth0.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      795 2023-02-28 00:24:44.000000 tendril_auth-0.4.1/src/tendril/authz/connector.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.983567 tendril_auth-0.4.1/src/tendril/authz/domains/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      245 2024-04-08 19:48:32.000000 tendril_auth-0.4.1/src/tendril/authz/domains/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      456 2024-04-15 05:12:04.000000 tendril_auth-0.4.1/src/tendril/authz/domains/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1218 2024-04-15 05:45:55.000000 tendril_auth-0.4.1/src/tendril/authz/domains/manager.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1094 2024-04-08 20:14:41.000000 tendril_auth-0.4.1/src/tendril/authz/domains/scopes.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.983567 tendril_auth-0.4.1/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:54:27.000000 tendril_auth-0.4.1/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      111 2023-02-28 00:52:46.000000 tendril_auth-0.4.1/src/tendril/authz/scopes/common.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1431 2024-04-10 20:39:39.000000 tendril_auth-0.4.1/src/tendril/authz/scopes/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.983567 tendril_auth-0.4.1/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril_auth-0.4.1/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3766 2024-04-15 05:50:52.000000 tendril_auth-0.4.1/src/tendril/config/auth.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.983567 tendril_auth-0.4.1/src/tendril/jwt/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-15 04:11:08.000000 tendril_auth-0.4.1/src/tendril/jwt/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      567 2024-04-15 05:56:45.000000 tendril_auth-0.4.1/src/tendril/jwt/secrets.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1093 2024-04-15 05:56:45.000000 tendril_auth-0.4.1/src/tendril/jwt/signer.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.983567 tendril_auth-0.4.1/src/tendril_auth.egg-info/
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5384 2024-04-15 06:50:05.000000 tendril_auth-0.4.1/src/tendril_auth.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1533 2024-04-15 06:50:05.000000 tendril_auth-0.4.1/src/tendril_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-15 06:50:05.000000 tendril_auth-0.4.1/src/tendril_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      604 2024-04-15 06:50:05.000000 tendril_auth-0.4.1/src/tendril_auth.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-15 06:50:05.000000 tendril_auth-0.4.1/src/tendril_auth.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.983567 tendril_auth-0.4.1/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.124229 tendril_auth-0.4.2/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5384 2024-04-20 00:25:32.124229 tendril_auth-0.4.2/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2144 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.096229 tendril_auth-0.4.2/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.100229 tendril_auth-0.4.2/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.100229 tendril_auth-0.4.2/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril_auth-0.4.2/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.100229 tendril_auth-0.4.2/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13454 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1518 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.100229 tendril_auth-0.4.2/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-20 00:25:32.124229 tendril_auth-0.4.2/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3286 2024-04-15 02:28:03.000000 tendril_auth-0.4.2/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.088229 tendril_auth-0.4.2/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.100229 tendril_auth-0.4.2/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.100229 tendril_auth-0.4.2/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril_auth-0.4.2/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.104229 tendril_auth-0.4.2/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril_auth-0.4.2/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1198 2024-04-08 19:39:52.000000 tendril_auth-0.4.2/src/tendril/apiserver/routers/authn.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2024-04-15 05:40:52.000000 tendril_auth-0.4.2/src/tendril/apiserver/routers/jwt.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.104229 tendril_auth-0.4.2/src/tendril/authn/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-16 14:15:27.000000 tendril_auth-0.4.2/src/tendril/authn/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6159 2024-04-17 22:29:06.000000 tendril_auth-0.4.2/src/tendril/authn/auth0.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1836 2023-04-21 09:10:22.000000 tendril_auth-0.4.2/src/tendril/authn/client.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.108229 tendril_auth-0.4.2/src/tendril/authn/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril_auth-0.4.2/src/tendril/authn/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2890 2023-02-28 04:21:34.000000 tendril_auth-0.4.2/src/tendril/authn/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      405 2022-12-10 17:21:52.000000 tendril_auth-0.4.2/src/tendril/authn/db/mixins.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1486 2022-12-09 17:58:03.000000 tendril_auth-0.4.2/src/tendril/authn/db/model.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1393 2023-04-21 12:28:51.000000 tendril_auth-0.4.2/src/tendril/authn/pydantic.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2945 2024-04-09 12:57:04.000000 tendril_auth-0.4.2/src/tendril/authn/users.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.108229 tendril_auth-0.4.2/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:30:01.000000 tendril_auth-0.4.2/src/tendril/authz/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1926 2023-09-12 04:42:42.000000 tendril_auth-0.4.2/src/tendril/authz/auth0.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      795 2023-02-28 00:24:44.000000 tendril_auth-0.4.2/src/tendril/authz/connector.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.112229 tendril_auth-0.4.2/src/tendril/authz/domains/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      245 2024-04-08 19:48:32.000000 tendril_auth-0.4.2/src/tendril/authz/domains/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      456 2024-04-15 05:12:04.000000 tendril_auth-0.4.2/src/tendril/authz/domains/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1218 2024-04-15 05:45:55.000000 tendril_auth-0.4.2/src/tendril/authz/domains/manager.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1094 2024-04-08 20:14:41.000000 tendril_auth-0.4.2/src/tendril/authz/domains/scopes.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.112229 tendril_auth-0.4.2/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:54:27.000000 tendril_auth-0.4.2/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      111 2023-02-28 00:52:46.000000 tendril_auth-0.4.2/src/tendril/authz/scopes/common.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1431 2024-04-10 20:39:39.000000 tendril_auth-0.4.2/src/tendril/authz/scopes/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.112229 tendril_auth-0.4.2/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril_auth-0.4.2/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3766 2024-04-15 05:50:52.000000 tendril_auth-0.4.2/src/tendril/config/auth.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.112229 tendril_auth-0.4.2/src/tendril/jwt/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-15 04:11:08.000000 tendril_auth-0.4.2/src/tendril/jwt/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      771 2024-04-20 00:25:06.000000 tendril_auth-0.4.2/src/tendril/jwt/secrets.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1093 2024-04-15 05:56:45.000000 tendril_auth-0.4.2/src/tendril/jwt/signer.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.116229 tendril_auth-0.4.2/src/tendril_auth.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5384 2024-04-20 00:25:31.000000 tendril_auth-0.4.2/src/tendril_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1533 2024-04-20 00:25:32.000000 tendril_auth-0.4.2/src/tendril_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-20 00:25:31.000000 tendril_auth-0.4.2/src/tendril_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      604 2024-04-20 00:25:31.000000 tendril_auth-0.4.2/src/tendril_auth.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-20 00:25:31.000000 tendril_auth-0.4.2/src/tendril_auth.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-20 00:25:32.116229 tendril_auth-0.4.2/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2021-08-13 17:52:37.000000 tendril_auth-0.4.2/tox.ini
```

### Comparing `tendril_auth-0.4.1/.gitignore` & `tendril_auth-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/.readthedocs.yml` & `tendril_auth-0.4.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/.travis.yml` & `tendril_auth-0.4.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/LICENSE` & `tendril_auth-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/PKG-INFO` & `tendril_auth-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-auth
-Version: 0.4.1
+Version: 0.4.2
 Summary: Authentication and User Management Core for Tendril
 Home-page: https://github.com/tendril-framework/tendril-auth
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-auth.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-auth/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-auth
```

### Comparing `tendril_auth-0.4.1/README.rst` & `tendril_auth-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/docs/Makefile` & `tendril_auth-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/docs/_static/custom.css` & `tendril_auth-0.4.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/docs/_static/favicon.ico` & `tendril_auth-0.4.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/docs/_static/logo.png` & `tendril_auth-0.4.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/docs/_static/logo_packed.png` & `tendril_auth-0.4.2/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/docs/_templates/about.html` & `tendril_auth-0.4.2/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/docs/conf.py` & `tendril_auth-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/docs/index.rst` & `tendril_auth-0.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/docs/installation.rst` & `tendril_auth-0.4.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/setup.py` & `tendril_auth-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/apiserver/routers/authn.py` & `tendril_auth-0.4.2/src/tendril/apiserver/routers/authn.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/apiserver/routers/jwt.py` & `tendril_auth-0.4.2/src/tendril/apiserver/routers/jwt.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/authn/auth0.py` & `tendril_auth-0.4.2/src/tendril/authn/auth0.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/authn/client.py` & `tendril_auth-0.4.2/src/tendril/authn/client.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/authn/db/controller.py` & `tendril_auth-0.4.2/src/tendril/authn/db/controller.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/authn/db/model.py` & `tendril_auth-0.4.2/src/tendril/authn/db/model.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/authn/pydantic.py` & `tendril_auth-0.4.2/src/tendril/authn/pydantic.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/authn/users.py` & `tendril_auth-0.4.2/src/tendril/authn/users.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/authz/auth0.py` & `tendril_auth-0.4.2/src/tendril/authz/auth0.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/authz/connector.py` & `tendril_auth-0.4.2/src/tendril/authz/connector.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/authz/domains/manager.py` & `tendril_auth-0.4.2/src/tendril/authz/domains/manager.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/authz/domains/scopes.py` & `tendril_auth-0.4.2/src/tendril/authz/domains/scopes.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/authz/scopes/manager.py` & `tendril_auth-0.4.2/src/tendril/authz/scopes/manager.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/config/__init__.py` & `tendril_auth-0.4.2/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/config/auth.py` & `tendril_auth-0.4.2/src/tendril/config/auth.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril/jwt/signer.py` & `tendril_auth-0.4.2/src/tendril/jwt/signer.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril_auth.egg-info/PKG-INFO` & `tendril_auth-0.4.2/src/tendril_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-auth
-Version: 0.4.1
+Version: 0.4.2
 Summary: Authentication and User Management Core for Tendril
 Home-page: https://github.com/tendril-framework/tendril-auth
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-auth.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-auth/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-auth
```

### Comparing `tendril_auth-0.4.1/src/tendril_auth.egg-info/SOURCES.txt` & `tendril_auth-0.4.2/src/tendril_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/src/tendril_auth.egg-info/requires.txt` & `tendril_auth-0.4.2/src/tendril_auth.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/tests/coveralls.py` & `tendril_auth-0.4.2/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril_auth-0.4.1/tox.ini` & `tendril_auth-0.4.2/tox.ini`

 * *Files identical despite different names*

