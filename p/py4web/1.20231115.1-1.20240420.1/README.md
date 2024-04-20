# Comparing `tmp/py4web-1.20231115.1.tar.gz` & `tmp/py4web-1.20240420.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20231115.1.tar", last modified: Thu Nov 16 06:17:09 2023, max compression
+gzip compressed data, was "py4web-1.20240420.1.tar", last modified: Sat Apr 20 18:25:31 2024, max compression
```

## Comparing `py4web-1.20231115.1.tar` & `py4web-1.20240420.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2023-11-16 06:17:09.394271 py4web-1.20231115.1/
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20231115.1/LICENSE.md
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8186 2023-11-16 06:17:09.390938 py4web-1.20231115.1/PKG-INFO
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     7120 2023-05-08 00:39:42.000000 py4web-1.20231115.1/README.rst
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2023-11-16 06:17:09.370938 py4web-1.20231115.1/py4web/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      728 2023-11-16 06:16:02.000000 py4web-1.20231115.1/py4web/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2023-11-16 06:17:09.380938 py4web-1.20231115.1/py4web/assets/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990682 2023-11-16 06:16:49.000000 py4web-1.20231115.1/py4web/assets/py4web.app._dashboard.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   187155 2023-11-16 06:16:49.000000 py4web-1.20231115.1/py4web/assets/py4web.app._default.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4359741 2023-11-16 06:16:50.000000 py4web-1.20231115.1/py4web/assets/py4web.app._documentation.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2023-11-16 06:16:49.000000 py4web-1.20231115.1/py4web/assets/py4web.app._minimal.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21792 2023-11-16 06:16:49.000000 py4web-1.20231115.1/py4web/assets/py4web.app._scaffold.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1392657 2023-11-16 06:16:50.000000 py4web-1.20231115.1/py4web/assets/py4web.app.showcase.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    68556 2023-11-14 06:31:07.000000 py4web-1.20231115.1/py4web/core.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18251 2023-11-16 06:14:36.000000 py4web-1.20231115.1/py4web/server_adapters.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2023-11-16 06:17:09.387605 py4web-1.20231115.1/py4web/utils/
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72230 2023-11-16 06:14:36.000000 py4web-1.20231115.1/py4web/utils/auth.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2023-11-16 06:17:09.390938 py4web-1.20231115.1/py4web/utils/auth_plugins/
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     6207 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/__init__.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      798 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     1441 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)    35513 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/ldap_plugin.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2discord.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2facebook.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      513 2023-07-08 16:23:32.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2github.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2google.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)    11279 2023-10-08 22:03:44.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2google_scoped.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2okta.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     2084 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2server.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     6090 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     5051 2023-10-08 22:03:44.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/pam.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/pam_plugin.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     6672 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/saml2_plugin.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     2848 2023-10-08 22:03:44.000000 py4web-1.20231115.1/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/cors.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/dbstore.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2117 2023-10-29 18:38:28.000000 py4web-1.20231115.1/py4web/utils/downloader.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     3142 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/factories.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35877 2023-11-14 06:31:36.000000 py4web-1.20231115.1/py4web/utils/form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69277 2023-10-08 22:03:44.000000 py4web-1.20231115.1/py4web/utils/grid.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     1647 2023-07-08 16:23:33.000000 py4web-1.20231115.1/py4web/utils/jsonrpc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34764 2023-10-08 22:03:34.000000 py4web-1.20231115.1/py4web/utils/mailer.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     9196 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/misc.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/param.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)    18269 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/populate.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     1632 2023-11-12 21:25:17.000000 py4web-1.20231115.1/py4web/utils/publisher.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     2495 2023-07-08 16:23:33.000000 py4web-1.20231115.1/py4web/utils/recaptcha.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     3728 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/security.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      158 2023-05-08 00:39:45.000000 py4web-1.20231115.1/py4web/utils/tags.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     6546 2023-07-08 16:23:33.000000 py4web-1.20231115.1/py4web/utils/url_signer.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2023-11-16 06:17:09.374271 py4web-1.20231115.1/py4web.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8186 2023-11-16 06:17:09.000000 py4web-1.20231115.1/py4web.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2023-11-16 06:17:09.000000 py4web-1.20231115.1/py4web.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-11-16 06:17:09.000000 py4web-1.20231115.1/py4web.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2023-11-16 06:17:09.000000 py4web-1.20231115.1/py4web.egg-info/entry_points.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      239 2023-11-16 06:17:09.000000 py4web-1.20231115.1/py4web.egg-info/requires.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2023-11-16 06:17:09.000000 py4web-1.20231115.1/py4web.egg-info/top_level.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      843 2023-11-16 06:16:14.000000 py4web-1.20231115.1/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      466 2023-11-15 07:11:07.000000 py4web-1.20231115.1/requirements.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2023-11-16 06:17:09.394271 py4web-1.20231115.1/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2023-11-16 06:17:09.390938 py4web-1.20231115.1/tests/
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     3462 2023-11-14 06:31:07.000000 py4web-1.20231115.1/tests/test_action.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     8508 2023-05-08 00:39:45.000000 py4web-1.20231115.1/tests/test_auth.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20231115.1/tests/test_cache.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20231115.1/tests/test_fixture.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20231115.1/tests/test_form.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20231115.1/tests/test_get_error_snapshot.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20231115.1/tests/test_json.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20231115.1/tests/test_main.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20231115.1/tests/test_session.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20231115.1/tests/test_tags.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20231115.1/tests/test_template.py
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      392 2023-05-08 00:39:45.000000 py4web-1.20231115.1/tests/test_url.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 18:25:31.034379 py4web-1.20240420.1/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240420.1/LICENSE.md
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-04-20 18:25:31.034379 py4web-1.20240420.1/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7174 2024-04-19 07:21:20.000000 py4web-1.20240420.1/README.rst
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 18:25:31.001045 py4web-1.20240420.1/py4web/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      752 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 18:25:31.021046 py4web-1.20240420.1/py4web/assets/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990688 2024-04-20 18:25:23.000000 py4web-1.20240420.1/py4web/assets/py4web.app._dashboard.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   187155 2024-04-20 18:25:23.000000 py4web-1.20240420.1/py4web/assets/py4web.app._default.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4359741 2024-04-20 18:25:24.000000 py4web-1.20240420.1/py4web/assets/py4web.app._documentation.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-04-20 18:25:23.000000 py4web-1.20240420.1/py4web/assets/py4web.app._minimal.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21723 2024-04-20 18:25:23.000000 py4web-1.20240420.1/py4web/assets/py4web.app._scaffold.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1392768 2024-04-20 18:25:24.000000 py4web-1.20240420.1/py4web/assets/py4web.app.showcase.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    68412 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/core.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20383 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/server_adapters.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 18:25:31.027713 py4web-1.20240420.1/py4web/utils/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240420.1/py4web/utils/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72493 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/auth.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 18:25:31.031046 py4web-1.20240420.1/py4web/utils/auth_plugins/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6443 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2discord.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      670 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2github.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2google_scoped.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2okta.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2server.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5082 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/pam.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/pam_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2811 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240420.1/py4web/utils/cors.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/dbstore.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2102 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/downloader.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/factories.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35880 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69698 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/grid.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/jsonrpc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/mailer.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/misc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240420.1/py4web/utils/param.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/populate.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1567 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/publisher.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/recaptcha.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/security.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      124 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6578 2024-04-20 18:21:20.000000 py4web-1.20240420.1/py4web/utils/url_signer.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 18:25:31.001045 py4web-1.20240420.1/py4web.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7746 2024-04-20 18:25:30.000000 py4web-1.20240420.1/py4web.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-04-20 18:25:30.000000 py4web-1.20240420.1/py4web.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-04-20 18:25:30.000000 py4web-1.20240420.1/py4web.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-04-20 18:25:30.000000 py4web-1.20240420.1/py4web.egg-info/entry_points.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-04-20 18:25:30.000000 py4web-1.20240420.1/py4web.egg-info/requires.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-04-20 18:25:30.000000 py4web-1.20240420.1/py4web.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      843 2024-04-20 18:24:47.000000 py4web-1.20240420.1/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-04-20 18:21:20.000000 py4web-1.20240420.1/requirements.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-04-20 18:25:31.034379 py4web-1.20240420.1/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-20 18:25:31.034379 py4web-1.20240420.1/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3462 2023-11-14 06:31:07.000000 py4web-1.20240420.1/tests/test_action.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8508 2023-05-08 00:39:45.000000 py4web-1.20240420.1/tests/test_auth.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20240420.1/tests/test_cache.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20240420.1/tests/test_fixture.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20240420.1/tests/test_form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20240420.1/tests/test_get_error_snapshot.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20240420.1/tests/test_json.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20240420.1/tests/test_main.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20240420.1/tests/test_session.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20240420.1/tests/test_tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20240420.1/tests/test_template.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      440 2024-04-07 06:47:57.000000 py4web-1.20240420.1/tests/test_url.py
```

### Comparing `py4web-1.20231115.1/LICENSE.md` & `py4web-1.20240420.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/PKG-INFO` & `py4web-1.20240420.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,21 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20231115.1
+Version: 1.20240420.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
-Requires-Dist: wheel
-Requires-Dist: ombott>=1.0.0
-Requires-Dist: click
-Requires-Dist: colorama
-Requires-Dist: cryptography
-Requires-Dist: portalocker
-Requires-Dist: tornado
-Requires-Dist: renoir>=1.4.0
-Requires-Dist: requests
-Requires-Dist: threadsafevariable>=20230507.1
-Requires-Dist: pyjwt>=2.0.1
-Requires-Dist: pycryptodome
-Requires-Dist: pluralize>=20231008.1
-Requires-Dist: rocket3>=20230507.1
-Requires-Dist: yatl>=20230507.3
-Requires-Dist: pydal>=20231114.3
-Requires-Dist: watchgod>=0.6
 
 What is py4web?
 ===============
 
 .. image:: https://travis-ci.com/web2py/py4web.svg?branch=master
     :target: https://travis-ci.com/web2py/py4web
 
@@ -67,23 +50,23 @@
 Editing a database in the Dashboard
 
 .. image:: docs/images/dashboard_restapi.png
 
 Installation
 ############
 
-PY4WEB runs fine on Windows, MacOS and Linux. There are many installation procedures (see the official documentation for details) but only two of them are summarized here.
+PY4WEB runs fine on Windows, MacOS and Linux. There are many installation procedures `(see the official documentation for details) <https://py4web.com/_documentation/static/en/chapter-03.html>`__ but only two of them are summarized here.
 
 The **simplest way** to install py4web is using binaries, but it's only available for Windows and MacOS. It's meant especially for newbies or students, because it does not require Python pre-installed on your system nor administrative rights. You just need to download the latest Windows or MacOS ZIP file from `this external repository <https://github.com/nicozanf/py4web-pyinstaller>`__. Unzip it on a local folder and open a command line there. Finally run the commands (omit './' if you're using Windows)
 
 
 .. code:: bash
 
-   ./py4web-start set_password
-   ./py4web-start run apps
+   ./py4web set_password
+   ./py4web run apps
 
 
 
 
 The **standard installation procedure** for py4web on Windows, MacOS and Linux  is using pip. Its only prerequisite is Python 3.7+.
 
 .. code:: bash
```

### Comparing `py4web-1.20231115.1/README.rst` & `py4web-1.20240420.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -35,23 +35,23 @@
 Editing a database in the Dashboard
 
 .. image:: docs/images/dashboard_restapi.png
 
 Installation
 ############
 
-PY4WEB runs fine on Windows, MacOS and Linux. There are many installation procedures (see the official documentation for details) but only two of them are summarized here.
+PY4WEB runs fine on Windows, MacOS and Linux. There are many installation procedures `(see the official documentation for details) <https://py4web.com/_documentation/static/en/chapter-03.html>`__ but only two of them are summarized here.
 
 The **simplest way** to install py4web is using binaries, but it's only available for Windows and MacOS. It's meant especially for newbies or students, because it does not require Python pre-installed on your system nor administrative rights. You just need to download the latest Windows or MacOS ZIP file from `this external repository <https://github.com/nicozanf/py4web-pyinstaller>`__. Unzip it on a local folder and open a command line there. Finally run the commands (omit './' if you're using Windows)
 
 
 .. code:: bash
 
-   ./py4web-start set_password
-   ./py4web-start run apps
+   ./py4web set_password
+   ./py4web run apps
 
 
 
 
 The **standard installation procedure** for py4web on Windows, MacOS and Linux  is using pip. Its only prerequisite is Python 3.7+.
 
 .. code:: bash
```

### Comparing `py4web-1.20231115.1/py4web/__init__.py` & `py4web-1.20240420.1/py4web/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSD-3-Clause"
-__version__ = "1.20231115.1"
+__version__ = "1.20240420.1"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
 
@@ -19,9 +19,19 @@
 
 from .core import HTTP  # checks for version compatibility; bottle
 from .core import URL  # custom helper
 from .core import Field  # pydal
 from .core import Translator  # from pluralize
 from .core import action  # main py4web decorator
 from .core import render  # yatl
-from .core import (DAL, Cache, Condition, Flash, Session, abort,
-                   check_compatible, redirect, request, response)
+from .core import (
+    DAL,
+    Cache,
+    Condition,
+    Flash,
+    Session,
+    abort,
+    check_compatible,
+    redirect,
+    request,
+    response,
+)
```

### Comparing `py4web-1.20231115.1/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20240420.1/py4web/assets/py4web.app._dashboard.zip`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,380 +1,380 @@
-Zip file size: 2990682 bytes, number of entries: 378
--rw-r--r--  3.0 unx    20586 tx defN 23-Nov-12 03:56 __init__.py
--rw-rw-r--  3.0 unx     1141 tx defN 23-May-08 00:39 templates/ticket.html
--rw-rw-r--  3.0 unx     4760 tx defN 23-Nov-12 21:32 templates/gitlog.html
--rw-rw-r--  3.0 unx     2953 tx defN 23-Nov-12 21:32 templates/translations.html
--rw-rw-r--  3.0 unx    13851 tx defN 23-May-08 00:39 templates/index.html
--rw-rw-r--  3.0 unx      951 tx defN 23-Nov-12 21:32 templates/dbadmin.html
--rw-rw-r--  3.0 unx     3751 tx defN 23-May-22 05:34 utils.py
--rw-rw-r--  3.0 unx        1 tx stor 23-May-08 00:39 translations/README.md
--rw-rw-r--  3.0 unx     6493 tx defN 23-May-08 00:39 diff2kryten.py
--rw-rw-r--  3.0 unx    12182 tx defN 23-Nov-12 21:18 static/js/utils.js
--rw-rw-r--  3.0 unx      484 tx defN 23-May-08 00:39 static/js/dbadmin.js
--rw-rw-r--  3.0 unx     4881 tx defN 23-May-08 00:39 static/js/ace/mode-maze.js
--rw-rw-r--  3.0 unx     6476 tx defN 23-May-08 00:39 static/js/ace/theme-iplastic.js
--rw-rw-r--  3.0 unx     3024 tx defN 23-May-08 00:39 static/js/ace/mode-rst.js
--rw-rw-r--  3.0 unx     2812 tx defN 23-May-08 00:39 static/js/ace/theme-crimson_editor.js
--rw-rw-r--  3.0 unx    26620 tx defN 23-May-08 00:39 static/js/ace/mode-lsl.js
--rw-rw-r--  3.0 unx     8367 tx defN 23-May-08 00:39 static/js/ace/mode-prolog.js
--rw-rw-r--  3.0 unx     3189 tx defN 23-May-08 00:39 static/js/ace/mode-mipsassembler.js
--rw-rw-r--  3.0 unx     2432 tx defN 23-May-08 00:39 static/js/ace/theme-clouds_midnight.js
--rw-rw-r--  3.0 unx     8226 tx defN 23-May-08 00:39 static/js/ace/mode-dockerfile.js
--rw-rw-r--  3.0 unx     5665 tx defN 23-May-08 00:39 static/js/ace/mode-io.js
--rw-rw-r--  3.0 unx   470435 tx defN 23-May-08 00:39 static/js/ace/mode-php.js
--rw-rw-r--  3.0 unx    62955 tx defN 23-May-08 00:39 static/js/ace/mode-rhtml.js
--rw-rw-r--  3.0 unx    31151 tx defN 23-May-08 00:39 static/js/ace/mode-swig.js
--rw-rw-r--  3.0 unx    14198 tx defN 23-May-08 00:39 static/js/ace/mode-dart.js
--rw-rw-r--  3.0 unx     2842 tx defN 23-May-08 00:39 static/js/ace/theme-chaos.js
--rw-rw-r--  3.0 unx     2913 tx defN 23-May-08 00:39 static/js/ace/theme-terminal.js
--rw-rw-r--  3.0 unx    11847 tx defN 23-May-08 00:39 static/js/ace/mode-xml.js
--rw-rw-r--  3.0 unx     8159 tx defN 23-May-08 00:39 static/js/ace/mode-asciidoc.js
--rw-rw-r--  3.0 unx    55911 tx defN 23-May-08 00:39 static/js/ace/mode-pgsql.js
--rw-rw-r--  3.0 unx     8028 tx defN 23-May-08 00:39 static/js/ace/mode-clojure.js
--rw-rw-r--  3.0 unx        0 bx stor 23-May-08 00:39 static/js/ace/mode-text.js
--rw-rw-r--  3.0 unx     3031 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night_blue.js
--rw-rw-r--  3.0 unx     2313 tx defN 23-May-08 00:39 static/js/ace/mode-cobol.js
--rw-rw-r--  3.0 unx    47114 tx defN 23-May-08 00:39 static/js/ace/worker-lua.js
--rw-rw-r--  3.0 unx     2296 tx defN 23-May-08 00:39 static/js/ace/theme-kr_theme.js
--rw-rw-r--  3.0 unx     2791 tx defN 23-May-08 00:39 static/js/ace/theme-mono_industrial.js
--rw-rw-r--  3.0 unx     8898 tx defN 23-May-08 00:39 static/js/ace/mode-assembly_x86.js
--rw-rw-r--  3.0 unx     2499 tx defN 23-May-08 00:39 static/js/ace/theme-twilight.js
--rw-rw-r--  3.0 unx     4104 bx defN 23-May-08 00:39 static/js/ace/mode-c9search.js
--rw-rw-r--  3.0 unx    75093 tx defN 23-May-08 00:39 static/js/ace/mode-html_elixir.js
--rw-rw-r--  3.0 unx      506 tx defN 23-May-08 00:39 static/js/ace/mode-plain_text.js
--rw-rw-r--  3.0 unx    22440 tx defN 23-May-08 00:39 static/js/ace/mode-groovy.js
--rw-rw-r--  3.0 unx     2236 tx defN 23-May-08 00:39 static/js/ace/theme-merbivore.js
--rw-rw-r--  3.0 unx     2556 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow.js
--rw-rw-r--  3.0 unx     2761 tx defN 23-May-08 00:39 static/js/ace/mode-tex.js
--rw-rw-r--  3.0 unx    13008 tx defN 23-May-08 00:39 static/js/ace/mode-glsl.js
--rw-rw-r--  3.0 unx    66385 tx defN 23-May-08 00:39 static/js/ace/mode-soy_template.js
--rw-rw-r--  3.0 unx  1177601 tx defN 23-May-08 00:39 static/js/ace/worker-xquery.js
--rw-rw-r--  3.0 unx    61356 tx defN 23-May-08 00:39 static/js/ace/mode-smarty.js
--rw-rw-r--  3.0 unx     4559 tx defN 23-May-08 00:39 static/js/ace/mode-pascal.js
--rw-rw-r--  3.0 unx    29711 tx defN 23-May-08 00:39 static/js/ace/mode-erlang.js
--rw-rw-r--  3.0 unx    55541 tx defN 23-May-08 00:39 static/js/ace/worker-xml.js
--rw-rw-r--  3.0 unx    11468 tx defN 23-May-08 00:39 static/js/ace/mode-haskell.js
--rw-rw-r--  3.0 unx    30271 tx defN 23-May-08 00:39 static/js/ace/mode-liquid.js
--rw-rw-r--  3.0 unx     2088 tx defN 23-May-08 00:39 static/js/ace/mode-vhdl.js
--rw-rw-r--  3.0 unx    37225 tx defN 23-May-08 00:39 static/js/ace/mode-haml.js
--rw-rw-r--  3.0 unx     1099 tx defN 23-May-08 00:39 static/js/ace/mode-properties.js
--rw-rw-r--  3.0 unx     2375 tx defN 23-May-08 00:39 static/js/ace/theme-monokai.js
--rw-rw-r--  3.0 unx     6965 tx defN 23-May-08 00:39 static/js/ace/mode-jsx.js
--rw-rw-r--  3.0 unx    10785 tx defN 23-May-08 00:39 static/js/ace/mode-drools.js
--rw-rw-r--  3.0 unx     3840 tx defN 23-May-08 00:39 static/js/ace/ext-elastic_tabstops_lite.js
--rw-rw-r--  3.0 unx     2176 tx defN 23-May-08 00:39 static/js/ace/theme-github.js
--rw-rw-r--  3.0 unx    54512 tx defN 23-May-08 00:39 static/js/ace/mode-objectivec.js
--rw-rw-r--  3.0 unx     4193 tx defN 23-May-08 00:39 static/js/ace/ext-split.js
--rw-rw-r--  3.0 unx     4709 tx defN 23-May-08 00:39 static/js/ace/mode-abc.js
--rw-rw-r--  3.0 unx    34464 tx defN 23-May-08 00:39 static/js/ace/ext-language_tools.js
--rw-rw-r--  3.0 unx    12235 tx defN 23-May-08 00:39 static/js/ace/mode-stylus.js
--rw-rw-r--  3.0 unx     1088 tx defN 23-May-08 00:39 static/js/ace/ext-statusbar.js
--rw-rw-r--  3.0 unx     6540 tx defN 23-May-08 00:39 static/js/ace/mode-haxe.js
--rw-rw-r--  3.0 unx     2572 tx defN 23-May-08 00:39 static/js/ace/ext-whitespace.js
--rw-rw-r--  3.0 unx     1811 tx defN 23-May-08 00:39 static/js/ace/mode-sql.js
--rw-rw-r--  3.0 unx     3126 tx defN 23-May-08 00:39 static/js/ace/theme-katzenmilch.js
--rw-rw-r--  3.0 unx    21273 tx defN 23-May-08 00:39 static/js/ace/mode-sjs.js
--rw-rw-r--  3.0 unx     5073 tx defN 23-May-08 00:39 static/js/ace/mode-vbscript.js
--rw-rw-r--  3.0 unx     2380 tx defN 23-May-08 00:39 static/js/ace/mode-gherkin.js
--rw-rw-r--  3.0 unx    78297 tx defN 23-May-08 00:39 static/js/ace/worker-php.js
--rw-rw-r--  3.0 unx     7382 tx defN 23-May-08 00:39 static/js/ace/mode-perl.js
--rw-rw-r--  3.0 unx     2633 tx defN 23-May-08 00:39 static/js/ace/theme-pastel_on_dark.js
--rw-rw-r--  3.0 unx      899 tx defN 23-May-08 00:39 static/js/ace/mode-gitignore.js
--rw-rw-r--  3.0 unx    12293 tx defN 23-May-08 00:39 static/js/ace/ext-settings_menu.js
--rw-rw-r--  3.0 unx     3003 tx defN 23-May-08 00:39 static/js/ace/mode-cirru.js
--rw-rw-r--  3.0 unx    11914 tx defN 23-May-08 00:39 static/js/ace/ext-old_ie.js
--rw-rw-r--  3.0 unx    68741 tx defN 23-May-08 00:39 static/js/ace/mode-html_ruby.js
--rw-rw-r--  3.0 unx     1173 tx defN 23-May-08 00:39 static/js/ace/mode-lucene.js
--rw-rw-r--  3.0 unx    21478 tx defN 23-May-08 00:39 static/js/ace/ext-emmet.js
--rw-rw-r--  3.0 unx    64800 tx defN 23-May-08 00:39 static/js/ace/mode-markdown.js
--rw-rw-r--  3.0 unx     5712 tx defN 23-May-08 00:39 static/js/ace/mode-logiql.js
--rw-rw-r--  3.0 unx     3496 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night_bright.js
--rw-rw-r--  3.0 unx     2236 tx defN 23-May-08 00:39 static/js/ace/mode-space.js
--rw-rw-r--  3.0 unx     1464 tx defN 23-May-08 00:39 static/js/ace/mode-gcode.js
--rw-rw-r--  3.0 unx    10035 tx defN 23-May-08 00:39 static/js/ace/mode-nsis.js
--rw-rw-r--  3.0 unx     9112 tx defN 23-May-08 00:39 static/js/ace/ext-textarea.js
--rw-rw-r--  3.0 unx    13129 tx defN 23-May-08 00:39 static/js/ace/mode-nix.js
--rw-rw-r--  3.0 unx   230322 tx defN 23-May-08 00:39 static/js/ace/mode-xquery.js
--rw-rw-r--  3.0 unx     4856 tx defN 23-May-08 00:39 static/js/ace/mode-batchfile.js
--rw-rw-r--  3.0 unx    24939 tx defN 23-May-08 00:39 static/js/ace/mode-mel.js
--rw-rw-r--  3.0 unx    18060 tx defN 23-May-08 00:39 static/js/ace/mode-javascript.js
--rw-rw-r--  3.0 unx     5764 tx defN 23-May-08 00:39 static/js/ace/mode-jack.js
--rw-rw-r--  3.0 unx    59769 tx defN 23-May-08 00:39 static/js/ace/mode-handlebars.js
--rw-rw-r--  3.0 unx     6929 tx defN 23-May-08 00:39 static/js/ace/mode-swift.js
--rw-rw-r--  3.0 unx     2819 tx defN 23-May-08 00:39 static/js/ace/ext-static_highlight.js
--rw-rw-r--  3.0 unx     2081 tx defN 23-May-08 00:39 static/js/ace/theme-clouds.js
--rw-rw-r--  3.0 unx     6913 tx defN 23-May-08 00:39 static/js/ace/mode-golang.js
--rw-rw-r--  3.0 unx     6712 tx defN 23-May-08 00:39 static/js/ace/mode-mushcode.js
--rw-rw-r--  3.0 unx    20085 tx defN 23-May-08 00:39 static/js/ace/mode-less.js
--rw-rw-r--  3.0 unx     3640 tx defN 23-May-08 00:39 static/js/ace/ext-keybinding_menu.js
--rw-rw-r--  3.0 unx     5005 tx defN 23-May-08 00:39 static/js/ace/mode-r.js
--rw-rw-r--  3.0 unx     7189 tx defN 23-May-08 00:39 static/js/ace/mode-sh.js
--rw-rw-r--  3.0 unx    59262 tx defN 23-May-08 00:39 static/js/ace/mode-django.js
--rw-rw-r--  3.0 unx     3994 tx defN 23-May-08 00:39 static/js/ace/mode-rdoc.js
--rw-rw-r--  3.0 unx    34689 tx defN 23-May-08 00:39 static/js/ace/mode-jsp.js
--rw-rw-r--  3.0 unx     1470 tx defN 23-May-08 00:39 static/js/ace/ext-themelist.js
--rw-rw-r--  3.0 unx    10025 tx defN 23-May-08 00:39 static/js/ace/mode-ruby.js
--rw-rw-r--  3.0 unx     6523 tx defN 23-May-08 00:39 static/js/ace/mode-mysql.js
--rw-rw-r--  3.0 unx     2240 tx defN 23-May-08 00:39 static/js/ace/theme-dawn.js
--rw-rw-r--  3.0 unx    62630 tx defN 23-May-08 00:39 static/js/ace/mode-velocity.js
--rw-rw-r--  3.0 unx    21805 tx defN 23-May-08 00:39 static/js/ace/mode-java.js
--rw-rw-r--  3.0 unx     2087 tx defN 23-May-08 00:39 static/js/ace/mode-textile.js
--rw-rw-r--  3.0 unx    64984 tx defN 23-May-08 00:39 static/js/ace/mode-razor.js
--rw-rw-r--  3.0 unx      825 tx defN 23-May-08 00:39 static/js/ace/ext-linking.js
--rw-rw-r--  3.0 unx     2353 tx defN 23-May-08 00:39 static/js/ace/theme-cobalt.js
--rw-rw-r--  3.0 unx     7416 tx defN 23-May-08 00:39 static/js/ace/mode-coffee.js
--rw-rw-r--  3.0 unx    20269 tx defN 23-May-08 00:39 static/js/ace/mode-wollok.js
--rw-rw-r--  3.0 unx    63640 tx defN 23-May-08 00:39 static/js/ace/mode-autohotkey.js
--rw-rw-r--  3.0 unx     2125 tx defN 23-May-08 00:39 static/js/ace/theme-eclipse.js
--rw-rw-r--  3.0 unx     6989 tx defN 23-May-08 00:39 static/js/ace/mode-forth.js
--rw-rw-r--  3.0 unx     2712 tx defN 23-May-08 00:39 static/js/ace/theme-chrome.js
--rw-rw-r--  3.0 unx    20198 tx defN 23-May-08 00:39 static/js/ace/mode-typescript.js
--rw-rw-r--  3.0 unx    30624 tx defN 23-May-08 00:39 static/js/ace/mode-ftl.js
--rw-rw-r--  3.0 unx    11837 tx defN 23-May-08 00:39 static/js/ace/mode-kotlin.js
--rw-rw-r--  3.0 unx     6120 tx defN 23-May-08 00:39 static/js/ace/mode-tcl.js
--rw-rw-r--  3.0 unx    16578 tx defN 23-May-08 00:39 static/js/ace/mode-vala.js
--rw-rw-r--  3.0 unx   190654 tx defN 23-May-08 00:39 static/js/ace/worker-coffee.js
--rw-rw-r--  3.0 unx     2585 tx defN 23-May-08 00:39 static/js/ace/theme-textmate.js
--rw-rw-r--  3.0 unx    32692 tx defN 23-May-08 00:39 static/js/ace/mode-powershell.js
--rw-rw-r--  3.0 unx     3658 tx defN 23-May-08 00:39 static/js/ace/mode-scheme.js
--rw-rw-r--  3.0 unx    10840 tx defN 23-May-08 00:39 static/js/ace/mode-c_cpp.js
--rw-rw-r--  3.0 unx     5813 tx defN 23-May-08 00:39 static/js/ace/mode-abap.js
--rw-rw-r--  3.0 unx     2409 tx defN 23-May-08 00:39 static/js/ace/mode-diff.js
--rw-rw-r--  3.0 unx    13909 tx defN 23-May-08 00:39 static/js/ace/mode-apache_conf.js
--rw-rw-r--  3.0 unx    20567 tx defN 23-May-08 00:39 static/js/ace/mode-matlab.js
--rw-rw-r--  3.0 unx    60415 tx defN 23-May-08 00:39 static/js/ace/mode-coldfusion.js
--rw-rw-r--  3.0 unx     5097 tx defN 23-May-08 00:39 static/js/ace/mode-json.js
--rw-rw-r--  3.0 unx     8428 tx defN 23-May-08 00:39 static/js/ace/mode-fortran.js
--rw-rw-r--  3.0 unx    58909 tx defN 23-May-08 00:39 static/js/ace/mode-curly.js
--rw-rw-r--  3.0 unx    61525 tx defN 23-May-08 00:39 static/js/ace/mode-twig.js
--rw-rw-r--  3.0 unx   354781 tx defN 23-May-08 00:39 static/js/ace/ace.js
--rw-rw-r--  3.0 unx    96918 tx defN 23-May-08 00:39 static/js/ace/keybinding-vim.js
--rw-rw-r--  3.0 unx     5970 tx defN 23-May-08 00:39 static/js/ace/mode-hjson.js
--rw-rw-r--  3.0 unx    27779 tx defN 23-May-08 00:39 static/js/ace/theme-ambiance.js
--rw-rw-r--  3.0 unx    24465 tx defN 23-May-08 00:39 static/js/ace/keybinding-emacs.js
--rw-rw-r--  3.0 unx     1440 bx defN 23-May-08 00:39 static/js/ace/ext-spellcheck.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/julia.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/matlab.js
--rw-rw-r--  3.0 unx      132 tx defN 23-May-08 00:39 static/js/ace/snippets/protobuf.js
--rw-rw-r--  3.0 unx      128 tx defN 23-May-08 00:39 static/js/ace/snippets/hjson.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/coldfusion.js
--rw-rw-r--  3.0 unx     1975 tx defN 23-May-08 00:39 static/js/ace/snippets/haskell.js
--rw-rw-r--  3.0 unx      164 tx defN 23-May-08 00:39 static/js/ace/snippets/razor.js
--rw-rw-r--  3.0 unx      134 tx defN 23-May-08 00:39 static/js/ace/snippets/live_script.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ada.js
--rw-rw-r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/verilog.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/svg.js
--rw-rw-r--  3.0 unx     6763 tx defN 23-May-08 00:39 static/js/ace/snippets/php.js
--rw-rw-r--  3.0 unx     1716 tx defN 23-May-08 00:39 static/js/ace/snippets/xquery.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/golang.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/rhtml.js
--rw-rw-r--  3.0 unx     2055 tx defN 23-May-08 00:39 static/js/ace/snippets/sh.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/elixir.js
--rw-rw-r--  3.0 unx     2233 tx defN 23-May-08 00:39 static/js/ace/snippets/coffee.js
--rw-rw-r--  3.0 unx      198 tx defN 23-May-08 00:39 static/js/ace/snippets/makefile.js
--rw-rw-r--  3.0 unx      370 tx defN 23-May-08 00:39 static/js/ace/snippets/drools.js
--rw-rw-r--  3.0 unx     2630 tx defN 23-May-08 00:39 static/js/ace/snippets/r.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/haxe.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/ocaml.js
--rw-rw-r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/fortran.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/space.js
--rw-rw-r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/luapage.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/typescript.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/nix.js
--rw-rw-r--  3.0 unx      947 tx defN 23-May-08 00:39 static/js/ace/snippets/abc.js
--rw-rw-r--  3.0 unx      448 tx defN 23-May-08 00:39 static/js/ace/snippets/haml.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/stylus.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/praat.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/mask.js
--rw-rw-r--  3.0 unx     2778 tx defN 23-May-08 00:39 static/js/ace/snippets/jsp.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/swig.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/lean.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/logiql.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/json.js
--rw-rw-r--  3.0 unx    21279 tx defN 23-May-08 00:39 static/js/ace/snippets/ruby.js
--rw-rw-r--  3.0 unx     4322 tx defN 23-May-08 00:39 static/js/ace/snippets/java.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/forth.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/scad.js
--rw-rw-r--  3.0 unx    35423 tx defN 23-May-08 00:39 static/js/ace/snippets/lsl.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/cirru.js
--rw-rw-r--  3.0 unx     3636 tx defN 23-May-08 00:39 static/js/ace/snippets/tex.js
--rw-rw-r--  3.0 unx     1319 tx defN 23-May-08 00:39 static/js/ace/snippets/dart.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/xml.js
--rw-rw-r--  3.0 unx      126 tx defN 23-May-08 00:39 static/js/ace/snippets/bro.js
--rw-rw-r--  3.0 unx      141 tx defN 23-May-08 00:39 static/js/ace/snippets/gitignore.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/jack.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/cobol.js
--rw-rw-r--  3.0 unx      270 tx defN 23-May-08 00:39 static/js/ace/snippets/maze.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ejs.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/text.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/prolog.js
--rw-rw-r--  3.0 unx      141 tx defN 23-May-08 00:39 static/js/ace/snippets/html_ruby.js
--rw-rw-r--  3.0 unx      540 tx defN 23-May-08 00:39 static/js/ace/snippets/textile.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/glsl.js
--rw-rw-r--  3.0 unx     1690 tx defN 23-May-08 00:39 static/js/ace/snippets/tcl.js
--rw-rw-r--  3.0 unx      151 tx defN 23-May-08 00:39 static/js/ace/snippets/mips_assembler.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ftl.js
--rw-rw-r--  3.0 unx      136 tx defN 23-May-08 00:39 static/js/ace/snippets/mipsassembler.js
--rw-rw-r--  3.0 unx      145 tx defN 23-May-08 00:39 static/js/ace/snippets/html_elixir.js
--rw-rw-r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/asciidoc.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/gcode.js
--rw-rw-r--  3.0 unx     3574 tx defN 23-May-08 00:39 static/js/ace/snippets/erlang.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/smarty.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/powershell.js
--rw-rw-r--  3.0 unx    19650 tx defN 23-May-08 00:39 static/js/ace/snippets/css.js
--rw-rw-r--  3.0 unx     5513 tx defN 23-May-08 00:39 static/js/ace/snippets/perl.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/jade.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/vhdl.js
--rw-rw-r--  3.0 unx     4000 tx defN 23-May-08 00:39 static/js/ace/snippets/django.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/csharp.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/latex.js
--rw-rw-r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/c9search.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/less.js
--rw-rw-r--  3.0 unx     1973 tx defN 23-May-08 00:39 static/js/ace/snippets/markdown.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/livescript.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/swift.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/jsx.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/handlebars.js
--rw-rw-r--  3.0 unx     2139 tx defN 23-May-08 00:39 static/js/ace/snippets/sqlserver.js
--rw-rw-r--  3.0 unx      125 tx defN 23-May-08 00:39 static/js/ace/snippets/d.js
--rw-rw-r--  3.0 unx      508 tx defN 23-May-08 00:39 static/js/ace/snippets/lua.js
--rw-rw-r--  3.0 unx      297 tx defN 23-May-08 00:39 static/js/ace/snippets/snippets.js
--rw-rw-r--  3.0 unx      145 tx defN 23-May-08 00:39 static/js/ace/snippets/apache_conf.js
--rw-rw-r--  3.0 unx     2040 tx defN 23-May-08 00:39 static/js/ace/snippets/clojure.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/autohotkey.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/plain_text.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/lisp.js
--rw-rw-r--  3.0 unx      145 tx defN 23-May-08 00:39 static/js/ace/snippets/applescript.js
--rw-rw-r--  3.0 unx      651 tx defN 23-May-08 00:39 static/js/ace/snippets/velocity.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/dockerfile.js
--rw-rw-r--  3.0 unx     2973 tx defN 23-May-08 00:39 static/js/ace/snippets/actionscript.js
--rw-rw-r--  3.0 unx     3127 tx defN 23-May-08 00:39 static/js/ace/snippets/vala.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/elm.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/tsx.js
--rw-rw-r--  3.0 unx     1219 tx defN 23-May-08 00:39 static/js/ace/snippets/io.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/objectivec.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/yaml.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/pascal.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/curly.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/scss.js
--rw-rw-r--  3.0 unx     3840 tx defN 23-May-08 00:39 static/js/ace/snippets/javascript.js
--rw-rw-r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/mushcode.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/mel.js
--rw-rw-r--  3.0 unx      149 tx defN 23-May-08 00:39 static/js/ace/snippets/haskell_cabal.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/mysql.js
--rw-rw-r--  3.0 unx      942 tx defN 23-May-08 00:39 static/js/ace/snippets/sql.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/lucene.js
--rw-rw-r--  3.0 unx     1263 tx defN 23-May-08 00:39 static/js/ace/snippets/wollok.js
--rw-rw-r--  3.0 unx      141 tx defN 23-May-08 00:39 static/js/ace/snippets/batchfile.js
--rw-rw-r--  3.0 unx     3672 tx defN 23-May-08 00:39 static/js/ace/snippets/python.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/rust.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ini.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/dot.js
--rw-rw-r--  3.0 unx      442 tx defN 23-May-08 00:39 static/js/ace/snippets/rst.js
--rw-rw-r--  3.0 unx      127 tx defN 23-May-08 00:39 static/js/ace/snippets/nsis.js
--rw-rw-r--  3.0 unx     1716 tx defN 23-May-08 00:39 static/js/ace/snippets/jsoniq.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/properties.js
--rw-rw-r--  3.0 unx     2663 tx defN 23-May-08 00:39 static/js/ace/snippets/c_cpp.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/kotlin.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/toml.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/scheme.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/twig.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/abap.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/sass.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/eiffel.js
--rw-rw-r--  3.0 unx      607 tx defN 23-May-08 00:39 static/js/ace/snippets/gobstones.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/scala.js
--rw-rw-r--  3.0 unx      551 tx defN 23-May-08 00:39 static/js/ace/snippets/diff.js
--rw-rw-r--  3.0 unx      147 tx defN 23-May-08 00:39 static/js/ace/snippets/assembly_x86.js
--rw-rw-r--  3.0 unx    18271 tx defN 23-May-08 00:39 static/js/ace/snippets/html.js
--rw-rw-r--  3.0 unx      147 tx defN 23-May-08 00:39 static/js/ace/snippets/soy_template.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/liquid.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/rdoc.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/sjs.js
--rw-rw-r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/gherkin.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/groovy.js
--rw-rw-r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/vbscript.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/pgsql.js
--rw-rw-r--  3.0 unx     5959 tx defN 23-May-08 00:39 static/js/ace/mode-mips_assembler.js
--rw-rw-r--  3.0 unx    18046 tx defN 23-May-08 00:39 static/js/ace/mode-css.js
--rw-rw-r--  3.0 unx   232939 tx defN 23-May-08 00:39 static/js/ace/mode-jsoniq.js
--rw-rw-r--  3.0 unx     4933 tx defN 23-May-08 00:39 static/js/ace/mode-elm.js
--rw-rw-r--  3.0 unx     2844 tx defN 23-May-08 00:39 static/js/ace/mode-eiffel.js
--rw-rw-r--  3.0 unx    12546 tx defN 23-May-08 00:39 static/js/ace/mode-protobuf.js
--rw-rw-r--  3.0 unx     1762 tx defN 23-May-08 00:39 static/js/ace/mode-ada.js
--rw-rw-r--  3.0 unx     6554 tx defN 23-May-08 00:39 static/js/ace/mode-makefile.js
--rw-rw-r--  3.0 unx    68412 tx defN 23-May-08 00:39 static/js/ace/mode-ejs.js
--rw-rw-r--  3.0 unx     3138 tx defN 23-May-08 00:39 static/js/ace/theme-dreamweaver.js
--rw-rw-r--  3.0 unx    15753 tx defN 23-May-08 00:39 static/js/ace/mode-elixir.js
--rw-rw-r--  3.0 unx    10005 tx defN 23-May-08 00:39 static/js/ace/ext-searchbox.js
--rw-rw-r--  3.0 unx     2204 tx defN 23-May-08 00:39 static/js/ace/mode-toml.js
--rw-rw-r--  3.0 unx    22619 tx defN 23-May-08 00:39 static/js/ace/mode-scala.js
--rw-rw-r--  3.0 unx    66336 tx defN 23-May-08 00:39 static/js/ace/mode-luapage.js
--rw-rw-r--  3.0 unx     6360 tx defN 23-May-08 00:39 static/js/ace/ext-chromevox.js
--rw-rw-r--  3.0 unx      140 tx defN 23-May-08 00:39 static/js/ace/ext-error_marker.js
--rw-rw-r--  3.0 unx     4681 tx defN 23-May-08 00:39 static/js/ace/mode-python.js
--rw-rw-r--  3.0 unx    20332 tx defN 23-May-08 00:39 static/js/ace/mode-gobstones.js
--rw-rw-r--  3.0 unx    10260 tx defN 23-May-08 00:39 static/js/ace/mode-praat.js
--rw-rw-r--  3.0 unx     6520 tx defN 23-May-08 00:39 static/js/ace/mode-scad.js
--rw-rw-r--  3.0 unx     2448 tx defN 23-May-08 00:39 static/js/ace/theme-merbivore_soft.js
--rw-rw-r--  3.0 unx     6211 tx defN 23-May-08 00:39 static/js/ace/mode-bro.js
--rw-rw-r--  3.0 unx     2892 tx defN 23-May-08 00:39 static/js/ace/theme-sqlserver.js
--rw-rw-r--  3.0 unx    20510 tx defN 23-May-08 00:39 static/js/ace/mode-tsx.js
--rw-rw-r--  3.0 unx     3874 tx defN 23-May-08 00:39 static/js/ace/mode-latex.js
--rw-rw-r--  3.0 unx     3994 tx defN 23-May-08 00:39 static/js/ace/mode-yaml.js
--rw-rw-r--  3.0 unx     2820 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night.js
--rw-rw-r--  3.0 unx    49991 tx defN 23-May-08 00:39 static/js/ace/mode-jade.js
--rw-rw-r--  3.0 unx     2689 tx defN 23-May-08 00:39 static/js/ace/mode-verilog.js
--rw-rw-r--  3.0 unx     3729 tx defN 23-May-08 00:39 static/js/ace/ext-modelist.js
--rw-rw-r--  3.0 unx     1918 tx defN 23-May-08 00:39 static/js/ace/theme-xcode.js
--rw-rw-r--  3.0 unx    10220 tx defN 23-May-08 00:39 static/js/ace/mode-sass.js
--rw-rw-r--  3.0 unx    19962 tx defN 23-May-08 00:39 static/js/ace/mode-live_script.js
--rw-rw-r--  3.0 unx   217401 tx defN 23-May-08 00:39 static/js/ace/worker-html.js
--rw-rw-r--  3.0 unx     2054 tx defN 23-May-08 00:39 static/js/ace/theme-kuroir.js
--rw-rw-r--  3.0 unx    31988 tx defN 23-May-08 00:39 static/js/ace/mode-svg.js
--rw-rw-r--  3.0 unx     3221 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night_eighties.js
--rw-rw-r--  3.0 unx     5399 tx defN 23-May-08 00:39 static/js/ace/mode-applescript.js
--rw-rw-r--  3.0 unx     2282 tx defN 23-May-08 00:39 static/js/ace/mode-haskell_cabal.js
--rw-rw-r--  3.0 unx     5576 tx defN 23-May-08 00:39 static/js/ace/mode-lean.js
--rw-rw-r--  3.0 unx     6495 tx defN 23-May-08 00:39 static/js/ace/mode-rust.js
--rw-rw-r--  3.0 unx     7595 tx defN 23-May-08 00:39 static/js/ace/mode-dot.js
--rw-rw-r--  3.0 unx    12951 tx defN 23-May-08 00:39 static/js/ace/mode-scss.js
--rw-rw-r--  3.0 unx    57890 tx defN 23-May-08 00:39 static/js/ace/mode-html.js
--rw-rw-r--  3.0 unx    20545 tx defN 23-May-08 00:39 static/js/ace/mode-actionscript.js
--rw-rw-r--  3.0 unx    16415 tx defN 23-May-08 00:39 static/js/ace/mode-sqlserver.js
--rw-rw-r--  3.0 unx     2360 tx defN 23-May-08 00:39 static/js/ace/theme-solarized_light.js
--rw-rw-r--  3.0 unx    40358 tx defN 23-May-08 00:39 static/js/ace/mode-mask.js
--rw-rw-r--  3.0 unx    15600 tx defN 23-May-08 00:39 static/js/ace/mode-ocaml.js
--rw-rw-r--  3.0 unx     8947 tx defN 23-May-08 00:39 static/js/ace/mode-d.js
--rw-rw-r--  3.0 unx     7283 tx defN 23-May-08 00:39 static/js/ace/mode-lua.js
--rw-rw-r--  3.0 unx   164518 tx defN 23-May-08 00:39 static/js/ace/worker-javascript.js
--rw-rw-r--  3.0 unx     2710 tx defN 23-May-08 00:39 static/js/ace/mode-ini.js
--rw-rw-r--  3.0 unx     2312 tx defN 23-May-08 00:39 static/js/ace/theme-solarized_dark.js
--rw-rw-r--  3.0 unx     3687 tx defN 23-May-08 00:39 static/js/ace/mode-snippets.js
--rw-rw-r--  3.0 unx     4984 tx defN 23-May-08 00:39 static/js/ace/mode-livescript.js
--rw-rw-r--  3.0 unx     2248 tx defN 23-May-08 00:39 static/js/ace/theme-idle_fingers.js
--rw-rw-r--  3.0 unx     2204 tx defN 23-May-08 00:39 static/js/ace/theme-vibrant_ink.js
--rw-rw-r--  3.0 unx   140879 tx defN 23-May-08 00:39 static/js/ace/worker-css.js
--rw-rw-r--  3.0 unx    32911 tx defN 23-May-08 00:39 static/js/ace/worker-json.js
--rw-rw-r--  3.0 unx     1961 tx defN 23-May-08 00:39 static/js/ace/mode-lisp.js
--rw-rw-r--  3.0 unx     8840 tx defN 23-May-08 00:39 static/js/ace/mode-csharp.js
--rw-rw-r--  3.0 unx     3818 tx defN 23-May-08 00:39 static/js/ace/ext-beautify.js
--rw-rw-r--  3.0 unx     7539 tx defN 23-May-08 00:39 static/js/ace/mode-julia.js
--rw-r--r--  3.0 unx    88145 tx defN 23-Nov-12 21:45 static/js/jquery.min.js
--rw-rw-r--  3.0 unx    68547 tx defN 23-May-08 00:39 static/js/sugar.min.js
--rw-r--r--  3.0 unx    10461 tx defN 23-Nov-12 21:19 static/js/index.js
--rw-rw-r--  3.0 unx    95432 tx defN 23-May-08 00:39 static/js/highlight.min.js
--rw-rw-r--  3.0 unx     3354 tx defN 23-Nov-12 21:29 static/js/translations.js
--rw-rw-r--  3.0 unx    93670 tx defN 23-May-08 00:39 static/js/vue.min.js
+Zip file size: 2990688 bytes, number of entries: 378
+-rw-r--r--  3.0 unx     6493 tx defN 23-May-08 00:39 diff2kryten.py
+-rw-r--r--  3.0 unx    20588 tx defN 24-Apr-19 07:21 __init__.py
+-rw-r--r--  3.0 unx     3751 tx defN 23-May-22 05:34 utils.py
+-rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 translations/README.md
+-rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
+-rw-r--r--  3.0 unx    12025 bx defN 23-May-08 00:39 static/images/alert-red.gif
+-rw-r--r--  3.0 unx     7927 bx defN 23-May-08 00:39 static/images/forkme.png
+-rw-r--r--  3.0 unx    12305 bx defN 23-May-08 00:39 static/images/alert-blue.gif
+-rw-r--r--  3.0 unx  1010153 bx defN 23-May-08 00:39 static/images/widget.gif
+-rw-r--r--  3.0 unx    13366 bx defN 23-May-08 00:39 static/images/alert-orange.gif
+-rw-r--r--  3.0 unx    11068 bx defN 23-May-08 00:39 static/images/alert-green.gif
+-rw-r--r--  3.0 unx    13380 bx defN 23-May-08 00:39 static/images/alert-yellow.gif
+-rw-r--r--  3.0 unx     5926 tx defN 23-May-08 00:39 static/css/future.css
+-rw-r--r--  3.0 unx      708 tx defN 23-May-08 00:39 static/css/gitlog.min.css
+-rw-r--r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components/mtable.html
 -rw-r--r--  3.0 unx     8104 tx defN 23-Nov-12 21:24 static/components/mtable.js
--rw-rw-r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components/mtable.html
--rw-rw-r--  3.0 unx     5926 tx defN 23-May-08 00:39 static/css/future.css
--rw-rw-r--  3.0 unx      708 tx defN 23-May-08 00:39 static/css/gitlog.min.css
--rw-rw-r--  3.0 unx    12305 bx defN 23-May-08 00:39 static/images/alert-blue.gif
--rw-rw-r--  3.0 unx    12025 bx defN 23-May-08 00:39 static/images/alert-red.gif
--rw-rw-r--  3.0 unx    13380 bx defN 23-May-08 00:39 static/images/alert-yellow.gif
--rw-rw-r--  3.0 unx     7927 bx defN 23-May-08 00:39 static/images/forkme.png
--rw-rw-r--  3.0 unx  1010153 bx defN 23-May-08 00:39 static/images/widget.gif
--rw-rw-r--  3.0 unx    13366 bx defN 23-May-08 00:39 static/images/alert-orange.gif
--rw-rw-r--  3.0 unx    11068 bx defN 23-May-08 00:39 static/images/alert-green.gif
--rw-rw-r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
-378 files, 8005825 bytes uncompressed, 2919896 bytes compressed:  63.5%
+-rw-r--r--  3.0 unx    10486 tx defN 23-Dec-28 07:17 static/js/index.js
+-rw-r--r--  3.0 unx    93670 tx defN 23-May-08 00:39 static/js/vue.min.js
+-rw-r--r--  3.0 unx     7189 tx defN 23-May-08 00:39 static/js/ace/mode-sh.js
+-rw-r--r--  3.0 unx     3874 tx defN 23-May-08 00:39 static/js/ace/mode-latex.js
+-rw-r--r--  3.0 unx    55541 tx defN 23-May-08 00:39 static/js/ace/worker-xml.js
+-rw-r--r--  3.0 unx    16415 tx defN 23-May-08 00:39 static/js/ace/mode-sqlserver.js
+-rw-r--r--  3.0 unx    54512 tx defN 23-May-08 00:39 static/js/ace/mode-objectivec.js
+-rw-r--r--  3.0 unx     6211 tx defN 23-May-08 00:39 static/js/ace/mode-bro.js
+-rw-r--r--  3.0 unx    20269 tx defN 23-May-08 00:39 static/js/ace/mode-wollok.js
+-rw-r--r--  3.0 unx     5073 tx defN 23-May-08 00:39 static/js/ace/mode-vbscript.js
+-rw-r--r--  3.0 unx    24465 tx defN 23-May-08 00:39 static/js/ace/keybinding-emacs.js
+-rw-r--r--  3.0 unx    10840 tx defN 23-May-08 00:39 static/js/ace/mode-c_cpp.js
+-rw-r--r--  3.0 unx    18046 tx defN 23-May-08 00:39 static/js/ace/mode-css.js
+-rw-r--r--  3.0 unx    30624 tx defN 23-May-08 00:39 static/js/ace/mode-ftl.js
+-rw-r--r--  3.0 unx   217401 tx defN 23-May-08 00:39 static/js/ace/worker-html.js
+-rw-r--r--  3.0 unx    78297 tx defN 23-May-08 00:39 static/js/ace/worker-php.js
+-rw-r--r--  3.0 unx     4933 tx defN 23-May-08 00:39 static/js/ace/mode-elm.js
+-rw-r--r--  3.0 unx     6913 tx defN 23-May-08 00:39 static/js/ace/mode-golang.js
+-rw-r--r--  3.0 unx    18060 tx defN 23-May-08 00:39 static/js/ace/mode-javascript.js
+-rw-r--r--  3.0 unx    15600 tx defN 23-May-08 00:39 static/js/ace/mode-ocaml.js
+-rw-r--r--  3.0 unx     8898 tx defN 23-May-08 00:39 static/js/ace/mode-assembly_x86.js
+-rw-r--r--  3.0 unx     2312 tx defN 23-May-08 00:39 static/js/ace/theme-solarized_dark.js
+-rw-r--r--  3.0 unx  1177601 tx defN 23-May-08 00:39 static/js/ace/worker-xquery.js
+-rw-r--r--  3.0 unx     8947 tx defN 23-May-08 00:39 static/js/ace/mode-d.js
+-rw-r--r--  3.0 unx     8428 tx defN 23-May-08 00:39 static/js/ace/mode-fortran.js
+-rw-r--r--  3.0 unx     8367 tx defN 23-May-08 00:39 static/js/ace/mode-prolog.js
+-rw-r--r--  3.0 unx     5712 tx defN 23-May-08 00:39 static/js/ace/mode-logiql.js
+-rw-r--r--  3.0 unx     2499 tx defN 23-May-08 00:39 static/js/ace/theme-twilight.js
+-rw-r--r--  3.0 unx     7416 tx defN 23-May-08 00:39 static/js/ace/mode-coffee.js
+-rw-r--r--  3.0 unx    12293 tx defN 23-May-08 00:39 static/js/ace/ext-settings_menu.js
+-rw-r--r--  3.0 unx     2088 tx defN 23-May-08 00:39 static/js/ace/mode-vhdl.js
+-rw-r--r--  3.0 unx     2236 tx defN 23-May-08 00:39 static/js/ace/mode-space.js
+-rw-r--r--  3.0 unx     2844 tx defN 23-May-08 00:39 static/js/ace/mode-eiffel.js
+-rw-r--r--  3.0 unx    68412 tx defN 23-May-08 00:39 static/js/ace/mode-ejs.js
+-rw-r--r--  3.0 unx     2448 tx defN 23-May-08 00:39 static/js/ace/theme-merbivore_soft.js
+-rw-r--r--  3.0 unx     2204 tx defN 23-May-08 00:39 static/js/ace/mode-toml.js
+-rw-r--r--  3.0 unx     6712 tx defN 23-May-08 00:39 static/js/ace/mode-mushcode.js
+-rw-r--r--  3.0 unx     1440 bx defN 23-May-08 00:39 static/js/ace/ext-spellcheck.js
+-rw-r--r--  3.0 unx      506 tx defN 23-May-08 00:39 static/js/ace/mode-plain_text.js
+-rw-r--r--  3.0 unx     2892 tx defN 23-May-08 00:39 static/js/ace/theme-sqlserver.js
+-rw-r--r--  3.0 unx     1173 tx defN 23-May-08 00:39 static/js/ace/mode-lucene.js
+-rw-r--r--  3.0 unx     3840 tx defN 23-May-08 00:39 static/js/ace/ext-elastic_tabstops_lite.js
+-rw-r--r--  3.0 unx    34464 tx defN 23-May-08 00:39 static/js/ace/ext-language_tools.js
+-rw-r--r--  3.0 unx    11468 tx defN 23-May-08 00:39 static/js/ace/mode-haskell.js
+-rw-r--r--  3.0 unx    62630 tx defN 23-May-08 00:39 static/js/ace/mode-velocity.js
+-rw-r--r--  3.0 unx    13909 tx defN 23-May-08 00:39 static/js/ace/mode-apache_conf.js
+-rw-r--r--  3.0 unx     4881 tx defN 23-May-08 00:39 static/js/ace/mode-maze.js
+-rw-r--r--  3.0 unx    12235 tx defN 23-May-08 00:39 static/js/ace/mode-stylus.js
+-rw-r--r--  3.0 unx     4104 bx defN 23-May-08 00:39 static/js/ace/mode-c9search.js
+-rw-r--r--  3.0 unx    20198 tx defN 23-May-08 00:39 static/js/ace/mode-typescript.js
+-rw-r--r--  3.0 unx     2585 tx defN 23-May-08 00:39 static/js/ace/theme-textmate.js
+-rw-r--r--  3.0 unx     2240 tx defN 23-May-08 00:39 static/js/ace/theme-dawn.js
+-rw-r--r--  3.0 unx     6540 tx defN 23-May-08 00:39 static/js/ace/mode-haxe.js
+-rw-r--r--  3.0 unx     3729 tx defN 23-May-08 00:39 static/js/ace/ext-modelist.js
+-rw-r--r--  3.0 unx   164518 tx defN 23-May-08 00:39 static/js/ace/worker-javascript.js
+-rw-r--r--  3.0 unx     6523 tx defN 23-May-08 00:39 static/js/ace/mode-mysql.js
+-rw-r--r--  3.0 unx     9112 tx defN 23-May-08 00:39 static/js/ace/ext-textarea.js
+-rw-r--r--  3.0 unx    13129 tx defN 23-May-08 00:39 static/js/ace/mode-nix.js
+-rw-r--r--  3.0 unx    10785 tx defN 23-May-08 00:39 static/js/ace/mode-drools.js
+-rw-r--r--  3.0 unx    22619 tx defN 23-May-08 00:39 static/js/ace/mode-scala.js
+-rw-r--r--  3.0 unx     2712 tx defN 23-May-08 00:39 static/js/ace/theme-chrome.js
+-rw-r--r--  3.0 unx     1088 tx defN 23-May-08 00:39 static/js/ace/ext-statusbar.js
+-rw-r--r--  3.0 unx    20567 tx defN 23-May-08 00:39 static/js/ace/mode-matlab.js
+-rw-r--r--  3.0 unx    49991 tx defN 23-May-08 00:39 static/js/ace/mode-jade.js
+-rw-r--r--  3.0 unx     4559 tx defN 23-May-08 00:39 static/js/ace/mode-pascal.js
+-rw-r--r--  3.0 unx      140 tx defN 23-May-08 00:39 static/js/ace/ext-error_marker.js
+-rw-r--r--  3.0 unx    27779 tx defN 23-May-08 00:39 static/js/ace/theme-ambiance.js
+-rw-r--r--  3.0 unx     2353 tx defN 23-May-08 00:39 static/js/ace/theme-cobalt.js
+-rw-r--r--  3.0 unx    47114 tx defN 23-May-08 00:39 static/js/ace/worker-lua.js
+-rw-r--r--  3.0 unx     7539 tx defN 23-May-08 00:39 static/js/ace/mode-julia.js
+-rw-r--r--  3.0 unx    21478 tx defN 23-May-08 00:39 static/js/ace/ext-emmet.js
+-rw-r--r--  3.0 unx     2820 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night.js
+-rw-r--r--  3.0 unx     5399 tx defN 23-May-08 00:39 static/js/ace/mode-applescript.js
+-rw-r--r--  3.0 unx     3126 tx defN 23-May-08 00:39 static/js/ace/theme-katzenmilch.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/livescript.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/properties.js
+-rw-r--r--  3.0 unx    21279 tx defN 23-May-08 00:39 static/js/ace/snippets/ruby.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/handlebars.js
+-rw-r--r--  3.0 unx     1263 tx defN 23-May-08 00:39 static/js/ace/snippets/wollok.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/abap.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/lisp.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/json.js
+-rw-r--r--  3.0 unx      145 tx defN 23-May-08 00:39 static/js/ace/snippets/applescript.js
+-rw-r--r--  3.0 unx      141 tx defN 23-May-08 00:39 static/js/ace/snippets/html_ruby.js
+-rw-r--r--  3.0 unx      147 tx defN 23-May-08 00:39 static/js/ace/snippets/assembly_x86.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/forth.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/swig.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/toml.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/golang.js
+-rw-r--r--  3.0 unx     2040 tx defN 23-May-08 00:39 static/js/ace/snippets/clojure.js
+-rw-r--r--  3.0 unx     4322 tx defN 23-May-08 00:39 static/js/ace/snippets/java.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/scala.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ftl.js
+-rw-r--r--  3.0 unx      145 tx defN 23-May-08 00:39 static/js/ace/snippets/apache_conf.js
+-rw-r--r--  3.0 unx      134 tx defN 23-May-08 00:39 static/js/ace/snippets/live_script.js
+-rw-r--r--  3.0 unx     2233 tx defN 23-May-08 00:39 static/js/ace/snippets/coffee.js
+-rw-r--r--  3.0 unx      508 tx defN 23-May-08 00:39 static/js/ace/snippets/lua.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/stylus.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/julia.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/cobol.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/dot.js
+-rw-r--r--  3.0 unx      132 tx defN 23-May-08 00:39 static/js/ace/snippets/protobuf.js
+-rw-r--r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/mushcode.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/groovy.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/twig.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/scad.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/glsl.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/rhtml.js
+-rw-r--r--  3.0 unx      448 tx defN 23-May-08 00:39 static/js/ace/snippets/haml.js
+-rw-r--r--  3.0 unx      651 tx defN 23-May-08 00:39 static/js/ace/snippets/velocity.js
+-rw-r--r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/luapage.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/curly.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/praat.js
+-rw-r--r--  3.0 unx      270 tx defN 23-May-08 00:39 static/js/ace/snippets/maze.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/matlab.js
+-rw-r--r--  3.0 unx      128 tx defN 23-May-08 00:39 static/js/ace/snippets/hjson.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/mel.js
+-rw-r--r--  3.0 unx     6763 tx defN 23-May-08 00:39 static/js/ace/snippets/php.js
+-rw-r--r--  3.0 unx     4000 tx defN 23-May-08 00:39 static/js/ace/snippets/django.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ejs.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/jade.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/liquid.js
+-rw-r--r--  3.0 unx     1716 tx defN 23-May-08 00:39 static/js/ace/snippets/jsoniq.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/gcode.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/kotlin.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/dockerfile.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/text.js
+-rw-r--r--  3.0 unx      145 tx defN 23-May-08 00:39 static/js/ace/snippets/html_elixir.js
+-rw-r--r--  3.0 unx     2055 tx defN 23-May-08 00:39 static/js/ace/snippets/sh.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/rust.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/lean.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/lucene.js
+-rw-r--r--  3.0 unx      297 tx defN 23-May-08 00:39 static/js/ace/snippets/snippets.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/rdoc.js
+-rw-r--r--  3.0 unx     5513 tx defN 23-May-08 00:39 static/js/ace/snippets/perl.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/swift.js
+-rw-r--r--  3.0 unx      540 tx defN 23-May-08 00:39 static/js/ace/snippets/textile.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/objectivec.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ada.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/less.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/elixir.js
+-rw-r--r--  3.0 unx      551 tx defN 23-May-08 00:39 static/js/ace/snippets/diff.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/space.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/sjs.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/typescript.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/mysql.js
+-rw-r--r--  3.0 unx     2663 tx defN 23-May-08 00:39 static/js/ace/snippets/c_cpp.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/autohotkey.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/eiffel.js
+-rw-r--r--  3.0 unx     1690 tx defN 23-May-08 00:39 static/js/ace/snippets/tcl.js
+-rw-r--r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/verilog.js
+-rw-r--r--  3.0 unx    19650 tx defN 23-May-08 00:39 static/js/ace/snippets/css.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ini.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/plain_text.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/csharp.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/mask.js
+-rw-r--r--  3.0 unx      198 tx defN 23-May-08 00:39 static/js/ace/snippets/makefile.js
+-rw-r--r--  3.0 unx     3636 tx defN 23-May-08 00:39 static/js/ace/snippets/tex.js
+-rw-r--r--  3.0 unx     3574 tx defN 23-May-08 00:39 static/js/ace/snippets/erlang.js
+-rw-r--r--  3.0 unx     2973 tx defN 23-May-08 00:39 static/js/ace/snippets/actionscript.js
+-rw-r--r--  3.0 unx      442 tx defN 23-May-08 00:39 static/js/ace/snippets/rst.js
+-rw-r--r--  3.0 unx      149 tx defN 23-May-08 00:39 static/js/ace/snippets/haskell_cabal.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/scss.js
+-rw-r--r--  3.0 unx     1716 tx defN 23-May-08 00:39 static/js/ace/snippets/xquery.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/jack.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/pgsql.js
+-rw-r--r--  3.0 unx     3672 tx defN 23-May-08 00:39 static/js/ace/snippets/python.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/logiql.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/tsx.js
+-rw-r--r--  3.0 unx      370 tx defN 23-May-08 00:39 static/js/ace/snippets/drools.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/smarty.js
+-rw-r--r--  3.0 unx      125 tx defN 23-May-08 00:39 static/js/ace/snippets/d.js
+-rw-r--r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/c9search.js
+-rw-r--r--  3.0 unx      136 tx defN 23-May-08 00:39 static/js/ace/snippets/mipsassembler.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/latex.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/ocaml.js
+-rw-r--r--  3.0 unx     1975 tx defN 23-May-08 00:39 static/js/ace/snippets/haskell.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/svg.js
+-rw-r--r--  3.0 unx    35423 tx defN 23-May-08 00:39 static/js/ace/snippets/lsl.js
+-rw-r--r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/asciidoc.js
+-rw-r--r--  3.0 unx     2630 tx defN 23-May-08 00:39 static/js/ace/snippets/r.js
+-rw-r--r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/fortran.js
+-rw-r--r--  3.0 unx      141 tx defN 23-May-08 00:39 static/js/ace/snippets/batchfile.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/elm.js
+-rw-r--r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/gherkin.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/powershell.js
+-rw-r--r--  3.0 unx     1973 tx defN 23-May-08 00:39 static/js/ace/snippets/markdown.js
+-rw-r--r--  3.0 unx      164 tx defN 23-May-08 00:39 static/js/ace/snippets/razor.js
+-rw-r--r--  3.0 unx      151 tx defN 23-May-08 00:39 static/js/ace/snippets/mips_assembler.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/jsx.js
+-rw-r--r--  3.0 unx      127 tx defN 23-May-08 00:39 static/js/ace/snippets/nsis.js
+-rw-r--r--  3.0 unx      126 tx defN 23-May-08 00:39 static/js/ace/snippets/bro.js
+-rw-r--r--  3.0 unx     3127 tx defN 23-May-08 00:39 static/js/ace/snippets/vala.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/nix.js
+-rw-r--r--  3.0 unx      607 tx defN 23-May-08 00:39 static/js/ace/snippets/gobstones.js
+-rw-r--r--  3.0 unx    18271 tx defN 23-May-08 00:39 static/js/ace/snippets/html.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/yaml.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/cirru.js
+-rw-r--r--  3.0 unx     1319 tx defN 23-May-08 00:39 static/js/ace/snippets/dart.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/coldfusion.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/haxe.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/prolog.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/scheme.js
+-rw-r--r--  3.0 unx     2778 tx defN 23-May-08 00:39 static/js/ace/snippets/jsp.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/pascal.js
+-rw-r--r--  3.0 unx      147 tx defN 23-May-08 00:39 static/js/ace/snippets/soy_template.js
+-rw-r--r--  3.0 unx      947 tx defN 23-May-08 00:39 static/js/ace/snippets/abc.js
+-rw-r--r--  3.0 unx     3840 tx defN 23-May-08 00:39 static/js/ace/snippets/javascript.js
+-rw-r--r--  3.0 unx     1219 tx defN 23-May-08 00:39 static/js/ace/snippets/io.js
+-rw-r--r--  3.0 unx     2139 tx defN 23-May-08 00:39 static/js/ace/snippets/sqlserver.js
+-rw-r--r--  3.0 unx      141 tx defN 23-May-08 00:39 static/js/ace/snippets/gitignore.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/vhdl.js
+-rw-r--r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/vbscript.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/xml.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/sass.js
+-rw-r--r--  3.0 unx      942 tx defN 23-May-08 00:39 static/js/ace/snippets/sql.js
+-rw-r--r--  3.0 unx     6965 tx defN 23-May-08 00:39 static/js/ace/mode-jsx.js
+-rw-r--r--  3.0 unx   190654 tx defN 23-May-08 00:39 static/js/ace/worker-coffee.js
+-rw-r--r--  3.0 unx     7382 tx defN 23-May-08 00:39 static/js/ace/mode-perl.js
+-rw-r--r--  3.0 unx    59769 tx defN 23-May-08 00:39 static/js/ace/mode-handlebars.js
+-rw-r--r--  3.0 unx    11837 tx defN 23-May-08 00:39 static/js/ace/mode-kotlin.js
+-rw-r--r--  3.0 unx    20510 tx defN 23-May-08 00:39 static/js/ace/mode-tsx.js
+-rw-r--r--  3.0 unx     2556 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow.js
+-rw-r--r--  3.0 unx     3994 tx defN 23-May-08 00:39 static/js/ace/mode-rdoc.js
+-rw-r--r--  3.0 unx     2432 tx defN 23-May-08 00:39 static/js/ace/theme-clouds_midnight.js
+-rw-r--r--  3.0 unx     2236 tx defN 23-May-08 00:39 static/js/ace/theme-merbivore.js
+-rw-r--r--  3.0 unx    61525 tx defN 23-May-08 00:39 static/js/ace/mode-twig.js
+-rw-r--r--  3.0 unx     2761 tx defN 23-May-08 00:39 static/js/ace/mode-tex.js
+-rw-r--r--  3.0 unx     5576 tx defN 23-May-08 00:39 static/js/ace/mode-lean.js
+-rw-r--r--  3.0 unx     5970 tx defN 23-May-08 00:39 static/js/ace/mode-hjson.js
+-rw-r--r--  3.0 unx     3003 tx defN 23-May-08 00:39 static/js/ace/mode-cirru.js
+-rw-r--r--  3.0 unx     3640 tx defN 23-May-08 00:39 static/js/ace/ext-keybinding_menu.js
+-rw-r--r--  3.0 unx    19962 tx defN 23-May-08 00:39 static/js/ace/mode-live_script.js
+-rw-r--r--  3.0 unx     6120 tx defN 23-May-08 00:39 static/js/ace/mode-tcl.js
+-rw-r--r--  3.0 unx     2087 tx defN 23-May-08 00:39 static/js/ace/mode-textile.js
+-rw-r--r--  3.0 unx    30271 tx defN 23-May-08 00:39 static/js/ace/mode-liquid.js
+-rw-r--r--  3.0 unx    68741 tx defN 23-May-08 00:39 static/js/ace/mode-html_ruby.js
+-rw-r--r--  3.0 unx    37225 tx defN 23-May-08 00:39 static/js/ace/mode-haml.js
+-rw-r--r--  3.0 unx    66336 tx defN 23-May-08 00:39 static/js/ace/mode-luapage.js
+-rw-r--r--  3.0 unx    13008 tx defN 23-May-08 00:39 static/js/ace/mode-glsl.js
+-rw-r--r--  3.0 unx     6554 tx defN 23-May-08 00:39 static/js/ace/mode-makefile.js
+-rw-r--r--  3.0 unx     3221 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night_eighties.js
+-rw-r--r--  3.0 unx     5764 tx defN 23-May-08 00:39 static/js/ace/mode-jack.js
+-rw-r--r--  3.0 unx    60415 tx defN 23-May-08 00:39 static/js/ace/mode-coldfusion.js
+-rw-r--r--  3.0 unx     4681 tx defN 23-May-08 00:39 static/js/ace/mode-python.js
+-rw-r--r--  3.0 unx     2689 tx defN 23-May-08 00:39 static/js/ace/mode-verilog.js
+-rw-r--r--  3.0 unx    75093 tx defN 23-May-08 00:39 static/js/ace/mode-html_elixir.js
+-rw-r--r--  3.0 unx    55911 tx defN 23-May-08 00:39 static/js/ace/mode-pgsql.js
+-rw-r--r--  3.0 unx     3687 tx defN 23-May-08 00:39 static/js/ace/mode-snippets.js
+-rw-r--r--  3.0 unx    16578 tx defN 23-May-08 00:39 static/js/ace/mode-vala.js
+-rw-r--r--  3.0 unx     2409 tx defN 23-May-08 00:39 static/js/ace/mode-diff.js
+-rw-r--r--  3.0 unx    10260 tx defN 23-May-08 00:39 static/js/ace/mode-praat.js
+-rw-r--r--  3.0 unx   354781 tx defN 23-May-08 00:39 static/js/ace/ace.js
+-rw-r--r--  3.0 unx     5813 tx defN 23-May-08 00:39 static/js/ace/mode-abap.js
+-rw-r--r--  3.0 unx    11914 tx defN 23-May-08 00:39 static/js/ace/ext-old_ie.js
+-rw-r--r--  3.0 unx     2380 tx defN 23-May-08 00:39 static/js/ace/mode-gherkin.js
+-rw-r--r--  3.0 unx     2125 tx defN 23-May-08 00:39 static/js/ace/theme-eclipse.js
+-rw-r--r--  3.0 unx    11847 tx defN 23-May-08 00:39 static/js/ace/mode-xml.js
+-rw-r--r--  3.0 unx     2248 tx defN 23-May-08 00:39 static/js/ace/theme-idle_fingers.js
+-rw-r--r--  3.0 unx     6929 tx defN 23-May-08 00:39 static/js/ace/mode-swift.js
+-rw-r--r--  3.0 unx     4856 tx defN 23-May-08 00:39 static/js/ace/mode-batchfile.js
+-rw-r--r--  3.0 unx      825 tx defN 23-May-08 00:39 static/js/ace/ext-linking.js
+-rw-r--r--  3.0 unx     3658 tx defN 23-May-08 00:39 static/js/ace/mode-scheme.js
+-rw-r--r--  3.0 unx     2633 tx defN 23-May-08 00:39 static/js/ace/theme-pastel_on_dark.js
+-rw-r--r--  3.0 unx    59262 tx defN 23-May-08 00:39 static/js/ace/mode-django.js
+-rw-r--r--  3.0 unx     2054 tx defN 23-May-08 00:39 static/js/ace/theme-kuroir.js
+-rw-r--r--  3.0 unx     3024 tx defN 23-May-08 00:39 static/js/ace/mode-rst.js
+-rw-r--r--  3.0 unx    10035 tx defN 23-May-08 00:39 static/js/ace/mode-nsis.js
+-rw-r--r--  3.0 unx    24939 tx defN 23-May-08 00:39 static/js/ace/mode-mel.js
+-rw-r--r--  3.0 unx     1811 tx defN 23-May-08 00:39 static/js/ace/mode-sql.js
+-rw-r--r--  3.0 unx     8226 tx defN 23-May-08 00:39 static/js/ace/mode-dockerfile.js
+-rw-r--r--  3.0 unx     2791 tx defN 23-May-08 00:39 static/js/ace/theme-mono_industrial.js
+-rw-r--r--  3.0 unx    12546 tx defN 23-May-08 00:39 static/js/ace/mode-protobuf.js
+-rw-r--r--  3.0 unx      899 tx defN 23-May-08 00:39 static/js/ace/mode-gitignore.js
+-rw-r--r--  3.0 unx   232939 tx defN 23-May-08 00:39 static/js/ace/mode-jsoniq.js
+-rw-r--r--  3.0 unx     5097 tx defN 23-May-08 00:39 static/js/ace/mode-json.js
+-rw-r--r--  3.0 unx     5959 tx defN 23-May-08 00:39 static/js/ace/mode-mips_assembler.js
+-rw-r--r--  3.0 unx     2360 tx defN 23-May-08 00:39 static/js/ace/theme-solarized_light.js
+-rw-r--r--  3.0 unx    26620 tx defN 23-May-08 00:39 static/js/ace/mode-lsl.js
+-rw-r--r--  3.0 unx    20085 tx defN 23-May-08 00:39 static/js/ace/mode-less.js
+-rw-r--r--  3.0 unx     4984 tx defN 23-May-08 00:39 static/js/ace/mode-livescript.js
+-rw-r--r--  3.0 unx     8028 tx defN 23-May-08 00:39 static/js/ace/mode-clojure.js
+-rw-r--r--  3.0 unx     2204 tx defN 23-May-08 00:39 static/js/ace/theme-vibrant_ink.js
+-rw-r--r--  3.0 unx    22440 tx defN 23-May-08 00:39 static/js/ace/mode-groovy.js
+-rw-r--r--  3.0 unx     6495 tx defN 23-May-08 00:39 static/js/ace/mode-rust.js
+-rw-r--r--  3.0 unx     7283 tx defN 23-May-08 00:39 static/js/ace/mode-lua.js
+-rw-r--r--  3.0 unx    61356 tx defN 23-May-08 00:39 static/js/ace/mode-smarty.js
+-rw-r--r--  3.0 unx     5665 tx defN 23-May-08 00:39 static/js/ace/mode-io.js
+-rw-r--r--  3.0 unx     1464 tx defN 23-May-08 00:39 static/js/ace/mode-gcode.js
+-rw-r--r--  3.0 unx    63640 tx defN 23-May-08 00:39 static/js/ace/mode-autohotkey.js
+-rw-r--r--  3.0 unx     2913 tx defN 23-May-08 00:39 static/js/ace/theme-terminal.js
+-rw-r--r--  3.0 unx     1470 tx defN 23-May-08 00:39 static/js/ace/ext-themelist.js
+-rw-r--r--  3.0 unx    57890 tx defN 23-May-08 00:39 static/js/ace/mode-html.js
+-rw-r--r--  3.0 unx     3138 tx defN 23-May-08 00:39 static/js/ace/theme-dreamweaver.js
+-rw-r--r--  3.0 unx    10025 tx defN 23-May-08 00:39 static/js/ace/mode-ruby.js
+-rw-r--r--  3.0 unx     8840 tx defN 23-May-08 00:39 static/js/ace/mode-csharp.js
+-rw-r--r--  3.0 unx    10005 tx defN 23-May-08 00:39 static/js/ace/ext-searchbox.js
+-rw-r--r--  3.0 unx     6989 tx defN 23-May-08 00:39 static/js/ace/mode-forth.js
+-rw-r--r--  3.0 unx    21273 tx defN 23-May-08 00:39 static/js/ace/mode-sjs.js
+-rw-r--r--  3.0 unx     5005 tx defN 23-May-08 00:39 static/js/ace/mode-r.js
+-rw-r--r--  3.0 unx    31988 tx defN 23-May-08 00:39 static/js/ace/mode-svg.js
+-rw-r--r--  3.0 unx     2710 tx defN 23-May-08 00:39 static/js/ace/mode-ini.js
+-rw-r--r--  3.0 unx     3496 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night_bright.js
+-rw-r--r--  3.0 unx    31151 tx defN 23-May-08 00:39 static/js/ace/mode-swig.js
+-rw-r--r--  3.0 unx   140879 tx defN 23-May-08 00:39 static/js/ace/worker-css.js
+-rw-r--r--  3.0 unx    40358 tx defN 23-May-08 00:39 static/js/ace/mode-mask.js
+-rw-r--r--  3.0 unx    58909 tx defN 23-May-08 00:39 static/js/ace/mode-curly.js
+-rw-r--r--  3.0 unx    62955 tx defN 23-May-08 00:39 static/js/ace/mode-rhtml.js
+-rw-r--r--  3.0 unx     2375 tx defN 23-May-08 00:39 static/js/ace/theme-monokai.js
+-rw-r--r--  3.0 unx     2282 tx defN 23-May-08 00:39 static/js/ace/mode-haskell_cabal.js
+-rw-r--r--  3.0 unx     2081 tx defN 23-May-08 00:39 static/js/ace/theme-clouds.js
+-rw-r--r--  3.0 unx    66385 tx defN 23-May-08 00:39 static/js/ace/mode-soy_template.js
+-rw-r--r--  3.0 unx    64800 tx defN 23-May-08 00:39 static/js/ace/mode-markdown.js
+-rw-r--r--  3.0 unx     4709 tx defN 23-May-08 00:39 static/js/ace/mode-abc.js
+-rw-r--r--  3.0 unx   470435 tx defN 23-May-08 00:39 static/js/ace/mode-php.js
+-rw-r--r--  3.0 unx     2819 tx defN 23-May-08 00:39 static/js/ace/ext-static_highlight.js
+-rw-r--r--  3.0 unx    14198 tx defN 23-May-08 00:39 static/js/ace/mode-dart.js
+-rw-r--r--  3.0 unx    20545 tx defN 23-May-08 00:39 static/js/ace/mode-actionscript.js
+-rw-r--r--  3.0 unx     1099 tx defN 23-May-08 00:39 static/js/ace/mode-properties.js
+-rw-r--r--  3.0 unx    32911 tx defN 23-May-08 00:39 static/js/ace/worker-json.js
+-rw-r--r--  3.0 unx   230322 tx defN 23-May-08 00:39 static/js/ace/mode-xquery.js
+-rw-r--r--  3.0 unx    21805 tx defN 23-May-08 00:39 static/js/ace/mode-java.js
+-rw-r--r--  3.0 unx     3031 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night_blue.js
+-rw-r--r--  3.0 unx    96918 tx defN 23-May-08 00:39 static/js/ace/keybinding-vim.js
+-rw-r--r--  3.0 unx     1918 tx defN 23-May-08 00:39 static/js/ace/theme-xcode.js
+-rw-r--r--  3.0 unx    15753 tx defN 23-May-08 00:39 static/js/ace/mode-elixir.js
+-rw-r--r--  3.0 unx    10220 tx defN 23-May-08 00:39 static/js/ace/mode-sass.js
+-rw-r--r--  3.0 unx     6520 tx defN 23-May-08 00:39 static/js/ace/mode-scad.js
+-rw-r--r--  3.0 unx     2842 tx defN 23-May-08 00:39 static/js/ace/theme-chaos.js
+-rw-r--r--  3.0 unx     1762 tx defN 23-May-08 00:39 static/js/ace/mode-ada.js
+-rw-r--r--  3.0 unx     3994 tx defN 23-May-08 00:39 static/js/ace/mode-yaml.js
+-rw-r--r--  3.0 unx        0 bx stor 23-May-08 00:39 static/js/ace/mode-text.js
+-rw-r--r--  3.0 unx     1961 tx defN 23-May-08 00:39 static/js/ace/mode-lisp.js
+-rw-r--r--  3.0 unx     8159 tx defN 23-May-08 00:39 static/js/ace/mode-asciidoc.js
+-rw-r--r--  3.0 unx     2313 tx defN 23-May-08 00:39 static/js/ace/mode-cobol.js
+-rw-r--r--  3.0 unx     2572 tx defN 23-May-08 00:39 static/js/ace/ext-whitespace.js
+-rw-r--r--  3.0 unx     7595 tx defN 23-May-08 00:39 static/js/ace/mode-dot.js
+-rw-r--r--  3.0 unx     2176 tx defN 23-May-08 00:39 static/js/ace/theme-github.js
+-rw-r--r--  3.0 unx    29711 tx defN 23-May-08 00:39 static/js/ace/mode-erlang.js
+-rw-r--r--  3.0 unx    64984 tx defN 23-May-08 00:39 static/js/ace/mode-razor.js
+-rw-r--r--  3.0 unx     4193 tx defN 23-May-08 00:39 static/js/ace/ext-split.js
+-rw-r--r--  3.0 unx    12951 tx defN 23-May-08 00:39 static/js/ace/mode-scss.js
+-rw-r--r--  3.0 unx    32692 tx defN 23-May-08 00:39 static/js/ace/mode-powershell.js
+-rw-r--r--  3.0 unx     6476 tx defN 23-May-08 00:39 static/js/ace/theme-iplastic.js
+-rw-r--r--  3.0 unx     6360 tx defN 23-May-08 00:39 static/js/ace/ext-chromevox.js
+-rw-r--r--  3.0 unx     2296 tx defN 23-May-08 00:39 static/js/ace/theme-kr_theme.js
+-rw-r--r--  3.0 unx    20332 tx defN 23-May-08 00:39 static/js/ace/mode-gobstones.js
+-rw-r--r--  3.0 unx     3189 tx defN 23-May-08 00:39 static/js/ace/mode-mipsassembler.js
+-rw-r--r--  3.0 unx     2812 tx defN 23-May-08 00:39 static/js/ace/theme-crimson_editor.js
+-rw-r--r--  3.0 unx    34689 tx defN 23-May-08 00:39 static/js/ace/mode-jsp.js
+-rw-r--r--  3.0 unx     3818 tx defN 23-May-08 00:39 static/js/ace/ext-beautify.js
+-rw-r--r--  3.0 unx      484 tx defN 23-May-08 00:39 static/js/dbadmin.js
+-rw-r--r--  3.0 unx    95432 tx defN 23-May-08 00:39 static/js/highlight.min.js
+-rw-r--r--  3.0 unx     3354 tx defN 23-Nov-12 21:29 static/js/translations.js
+-rw-r--r--  3.0 unx    12182 tx defN 23-Nov-12 21:18 static/js/utils.js
+-rw-r--r--  3.0 unx    68547 tx defN 23-May-08 00:39 static/js/sugar.min.js
+-rw-r--r--  3.0 unx    88145 tx defN 23-Nov-12 21:44 static/js/jquery.min.js
+-rw-r--r--  3.0 unx      951 tx defN 23-Nov-12 21:32 templates/dbadmin.html
+-rw-r--r--  3.0 unx     4760 tx defN 23-Nov-12 21:32 templates/gitlog.html
+-rw-r--r--  3.0 unx    13851 tx defN 23-May-08 00:39 templates/index.html
+-rw-r--r--  3.0 unx     1141 tx defN 23-May-08 00:39 templates/ticket.html
+-rw-r--r--  3.0 unx     2953 tx defN 23-Nov-12 21:32 templates/translations.html
+378 files, 8005852 bytes uncompressed, 2919902 bytes compressed:  63.5%
```

#### zipnote {}

```diff
@@ -1,1135 +1,1135 @@
-Filename: __init__.py
-Comment: 
-
-Filename: templates/ticket.html
+Filename: diff2kryten.py
 Comment: 
 
-Filename: templates/gitlog.html
+Filename: __init__.py
 Comment: 
 
-Filename: templates/translations.html
+Filename: utils.py
 Comment: 
 
-Filename: templates/index.html
+Filename: translations/README.md
 Comment: 
 
-Filename: templates/dbadmin.html
+Filename: static/favicon.ico
 Comment: 
 
-Filename: utils.py
+Filename: static/images/alert-red.gif
 Comment: 
 
-Filename: translations/README.md
+Filename: static/images/forkme.png
 Comment: 
 
-Filename: diff2kryten.py
+Filename: static/images/alert-blue.gif
 Comment: 
 
-Filename: static/js/utils.js
+Filename: static/images/widget.gif
 Comment: 
 
-Filename: static/js/dbadmin.js
+Filename: static/images/alert-orange.gif
 Comment: 
 
-Filename: static/js/ace/mode-maze.js
+Filename: static/images/alert-green.gif
 Comment: 
 
-Filename: static/js/ace/theme-iplastic.js
+Filename: static/images/alert-yellow.gif
 Comment: 
 
-Filename: static/js/ace/mode-rst.js
+Filename: static/css/future.css
 Comment: 
 
-Filename: static/js/ace/theme-crimson_editor.js
+Filename: static/css/gitlog.min.css
 Comment: 
 
-Filename: static/js/ace/mode-lsl.js
+Filename: static/components/mtable.html
 Comment: 
 
-Filename: static/js/ace/mode-prolog.js
+Filename: static/components/mtable.js
 Comment: 
 
-Filename: static/js/ace/mode-mipsassembler.js
+Filename: static/js/index.js
 Comment: 
 
-Filename: static/js/ace/theme-clouds_midnight.js
+Filename: static/js/vue.min.js
 Comment: 
 
-Filename: static/js/ace/mode-dockerfile.js
+Filename: static/js/ace/mode-sh.js
 Comment: 
 
-Filename: static/js/ace/mode-io.js
+Filename: static/js/ace/mode-latex.js
 Comment: 
 
-Filename: static/js/ace/mode-php.js
+Filename: static/js/ace/worker-xml.js
 Comment: 
 
-Filename: static/js/ace/mode-rhtml.js
+Filename: static/js/ace/mode-sqlserver.js
 Comment: 
 
-Filename: static/js/ace/mode-swig.js
+Filename: static/js/ace/mode-objectivec.js
 Comment: 
 
-Filename: static/js/ace/mode-dart.js
+Filename: static/js/ace/mode-bro.js
 Comment: 
 
-Filename: static/js/ace/theme-chaos.js
+Filename: static/js/ace/mode-wollok.js
 Comment: 
 
-Filename: static/js/ace/theme-terminal.js
+Filename: static/js/ace/mode-vbscript.js
 Comment: 
 
-Filename: static/js/ace/mode-xml.js
+Filename: static/js/ace/keybinding-emacs.js
 Comment: 
 
-Filename: static/js/ace/mode-asciidoc.js
+Filename: static/js/ace/mode-c_cpp.js
 Comment: 
 
-Filename: static/js/ace/mode-pgsql.js
+Filename: static/js/ace/mode-css.js
 Comment: 
 
-Filename: static/js/ace/mode-clojure.js
+Filename: static/js/ace/mode-ftl.js
 Comment: 
 
-Filename: static/js/ace/mode-text.js
+Filename: static/js/ace/worker-html.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow_night_blue.js
+Filename: static/js/ace/worker-php.js
 Comment: 
 
-Filename: static/js/ace/mode-cobol.js
+Filename: static/js/ace/mode-elm.js
 Comment: 
 
-Filename: static/js/ace/worker-lua.js
+Filename: static/js/ace/mode-golang.js
 Comment: 
 
-Filename: static/js/ace/theme-kr_theme.js
+Filename: static/js/ace/mode-javascript.js
 Comment: 
 
-Filename: static/js/ace/theme-mono_industrial.js
+Filename: static/js/ace/mode-ocaml.js
 Comment: 
 
 Filename: static/js/ace/mode-assembly_x86.js
 Comment: 
 
-Filename: static/js/ace/theme-twilight.js
+Filename: static/js/ace/theme-solarized_dark.js
 Comment: 
 
-Filename: static/js/ace/mode-c9search.js
+Filename: static/js/ace/worker-xquery.js
 Comment: 
 
-Filename: static/js/ace/mode-html_elixir.js
+Filename: static/js/ace/mode-d.js
 Comment: 
 
-Filename: static/js/ace/mode-plain_text.js
+Filename: static/js/ace/mode-fortran.js
 Comment: 
 
-Filename: static/js/ace/mode-groovy.js
+Filename: static/js/ace/mode-prolog.js
 Comment: 
 
-Filename: static/js/ace/theme-merbivore.js
+Filename: static/js/ace/mode-logiql.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow.js
+Filename: static/js/ace/theme-twilight.js
 Comment: 
 
-Filename: static/js/ace/mode-tex.js
+Filename: static/js/ace/mode-coffee.js
 Comment: 
 
-Filename: static/js/ace/mode-glsl.js
+Filename: static/js/ace/ext-settings_menu.js
 Comment: 
 
-Filename: static/js/ace/mode-soy_template.js
+Filename: static/js/ace/mode-vhdl.js
 Comment: 
 
-Filename: static/js/ace/worker-xquery.js
+Filename: static/js/ace/mode-space.js
 Comment: 
 
-Filename: static/js/ace/mode-smarty.js
+Filename: static/js/ace/mode-eiffel.js
 Comment: 
 
-Filename: static/js/ace/mode-pascal.js
+Filename: static/js/ace/mode-ejs.js
 Comment: 
 
-Filename: static/js/ace/mode-erlang.js
+Filename: static/js/ace/theme-merbivore_soft.js
 Comment: 
 
-Filename: static/js/ace/worker-xml.js
+Filename: static/js/ace/mode-toml.js
 Comment: 
 
-Filename: static/js/ace/mode-haskell.js
+Filename: static/js/ace/mode-mushcode.js
 Comment: 
 
-Filename: static/js/ace/mode-liquid.js
+Filename: static/js/ace/ext-spellcheck.js
 Comment: 
 
-Filename: static/js/ace/mode-vhdl.js
+Filename: static/js/ace/mode-plain_text.js
 Comment: 
 
-Filename: static/js/ace/mode-haml.js
+Filename: static/js/ace/theme-sqlserver.js
 Comment: 
 
-Filename: static/js/ace/mode-properties.js
+Filename: static/js/ace/mode-lucene.js
 Comment: 
 
-Filename: static/js/ace/theme-monokai.js
+Filename: static/js/ace/ext-elastic_tabstops_lite.js
 Comment: 
 
-Filename: static/js/ace/mode-jsx.js
+Filename: static/js/ace/ext-language_tools.js
 Comment: 
 
-Filename: static/js/ace/mode-drools.js
+Filename: static/js/ace/mode-haskell.js
 Comment: 
 
-Filename: static/js/ace/ext-elastic_tabstops_lite.js
+Filename: static/js/ace/mode-velocity.js
 Comment: 
 
-Filename: static/js/ace/theme-github.js
+Filename: static/js/ace/mode-apache_conf.js
 Comment: 
 
-Filename: static/js/ace/mode-objectivec.js
+Filename: static/js/ace/mode-maze.js
 Comment: 
 
-Filename: static/js/ace/ext-split.js
+Filename: static/js/ace/mode-stylus.js
 Comment: 
 
-Filename: static/js/ace/mode-abc.js
+Filename: static/js/ace/mode-c9search.js
 Comment: 
 
-Filename: static/js/ace/ext-language_tools.js
+Filename: static/js/ace/mode-typescript.js
 Comment: 
 
-Filename: static/js/ace/mode-stylus.js
+Filename: static/js/ace/theme-textmate.js
 Comment: 
 
-Filename: static/js/ace/ext-statusbar.js
+Filename: static/js/ace/theme-dawn.js
 Comment: 
 
 Filename: static/js/ace/mode-haxe.js
 Comment: 
 
-Filename: static/js/ace/ext-whitespace.js
+Filename: static/js/ace/ext-modelist.js
 Comment: 
 
-Filename: static/js/ace/mode-sql.js
+Filename: static/js/ace/worker-javascript.js
 Comment: 
 
-Filename: static/js/ace/theme-katzenmilch.js
+Filename: static/js/ace/mode-mysql.js
 Comment: 
 
-Filename: static/js/ace/mode-sjs.js
+Filename: static/js/ace/ext-textarea.js
 Comment: 
 
-Filename: static/js/ace/mode-vbscript.js
+Filename: static/js/ace/mode-nix.js
 Comment: 
 
-Filename: static/js/ace/mode-gherkin.js
+Filename: static/js/ace/mode-drools.js
 Comment: 
 
-Filename: static/js/ace/worker-php.js
+Filename: static/js/ace/mode-scala.js
 Comment: 
 
-Filename: static/js/ace/mode-perl.js
+Filename: static/js/ace/theme-chrome.js
 Comment: 
 
-Filename: static/js/ace/theme-pastel_on_dark.js
+Filename: static/js/ace/ext-statusbar.js
 Comment: 
 
-Filename: static/js/ace/mode-gitignore.js
+Filename: static/js/ace/mode-matlab.js
 Comment: 
 
-Filename: static/js/ace/ext-settings_menu.js
+Filename: static/js/ace/mode-jade.js
 Comment: 
 
-Filename: static/js/ace/mode-cirru.js
+Filename: static/js/ace/mode-pascal.js
 Comment: 
 
-Filename: static/js/ace/ext-old_ie.js
+Filename: static/js/ace/ext-error_marker.js
 Comment: 
 
-Filename: static/js/ace/mode-html_ruby.js
+Filename: static/js/ace/theme-ambiance.js
 Comment: 
 
-Filename: static/js/ace/mode-lucene.js
+Filename: static/js/ace/theme-cobalt.js
 Comment: 
 
-Filename: static/js/ace/ext-emmet.js
+Filename: static/js/ace/worker-lua.js
 Comment: 
 
-Filename: static/js/ace/mode-markdown.js
+Filename: static/js/ace/mode-julia.js
 Comment: 
 
-Filename: static/js/ace/mode-logiql.js
+Filename: static/js/ace/ext-emmet.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow_night_bright.js
+Filename: static/js/ace/theme-tomorrow_night.js
 Comment: 
 
-Filename: static/js/ace/mode-space.js
+Filename: static/js/ace/mode-applescript.js
 Comment: 
 
-Filename: static/js/ace/mode-gcode.js
+Filename: static/js/ace/theme-katzenmilch.js
 Comment: 
 
-Filename: static/js/ace/mode-nsis.js
+Filename: static/js/ace/snippets/livescript.js
 Comment: 
 
-Filename: static/js/ace/ext-textarea.js
+Filename: static/js/ace/snippets/properties.js
 Comment: 
 
-Filename: static/js/ace/mode-nix.js
+Filename: static/js/ace/snippets/ruby.js
 Comment: 
 
-Filename: static/js/ace/mode-xquery.js
+Filename: static/js/ace/snippets/handlebars.js
 Comment: 
 
-Filename: static/js/ace/mode-batchfile.js
+Filename: static/js/ace/snippets/wollok.js
 Comment: 
 
-Filename: static/js/ace/mode-mel.js
+Filename: static/js/ace/snippets/abap.js
 Comment: 
 
-Filename: static/js/ace/mode-javascript.js
+Filename: static/js/ace/snippets/lisp.js
 Comment: 
 
-Filename: static/js/ace/mode-jack.js
+Filename: static/js/ace/snippets/json.js
 Comment: 
 
-Filename: static/js/ace/mode-handlebars.js
+Filename: static/js/ace/snippets/applescript.js
 Comment: 
 
-Filename: static/js/ace/mode-swift.js
+Filename: static/js/ace/snippets/html_ruby.js
 Comment: 
 
-Filename: static/js/ace/ext-static_highlight.js
+Filename: static/js/ace/snippets/assembly_x86.js
 Comment: 
 
-Filename: static/js/ace/theme-clouds.js
+Filename: static/js/ace/snippets/forth.js
 Comment: 
 
-Filename: static/js/ace/mode-golang.js
+Filename: static/js/ace/snippets/swig.js
 Comment: 
 
-Filename: static/js/ace/mode-mushcode.js
+Filename: static/js/ace/snippets/toml.js
 Comment: 
 
-Filename: static/js/ace/mode-less.js
+Filename: static/js/ace/snippets/golang.js
 Comment: 
 
-Filename: static/js/ace/ext-keybinding_menu.js
+Filename: static/js/ace/snippets/clojure.js
 Comment: 
 
-Filename: static/js/ace/mode-r.js
+Filename: static/js/ace/snippets/java.js
 Comment: 
 
-Filename: static/js/ace/mode-sh.js
+Filename: static/js/ace/snippets/scala.js
 Comment: 
 
-Filename: static/js/ace/mode-django.js
+Filename: static/js/ace/snippets/ftl.js
 Comment: 
 
-Filename: static/js/ace/mode-rdoc.js
+Filename: static/js/ace/snippets/apache_conf.js
 Comment: 
 
-Filename: static/js/ace/mode-jsp.js
+Filename: static/js/ace/snippets/live_script.js
 Comment: 
 
-Filename: static/js/ace/ext-themelist.js
+Filename: static/js/ace/snippets/coffee.js
 Comment: 
 
-Filename: static/js/ace/mode-ruby.js
+Filename: static/js/ace/snippets/lua.js
 Comment: 
 
-Filename: static/js/ace/mode-mysql.js
+Filename: static/js/ace/snippets/stylus.js
 Comment: 
 
-Filename: static/js/ace/theme-dawn.js
+Filename: static/js/ace/snippets/julia.js
 Comment: 
 
-Filename: static/js/ace/mode-velocity.js
+Filename: static/js/ace/snippets/cobol.js
 Comment: 
 
-Filename: static/js/ace/mode-java.js
+Filename: static/js/ace/snippets/dot.js
 Comment: 
 
-Filename: static/js/ace/mode-textile.js
+Filename: static/js/ace/snippets/protobuf.js
 Comment: 
 
-Filename: static/js/ace/mode-razor.js
+Filename: static/js/ace/snippets/mushcode.js
 Comment: 
 
-Filename: static/js/ace/ext-linking.js
+Filename: static/js/ace/snippets/groovy.js
 Comment: 
 
-Filename: static/js/ace/theme-cobalt.js
+Filename: static/js/ace/snippets/twig.js
 Comment: 
 
-Filename: static/js/ace/mode-coffee.js
+Filename: static/js/ace/snippets/scad.js
 Comment: 
 
-Filename: static/js/ace/mode-wollok.js
+Filename: static/js/ace/snippets/glsl.js
 Comment: 
 
-Filename: static/js/ace/mode-autohotkey.js
+Filename: static/js/ace/snippets/rhtml.js
 Comment: 
 
-Filename: static/js/ace/theme-eclipse.js
+Filename: static/js/ace/snippets/haml.js
 Comment: 
 
-Filename: static/js/ace/mode-forth.js
+Filename: static/js/ace/snippets/velocity.js
 Comment: 
 
-Filename: static/js/ace/theme-chrome.js
+Filename: static/js/ace/snippets/luapage.js
 Comment: 
 
-Filename: static/js/ace/mode-typescript.js
+Filename: static/js/ace/snippets/curly.js
 Comment: 
 
-Filename: static/js/ace/mode-ftl.js
+Filename: static/js/ace/snippets/praat.js
 Comment: 
 
-Filename: static/js/ace/mode-kotlin.js
+Filename: static/js/ace/snippets/maze.js
 Comment: 
 
-Filename: static/js/ace/mode-tcl.js
+Filename: static/js/ace/snippets/matlab.js
 Comment: 
 
-Filename: static/js/ace/mode-vala.js
+Filename: static/js/ace/snippets/hjson.js
 Comment: 
 
-Filename: static/js/ace/worker-coffee.js
+Filename: static/js/ace/snippets/mel.js
 Comment: 
 
-Filename: static/js/ace/theme-textmate.js
+Filename: static/js/ace/snippets/php.js
 Comment: 
 
-Filename: static/js/ace/mode-powershell.js
+Filename: static/js/ace/snippets/django.js
 Comment: 
 
-Filename: static/js/ace/mode-scheme.js
+Filename: static/js/ace/snippets/ejs.js
 Comment: 
 
-Filename: static/js/ace/mode-c_cpp.js
+Filename: static/js/ace/snippets/jade.js
 Comment: 
 
-Filename: static/js/ace/mode-abap.js
+Filename: static/js/ace/snippets/liquid.js
 Comment: 
 
-Filename: static/js/ace/mode-diff.js
+Filename: static/js/ace/snippets/jsoniq.js
 Comment: 
 
-Filename: static/js/ace/mode-apache_conf.js
+Filename: static/js/ace/snippets/gcode.js
 Comment: 
 
-Filename: static/js/ace/mode-matlab.js
+Filename: static/js/ace/snippets/kotlin.js
 Comment: 
 
-Filename: static/js/ace/mode-coldfusion.js
+Filename: static/js/ace/snippets/dockerfile.js
 Comment: 
 
-Filename: static/js/ace/mode-json.js
+Filename: static/js/ace/snippets/text.js
 Comment: 
 
-Filename: static/js/ace/mode-fortran.js
+Filename: static/js/ace/snippets/html_elixir.js
 Comment: 
 
-Filename: static/js/ace/mode-curly.js
+Filename: static/js/ace/snippets/sh.js
 Comment: 
 
-Filename: static/js/ace/mode-twig.js
+Filename: static/js/ace/snippets/rust.js
 Comment: 
 
-Filename: static/js/ace/ace.js
+Filename: static/js/ace/snippets/lean.js
 Comment: 
 
-Filename: static/js/ace/keybinding-vim.js
+Filename: static/js/ace/snippets/lucene.js
 Comment: 
 
-Filename: static/js/ace/mode-hjson.js
+Filename: static/js/ace/snippets/snippets.js
 Comment: 
 
-Filename: static/js/ace/theme-ambiance.js
+Filename: static/js/ace/snippets/rdoc.js
 Comment: 
 
-Filename: static/js/ace/keybinding-emacs.js
+Filename: static/js/ace/snippets/perl.js
 Comment: 
 
-Filename: static/js/ace/ext-spellcheck.js
+Filename: static/js/ace/snippets/swift.js
 Comment: 
 
-Filename: static/js/ace/snippets/julia.js
+Filename: static/js/ace/snippets/textile.js
 Comment: 
 
-Filename: static/js/ace/snippets/matlab.js
+Filename: static/js/ace/snippets/objectivec.js
 Comment: 
 
-Filename: static/js/ace/snippets/protobuf.js
+Filename: static/js/ace/snippets/ada.js
 Comment: 
 
-Filename: static/js/ace/snippets/hjson.js
+Filename: static/js/ace/snippets/less.js
 Comment: 
 
-Filename: static/js/ace/snippets/coldfusion.js
+Filename: static/js/ace/snippets/elixir.js
 Comment: 
 
-Filename: static/js/ace/snippets/haskell.js
+Filename: static/js/ace/snippets/diff.js
 Comment: 
 
-Filename: static/js/ace/snippets/razor.js
+Filename: static/js/ace/snippets/space.js
 Comment: 
 
-Filename: static/js/ace/snippets/live_script.js
+Filename: static/js/ace/snippets/sjs.js
 Comment: 
 
-Filename: static/js/ace/snippets/ada.js
+Filename: static/js/ace/snippets/typescript.js
 Comment: 
 
-Filename: static/js/ace/snippets/verilog.js
+Filename: static/js/ace/snippets/mysql.js
 Comment: 
 
-Filename: static/js/ace/snippets/svg.js
+Filename: static/js/ace/snippets/c_cpp.js
 Comment: 
 
-Filename: static/js/ace/snippets/php.js
+Filename: static/js/ace/snippets/autohotkey.js
 Comment: 
 
-Filename: static/js/ace/snippets/xquery.js
+Filename: static/js/ace/snippets/eiffel.js
 Comment: 
 
-Filename: static/js/ace/snippets/golang.js
+Filename: static/js/ace/snippets/tcl.js
 Comment: 
 
-Filename: static/js/ace/snippets/rhtml.js
+Filename: static/js/ace/snippets/verilog.js
 Comment: 
 
-Filename: static/js/ace/snippets/sh.js
+Filename: static/js/ace/snippets/css.js
 Comment: 
 
-Filename: static/js/ace/snippets/elixir.js
+Filename: static/js/ace/snippets/ini.js
 Comment: 
 
-Filename: static/js/ace/snippets/coffee.js
+Filename: static/js/ace/snippets/plain_text.js
 Comment: 
 
-Filename: static/js/ace/snippets/makefile.js
+Filename: static/js/ace/snippets/csharp.js
 Comment: 
 
-Filename: static/js/ace/snippets/drools.js
+Filename: static/js/ace/snippets/mask.js
 Comment: 
 
-Filename: static/js/ace/snippets/r.js
+Filename: static/js/ace/snippets/makefile.js
 Comment: 
 
-Filename: static/js/ace/snippets/haxe.js
+Filename: static/js/ace/snippets/tex.js
 Comment: 
 
-Filename: static/js/ace/snippets/ocaml.js
+Filename: static/js/ace/snippets/erlang.js
 Comment: 
 
-Filename: static/js/ace/snippets/fortran.js
+Filename: static/js/ace/snippets/actionscript.js
 Comment: 
 
-Filename: static/js/ace/snippets/space.js
+Filename: static/js/ace/snippets/rst.js
 Comment: 
 
-Filename: static/js/ace/snippets/luapage.js
+Filename: static/js/ace/snippets/haskell_cabal.js
 Comment: 
 
-Filename: static/js/ace/snippets/typescript.js
+Filename: static/js/ace/snippets/scss.js
 Comment: 
 
-Filename: static/js/ace/snippets/nix.js
+Filename: static/js/ace/snippets/xquery.js
 Comment: 
 
-Filename: static/js/ace/snippets/abc.js
+Filename: static/js/ace/snippets/jack.js
 Comment: 
 
-Filename: static/js/ace/snippets/haml.js
+Filename: static/js/ace/snippets/pgsql.js
 Comment: 
 
-Filename: static/js/ace/snippets/stylus.js
+Filename: static/js/ace/snippets/python.js
 Comment: 
 
-Filename: static/js/ace/snippets/praat.js
+Filename: static/js/ace/snippets/logiql.js
 Comment: 
 
-Filename: static/js/ace/snippets/mask.js
+Filename: static/js/ace/snippets/tsx.js
 Comment: 
 
-Filename: static/js/ace/snippets/jsp.js
+Filename: static/js/ace/snippets/drools.js
 Comment: 
 
-Filename: static/js/ace/snippets/swig.js
+Filename: static/js/ace/snippets/smarty.js
 Comment: 
 
-Filename: static/js/ace/snippets/lean.js
+Filename: static/js/ace/snippets/d.js
 Comment: 
 
-Filename: static/js/ace/snippets/logiql.js
+Filename: static/js/ace/snippets/c9search.js
 Comment: 
 
-Filename: static/js/ace/snippets/json.js
+Filename: static/js/ace/snippets/mipsassembler.js
 Comment: 
 
-Filename: static/js/ace/snippets/ruby.js
+Filename: static/js/ace/snippets/latex.js
 Comment: 
 
-Filename: static/js/ace/snippets/java.js
+Filename: static/js/ace/snippets/ocaml.js
 Comment: 
 
-Filename: static/js/ace/snippets/forth.js
+Filename: static/js/ace/snippets/haskell.js
 Comment: 
 
-Filename: static/js/ace/snippets/scad.js
+Filename: static/js/ace/snippets/svg.js
 Comment: 
 
 Filename: static/js/ace/snippets/lsl.js
 Comment: 
 
-Filename: static/js/ace/snippets/cirru.js
+Filename: static/js/ace/snippets/asciidoc.js
 Comment: 
 
-Filename: static/js/ace/snippets/tex.js
+Filename: static/js/ace/snippets/r.js
 Comment: 
 
-Filename: static/js/ace/snippets/dart.js
+Filename: static/js/ace/snippets/fortran.js
 Comment: 
 
-Filename: static/js/ace/snippets/xml.js
+Filename: static/js/ace/snippets/batchfile.js
 Comment: 
 
-Filename: static/js/ace/snippets/bro.js
+Filename: static/js/ace/snippets/elm.js
 Comment: 
 
-Filename: static/js/ace/snippets/gitignore.js
+Filename: static/js/ace/snippets/gherkin.js
 Comment: 
 
-Filename: static/js/ace/snippets/jack.js
+Filename: static/js/ace/snippets/powershell.js
 Comment: 
 
-Filename: static/js/ace/snippets/cobol.js
+Filename: static/js/ace/snippets/markdown.js
 Comment: 
 
-Filename: static/js/ace/snippets/maze.js
+Filename: static/js/ace/snippets/razor.js
 Comment: 
 
-Filename: static/js/ace/snippets/ejs.js
+Filename: static/js/ace/snippets/mips_assembler.js
 Comment: 
 
-Filename: static/js/ace/snippets/text.js
+Filename: static/js/ace/snippets/jsx.js
 Comment: 
 
-Filename: static/js/ace/snippets/prolog.js
+Filename: static/js/ace/snippets/nsis.js
 Comment: 
 
-Filename: static/js/ace/snippets/html_ruby.js
+Filename: static/js/ace/snippets/bro.js
 Comment: 
 
-Filename: static/js/ace/snippets/textile.js
+Filename: static/js/ace/snippets/vala.js
 Comment: 
 
-Filename: static/js/ace/snippets/glsl.js
+Filename: static/js/ace/snippets/nix.js
 Comment: 
 
-Filename: static/js/ace/snippets/tcl.js
+Filename: static/js/ace/snippets/gobstones.js
 Comment: 
 
-Filename: static/js/ace/snippets/mips_assembler.js
+Filename: static/js/ace/snippets/html.js
 Comment: 
 
-Filename: static/js/ace/snippets/ftl.js
+Filename: static/js/ace/snippets/yaml.js
 Comment: 
 
-Filename: static/js/ace/snippets/mipsassembler.js
+Filename: static/js/ace/snippets/cirru.js
 Comment: 
 
-Filename: static/js/ace/snippets/html_elixir.js
+Filename: static/js/ace/snippets/dart.js
 Comment: 
 
-Filename: static/js/ace/snippets/asciidoc.js
+Filename: static/js/ace/snippets/coldfusion.js
 Comment: 
 
-Filename: static/js/ace/snippets/gcode.js
+Filename: static/js/ace/snippets/haxe.js
 Comment: 
 
-Filename: static/js/ace/snippets/erlang.js
+Filename: static/js/ace/snippets/prolog.js
 Comment: 
 
-Filename: static/js/ace/snippets/smarty.js
+Filename: static/js/ace/snippets/scheme.js
 Comment: 
 
-Filename: static/js/ace/snippets/powershell.js
+Filename: static/js/ace/snippets/jsp.js
 Comment: 
 
-Filename: static/js/ace/snippets/css.js
+Filename: static/js/ace/snippets/pascal.js
 Comment: 
 
-Filename: static/js/ace/snippets/perl.js
+Filename: static/js/ace/snippets/soy_template.js
 Comment: 
 
-Filename: static/js/ace/snippets/jade.js
+Filename: static/js/ace/snippets/abc.js
 Comment: 
 
-Filename: static/js/ace/snippets/vhdl.js
+Filename: static/js/ace/snippets/javascript.js
 Comment: 
 
-Filename: static/js/ace/snippets/django.js
+Filename: static/js/ace/snippets/io.js
 Comment: 
 
-Filename: static/js/ace/snippets/csharp.js
+Filename: static/js/ace/snippets/sqlserver.js
 Comment: 
 
-Filename: static/js/ace/snippets/latex.js
+Filename: static/js/ace/snippets/gitignore.js
 Comment: 
 
-Filename: static/js/ace/snippets/c9search.js
+Filename: static/js/ace/snippets/vhdl.js
 Comment: 
 
-Filename: static/js/ace/snippets/less.js
+Filename: static/js/ace/snippets/vbscript.js
 Comment: 
 
-Filename: static/js/ace/snippets/markdown.js
+Filename: static/js/ace/snippets/xml.js
 Comment: 
 
-Filename: static/js/ace/snippets/livescript.js
+Filename: static/js/ace/snippets/sass.js
 Comment: 
 
-Filename: static/js/ace/snippets/swift.js
+Filename: static/js/ace/snippets/sql.js
 Comment: 
 
-Filename: static/js/ace/snippets/jsx.js
+Filename: static/js/ace/mode-jsx.js
 Comment: 
 
-Filename: static/js/ace/snippets/handlebars.js
+Filename: static/js/ace/worker-coffee.js
 Comment: 
 
-Filename: static/js/ace/snippets/sqlserver.js
+Filename: static/js/ace/mode-perl.js
 Comment: 
 
-Filename: static/js/ace/snippets/d.js
+Filename: static/js/ace/mode-handlebars.js
 Comment: 
 
-Filename: static/js/ace/snippets/lua.js
+Filename: static/js/ace/mode-kotlin.js
 Comment: 
 
-Filename: static/js/ace/snippets/snippets.js
+Filename: static/js/ace/mode-tsx.js
 Comment: 
 
-Filename: static/js/ace/snippets/apache_conf.js
+Filename: static/js/ace/theme-tomorrow.js
 Comment: 
 
-Filename: static/js/ace/snippets/clojure.js
+Filename: static/js/ace/mode-rdoc.js
 Comment: 
 
-Filename: static/js/ace/snippets/autohotkey.js
+Filename: static/js/ace/theme-clouds_midnight.js
 Comment: 
 
-Filename: static/js/ace/snippets/plain_text.js
+Filename: static/js/ace/theme-merbivore.js
 Comment: 
 
-Filename: static/js/ace/snippets/lisp.js
+Filename: static/js/ace/mode-twig.js
 Comment: 
 
-Filename: static/js/ace/snippets/applescript.js
+Filename: static/js/ace/mode-tex.js
 Comment: 
 
-Filename: static/js/ace/snippets/velocity.js
+Filename: static/js/ace/mode-lean.js
 Comment: 
 
-Filename: static/js/ace/snippets/dockerfile.js
+Filename: static/js/ace/mode-hjson.js
 Comment: 
 
-Filename: static/js/ace/snippets/actionscript.js
+Filename: static/js/ace/mode-cirru.js
 Comment: 
 
-Filename: static/js/ace/snippets/vala.js
+Filename: static/js/ace/ext-keybinding_menu.js
 Comment: 
 
-Filename: static/js/ace/snippets/elm.js
+Filename: static/js/ace/mode-live_script.js
 Comment: 
 
-Filename: static/js/ace/snippets/tsx.js
+Filename: static/js/ace/mode-tcl.js
 Comment: 
 
-Filename: static/js/ace/snippets/io.js
+Filename: static/js/ace/mode-textile.js
 Comment: 
 
-Filename: static/js/ace/snippets/objectivec.js
+Filename: static/js/ace/mode-liquid.js
 Comment: 
 
-Filename: static/js/ace/snippets/yaml.js
+Filename: static/js/ace/mode-html_ruby.js
 Comment: 
 
-Filename: static/js/ace/snippets/pascal.js
+Filename: static/js/ace/mode-haml.js
 Comment: 
 
-Filename: static/js/ace/snippets/curly.js
+Filename: static/js/ace/mode-luapage.js
 Comment: 
 
-Filename: static/js/ace/snippets/scss.js
+Filename: static/js/ace/mode-glsl.js
 Comment: 
 
-Filename: static/js/ace/snippets/javascript.js
+Filename: static/js/ace/mode-makefile.js
 Comment: 
 
-Filename: static/js/ace/snippets/mushcode.js
+Filename: static/js/ace/theme-tomorrow_night_eighties.js
 Comment: 
 
-Filename: static/js/ace/snippets/mel.js
+Filename: static/js/ace/mode-jack.js
 Comment: 
 
-Filename: static/js/ace/snippets/haskell_cabal.js
+Filename: static/js/ace/mode-coldfusion.js
 Comment: 
 
-Filename: static/js/ace/snippets/mysql.js
+Filename: static/js/ace/mode-python.js
 Comment: 
 
-Filename: static/js/ace/snippets/sql.js
+Filename: static/js/ace/mode-verilog.js
 Comment: 
 
-Filename: static/js/ace/snippets/lucene.js
+Filename: static/js/ace/mode-html_elixir.js
 Comment: 
 
-Filename: static/js/ace/snippets/wollok.js
+Filename: static/js/ace/mode-pgsql.js
 Comment: 
 
-Filename: static/js/ace/snippets/batchfile.js
+Filename: static/js/ace/mode-snippets.js
 Comment: 
 
-Filename: static/js/ace/snippets/python.js
+Filename: static/js/ace/mode-vala.js
 Comment: 
 
-Filename: static/js/ace/snippets/rust.js
+Filename: static/js/ace/mode-diff.js
 Comment: 
 
-Filename: static/js/ace/snippets/ini.js
+Filename: static/js/ace/mode-praat.js
 Comment: 
 
-Filename: static/js/ace/snippets/dot.js
+Filename: static/js/ace/ace.js
 Comment: 
 
-Filename: static/js/ace/snippets/rst.js
+Filename: static/js/ace/mode-abap.js
 Comment: 
 
-Filename: static/js/ace/snippets/nsis.js
+Filename: static/js/ace/ext-old_ie.js
 Comment: 
 
-Filename: static/js/ace/snippets/jsoniq.js
+Filename: static/js/ace/mode-gherkin.js
 Comment: 
 
-Filename: static/js/ace/snippets/properties.js
+Filename: static/js/ace/theme-eclipse.js
 Comment: 
 
-Filename: static/js/ace/snippets/c_cpp.js
+Filename: static/js/ace/mode-xml.js
 Comment: 
 
-Filename: static/js/ace/snippets/kotlin.js
+Filename: static/js/ace/theme-idle_fingers.js
 Comment: 
 
-Filename: static/js/ace/snippets/toml.js
+Filename: static/js/ace/mode-swift.js
 Comment: 
 
-Filename: static/js/ace/snippets/scheme.js
+Filename: static/js/ace/mode-batchfile.js
 Comment: 
 
-Filename: static/js/ace/snippets/twig.js
+Filename: static/js/ace/ext-linking.js
 Comment: 
 
-Filename: static/js/ace/snippets/abap.js
+Filename: static/js/ace/mode-scheme.js
 Comment: 
 
-Filename: static/js/ace/snippets/sass.js
+Filename: static/js/ace/theme-pastel_on_dark.js
 Comment: 
 
-Filename: static/js/ace/snippets/eiffel.js
+Filename: static/js/ace/mode-django.js
 Comment: 
 
-Filename: static/js/ace/snippets/gobstones.js
+Filename: static/js/ace/theme-kuroir.js
 Comment: 
 
-Filename: static/js/ace/snippets/scala.js
+Filename: static/js/ace/mode-rst.js
 Comment: 
 
-Filename: static/js/ace/snippets/diff.js
+Filename: static/js/ace/mode-nsis.js
 Comment: 
 
-Filename: static/js/ace/snippets/assembly_x86.js
+Filename: static/js/ace/mode-mel.js
 Comment: 
 
-Filename: static/js/ace/snippets/html.js
+Filename: static/js/ace/mode-sql.js
 Comment: 
 
-Filename: static/js/ace/snippets/soy_template.js
+Filename: static/js/ace/mode-dockerfile.js
 Comment: 
 
-Filename: static/js/ace/snippets/liquid.js
+Filename: static/js/ace/theme-mono_industrial.js
 Comment: 
 
-Filename: static/js/ace/snippets/rdoc.js
+Filename: static/js/ace/mode-protobuf.js
 Comment: 
 
-Filename: static/js/ace/snippets/sjs.js
+Filename: static/js/ace/mode-gitignore.js
 Comment: 
 
-Filename: static/js/ace/snippets/gherkin.js
+Filename: static/js/ace/mode-jsoniq.js
 Comment: 
 
-Filename: static/js/ace/snippets/groovy.js
+Filename: static/js/ace/mode-json.js
 Comment: 
 
-Filename: static/js/ace/snippets/vbscript.js
+Filename: static/js/ace/mode-mips_assembler.js
 Comment: 
 
-Filename: static/js/ace/snippets/pgsql.js
+Filename: static/js/ace/theme-solarized_light.js
 Comment: 
 
-Filename: static/js/ace/mode-mips_assembler.js
+Filename: static/js/ace/mode-lsl.js
 Comment: 
 
-Filename: static/js/ace/mode-css.js
+Filename: static/js/ace/mode-less.js
 Comment: 
 
-Filename: static/js/ace/mode-jsoniq.js
+Filename: static/js/ace/mode-livescript.js
 Comment: 
 
-Filename: static/js/ace/mode-elm.js
+Filename: static/js/ace/mode-clojure.js
 Comment: 
 
-Filename: static/js/ace/mode-eiffel.js
+Filename: static/js/ace/theme-vibrant_ink.js
 Comment: 
 
-Filename: static/js/ace/mode-protobuf.js
+Filename: static/js/ace/mode-groovy.js
 Comment: 
 
-Filename: static/js/ace/mode-ada.js
+Filename: static/js/ace/mode-rust.js
 Comment: 
 
-Filename: static/js/ace/mode-makefile.js
+Filename: static/js/ace/mode-lua.js
 Comment: 
 
-Filename: static/js/ace/mode-ejs.js
+Filename: static/js/ace/mode-smarty.js
 Comment: 
 
-Filename: static/js/ace/theme-dreamweaver.js
+Filename: static/js/ace/mode-io.js
 Comment: 
 
-Filename: static/js/ace/mode-elixir.js
+Filename: static/js/ace/mode-gcode.js
 Comment: 
 
-Filename: static/js/ace/ext-searchbox.js
+Filename: static/js/ace/mode-autohotkey.js
 Comment: 
 
-Filename: static/js/ace/mode-toml.js
+Filename: static/js/ace/theme-terminal.js
 Comment: 
 
-Filename: static/js/ace/mode-scala.js
+Filename: static/js/ace/ext-themelist.js
 Comment: 
 
-Filename: static/js/ace/mode-luapage.js
+Filename: static/js/ace/mode-html.js
 Comment: 
 
-Filename: static/js/ace/ext-chromevox.js
+Filename: static/js/ace/theme-dreamweaver.js
 Comment: 
 
-Filename: static/js/ace/ext-error_marker.js
+Filename: static/js/ace/mode-ruby.js
 Comment: 
 
-Filename: static/js/ace/mode-python.js
+Filename: static/js/ace/mode-csharp.js
 Comment: 
 
-Filename: static/js/ace/mode-gobstones.js
+Filename: static/js/ace/ext-searchbox.js
 Comment: 
 
-Filename: static/js/ace/mode-praat.js
+Filename: static/js/ace/mode-forth.js
 Comment: 
 
-Filename: static/js/ace/mode-scad.js
+Filename: static/js/ace/mode-sjs.js
 Comment: 
 
-Filename: static/js/ace/theme-merbivore_soft.js
+Filename: static/js/ace/mode-r.js
 Comment: 
 
-Filename: static/js/ace/mode-bro.js
+Filename: static/js/ace/mode-svg.js
 Comment: 
 
-Filename: static/js/ace/theme-sqlserver.js
+Filename: static/js/ace/mode-ini.js
 Comment: 
 
-Filename: static/js/ace/mode-tsx.js
+Filename: static/js/ace/theme-tomorrow_night_bright.js
 Comment: 
 
-Filename: static/js/ace/mode-latex.js
+Filename: static/js/ace/mode-swig.js
 Comment: 
 
-Filename: static/js/ace/mode-yaml.js
+Filename: static/js/ace/worker-css.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow_night.js
+Filename: static/js/ace/mode-mask.js
 Comment: 
 
-Filename: static/js/ace/mode-jade.js
+Filename: static/js/ace/mode-curly.js
 Comment: 
 
-Filename: static/js/ace/mode-verilog.js
+Filename: static/js/ace/mode-rhtml.js
 Comment: 
 
-Filename: static/js/ace/ext-modelist.js
+Filename: static/js/ace/theme-monokai.js
 Comment: 
 
-Filename: static/js/ace/theme-xcode.js
+Filename: static/js/ace/mode-haskell_cabal.js
 Comment: 
 
-Filename: static/js/ace/mode-sass.js
+Filename: static/js/ace/theme-clouds.js
 Comment: 
 
-Filename: static/js/ace/mode-live_script.js
+Filename: static/js/ace/mode-soy_template.js
 Comment: 
 
-Filename: static/js/ace/worker-html.js
+Filename: static/js/ace/mode-markdown.js
 Comment: 
 
-Filename: static/js/ace/theme-kuroir.js
+Filename: static/js/ace/mode-abc.js
 Comment: 
 
-Filename: static/js/ace/mode-svg.js
+Filename: static/js/ace/mode-php.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow_night_eighties.js
+Filename: static/js/ace/ext-static_highlight.js
 Comment: 
 
-Filename: static/js/ace/mode-applescript.js
+Filename: static/js/ace/mode-dart.js
 Comment: 
 
-Filename: static/js/ace/mode-haskell_cabal.js
+Filename: static/js/ace/mode-actionscript.js
 Comment: 
 
-Filename: static/js/ace/mode-lean.js
+Filename: static/js/ace/mode-properties.js
 Comment: 
 
-Filename: static/js/ace/mode-rust.js
+Filename: static/js/ace/worker-json.js
 Comment: 
 
-Filename: static/js/ace/mode-dot.js
+Filename: static/js/ace/mode-xquery.js
 Comment: 
 
-Filename: static/js/ace/mode-scss.js
+Filename: static/js/ace/mode-java.js
 Comment: 
 
-Filename: static/js/ace/mode-html.js
+Filename: static/js/ace/theme-tomorrow_night_blue.js
 Comment: 
 
-Filename: static/js/ace/mode-actionscript.js
+Filename: static/js/ace/keybinding-vim.js
 Comment: 
 
-Filename: static/js/ace/mode-sqlserver.js
+Filename: static/js/ace/theme-xcode.js
 Comment: 
 
-Filename: static/js/ace/theme-solarized_light.js
+Filename: static/js/ace/mode-elixir.js
 Comment: 
 
-Filename: static/js/ace/mode-mask.js
+Filename: static/js/ace/mode-sass.js
 Comment: 
 
-Filename: static/js/ace/mode-ocaml.js
+Filename: static/js/ace/mode-scad.js
 Comment: 
 
-Filename: static/js/ace/mode-d.js
+Filename: static/js/ace/theme-chaos.js
 Comment: 
 
-Filename: static/js/ace/mode-lua.js
+Filename: static/js/ace/mode-ada.js
 Comment: 
 
-Filename: static/js/ace/worker-javascript.js
+Filename: static/js/ace/mode-yaml.js
 Comment: 
 
-Filename: static/js/ace/mode-ini.js
+Filename: static/js/ace/mode-text.js
 Comment: 
 
-Filename: static/js/ace/theme-solarized_dark.js
+Filename: static/js/ace/mode-lisp.js
 Comment: 
 
-Filename: static/js/ace/mode-snippets.js
+Filename: static/js/ace/mode-asciidoc.js
 Comment: 
 
-Filename: static/js/ace/mode-livescript.js
+Filename: static/js/ace/mode-cobol.js
 Comment: 
 
-Filename: static/js/ace/theme-idle_fingers.js
+Filename: static/js/ace/ext-whitespace.js
 Comment: 
 
-Filename: static/js/ace/theme-vibrant_ink.js
+Filename: static/js/ace/mode-dot.js
 Comment: 
 
-Filename: static/js/ace/worker-css.js
+Filename: static/js/ace/theme-github.js
 Comment: 
 
-Filename: static/js/ace/worker-json.js
+Filename: static/js/ace/mode-erlang.js
 Comment: 
 
-Filename: static/js/ace/mode-lisp.js
+Filename: static/js/ace/mode-razor.js
 Comment: 
 
-Filename: static/js/ace/mode-csharp.js
+Filename: static/js/ace/ext-split.js
 Comment: 
 
-Filename: static/js/ace/ext-beautify.js
+Filename: static/js/ace/mode-scss.js
 Comment: 
 
-Filename: static/js/ace/mode-julia.js
+Filename: static/js/ace/mode-powershell.js
 Comment: 
 
-Filename: static/js/jquery.min.js
+Filename: static/js/ace/theme-iplastic.js
 Comment: 
 
-Filename: static/js/sugar.min.js
+Filename: static/js/ace/ext-chromevox.js
 Comment: 
 
-Filename: static/js/index.js
+Filename: static/js/ace/theme-kr_theme.js
 Comment: 
 
-Filename: static/js/highlight.min.js
+Filename: static/js/ace/mode-gobstones.js
 Comment: 
 
-Filename: static/js/translations.js
+Filename: static/js/ace/mode-mipsassembler.js
 Comment: 
 
-Filename: static/js/vue.min.js
+Filename: static/js/ace/theme-crimson_editor.js
 Comment: 
 
-Filename: static/components/mtable.js
+Filename: static/js/ace/mode-jsp.js
 Comment: 
 
-Filename: static/components/mtable.html
+Filename: static/js/ace/ext-beautify.js
 Comment: 
 
-Filename: static/css/future.css
+Filename: static/js/dbadmin.js
 Comment: 
 
-Filename: static/css/gitlog.min.css
+Filename: static/js/highlight.min.js
 Comment: 
 
-Filename: static/images/alert-blue.gif
+Filename: static/js/translations.js
 Comment: 
 
-Filename: static/images/alert-red.gif
+Filename: static/js/utils.js
 Comment: 
 
-Filename: static/images/alert-yellow.gif
+Filename: static/js/sugar.min.js
 Comment: 
 
-Filename: static/images/forkme.png
+Filename: static/js/jquery.min.js
 Comment: 
 
-Filename: static/images/widget.gif
+Filename: templates/dbadmin.html
 Comment: 
 
-Filename: static/images/alert-orange.gif
+Filename: templates/gitlog.html
 Comment: 
 
-Filename: static/images/alert-green.gif
+Filename: templates/index.html
 Comment: 
 
-Filename: static/favicon.ico
+Filename: templates/ticket.html
+Comment: 
+
+Filename: templates/translations.html
 Comment: 
 
 Zip file comment:
```

#### __init__.py

```diff
@@ -190,30 +190,30 @@
             and not app.startswith("__")
             and not app.startswith(".")
             and (not exposed_names or app in exposed_names)
         ]
         apps.sort(key=lambda item: item["name"])
         return {"payload": apps, "status": "success"}
 
-    @action("delete_app/<name:re:\w+>", method="POST")
+    @action("delete_app/<name:re:\\w+>", method="POST")
     @session_secured
     def delete_app(name):
         """delete the app"""
         path = os.path.join(FOLDER, name)
         timestamp = datetime.datetime.now().strftime("%Y-%m-%d")
         archive = os.path.join(FOLDER, "%s.%s.zip" % (name, timestamp))
         if os.path.exists(path) and os.path.isdir(path):
             # zip the folder, just in case
             shutil.make_archive(archive, "zip", path)
             # then remove the app
             shutil.rmtree(path)
             return {"status": "success", "payload": "Deleted"}
         return {"status": "success", "payload": "App does not exist"}
 
-    @action("new_file/<name:re:\w+>/<file_name:path>", method="POST")
+    @action("new_file/<name:re:\\w+>/<file_name:path>", method="POST")
     @session_secured
     def new_file(name, file_name):
         """creates a new file"""
         path = os.path.join(FOLDER, name)
         form = request.json
         if not os.path.exists(path):
             return {"status": "success", "payload": "App does not exist"}
```

#### static/js/index.js

##### js-beautify {}

```diff
@@ -280,14 +280,15 @@
 
             .then(r => {
                 app.vue.password = '';
                 if (r.user) {
                     app.vue.user = true;
                     app.init();
                 }
+                location.reload();
             });
     };
     app.logout = () => {
         Q.post('../logout').then(r => window.location.reload());
     };
     app.methods = {
         select: app.select_app,
```

### Comparing `py4web-1.20231115.1/py4web/assets/py4web.app._default.zip` & `py4web-1.20240420.1/py4web/assets/py4web.app._default.zip`

 * *Files 1% similar despite different names*

#### zipinfo {}

```diff
@@ -1,6 +1,6 @@
 Zip file size: 187155 bytes, number of entries: 4
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 __init__.py
--rw-rw-r--  3.0 unx     1811 tx defN 23-May-08 00:39 templates/index.html
--rw-rw-r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/images/logo.png
--rw-rw-r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 __init__.py
+-rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
+-rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/images/logo.png
+-rw-r--r--  3.0 unx     1811 tx defN 23-May-08 00:39 templates/index.html
 4 files, 215409 bytes uncompressed, 186479 bytes compressed:  13.4%
```

#### zipnote {}

```diff
@@ -1,13 +1,13 @@
 Filename: __init__.py
 Comment: 
 
-Filename: templates/index.html
+Filename: static/favicon.ico
 Comment: 
 
 Filename: static/images/logo.png
 Comment: 
 
-Filename: static/favicon.ico
+Filename: templates/index.html
 Comment: 
 
 Zip file comment:
```

### Comparing `py4web-1.20231115.1/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20240420.1/py4web/assets/py4web.app._documentation.zip`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,158 +1,158 @@
 Zip file size: 4359741 bytes, number of entries: 156
--rw-rw-r--  3.0 unx      112 tx defN 23-Oct-23 01:17 __init__.py
--rw-r--r--  3.0 unx    54626 tx defN 23-Nov-15 07:18 static/pt/chapter-14.html
--rw-r--r--  3.0 unx   125929 tx defN 23-Nov-15 07:18 static/pt/searchindex.js
--rw-r--r--  3.0 unx    18732 tx defN 23-Oct-30 01:31 static/pt/_static/searchtools.js
--rw-r--r--  3.0 unx     4289 tx defN 23-Nov-15 07:18 static/pt/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     5023 tx defN 23-Oct-30 01:31 static/pt/_static/js/theme.js
--rw-r--r--  3.0 unx     2734 tx defN 23-Oct-30 01:31 static/pt/_static/js/html5shiv.min.js
--rw-r--r--  3.0 unx     1333 tx defN 23-May-08 00:39 static/pt/_static/js/toggle.js
--rw-r--r--  3.0 unx     4370 tx defN 23-Oct-30 01:31 static/pt/_static/js/html5shiv-printshiv.min.js
--rw-r--r--  3.0 unx      934 tx defN 23-Oct-30 01:31 static/pt/_static/js/badge_only.js
--rw-r--r--  3.0 unx      335 tx defN 23-Nov-15 07:18 static/pt/_static/documentation_options.js
--rw-r--r--  3.0 unx     4902 tx defN 23-Nov-15 07:18 static/pt/_static/pygments.css
--rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/pt/_static/logo.png
--rw-r--r--  3.0 unx    14417 tx defN 23-Nov-15 07:18 static/pt/_static/language_data.js
--rw-r--r--  3.0 unx     1989 bx stor 23-May-08 00:39 static/pt/_static/logo-32x32.ico
--rw-r--r--  3.0 unx       90 bx defN 23-Oct-30 01:31 static/pt/_static/plus.png
+-rw-r--r--  3.0 unx      112 tx defN 23-May-08 00:39 __init__.py
+-rw-r--r--  3.0 unx    32038 bx defN 23-Nov-15 07:16 static/favicon.ico
+-rw-r--r--  3.0 unx    53993 tx defN 23-Nov-15 07:16 static/en/chapter-14.html
+-rw-r--r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/en/dark.css
+-rw-r--r--  3.0 unx    94790 tx defN 23-Nov-15 07:16 static/en/chapter-06.html
+-rw-r--r--  3.0 unx    63512 tx defN 23-Nov-15 07:16 static/en/chapter-09.html
+-rw-r--r--  3.0 unx     7103 tx defN 23-Nov-15 07:16 static/en/search.html
+-rw-r--r--  3.0 unx   189442 tx defN 23-Nov-15 07:16 static/en/chapter-12.html
+-rw-r--r--  3.0 unx   499548 tx defN 23-Nov-15 07:18 static/en/chapter-07.html
+-rw-r--r--  3.0 unx    19102 tx defN 23-Nov-15 07:16 static/en/chapter-02.html
+-rw-r--r--  3.0 unx    12032 tx defN 23-Nov-15 07:16 static/en/chapter-04.html
+-rw-r--r--  3.0 unx     6828 tx defN 23-Nov-15 07:16 static/en/genindex.html
+-rw-r--r--  3.0 unx   111513 tx defN 23-Nov-15 07:16 static/en/chapter-10.html
+-rw-r--r--  3.0 unx       90 bx defN 23-Oct-30 01:31 static/en/_static/minus.png
+-rw-r--r--  3.0 unx     4231 tx defN 23-Oct-30 01:31 static/en/_static/tabs.js
+-rw-r--r--  3.0 unx     4902 tx defN 23-Nov-15 07:18 static/en/_static/pygments.css
+-rw-r--r--  3.0 unx     4472 tx defN 23-Oct-30 01:31 static/en/_static/doctools.js
+-rw-r--r--  3.0 unx     4289 tx defN 23-Nov-15 07:18 static/en/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--  3.0 unx    89501 tx defN 23-Nov-15 07:18 static/en/_static/jquery.js
+-rw-r--r--  3.0 unx      286 bx stor 23-Oct-30 01:31 static/en/_static/file.png
+-rw-r--r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/en/_static/css/dark.css
+-rw-r--r--  3.0 unx     3229 tx defN 23-Oct-30 01:31 static/en/_static/css/badge_only.css
+-rw-r--r--  3.0 unx   135314 tx defN 23-Oct-30 01:31 static/en/_static/css/theme.css
+-rw-r--r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/en/_static/css/toggle.css
+-rw-r--r--  3.0 unx     5123 tx defN 23-Oct-30 01:31 static/en/_static/sphinx_highlight.js
+-rw-r--r--  3.0 unx     1989 bx stor 23-May-08 00:39 static/en/_static/logo-32x32.ico
+-rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/en/_static/logo.png
+-rw-r--r--  3.0 unx      335 tx defN 23-Nov-15 07:18 static/en/_static/documentation_options.js
+-rw-r--r--  3.0 unx     4758 tx defN 23-Nov-15 07:18 static/en/_static/language_data.js
+-rw-r--r--  3.0 unx    18732 tx defN 23-Oct-30 01:31 static/en/_static/searchtools.js
+-rw-r--r--  3.0 unx     2734 tx defN 23-Oct-30 01:31 static/en/_static/js/html5shiv.min.js
+-rw-r--r--  3.0 unx      934 tx defN 23-Oct-30 01:31 static/en/_static/js/badge_only.js
+-rw-r--r--  3.0 unx     5023 tx defN 23-Oct-30 01:31 static/en/_static/js/theme.js
+-rw-r--r--  3.0 unx     1333 tx defN 23-May-08 00:39 static/en/_static/js/toggle.js
+-rw-r--r--  3.0 unx     4370 tx defN 23-Oct-30 01:31 static/en/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--  3.0 unx       90 bx defN 23-Oct-30 01:31 static/en/_static/plus.png
+-rw-r--r--  3.0 unx    15094 tx defN 23-Nov-15 07:18 static/en/_static/basic.css
+-rw-r--r--  3.0 unx     1804 tx defN 23-Oct-30 01:31 static/en/_static/tabs.css
+-rw-r--r--  3.0 unx    91743 tx defN 23-Nov-15 07:16 static/en/searchindex.js
+-rw-r--r--  3.0 unx    19991 tx defN 23-Nov-15 07:16 static/en/index.html
+-rw-r--r--  3.0 unx    54280 tx defN 23-Nov-15 07:16 static/en/chapter-13.html
+-rw-r--r--  3.0 unx    11257 bx defN 23-May-08 00:39 static/en/_images/form1.png
+-rw-r--r--  3.0 unx    53747 bx defN 23-May-08 00:39 static/en/_images/dashboard_error.png
+-rw-r--r--  3.0 unx    41285 bx defN 23-May-08 00:39 static/en/_images/grid.png
+-rw-r--r--  3.0 unx    44559 bx defN 23-May-08 00:39 static/en/_images/grid_nocss.png
+-rw-r--r--  3.0 unx    52898 bx defN 23-May-08 00:39 static/en/_images/dashboard.png
+-rw-r--r--  3.0 unx   154315 bx defN 23-May-08 00:39 static/en/_images/dashboard_ticket.png
+-rw-r--r--  3.0 unx   135864 bx defN 23-May-08 00:39 static/en/_images/dashboard_main.png
+-rw-r--r--  3.0 unx    12086 bx defN 23-May-08 00:39 static/en/_images/_scaffold.png
+-rw-r--r--  3.0 unx    30931 bx defN 23-May-08 00:39 static/en/_images/tags2.png
+-rw-r--r--  3.0 unx   174817 bx defN 23-May-08 00:39 static/en/_images/dashboard_edit.png
+-rw-r--r--  3.0 unx    58653 bx defN 23-May-08 00:39 static/en/_images/grid_columns.png
+-rw-r--r--  3.0 unx    40409 bx defN 23-May-08 00:39 static/en/_images/form2.png
+-rw-r--r--  3.0 unx    24753 bx defN 23-May-08 00:39 static/en/_images/tags_db.png
+-rw-r--r--  3.0 unx    46250 bx defN 23-May-08 00:39 static/en/_images/form4.png
+-rw-r--r--  3.0 unx    40478 bx defN 23-May-08 00:39 static/en/_images/command.png
+-rw-r--r--  3.0 unx    38066 bx defN 23-May-08 00:39 static/en/_images/form6.png
+-rw-r--r--  3.0 unx    30536 bx defN 23-May-08 00:39 static/en/_images/restapi.png
+-rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/en/_images/logo.png
+-rw-r--r--  3.0 unx    29268 bx defN 23-May-08 00:39 static/en/_images/restapi2.png
+-rw-r--r--  3.0 unx    39765 bx defN 23-May-08 00:39 static/en/_images/form5.png
+-rw-r--r--  3.0 unx    16627 bx defN 23-May-08 00:39 static/en/_images/simple_counter.png
+-rw-r--r--  3.0 unx    37805 bx defN 23-May-08 00:39 static/en/_images/form3.png
+-rw-r--r--  3.0 unx    40745 bx defN 23-May-08 00:39 static/en/_images/grid_bulmacss.png
+-rw-r--r--  3.0 unx    40467 bx defN 23-May-08 00:39 static/en/_images/dashboard_new_app.png
+-rw-r--r--  3.0 unx    77606 bx defN 23-May-08 00:39 static/en/_images/main_page.png
+-rw-r--r--  3.0 unx    86267 bx defN 23-May-08 00:39 static/en/_images/dashboard_login.png
+-rw-r--r--  3.0 unx    50011 bx defN 23-May-08 00:39 static/en/_images/first_run.png
+-rw-r--r--  3.0 unx   147429 bx defN 23-May-08 00:39 static/en/_images/dashboard_restapi.png
+-rw-r--r--  3.0 unx    11524 tx defN 23-Nov-15 07:16 static/en/chapter-11.html
+-rw-r--r--  3.0 unx    45695 tx defN 23-Nov-15 07:16 static/en/chapter-03.html
+-rw-r--r--  3.0 unx    15659 tx defN 23-Nov-15 07:16 static/en/chapter-01.html
+-rw-r--r--  3.0 unx    42508 tx defN 23-Nov-15 07:16 static/en/chapter-05.html
+-rw-r--r--  3.0 unx    43157 tx defN 23-Nov-15 07:16 static/en/chapter-15.html
+-rw-r--r--  3.0 unx    85384 tx defN 23-Nov-15 07:16 static/en/chapter-16.html
+-rw-r--r--  3.0 unx   129405 tx defN 23-Nov-15 07:16 static/en/chapter-08.html
+-rw-r--r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/en/toggle.css
+-rw-r--r--  3.0 unx      248 tx defN 23-Nov-15 07:16 static/index.html
+-rw-r--r--  3.0 unx    54626 tx defN 23-Nov-15 07:16 static/pt/chapter-14.html
+-rw-r--r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/pt/dark.css
+-rw-r--r--  3.0 unx    93424 tx defN 23-Nov-15 07:16 static/pt/chapter-06.html
+-rw-r--r--  3.0 unx    61453 tx defN 23-Nov-15 07:16 static/pt/chapter-09.html
+-rw-r--r--  3.0 unx     7255 tx defN 23-Nov-15 07:16 static/pt/search.html
+-rw-r--r--  3.0 unx   189143 tx defN 23-Nov-15 07:16 static/pt/chapter-12.html
+-rw-r--r--  3.0 unx   464454 tx defN 23-Nov-15 07:18 static/pt/chapter-07.html
+-rw-r--r--  3.0 unx    19651 tx defN 23-Nov-15 07:16 static/pt/chapter-02.html
+-rw-r--r--  3.0 unx    12207 tx defN 23-Nov-15 07:16 static/pt/chapter-04.html
+-rw-r--r--  3.0 unx     6976 tx defN 23-Nov-15 07:16 static/pt/genindex.html
+-rw-r--r--  3.0 unx   105050 tx defN 23-Nov-15 07:16 static/pt/chapter-10.html
+-rw-r--r--  3.0 unx       90 bx defN 23-Oct-30 01:31 static/pt/_static/minus.png
 -rw-r--r--  3.0 unx     4231 tx defN 23-Oct-30 01:31 static/pt/_static/tabs.js
+-rw-r--r--  3.0 unx     4902 tx defN 23-Nov-15 07:18 static/pt/_static/pygments.css
+-rw-r--r--  3.0 unx     4472 tx defN 23-Oct-30 01:31 static/pt/_static/doctools.js
+-rw-r--r--  3.0 unx     4289 tx defN 23-Nov-15 07:18 static/pt/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--  3.0 unx    89501 tx defN 23-Nov-15 07:18 static/pt/_static/jquery.js
+-rw-r--r--  3.0 unx    26718 tx defN 23-Oct-30 01:31 static/pt/_static/portuguese-stemmer.js
+-rw-r--r--  3.0 unx     2351 tx defN 23-Oct-30 01:31 static/pt/_static/translations.js
+-rw-r--r--  3.0 unx      286 bx stor 23-Oct-30 01:31 static/pt/_static/file.png
 -rw-r--r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/pt/_static/css/dark.css
 -rw-r--r--  3.0 unx     3229 tx defN 23-Oct-30 01:31 static/pt/_static/css/badge_only.css
 -rw-r--r--  3.0 unx   135314 tx defN 23-Oct-30 01:31 static/pt/_static/css/theme.css
 -rw-r--r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/pt/_static/css/toggle.css
--rw-r--r--  3.0 unx    26718 tx defN 23-Oct-30 01:31 static/pt/_static/portuguese-stemmer.js
--rw-r--r--  3.0 unx     4472 tx defN 23-Oct-30 01:31 static/pt/_static/doctools.js
--rw-r--r--  3.0 unx      286 bx stor 23-Oct-30 01:31 static/pt/_static/file.png
 -rw-r--r--  3.0 unx     5123 tx defN 23-Oct-30 01:31 static/pt/_static/sphinx_highlight.js
--rw-r--r--  3.0 unx     2351 tx defN 23-Oct-30 01:31 static/pt/_static/translations.js
--rw-r--r--  3.0 unx    89501 tx defN 23-Nov-15 07:18 static/pt/_static/jquery.js
+-rw-r--r--  3.0 unx     1989 bx stor 23-May-08 00:39 static/pt/_static/logo-32x32.ico
+-rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/pt/_static/logo.png
 -rw-r--r--  3.0 unx     8133 tx defN 23-Oct-30 01:31 static/pt/_static/base-stemmer.js
--rw-r--r--  3.0 unx       90 bx defN 23-Oct-30 01:31 static/pt/_static/minus.png
+-rw-r--r--  3.0 unx      335 tx defN 23-Nov-15 07:18 static/pt/_static/documentation_options.js
+-rw-r--r--  3.0 unx    14417 tx defN 23-Nov-15 07:18 static/pt/_static/language_data.js
+-rw-r--r--  3.0 unx    18732 tx defN 23-Oct-30 01:31 static/pt/_static/searchtools.js
+-rw-r--r--  3.0 unx     2734 tx defN 23-Oct-30 01:31 static/pt/_static/js/html5shiv.min.js
+-rw-r--r--  3.0 unx      934 tx defN 23-Oct-30 01:31 static/pt/_static/js/badge_only.js
+-rw-r--r--  3.0 unx     5023 tx defN 23-Oct-30 01:31 static/pt/_static/js/theme.js
+-rw-r--r--  3.0 unx     1333 tx defN 23-May-08 00:39 static/pt/_static/js/toggle.js
+-rw-r--r--  3.0 unx     4370 tx defN 23-Oct-30 01:31 static/pt/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--  3.0 unx       90 bx defN 23-Oct-30 01:31 static/pt/_static/plus.png
 -rw-r--r--  3.0 unx    15094 tx defN 23-Nov-15 07:18 static/pt/_static/basic.css
 -rw-r--r--  3.0 unx     1804 tx defN 23-Oct-30 01:31 static/pt/_static/tabs.css
--rw-r--r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/pt/dark.css
--rw-r--r--  3.0 unx    41269 tx defN 23-Nov-15 07:18 static/pt/chapter-05.html
--rw-r--r--  3.0 unx   129331 tx defN 23-Nov-15 07:18 static/pt/chapter-08.html
--rw-r--r--  3.0 unx    12207 tx defN 23-Nov-15 07:18 static/pt/chapter-04.html
--rw-r--r--  3.0 unx     6976 tx defN 23-Nov-15 07:18 static/pt/genindex.html
--rw-r--r--  3.0 unx   464454 tx defN 23-Nov-15 07:18 static/pt/chapter-07.html
--rw-r--r--  3.0 unx    44996 tx defN 23-Nov-15 07:18 static/pt/chapter-03.html
--rw-r--r--  3.0 unx    93424 tx defN 23-Nov-15 07:18 static/pt/chapter-06.html
--rw-r--r--  3.0 unx    43327 tx defN 23-Nov-15 07:18 static/pt/chapter-15.html
--rw-r--r--  3.0 unx    19651 tx defN 23-Nov-15 07:18 static/pt/chapter-02.html
--rw-r--r--  3.0 unx     7255 tx defN 23-Nov-15 07:18 static/pt/search.html
--rw-r--r--  3.0 unx    61453 tx defN 23-Nov-15 07:18 static/pt/chapter-09.html
--rw-r--r--  3.0 unx    20017 tx defN 23-Nov-15 07:18 static/pt/index.html
+-rw-r--r--  3.0 unx   125929 tx defN 23-Nov-15 07:18 static/pt/searchindex.js
+-rw-r--r--  3.0 unx    20017 tx defN 23-Nov-15 07:16 static/pt/index.html
+-rw-r--r--  3.0 unx    54243 tx defN 23-Nov-15 07:16 static/pt/chapter-13.html
+-rw-r--r--  3.0 unx    11257 bx defN 23-May-08 00:39 static/pt/_images/form1.png
+-rw-r--r--  3.0 unx    53747 bx defN 23-May-08 00:39 static/pt/_images/dashboard_error.png
 -rw-r--r--  3.0 unx    41285 bx defN 23-May-08 00:39 static/pt/_images/grid.png
--rw-r--r--  3.0 unx    40745 bx defN 23-May-08 00:39 static/pt/_images/grid_bulmacss.png
+-rw-r--r--  3.0 unx    44559 bx defN 23-May-08 00:39 static/pt/_images/grid_nocss.png
 -rw-r--r--  3.0 unx    52898 bx defN 23-May-08 00:39 static/pt/_images/dashboard.png
--rw-r--r--  3.0 unx    53747 bx defN 23-May-08 00:39 static/pt/_images/dashboard_error.png
+-rw-r--r--  3.0 unx   154315 bx defN 23-May-08 00:39 static/pt/_images/dashboard_ticket.png
+-rw-r--r--  3.0 unx   135864 bx defN 23-May-08 00:39 static/pt/_images/dashboard_main.png
+-rw-r--r--  3.0 unx    12086 bx defN 23-May-08 00:39 static/pt/_images/_scaffold.png
+-rw-r--r--  3.0 unx    30931 bx defN 23-May-08 00:39 static/pt/_images/tags2.png
+-rw-r--r--  3.0 unx   174817 bx defN 23-May-08 00:39 static/pt/_images/dashboard_edit.png
+-rw-r--r--  3.0 unx    58653 bx defN 23-May-08 00:39 static/pt/_images/grid_columns.png
+-rw-r--r--  3.0 unx    40409 bx defN 23-May-08 00:39 static/pt/_images/form2.png
+-rw-r--r--  3.0 unx    24753 bx defN 23-May-08 00:39 static/pt/_images/tags_db.png
+-rw-r--r--  3.0 unx    46250 bx defN 23-May-08 00:39 static/pt/_images/form4.png
 -rw-r--r--  3.0 unx    40478 bx defN 23-May-08 00:39 static/pt/_images/command.png
+-rw-r--r--  3.0 unx    38066 bx defN 23-May-08 00:39 static/pt/_images/form6.png
+-rw-r--r--  3.0 unx    30536 bx defN 23-May-08 00:39 static/pt/_images/restapi.png
+-rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/pt/_images/logo.png
 -rw-r--r--  3.0 unx    29268 bx defN 23-May-08 00:39 static/pt/_images/restapi2.png
+-rw-r--r--  3.0 unx    39765 bx defN 23-May-08 00:39 static/pt/_images/form5.png
+-rw-r--r--  3.0 unx    16627 bx defN 23-May-08 00:39 static/pt/_images/simple_counter.png
+-rw-r--r--  3.0 unx    37805 bx defN 23-May-08 00:39 static/pt/_images/form3.png
+-rw-r--r--  3.0 unx    40745 bx defN 23-May-08 00:39 static/pt/_images/grid_bulmacss.png
 -rw-r--r--  3.0 unx    40467 bx defN 23-May-08 00:39 static/pt/_images/dashboard_new_app.png
 -rw-r--r--  3.0 unx    77606 bx defN 23-May-08 00:39 static/pt/_images/main_page.png
--rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/pt/_images/logo.png
--rw-r--r--  3.0 unx    37805 bx defN 23-May-08 00:39 static/pt/_images/form3.png
--rw-r--r--  3.0 unx    11257 bx defN 23-May-08 00:39 static/pt/_images/form1.png
--rw-r--r--  3.0 unx    16627 bx defN 23-May-08 00:39 static/pt/_images/simple_counter.png
--rw-r--r--  3.0 unx    30931 bx defN 23-May-08 00:39 static/pt/_images/tags2.png
--rw-r--r--  3.0 unx    44559 bx defN 23-May-08 00:39 static/pt/_images/grid_nocss.png
--rw-r--r--  3.0 unx    39765 bx defN 23-May-08 00:39 static/pt/_images/form5.png
--rw-r--r--  3.0 unx   147429 bx defN 23-May-08 00:39 static/pt/_images/dashboard_restapi.png
 -rw-r--r--  3.0 unx    86267 bx defN 23-May-08 00:39 static/pt/_images/dashboard_login.png
--rw-r--r--  3.0 unx   135864 bx defN 23-May-08 00:39 static/pt/_images/dashboard_main.png
--rw-r--r--  3.0 unx    30536 bx defN 23-May-08 00:39 static/pt/_images/restapi.png
--rw-r--r--  3.0 unx    58653 bx defN 23-May-08 00:39 static/pt/_images/grid_columns.png
--rw-r--r--  3.0 unx    24753 bx defN 23-May-08 00:39 static/pt/_images/tags_db.png
--rw-r--r--  3.0 unx   154315 bx defN 23-May-08 00:39 static/pt/_images/dashboard_ticket.png
--rw-r--r--  3.0 unx    40409 bx defN 23-May-08 00:39 static/pt/_images/form2.png
--rw-r--r--  3.0 unx    12086 bx defN 23-May-08 00:39 static/pt/_images/_scaffold.png
--rw-r--r--  3.0 unx    38066 bx defN 23-May-08 00:39 static/pt/_images/form6.png
--rw-r--r--  3.0 unx    46250 bx defN 23-May-08 00:39 static/pt/_images/form4.png
--rw-r--r--  3.0 unx   174817 bx defN 23-May-08 00:39 static/pt/_images/dashboard_edit.png
 -rw-r--r--  3.0 unx    50011 bx defN 23-May-08 00:39 static/pt/_images/first_run.png
+-rw-r--r--  3.0 unx   147429 bx defN 23-May-08 00:39 static/pt/_images/dashboard_restapi.png
+-rw-r--r--  3.0 unx    11831 tx defN 23-Nov-15 07:16 static/pt/chapter-11.html
+-rw-r--r--  3.0 unx    44996 tx defN 23-Nov-15 07:16 static/pt/chapter-03.html
+-rw-r--r--  3.0 unx    16062 tx defN 23-Nov-15 07:16 static/pt/chapter-01.html
+-rw-r--r--  3.0 unx    41269 tx defN 23-Nov-15 07:16 static/pt/chapter-05.html
+-rw-r--r--  3.0 unx    43327 tx defN 23-Nov-15 07:16 static/pt/chapter-15.html
+-rw-r--r--  3.0 unx    85517 tx defN 23-Nov-15 07:16 static/pt/chapter-16.html
+-rw-r--r--  3.0 unx   129331 tx defN 23-Nov-15 07:16 static/pt/chapter-08.html
 -rw-r--r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/pt/toggle.css
--rw-r--r--  3.0 unx    16062 tx defN 23-Nov-15 07:18 static/pt/chapter-01.html
--rw-r--r--  3.0 unx    54243 tx defN 23-Nov-15 07:18 static/pt/chapter-13.html
--rw-r--r--  3.0 unx    85517 tx defN 23-Nov-15 07:18 static/pt/chapter-16.html
--rw-r--r--  3.0 unx   189143 tx defN 23-Nov-15 07:18 static/pt/chapter-12.html
--rw-r--r--  3.0 unx    11831 tx defN 23-Nov-15 07:18 static/pt/chapter-11.html
--rw-r--r--  3.0 unx   105050 tx defN 23-Nov-15 07:18 static/pt/chapter-10.html
--rw-r--r--  3.0 unx    53993 tx defN 23-Nov-15 07:18 static/en/chapter-14.html
--rw-r--r--  3.0 unx    91743 tx defN 23-Nov-15 07:18 static/en/searchindex.js
--rw-r--r--  3.0 unx    18732 tx defN 23-Oct-30 01:31 static/en/_static/searchtools.js
--rw-r--r--  3.0 unx     4289 tx defN 23-Nov-15 07:18 static/en/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     5023 tx defN 23-Oct-30 01:31 static/en/_static/js/theme.js
--rw-r--r--  3.0 unx     2734 tx defN 23-Oct-30 01:31 static/en/_static/js/html5shiv.min.js
--rw-r--r--  3.0 unx     1333 tx defN 23-May-08 00:39 static/en/_static/js/toggle.js
--rw-r--r--  3.0 unx     4370 tx defN 23-Oct-30 01:31 static/en/_static/js/html5shiv-printshiv.min.js
--rw-r--r--  3.0 unx      934 tx defN 23-Oct-30 01:31 static/en/_static/js/badge_only.js
--rw-r--r--  3.0 unx      335 tx defN 23-Nov-15 07:18 static/en/_static/documentation_options.js
--rw-r--r--  3.0 unx     4902 tx defN 23-Nov-15 07:18 static/en/_static/pygments.css
--rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/en/_static/logo.png
--rw-r--r--  3.0 unx     4758 tx defN 23-Nov-15 07:18 static/en/_static/language_data.js
--rw-r--r--  3.0 unx     1989 bx stor 23-May-08 00:39 static/en/_static/logo-32x32.ico
--rw-r--r--  3.0 unx       90 bx defN 23-Oct-30 01:31 static/en/_static/plus.png
--rw-r--r--  3.0 unx     4231 tx defN 23-Oct-30 01:31 static/en/_static/tabs.js
--rw-r--r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/en/_static/css/dark.css
--rw-r--r--  3.0 unx     3229 tx defN 23-Oct-30 01:31 static/en/_static/css/badge_only.css
--rw-r--r--  3.0 unx   135314 tx defN 23-Oct-30 01:31 static/en/_static/css/theme.css
--rw-r--r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/en/_static/css/toggle.css
--rw-r--r--  3.0 unx     4472 tx defN 23-Oct-30 01:31 static/en/_static/doctools.js
--rw-r--r--  3.0 unx      286 bx stor 23-Oct-30 01:31 static/en/_static/file.png
--rw-r--r--  3.0 unx     5123 tx defN 23-Oct-30 01:31 static/en/_static/sphinx_highlight.js
--rw-r--r--  3.0 unx    89501 tx defN 23-Nov-15 07:18 static/en/_static/jquery.js
--rw-r--r--  3.0 unx       90 bx defN 23-Oct-30 01:31 static/en/_static/minus.png
--rw-r--r--  3.0 unx    15094 tx defN 23-Nov-15 07:18 static/en/_static/basic.css
--rw-r--r--  3.0 unx     1804 tx defN 23-Oct-30 01:31 static/en/_static/tabs.css
--rw-r--r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/en/dark.css
--rw-r--r--  3.0 unx    42508 tx defN 23-Nov-15 07:18 static/en/chapter-05.html
--rw-r--r--  3.0 unx   129405 tx defN 23-Nov-15 07:18 static/en/chapter-08.html
--rw-r--r--  3.0 unx    12032 tx defN 23-Nov-15 07:18 static/en/chapter-04.html
--rw-r--r--  3.0 unx     6828 tx defN 23-Nov-15 07:18 static/en/genindex.html
--rw-r--r--  3.0 unx   499548 tx defN 23-Nov-15 07:18 static/en/chapter-07.html
--rw-r--r--  3.0 unx    45695 tx defN 23-Nov-15 07:18 static/en/chapter-03.html
--rw-r--r--  3.0 unx    94790 tx defN 23-Nov-15 07:18 static/en/chapter-06.html
--rw-r--r--  3.0 unx    43157 tx defN 23-Nov-15 07:18 static/en/chapter-15.html
--rw-r--r--  3.0 unx    19102 tx defN 23-Nov-15 07:18 static/en/chapter-02.html
--rw-r--r--  3.0 unx     7103 tx defN 23-Nov-15 07:18 static/en/search.html
--rw-r--r--  3.0 unx    63512 tx defN 23-Nov-15 07:18 static/en/chapter-09.html
--rw-r--r--  3.0 unx    19991 tx defN 23-Nov-15 07:18 static/en/index.html
--rw-r--r--  3.0 unx    41285 bx defN 23-May-08 00:39 static/en/_images/grid.png
--rw-r--r--  3.0 unx    40745 bx defN 23-May-08 00:39 static/en/_images/grid_bulmacss.png
--rw-r--r--  3.0 unx    52898 bx defN 23-May-08 00:39 static/en/_images/dashboard.png
--rw-r--r--  3.0 unx    53747 bx defN 23-May-08 00:39 static/en/_images/dashboard_error.png
--rw-r--r--  3.0 unx    40478 bx defN 23-May-08 00:39 static/en/_images/command.png
--rw-r--r--  3.0 unx    29268 bx defN 23-May-08 00:39 static/en/_images/restapi2.png
--rw-r--r--  3.0 unx    40467 bx defN 23-May-08 00:39 static/en/_images/dashboard_new_app.png
--rw-r--r--  3.0 unx    77606 bx defN 23-May-08 00:39 static/en/_images/main_page.png
--rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/en/_images/logo.png
--rw-r--r--  3.0 unx    37805 bx defN 23-May-08 00:39 static/en/_images/form3.png
--rw-r--r--  3.0 unx    11257 bx defN 23-May-08 00:39 static/en/_images/form1.png
--rw-r--r--  3.0 unx    16627 bx defN 23-May-08 00:39 static/en/_images/simple_counter.png
--rw-r--r--  3.0 unx    30931 bx defN 23-May-08 00:39 static/en/_images/tags2.png
--rw-r--r--  3.0 unx    44559 bx defN 23-May-08 00:39 static/en/_images/grid_nocss.png
--rw-r--r--  3.0 unx    39765 bx defN 23-May-08 00:39 static/en/_images/form5.png
--rw-r--r--  3.0 unx   147429 bx defN 23-May-08 00:39 static/en/_images/dashboard_restapi.png
--rw-r--r--  3.0 unx    86267 bx defN 23-May-08 00:39 static/en/_images/dashboard_login.png
--rw-r--r--  3.0 unx   135864 bx defN 23-May-08 00:39 static/en/_images/dashboard_main.png
--rw-r--r--  3.0 unx    30536 bx defN 23-May-08 00:39 static/en/_images/restapi.png
--rw-r--r--  3.0 unx    58653 bx defN 23-May-08 00:39 static/en/_images/grid_columns.png
--rw-r--r--  3.0 unx    24753 bx defN 23-May-08 00:39 static/en/_images/tags_db.png
--rw-r--r--  3.0 unx   154315 bx defN 23-May-08 00:39 static/en/_images/dashboard_ticket.png
--rw-r--r--  3.0 unx    40409 bx defN 23-May-08 00:39 static/en/_images/form2.png
--rw-r--r--  3.0 unx    12086 bx defN 23-May-08 00:39 static/en/_images/_scaffold.png
--rw-r--r--  3.0 unx    38066 bx defN 23-May-08 00:39 static/en/_images/form6.png
--rw-r--r--  3.0 unx    46250 bx defN 23-May-08 00:39 static/en/_images/form4.png
--rw-r--r--  3.0 unx   174817 bx defN 23-May-08 00:39 static/en/_images/dashboard_edit.png
--rw-r--r--  3.0 unx    50011 bx defN 23-May-08 00:39 static/en/_images/first_run.png
--rw-r--r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/en/toggle.css
--rw-r--r--  3.0 unx    15659 tx defN 23-Nov-15 07:18 static/en/chapter-01.html
--rw-r--r--  3.0 unx    54280 tx defN 23-Nov-15 07:18 static/en/chapter-13.html
--rw-r--r--  3.0 unx    85384 tx defN 23-Nov-15 07:18 static/en/chapter-16.html
--rw-r--r--  3.0 unx   189442 tx defN 23-Nov-15 07:18 static/en/chapter-12.html
--rw-r--r--  3.0 unx    11524 tx defN 23-Nov-15 07:18 static/en/chapter-11.html
--rw-r--r--  3.0 unx   111513 tx defN 23-Nov-15 07:18 static/en/chapter-10.html
--rw-r--r--  3.0 unx    32038 bx defN 23-Nov-15 07:18 static/favicon.ico
--rw-r--r--  3.0 unx      248 tx defN 23-Nov-15 07:18 static/index.html
 156 files, 7751867 bytes uncompressed, 4330585 bytes compressed:  44.1%
```

#### zipnote {}

```diff
@@ -1,469 +1,469 @@
 Filename: __init__.py
 Comment: 
 
-Filename: static/pt/chapter-14.html
+Filename: static/favicon.ico
 Comment: 
 
-Filename: static/pt/searchindex.js
+Filename: static/en/chapter-14.html
 Comment: 
 
-Filename: static/pt/_static/searchtools.js
+Filename: static/en/dark.css
 Comment: 
 
-Filename: static/pt/_static/_sphinx_javascript_frameworks_compat.js
+Filename: static/en/chapter-06.html
 Comment: 
 
-Filename: static/pt/_static/js/theme.js
+Filename: static/en/chapter-09.html
 Comment: 
 
-Filename: static/pt/_static/js/html5shiv.min.js
+Filename: static/en/search.html
 Comment: 
 
-Filename: static/pt/_static/js/toggle.js
+Filename: static/en/chapter-12.html
 Comment: 
 
-Filename: static/pt/_static/js/html5shiv-printshiv.min.js
+Filename: static/en/chapter-07.html
 Comment: 
 
-Filename: static/pt/_static/js/badge_only.js
+Filename: static/en/chapter-02.html
 Comment: 
 
-Filename: static/pt/_static/documentation_options.js
+Filename: static/en/chapter-04.html
 Comment: 
 
-Filename: static/pt/_static/pygments.css
+Filename: static/en/genindex.html
 Comment: 
 
-Filename: static/pt/_static/logo.png
+Filename: static/en/chapter-10.html
 Comment: 
 
-Filename: static/pt/_static/language_data.js
+Filename: static/en/_static/minus.png
 Comment: 
 
-Filename: static/pt/_static/logo-32x32.ico
+Filename: static/en/_static/tabs.js
 Comment: 
 
-Filename: static/pt/_static/plus.png
+Filename: static/en/_static/pygments.css
 Comment: 
 
-Filename: static/pt/_static/tabs.js
+Filename: static/en/_static/doctools.js
 Comment: 
 
-Filename: static/pt/_static/css/dark.css
+Filename: static/en/_static/_sphinx_javascript_frameworks_compat.js
 Comment: 
 
-Filename: static/pt/_static/css/badge_only.css
+Filename: static/en/_static/jquery.js
 Comment: 
 
-Filename: static/pt/_static/css/theme.css
+Filename: static/en/_static/file.png
 Comment: 
 
-Filename: static/pt/_static/css/toggle.css
+Filename: static/en/_static/css/dark.css
 Comment: 
 
-Filename: static/pt/_static/portuguese-stemmer.js
+Filename: static/en/_static/css/badge_only.css
 Comment: 
 
-Filename: static/pt/_static/doctools.js
+Filename: static/en/_static/css/theme.css
 Comment: 
 
-Filename: static/pt/_static/file.png
+Filename: static/en/_static/css/toggle.css
 Comment: 
 
-Filename: static/pt/_static/sphinx_highlight.js
+Filename: static/en/_static/sphinx_highlight.js
 Comment: 
 
-Filename: static/pt/_static/translations.js
+Filename: static/en/_static/logo-32x32.ico
 Comment: 
 
-Filename: static/pt/_static/jquery.js
+Filename: static/en/_static/logo.png
 Comment: 
 
-Filename: static/pt/_static/base-stemmer.js
+Filename: static/en/_static/documentation_options.js
 Comment: 
 
-Filename: static/pt/_static/minus.png
+Filename: static/en/_static/language_data.js
 Comment: 
 
-Filename: static/pt/_static/basic.css
+Filename: static/en/_static/searchtools.js
 Comment: 
 
-Filename: static/pt/_static/tabs.css
+Filename: static/en/_static/js/html5shiv.min.js
 Comment: 
 
-Filename: static/pt/dark.css
+Filename: static/en/_static/js/badge_only.js
 Comment: 
 
-Filename: static/pt/chapter-05.html
+Filename: static/en/_static/js/theme.js
 Comment: 
 
-Filename: static/pt/chapter-08.html
+Filename: static/en/_static/js/toggle.js
 Comment: 
 
-Filename: static/pt/chapter-04.html
+Filename: static/en/_static/js/html5shiv-printshiv.min.js
 Comment: 
 
-Filename: static/pt/genindex.html
+Filename: static/en/_static/plus.png
 Comment: 
 
-Filename: static/pt/chapter-07.html
+Filename: static/en/_static/basic.css
 Comment: 
 
-Filename: static/pt/chapter-03.html
+Filename: static/en/_static/tabs.css
 Comment: 
 
-Filename: static/pt/chapter-06.html
+Filename: static/en/searchindex.js
 Comment: 
 
-Filename: static/pt/chapter-15.html
+Filename: static/en/index.html
 Comment: 
 
-Filename: static/pt/chapter-02.html
+Filename: static/en/chapter-13.html
 Comment: 
 
-Filename: static/pt/search.html
+Filename: static/en/_images/form1.png
 Comment: 
 
-Filename: static/pt/chapter-09.html
+Filename: static/en/_images/dashboard_error.png
 Comment: 
 
-Filename: static/pt/index.html
+Filename: static/en/_images/grid.png
 Comment: 
 
-Filename: static/pt/_images/grid.png
+Filename: static/en/_images/grid_nocss.png
 Comment: 
 
-Filename: static/pt/_images/grid_bulmacss.png
+Filename: static/en/_images/dashboard.png
 Comment: 
 
-Filename: static/pt/_images/dashboard.png
+Filename: static/en/_images/dashboard_ticket.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_error.png
+Filename: static/en/_images/dashboard_main.png
 Comment: 
 
-Filename: static/pt/_images/command.png
+Filename: static/en/_images/_scaffold.png
 Comment: 
 
-Filename: static/pt/_images/restapi2.png
+Filename: static/en/_images/tags2.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_new_app.png
+Filename: static/en/_images/dashboard_edit.png
 Comment: 
 
-Filename: static/pt/_images/main_page.png
+Filename: static/en/_images/grid_columns.png
 Comment: 
 
-Filename: static/pt/_images/logo.png
+Filename: static/en/_images/form2.png
 Comment: 
 
-Filename: static/pt/_images/form3.png
+Filename: static/en/_images/tags_db.png
 Comment: 
 
-Filename: static/pt/_images/form1.png
+Filename: static/en/_images/form4.png
 Comment: 
 
-Filename: static/pt/_images/simple_counter.png
+Filename: static/en/_images/command.png
 Comment: 
 
-Filename: static/pt/_images/tags2.png
+Filename: static/en/_images/form6.png
 Comment: 
 
-Filename: static/pt/_images/grid_nocss.png
+Filename: static/en/_images/restapi.png
 Comment: 
 
-Filename: static/pt/_images/form5.png
+Filename: static/en/_images/logo.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_restapi.png
+Filename: static/en/_images/restapi2.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_login.png
+Filename: static/en/_images/form5.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_main.png
+Filename: static/en/_images/simple_counter.png
 Comment: 
 
-Filename: static/pt/_images/restapi.png
+Filename: static/en/_images/form3.png
 Comment: 
 
-Filename: static/pt/_images/grid_columns.png
+Filename: static/en/_images/grid_bulmacss.png
 Comment: 
 
-Filename: static/pt/_images/tags_db.png
+Filename: static/en/_images/dashboard_new_app.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_ticket.png
+Filename: static/en/_images/main_page.png
 Comment: 
 
-Filename: static/pt/_images/form2.png
+Filename: static/en/_images/dashboard_login.png
 Comment: 
 
-Filename: static/pt/_images/_scaffold.png
+Filename: static/en/_images/first_run.png
 Comment: 
 
-Filename: static/pt/_images/form6.png
+Filename: static/en/_images/dashboard_restapi.png
 Comment: 
 
-Filename: static/pt/_images/form4.png
+Filename: static/en/chapter-11.html
 Comment: 
 
-Filename: static/pt/_images/dashboard_edit.png
+Filename: static/en/chapter-03.html
 Comment: 
 
-Filename: static/pt/_images/first_run.png
+Filename: static/en/chapter-01.html
 Comment: 
 
-Filename: static/pt/toggle.css
+Filename: static/en/chapter-05.html
 Comment: 
 
-Filename: static/pt/chapter-01.html
+Filename: static/en/chapter-15.html
 Comment: 
 
-Filename: static/pt/chapter-13.html
+Filename: static/en/chapter-16.html
 Comment: 
 
-Filename: static/pt/chapter-16.html
+Filename: static/en/chapter-08.html
 Comment: 
 
-Filename: static/pt/chapter-12.html
+Filename: static/en/toggle.css
 Comment: 
 
-Filename: static/pt/chapter-11.html
+Filename: static/index.html
 Comment: 
 
-Filename: static/pt/chapter-10.html
+Filename: static/pt/chapter-14.html
 Comment: 
 
-Filename: static/en/chapter-14.html
+Filename: static/pt/dark.css
 Comment: 
 
-Filename: static/en/searchindex.js
+Filename: static/pt/chapter-06.html
 Comment: 
 
-Filename: static/en/_static/searchtools.js
+Filename: static/pt/chapter-09.html
 Comment: 
 
-Filename: static/en/_static/_sphinx_javascript_frameworks_compat.js
+Filename: static/pt/search.html
 Comment: 
 
-Filename: static/en/_static/js/theme.js
+Filename: static/pt/chapter-12.html
 Comment: 
 
-Filename: static/en/_static/js/html5shiv.min.js
+Filename: static/pt/chapter-07.html
 Comment: 
 
-Filename: static/en/_static/js/toggle.js
+Filename: static/pt/chapter-02.html
 Comment: 
 
-Filename: static/en/_static/js/html5shiv-printshiv.min.js
+Filename: static/pt/chapter-04.html
 Comment: 
 
-Filename: static/en/_static/js/badge_only.js
+Filename: static/pt/genindex.html
 Comment: 
 
-Filename: static/en/_static/documentation_options.js
+Filename: static/pt/chapter-10.html
 Comment: 
 
-Filename: static/en/_static/pygments.css
+Filename: static/pt/_static/minus.png
 Comment: 
 
-Filename: static/en/_static/logo.png
+Filename: static/pt/_static/tabs.js
 Comment: 
 
-Filename: static/en/_static/language_data.js
+Filename: static/pt/_static/pygments.css
 Comment: 
 
-Filename: static/en/_static/logo-32x32.ico
+Filename: static/pt/_static/doctools.js
 Comment: 
 
-Filename: static/en/_static/plus.png
+Filename: static/pt/_static/_sphinx_javascript_frameworks_compat.js
 Comment: 
 
-Filename: static/en/_static/tabs.js
+Filename: static/pt/_static/jquery.js
 Comment: 
 
-Filename: static/en/_static/css/dark.css
+Filename: static/pt/_static/portuguese-stemmer.js
 Comment: 
 
-Filename: static/en/_static/css/badge_only.css
+Filename: static/pt/_static/translations.js
 Comment: 
 
-Filename: static/en/_static/css/theme.css
+Filename: static/pt/_static/file.png
 Comment: 
 
-Filename: static/en/_static/css/toggle.css
+Filename: static/pt/_static/css/dark.css
 Comment: 
 
-Filename: static/en/_static/doctools.js
+Filename: static/pt/_static/css/badge_only.css
 Comment: 
 
-Filename: static/en/_static/file.png
+Filename: static/pt/_static/css/theme.css
 Comment: 
 
-Filename: static/en/_static/sphinx_highlight.js
+Filename: static/pt/_static/css/toggle.css
 Comment: 
 
-Filename: static/en/_static/jquery.js
+Filename: static/pt/_static/sphinx_highlight.js
 Comment: 
 
-Filename: static/en/_static/minus.png
+Filename: static/pt/_static/logo-32x32.ico
 Comment: 
 
-Filename: static/en/_static/basic.css
+Filename: static/pt/_static/logo.png
 Comment: 
 
-Filename: static/en/_static/tabs.css
+Filename: static/pt/_static/base-stemmer.js
 Comment: 
 
-Filename: static/en/dark.css
+Filename: static/pt/_static/documentation_options.js
 Comment: 
 
-Filename: static/en/chapter-05.html
+Filename: static/pt/_static/language_data.js
 Comment: 
 
-Filename: static/en/chapter-08.html
+Filename: static/pt/_static/searchtools.js
 Comment: 
 
-Filename: static/en/chapter-04.html
+Filename: static/pt/_static/js/html5shiv.min.js
 Comment: 
 
-Filename: static/en/genindex.html
+Filename: static/pt/_static/js/badge_only.js
 Comment: 
 
-Filename: static/en/chapter-07.html
+Filename: static/pt/_static/js/theme.js
 Comment: 
 
-Filename: static/en/chapter-03.html
+Filename: static/pt/_static/js/toggle.js
 Comment: 
 
-Filename: static/en/chapter-06.html
+Filename: static/pt/_static/js/html5shiv-printshiv.min.js
 Comment: 
 
-Filename: static/en/chapter-15.html
+Filename: static/pt/_static/plus.png
 Comment: 
 
-Filename: static/en/chapter-02.html
+Filename: static/pt/_static/basic.css
 Comment: 
 
-Filename: static/en/search.html
+Filename: static/pt/_static/tabs.css
 Comment: 
 
-Filename: static/en/chapter-09.html
+Filename: static/pt/searchindex.js
 Comment: 
 
-Filename: static/en/index.html
+Filename: static/pt/index.html
 Comment: 
 
-Filename: static/en/_images/grid.png
+Filename: static/pt/chapter-13.html
 Comment: 
 
-Filename: static/en/_images/grid_bulmacss.png
+Filename: static/pt/_images/form1.png
 Comment: 
 
-Filename: static/en/_images/dashboard.png
+Filename: static/pt/_images/dashboard_error.png
 Comment: 
 
-Filename: static/en/_images/dashboard_error.png
+Filename: static/pt/_images/grid.png
 Comment: 
 
-Filename: static/en/_images/command.png
+Filename: static/pt/_images/grid_nocss.png
 Comment: 
 
-Filename: static/en/_images/restapi2.png
+Filename: static/pt/_images/dashboard.png
 Comment: 
 
-Filename: static/en/_images/dashboard_new_app.png
+Filename: static/pt/_images/dashboard_ticket.png
 Comment: 
 
-Filename: static/en/_images/main_page.png
+Filename: static/pt/_images/dashboard_main.png
 Comment: 
 
-Filename: static/en/_images/logo.png
+Filename: static/pt/_images/_scaffold.png
 Comment: 
 
-Filename: static/en/_images/form3.png
+Filename: static/pt/_images/tags2.png
 Comment: 
 
-Filename: static/en/_images/form1.png
+Filename: static/pt/_images/dashboard_edit.png
 Comment: 
 
-Filename: static/en/_images/simple_counter.png
+Filename: static/pt/_images/grid_columns.png
 Comment: 
 
-Filename: static/en/_images/tags2.png
+Filename: static/pt/_images/form2.png
 Comment: 
 
-Filename: static/en/_images/grid_nocss.png
+Filename: static/pt/_images/tags_db.png
 Comment: 
 
-Filename: static/en/_images/form5.png
+Filename: static/pt/_images/form4.png
 Comment: 
 
-Filename: static/en/_images/dashboard_restapi.png
+Filename: static/pt/_images/command.png
 Comment: 
 
-Filename: static/en/_images/dashboard_login.png
+Filename: static/pt/_images/form6.png
 Comment: 
 
-Filename: static/en/_images/dashboard_main.png
+Filename: static/pt/_images/restapi.png
 Comment: 
 
-Filename: static/en/_images/restapi.png
+Filename: static/pt/_images/logo.png
 Comment: 
 
-Filename: static/en/_images/grid_columns.png
+Filename: static/pt/_images/restapi2.png
 Comment: 
 
-Filename: static/en/_images/tags_db.png
+Filename: static/pt/_images/form5.png
 Comment: 
 
-Filename: static/en/_images/dashboard_ticket.png
+Filename: static/pt/_images/simple_counter.png
 Comment: 
 
-Filename: static/en/_images/form2.png
+Filename: static/pt/_images/form3.png
 Comment: 
 
-Filename: static/en/_images/_scaffold.png
+Filename: static/pt/_images/grid_bulmacss.png
 Comment: 
 
-Filename: static/en/_images/form6.png
+Filename: static/pt/_images/dashboard_new_app.png
 Comment: 
 
-Filename: static/en/_images/form4.png
+Filename: static/pt/_images/main_page.png
 Comment: 
 
-Filename: static/en/_images/dashboard_edit.png
+Filename: static/pt/_images/dashboard_login.png
 Comment: 
 
-Filename: static/en/_images/first_run.png
+Filename: static/pt/_images/first_run.png
 Comment: 
 
-Filename: static/en/toggle.css
+Filename: static/pt/_images/dashboard_restapi.png
 Comment: 
 
-Filename: static/en/chapter-01.html
+Filename: static/pt/chapter-11.html
 Comment: 
 
-Filename: static/en/chapter-13.html
+Filename: static/pt/chapter-03.html
 Comment: 
 
-Filename: static/en/chapter-16.html
+Filename: static/pt/chapter-01.html
 Comment: 
 
-Filename: static/en/chapter-12.html
+Filename: static/pt/chapter-05.html
 Comment: 
 
-Filename: static/en/chapter-11.html
+Filename: static/pt/chapter-15.html
 Comment: 
 
-Filename: static/en/chapter-10.html
+Filename: static/pt/chapter-16.html
 Comment: 
 
-Filename: static/favicon.ico
+Filename: static/pt/chapter-08.html
 Comment: 
 
-Filename: static/index.html
+Filename: static/pt/toggle.css
 Comment: 
 
 Zip file comment:
```

### Comparing `py4web-1.20231115.1/py4web/assets/py4web.app._minimal.zip` & `py4web-1.20240420.1/py4web/assets/py4web.app._minimal.zip`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,5 +1,5 @@
 Zip file size: 5245 bytes, number of entries: 3
--rw-rw-r--  3.0 unx       83 tx defN 23-May-08 00:39 __init__.py
--rw-rw-r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
--rw-rw-r--  3.0 unx        1 tx stor 23-May-08 00:39 static/README.md
+-rw-r--r--  3.0 unx       83 tx defN 23-May-08 00:39 __init__.py
+-rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
+-rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 static/README.md
 3 files, 32122 bytes uncompressed, 4749 bytes compressed:  85.2%
```

### Comparing `py4web-1.20231115.1/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20240420.1/py4web/assets/py4web.app._scaffold.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 21792 bytes, number of entries: 16
--rw-rw-r--  3.0 unx      254 tx defN 23-May-08 00:39 models.py
--rw-rw-r--  3.0 unx     1473 tx defN 23-Oct-08 21:52 controllers.py
--rw-rw-r--  3.0 unx      375 tx defN 23-May-08 00:39 __init__.py
--rw-r--r--  3.0 unx     2860 tx defN 23-Nov-12 20:43 templates/layout.html
--rw-rw-r--  3.0 unx      278 tx defN 23-May-08 00:39 templates/auth.html
--rw-rw-r--  3.0 unx      103 tx defN 23-May-08 00:39 templates/index.html
--rw-rw-r--  3.0 unx      264 tx defN 23-May-08 00:39 templates/generic.html
--rw-rw-r--  3.0 unx        1 tx stor 23-May-08 00:39 templates/README.md
+Zip file size: 21723 bytes, number of entries: 16
+-rw-r--r--  3.0 unx     1394 tx defN 24-Apr-13 17:46 controllers.py
+-rw-r--r--  3.0 unx      852 tx defN 23-May-08 00:39 tasks.py
+-rw-r--r--  3.0 unx      254 tx defN 23-May-08 00:39 models.py
 -rw-r--r--  3.0 unx     8029 tx defN 23-Aug-06 13:41 common.py
--rw-rw-r--  3.0 unx      852 tx defN 23-May-08 00:39 tasks.py
+-rw-r--r--  3.0 unx      375 tx defN 23-May-08 00:39 __init__.py
 -rw-r--r--  3.0 unx     3212 tx defN 23-Aug-06 13:41 settings.py
--rw-rw-r--  3.0 unx       97 tx defN 23-May-08 00:39 translations/it.json
--rw-rw-r--  3.0 unx    12182 tx defN 23-Nov-12 21:26 static/js/utils.js
--rw-rw-r--  3.0 unx    11431 tx defN 23-May-08 00:39 static/css/no.css
--rw-rw-r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
--rw-rw-r--  3.0 unx        1 tx stor 23-May-08 00:39 static/README.md
-16 files, 73450 bytes uncompressed, 19218 bytes compressed:  73.8%
+-rw-r--r--  3.0 unx       97 tx defN 23-May-08 00:39 translations/it.json
+-rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
+-rw-r--r--  3.0 unx    11431 tx defN 23-May-08 00:39 static/css/no.css
+-rw-r--r--  3.0 unx    12182 tx defN 23-Nov-12 21:26 static/js/utils.js
+-rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 static/README.md
+-rw-r--r--  3.0 unx      103 tx defN 23-May-08 00:39 templates/index.html
+-rw-r--r--  3.0 unx     2738 tx defN 24-Apr-13 17:47 templates/layout.html
+-rw-r--r--  3.0 unx      264 tx defN 23-May-08 00:39 templates/generic.html
+-rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 templates/README.md
+-rw-r--r--  3.0 unx      278 tx defN 23-May-08 00:39 templates/auth.html
+16 files, 73249 bytes uncompressed, 19149 bytes compressed:  73.9%
```

#### zipnote {}

```diff
@@ -1,49 +1,49 @@
-Filename: models.py
+Filename: controllers.py
 Comment: 
 
-Filename: controllers.py
+Filename: tasks.py
 Comment: 
 
-Filename: __init__.py
+Filename: models.py
 Comment: 
 
-Filename: templates/layout.html
+Filename: common.py
 Comment: 
 
-Filename: templates/auth.html
+Filename: __init__.py
 Comment: 
 
-Filename: templates/index.html
+Filename: settings.py
 Comment: 
 
-Filename: templates/generic.html
+Filename: translations/it.json
 Comment: 
 
-Filename: templates/README.md
+Filename: static/favicon.ico
 Comment: 
 
-Filename: common.py
+Filename: static/css/no.css
 Comment: 
 
-Filename: tasks.py
+Filename: static/js/utils.js
 Comment: 
 
-Filename: settings.py
+Filename: static/README.md
 Comment: 
 
-Filename: translations/it.json
+Filename: templates/index.html
 Comment: 
 
-Filename: static/js/utils.js
+Filename: templates/layout.html
 Comment: 
 
-Filename: static/css/no.css
+Filename: templates/generic.html
 Comment: 
 
-Filename: static/favicon.ico
+Filename: templates/README.md
 Comment: 
 
-Filename: static/README.md
+Filename: templates/auth.html
 Comment: 
 
 Zip file comment:
```

#### controllers.py

```diff
@@ -31,9 +31,8 @@
 
 
 @action("index")
 @action.uses("index.html", auth, T)
 def index():
     user = auth.get_user()
     message = T("Hello {first_name}").format(**user) if user else T("Hello")
-    actions = {"allowed_actions": auth.param.allowed_actions}
-    return dict(message=message, actions=actions)
+    return dict(message=message)
```

#### templates/layout.html

```diff
@@ -27,17 +27,15 @@
           [[if globals().get('user'):]]
           <li>
             <a class="navbar-link is-primary">
               [[=globals().get('user',{}).get('email')]]
             </a>
             <ul>
               <li><a href="[[=URL('auth/profile')]]">Edit Profile</a></li>
-              [[if 'change_password' in globals().get('actions',{}).get('allowed_actions',{}):]]
-                <li><a href="[[=URL('auth/change_password')]]">Change Password</a></li>
-              [[pass]]
+              <li><a href="[[=URL('auth/change_password')]]">Change Password</a></li>
               <li><a href="[[=URL('auth/logout')]]">Logout</a></li>
             </ul>
           </li>
           [[else:]]
           <li>
             Login
             <ul>
```

##### html2text {}

```diff
@@ -1,17 +1,14 @@
 [[block page_head]][[end]]
 _pp_yy_44_ww_ee_bb
 â° ??[[block page_left_menu]][[end]]
     * [[if globals().get('user'):]]
     * [[=globals().get('user',{}).get('email')]]
           o _E_d_i_t_ _P_r_o_f_i_l_e
-          o [[if 'change_password' in globals().get('actions',{}).get
-            ('allowed_actions',{}):]]
           o _C_h_a_n_g_e_ _P_a_s_s_w_o_r_d
-          o [[pass]]
           o _L_o_g_o_u_t
     * [[else:]]
     * Login
           o _S_i_g_n_ _u_p
           o _L_o_g_ _i_n
     * [[pass]]
                                   [[include]]
```

### Comparing `py4web-1.20231115.1/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20240420.1/py4web/assets/py4web.app.showcase.zip`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,145 +1,145 @@
-Zip file size: 1392657 bytes, number of entries: 143
--rw-r--r--  3.0 unx     4205 tx defN 23-Aug-06 14:14 __init__.py
--rw-rw-r--  3.0 unx       20 tx stor 23-May-08 00:39 uploads/README.md
--rw-rw-r--  3.0 unx     2778 tx defN 23-May-08 00:39 templates/layout.html
--rw-rw-r--  3.0 unx     2156 tx defN 23-May-08 00:39 templates/layout_bulma.html
--rw-rw-r--  3.0 unx      683 tx defN 23-May-08 00:39 templates/vue/vue_grid_and_forms.html
--rw-rw-r--  3.0 unx      544 tx defN 23-May-08 00:39 templates/vue/star_rater_vue_bulma.html
--rw-rw-r--  3.0 unx      502 tx defN 23-May-08 00:39 templates/vue/star_rater_vue.html
--rw-rw-r--  3.0 unx      486 tx defN 23-May-08 00:39 templates/vue/view_form.html
--rw-rw-r--  3.0 unx      488 tx defN 23-May-08 00:39 templates/vue/insert_form.html
--rw-rw-r--  3.0 unx      392 tx defN 23-May-08 00:39 templates/vue/vuegrid_bulma.html
--rw-rw-r--  3.0 unx      448 tx defN 23-May-08 00:39 templates/vue/starrating.html
--rw-rw-r--  3.0 unx      372 tx defN 23-May-08 00:39 templates/vue/file_uploader.html
--rw-rw-r--  3.0 unx      374 tx defN 23-May-08 00:39 templates/vue/vuegrid.html
--rw-rw-r--  3.0 unx      486 tx defN 23-May-08 00:39 templates/vue/edit_form.html
--rw-rw-r--  3.0 unx     2172 tx defN 23-May-08 00:39 templates/ws/ws_index.html
--rw-rw-r--  3.0 unx     1913 tx defN 23-May-08 00:39 templates/socketio/socketio_index.html
--rw-rw-r--  3.0 unx      242 tx defN 23-May-08 00:39 templates/examples/flash_example.html
--rw-rw-r--  3.0 unx      869 tx defN 23-May-08 00:39 templates/examples/custom_form.html
--rw-rw-r--  3.0 unx      242 tx defN 23-May-08 00:39 templates/examples/forms.html
--rw-rw-r--  3.0 unx       82 tx defN 23-May-08 00:39 templates/examples/page_with_template.html
--rw-rw-r--  3.0 unx     1711 tx defN 23-May-08 00:39 templates/examples/tagsinput_form.html
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/html_grid.html
--rw-rw-r--  3.0 unx      189 tx defN 23-May-08 00:39 templates/examples/hcaptcha_form.html
--rw-rw-r--  3.0 unx      551 tx defN 23-May-08 00:39 templates/examples/auth_custom_login.html
--rw-rw-r--  3.0 unx      193 tx defN 23-May-08 00:39 templates/examples/auth_form.html
--rw-rw-r--  3.0 unx       26 tx stor 23-May-08 00:39 templates/examples/flash_example_next.html
--rw-rw-r--  3.0 unx      305 tx defN 23-May-08 00:39 templates/examples/form.html
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/component_loader.html
--rw-rw-r--  3.0 unx      228 tx defN 23-May-08 00:39 templates/examples/generic.html
--rw-rw-r--  3.0 unx     1025 tx defN 23-May-08 00:39 templates/examples/rest_info.html
--rw-rw-r--  3.0 unx       69 tx defN 23-May-08 00:39 templates/examples/ajax_grid.html
--rw-rw-r--  3.0 unx      263 tx defN 23-May-08 00:39 templates/examples/session_counter.html
--rw-rw-r--  3.0 unx      646 tx defN 23-May-08 00:39 templates/examples/auth_forms.html
--rw-rw-r--  3.0 unx      278 tx defN 23-May-08 00:39 templates/auth.html
--rw-rw-r--  3.0 unx     6788 tx defN 23-May-08 00:39 templates/index.html
--rw-r--r--  3.0 unx      430 tx defN 23-Aug-06 14:14 templates/show.html
--rw-rw-r--  3.0 unx     2617 tx defN 23-May-08 00:39 examples/models.py
--rw-rw-r--  3.0 unx      378 tx defN 23-May-08 00:39 examples/auth_form.py
--rw-rw-r--  3.0 unx      228 tx defN 23-May-08 00:39 examples/flash_example_naive.py
--rw-rw-r--  3.0 unx     2749 tx defN 23-May-08 00:39 examples/rest.py
--rw-rw-r--  3.0 unx      456 tx defN 23-May-08 00:39 examples/create_form.py
--rw-rw-r--  3.0 unx      145 tx defN 23-May-08 00:39 examples/hello_world_msg.py
--rw-rw-r--  3.0 unx     1583 tx defN 23-May-08 00:39 examples/example_html_grid.py
--rw-rw-r--  3.0 unx      465 tx defN 23-May-08 00:39 examples/update_form.py
--rw-rw-r--  3.0 unx      272 tx defN 23-May-08 00:39 examples/ws.py
--rw-rw-r--  3.0 unx      264 tx defN 23-May-08 00:39 examples/session_counter.py
--rw-rw-r--  3.0 unx      870 tx defN 23-May-08 00:39 examples/component_loader.py
--rw-rw-r--  3.0 unx      255 tx defN 23-May-08 00:39 examples/show_a_button.py
--rw-rw-r--  3.0 unx      130 tx defN 23-May-08 00:39 examples/hello.py
--rwxrwxr-x  3.0 unx      422 tx defN 23-May-08 00:39 examples/ws_client_example.py
--rw-rw-r--  3.0 unx      236 tx defN 23-May-08 00:39 examples/example_helpers.py
--rw-rw-r--  3.0 unx      112 tx defN 23-May-08 00:39 examples/page_with_raise.py
--rw-rw-r--  3.0 unx     1966 tx defN 23-May-08 00:39 examples/example_multiple_forms.py
--rw-rw-r--  3.0 unx      171 tx defN 23-May-08 00:39 examples/page_with_template.py
--rw-rw-r--  3.0 unx      396 tx defN 23-May-08 00:39 examples/custom_form.py
--rw-rw-r--  3.0 unx      349 tx defN 23-May-08 00:39 examples/count.py
--rw-rw-r--  3.0 unx      517 tx defN 23-May-08 00:39 examples/socketio.py
--rw-rw-r--  3.0 unx      227 tx defN 23-May-08 00:39 examples/page_with_query.py
--rw-rw-r--  3.0 unx      647 tx defN 23-May-08 00:39 examples/auth_forms.py
--rw-rw-r--  3.0 unx     4809 tx defN 23-May-08 00:39 examples/common.py
--rw-rw-r--  3.0 unx      420 tx defN 23-May-08 00:39 examples/page_with_postback.py
--rw-rw-r--  3.0 unx      414 tx defN 23-May-08 00:39 examples/test_expose.py
--rw-rw-r--  3.0 unx      125 tx defN 23-May-08 00:39 examples/hello_world.py
--rw-rw-r--  3.0 unx     1470 tx defN 23-May-08 00:39 examples/settings.py
--rw-rw-r--  3.0 unx      644 tx defN 23-May-08 00:39 examples/rpc.py
--rw-rw-r--  3.0 unx       88 tx defN 23-May-08 00:39 examples/page_with_error.py
--rw-rw-r--  3.0 unx      370 tx defN 23-May-08 00:39 examples/example_ajax_grid.py
--rw-rw-r--  3.0 unx      372 tx defN 23-May-08 00:39 examples/flash_example_fixture.py
--rw-rw-r--  3.0 unx      106 tx defN 23-May-08 00:39 examples/page_without_template.py
--rw-rw-r--  3.0 unx      281 tx defN 23-May-08 00:39 examples/page_with_parameters.py
--rw-rw-r--  3.0 unx      181 tx defN 23-May-08 00:39 examples/page_with_redirect.py
--rw-rw-r--  3.0 unx      197 tx defN 23-May-08 00:39 examples/session_clear.py
--rw-rw-r--  3.0 unx     1616 tx defN 23-May-08 00:39 examples/hcaptcha_form.py
--rw-rw-r--  3.0 unx      375 tx defN 23-May-08 00:39 examples/tagsinput_form.py
--rw-rw-r--  3.0 unx     1390 tx defN 23-May-08 00:39 vue_components_examples/models.py
--rw-rw-r--  3.0 unx     1124 tx defN 23-May-08 00:39 vue_components_examples/vue_edit_form.py
--rw-rw-r--  3.0 unx     1149 tx defN 23-May-08 00:39 vue_components_examples/vue_view_form.py
--rw-rw-r--  3.0 unx     1597 tx defN 23-May-08 00:39 vue_components_examples/components/fileupload.py
--rw-rw-r--  3.0 unx     7777 tx defN 23-May-08 00:39 vue_components_examples/components/grid.py
--rw-rw-r--  3.0 unx     2078 tx defN 23-May-08 00:39 vue_components_examples/components/starrater.py
--rw-rw-r--  3.0 unx    10333 tx defN 23-May-08 00:39 vue_components_examples/components/vueform.py
--rw-rw-r--  3.0 unx     7858 tx defN 23-May-08 00:39 vue_components_examples/components/README.md
--rw-rw-r--  3.0 unx     1215 tx defN 23-May-08 00:39 vue_components_examples/vue_star_rater.py
--rw-rw-r--  3.0 unx      853 tx defN 23-May-08 00:39 vue_components_examples/vue_insert_form.py
--rw-rw-r--  3.0 unx       32 tx stor 23-May-08 00:39 vue_components_examples/common.py
--rw-rw-r--  3.0 unx     3031 tx defN 23-May-08 00:39 vue_components_examples/vue_grid_and_forms.py
--rw-rw-r--  3.0 unx       34 tx stor 23-May-08 00:39 vue_components_examples/settings.py
--rw-rw-r--  3.0 unx      324 tx defN 23-May-08 00:39 vue_components_examples/vue_file_uploader.py
--rw-rw-r--  3.0 unx      302 tx defN 23-May-08 00:39 vue_components_examples/vue_grid.py
--rw-rw-r--  3.0 unx      236 tx defN 23-May-08 00:39 translations/it.json
--rw-rw-r--  3.0 unx      196 tx defN 23-May-08 00:39 translations/en.json
--rw-r--r--  3.0 unx    11888 tx defN 23-Nov-12 21:35 static/js/utils.js
--rw-rw-r--  3.0 unx      496 tx defN 23-May-08 00:39 static/js/star_rater_vue.js
--rw-rw-r--  3.0 unx      868 tx defN 23-May-08 00:39 static/js/firebase-push.js
--rw-rw-r--  3.0 unx   341462 tx defN 23-May-08 00:39 static/js/vue.js
--rw-rw-r--  3.0 unx    68547 tx defN 23-May-08 00:39 static/js/sugar.min.js
--rw-rw-r--  3.0 unx    19055 tx defN 23-May-08 00:39 static/js/prism.js
--rw-r--r--  3.0 unx    32337 tx defN 23-Nov-12 21:45 static/js/axios.min.js
--rw-rw-r--  3.0 unx     8311 tx defN 23-May-08 00:39 static/js/utils.min.js
--rw-rw-r--  3.0 unx    93670 tx defN 23-May-08 00:39 static/js/vue.min.js
--rw-rw-r--  3.0 unx        1 tx stor 23-May-08 00:39 static/ws/README.md
--rw-rw-r--  3.0 unx       12 tx stor 23-May-08 00:39 static/hello.txt
--rw-rw-r--  3.0 unx        1 tx stor 23-May-08 00:39 static/socketio/README.md
--rw-r--r--  3.0 unx     8097 tx defN 23-Nov-12 21:35 static/components/mtable.js
--rw-rw-r--  3.0 unx      308 tx defN 23-May-08 00:39 static/components/starrater/starrater.html
--rw-rw-r--  3.0 unx        0 bx stor 23-May-08 00:39 static/components/starrater/starrater.css
--rw-r--r--  3.0 unx     1681 tx defN 23-Nov-12 21:35 static/components/starrater/starrater.js
--rw-r--r--  3.0 unx     7447 tx defN 23-Nov-12 21:35 static/components/mtable.html
--rw-rw-r--  3.0 unx       43 tx stor 23-May-08 00:39 static/components/vueform/vueform.css
--rw-rw-r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components/vueform/luxon.js
--rw-r--r--  3.0 unx     7263 tx defN 23-Nov-12 21:35 static/components/vueform/vueform.js
--rw-rw-r--  3.0 unx     3400 tx defN 23-May-08 00:39 static/components/vueform/vueform.html
--rw-rw-r--  3.0 unx    70115 tx defN 23-May-08 00:39 static/components/vueform/luxon.min.js
--rw-rw-r--  3.0 unx       83 tx defN 23-May-08 00:39 static/components/fileupload/fileupload.html
+Zip file size: 1392768 bytes, number of entries: 143
+-rw-r--r--  3.0 unx       20 tx stor 23-May-08 00:39 uploads/README.md
+-rw-r--r--  3.0 unx     4206 tx defN 24-Apr-19 07:21 __init__.py
+-rw-r--r--  3.0 unx      349 tx defN 23-May-08 00:39 examples/count.py
+-rwxr--r--  3.0 unx      422 tx defN 23-May-08 00:39 examples/ws_client_example.py
+-rw-r--r--  3.0 unx       88 tx defN 23-May-08 00:39 examples/page_with_error.py
+-rw-r--r--  3.0 unx      112 tx defN 23-May-08 00:39 examples/page_with_raise.py
+-rw-r--r--  3.0 unx      145 tx defN 23-May-08 00:39 examples/hello_world_msg.py
+-rw-r--r--  3.0 unx      414 tx defN 23-May-08 00:39 examples/test_expose.py
+-rw-r--r--  3.0 unx      281 tx defN 23-May-08 00:39 examples/page_with_parameters.py
+-rw-r--r--  3.0 unx      125 tx defN 23-May-08 00:39 examples/hello_world.py
+-rw-r--r--  3.0 unx      227 tx defN 23-May-08 00:39 examples/page_with_query.py
+-rw-r--r--  3.0 unx     1583 tx defN 23-May-08 00:39 examples/example_html_grid.py
+-rw-r--r--  3.0 unx      181 tx defN 23-May-08 00:39 examples/page_with_redirect.py
+-rw-r--r--  3.0 unx      197 tx defN 23-May-08 00:39 examples/session_clear.py
+-rw-r--r--  3.0 unx     2617 tx defN 23-May-08 00:39 examples/models.py
+-rw-r--r--  3.0 unx      372 tx defN 23-May-08 00:39 examples/flash_example_fixture.py
+-rw-r--r--  3.0 unx      396 tx defN 23-May-08 00:39 examples/custom_form.py
+-rw-r--r--  3.0 unx      644 tx defN 23-May-08 00:39 examples/rpc.py
+-rw-r--r--  3.0 unx      264 tx defN 23-May-08 00:39 examples/session_counter.py
+-rw-r--r--  3.0 unx      517 tx defN 23-May-08 00:39 examples/socketio.py
+-rw-r--r--  3.0 unx      647 tx defN 23-May-08 00:39 examples/auth_forms.py
+-rw-r--r--  3.0 unx     2749 tx defN 23-May-08 00:39 examples/rest.py
+-rw-r--r--  3.0 unx     4809 tx defN 23-May-08 00:39 examples/common.py
+-rw-r--r--  3.0 unx      171 tx defN 23-May-08 00:39 examples/page_with_template.py
+-rw-r--r--  3.0 unx      378 tx defN 23-May-08 00:39 examples/auth_form.py
+-rw-r--r--  3.0 unx      456 tx defN 23-May-08 00:39 examples/create_form.py
+-rw-r--r--  3.0 unx      272 tx defN 23-May-08 00:39 examples/ws.py
+-rw-r--r--  3.0 unx      255 tx defN 23-May-08 00:39 examples/show_a_button.py
+-rw-r--r--  3.0 unx      106 tx defN 23-May-08 00:39 examples/page_without_template.py
+-rw-r--r--  3.0 unx     1470 tx defN 23-May-08 00:39 examples/settings.py
+-rw-r--r--  3.0 unx      420 tx defN 23-May-08 00:39 examples/page_with_postback.py
+-rw-r--r--  3.0 unx      465 tx defN 23-May-08 00:39 examples/update_form.py
+-rw-r--r--  3.0 unx     1966 tx defN 23-May-08 00:39 examples/example_multiple_forms.py
+-rw-r--r--  3.0 unx      870 tx defN 23-May-08 00:39 examples/component_loader.py
+-rw-r--r--  3.0 unx      130 tx defN 23-May-08 00:39 examples/hello.py
+-rw-r--r--  3.0 unx      375 tx defN 23-May-08 00:39 examples/tagsinput_form.py
+-rw-r--r--  3.0 unx      236 tx defN 23-May-08 00:39 examples/example_helpers.py
+-rw-r--r--  3.0 unx      370 tx defN 23-May-08 00:39 examples/example_ajax_grid.py
+-rw-r--r--  3.0 unx     1616 tx defN 23-May-08 00:39 examples/hcaptcha_form.py
+-rw-r--r--  3.0 unx      228 tx defN 23-May-08 00:39 examples/flash_example_naive.py
+-rw-r--r--  3.0 unx      853 tx defN 23-May-08 00:39 vue_components_examples/vue_insert_form.py
+-rw-r--r--  3.0 unx     3031 tx defN 23-May-08 00:39 vue_components_examples/vue_grid_and_forms.py
+-rw-r--r--  3.0 unx     1390 tx defN 23-May-08 00:39 vue_components_examples/models.py
+-rw-r--r--  3.0 unx      324 tx defN 23-May-08 00:39 vue_components_examples/vue_file_uploader.py
+-rw-r--r--  3.0 unx       32 tx stor 23-May-08 00:39 vue_components_examples/common.py
+-rw-r--r--  3.0 unx      302 tx defN 23-May-08 00:39 vue_components_examples/vue_grid.py
+-rw-r--r--  3.0 unx     1597 tx defN 23-May-08 00:39 vue_components_examples/components/fileupload.py
+-rw-r--r--  3.0 unx     2078 tx defN 23-May-08 00:39 vue_components_examples/components/starrater.py
+-rw-r--r--  3.0 unx    10333 tx defN 23-May-08 00:39 vue_components_examples/components/vueform.py
+-rw-r--r--  3.0 unx     7777 tx defN 23-May-08 00:39 vue_components_examples/components/grid.py
+-rw-r--r--  3.0 unx     7858 tx defN 23-May-08 00:39 vue_components_examples/components/README.md
+-rw-r--r--  3.0 unx       34 tx stor 23-May-08 00:39 vue_components_examples/settings.py
+-rw-r--r--  3.0 unx     1149 tx defN 23-May-08 00:39 vue_components_examples/vue_view_form.py
+-rw-r--r--  3.0 unx     1124 tx defN 23-May-08 00:39 vue_components_examples/vue_edit_form.py
+-rw-r--r--  3.0 unx     1215 tx defN 23-May-08 00:39 vue_components_examples/vue_star_rater.py
+-rw-r--r--  3.0 unx      236 tx defN 23-May-08 00:39 translations/it.json
+-rw-r--r--  3.0 unx      196 tx defN 23-May-08 00:39 translations/en.json
+-rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 static/socketio/README.md
+-rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
+-rw-r--r--  3.0 unx     9998 tx defN 23-May-08 00:39 static/error.html
+-rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 static/ws/README.md
+-rw-r--r--  3.0 unx  7330359 tx defN 23-May-08 00:39 static/data/uscities.json
+-rw-r--r--  3.0 unx   295408 tx defN 23-May-08 00:39 static/data/zip_codes.json
+-rw-r--r--  3.0 unx      977 tx defN 23-May-08 00:39 static/firebase-push.html
+-rw-r--r--  3.0 unx    11417 tx defN 23-May-08 00:39 static/css/no.css
+-rw-r--r--  3.0 unx     1903 tx defN 23-May-08 00:39 static/css/prism.css
+-rw-r--r--  3.0 unx       35 tx stor 23-May-08 00:39 static/components/fileupload/fileupload.css
 -rw-r--r--  3.0 unx     1232 tx defN 23-Nov-12 21:35 static/components/fileupload/fileupload.js
--rw-rw-r--  3.0 unx       35 tx stor 23-May-08 00:39 static/components/fileupload/fileupload.css
+-rw-r--r--  3.0 unx       83 tx defN 23-May-08 00:39 static/components/fileupload/fileupload.html
+-rw-r--r--  3.0 unx        0 bx stor 23-May-08 00:39 static/components/starrater/starrater.css
+-rw-r--r--  3.0 unx     1681 tx defN 23-Nov-12 21:35 static/components/starrater/starrater.js
+-rw-r--r--  3.0 unx      308 tx defN 23-May-08 00:39 static/components/starrater/starrater.html
+-rw-r--r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components/mtable.html
+-rw-r--r--  3.0 unx      411 tx defN 23-May-08 00:39 static/components/grid/grid.css
 -rw-r--r--  3.0 unx     5384 tx defN 23-Nov-12 21:35 static/components/grid/grid.js
--rw-rw-r--  3.0 unx      411 tx defN 23-May-08 00:39 static/components/grid/grid.css
--rw-rw-r--  3.0 unx     3299 tx defN 23-May-08 00:39 static/components/grid/grid.html
--rw-rw-r--  3.0 unx    11417 tx defN 23-May-08 00:39 static/css/no.css
--rw-rw-r--  3.0 unx     1903 tx defN 23-May-08 00:39 static/css/prism.css
--rw-rw-r--  3.0 unx  7330359 tx defN 23-May-08 00:39 static/data/uscities.json
--rw-rw-r--  3.0 unx   295408 tx defN 23-May-08 00:39 static/data/zip_codes.json
--rw-rw-r--  3.0 unx     8097 tx defN 23-May-08 00:39 static/components-bulma/mtable.js
--rw-rw-r--  3.0 unx      308 tx defN 23-May-08 00:39 static/components-bulma/starrater/starrater.html
--rw-rw-r--  3.0 unx        0 bx stor 23-May-08 00:39 static/components-bulma/starrater/starrater.css
--rw-rw-r--  3.0 unx     1687 tx defN 23-May-08 00:39 static/components-bulma/starrater/starrater.js
--rw-rw-r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components-bulma/mtable.html
--rw-rw-r--  3.0 unx       43 tx stor 23-May-08 00:39 static/components-bulma/vueform/vueform.css
--rw-rw-r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components-bulma/vueform/luxon.js
--rw-rw-r--  3.0 unx     7257 tx defN 23-May-08 00:39 static/components-bulma/vueform/vueform.js
--rw-rw-r--  3.0 unx     3400 tx defN 23-May-08 00:39 static/components-bulma/vueform/vueform.html
--rw-rw-r--  3.0 unx    70115 tx defN 23-May-08 00:39 static/components-bulma/vueform/luxon.min.js
--rw-rw-r--  3.0 unx       83 tx defN 23-May-08 00:39 static/components-bulma/fileupload/fileupload.html
--rw-rw-r--  3.0 unx     1232 tx defN 23-May-08 00:39 static/components-bulma/fileupload/fileupload.js
--rw-rw-r--  3.0 unx       35 tx stor 23-May-08 00:39 static/components-bulma/fileupload/fileupload.css
--rw-rw-r--  3.0 unx     5384 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.js
--rw-rw-r--  3.0 unx      411 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.css
--rw-rw-r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components-bulma/grid/luxon.js
--rw-rw-r--  3.0 unx     3369 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.html
--rw-rw-r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
--rw-rw-r--  3.0 unx     9998 tx defN 23-May-08 00:39 static/error.html
--rw-rw-r--  3.0 unx      977 tx defN 23-May-08 00:39 static/firebase-push.html
-143 files, 9348216 bytes uncompressed, 1365501 bytes compressed:  85.4%
+-rw-r--r--  3.0 unx     3299 tx defN 23-May-08 00:39 static/components/grid/grid.html
+-rw-r--r--  3.0 unx       43 tx stor 23-May-08 00:39 static/components/vueform/vueform.css
+-rw-r--r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components/vueform/luxon.js
+-rw-r--r--  3.0 unx     7263 tx defN 23-Nov-12 21:35 static/components/vueform/vueform.js
+-rw-r--r--  3.0 unx    70115 tx defN 23-May-08 00:39 static/components/vueform/luxon.min.js
+-rw-r--r--  3.0 unx     3400 tx defN 23-May-08 00:39 static/components/vueform/vueform.html
+-rw-r--r--  3.0 unx     8097 tx defN 23-Nov-12 21:35 static/components/mtable.js
+-rw-r--r--  3.0 unx    93670 tx defN 23-May-08 00:39 static/js/vue.min.js
+-rw-r--r--  3.0 unx    19055 tx defN 23-May-08 00:39 static/js/prism.js
+-rw-r--r--  3.0 unx      868 tx defN 23-May-08 00:39 static/js/firebase-push.js
+-rw-r--r--  3.0 unx     8311 tx defN 23-May-08 00:39 static/js/utils.min.js
+-rw-r--r--  3.0 unx    11888 tx defN 23-Nov-12 21:35 static/js/utils.js
+-rw-r--r--  3.0 unx    68547 tx defN 23-May-08 00:39 static/js/sugar.min.js
+-rw-r--r--  3.0 unx    32337 tx defN 23-Nov-12 21:45 static/js/axios.min.js
+-rw-r--r--  3.0 unx   342147 tx defN 23-Dec-11 08:15 static/js/vue.js
+-rw-r--r--  3.0 unx      496 tx defN 23-May-08 00:39 static/js/star_rater_vue.js
+-rw-r--r--  3.0 unx       35 tx stor 23-May-08 00:39 static/components-bulma/fileupload/fileupload.css
+-rw-r--r--  3.0 unx     1232 tx defN 23-May-08 00:39 static/components-bulma/fileupload/fileupload.js
+-rw-r--r--  3.0 unx       83 tx defN 23-May-08 00:39 static/components-bulma/fileupload/fileupload.html
+-rw-r--r--  3.0 unx        0 bx stor 23-May-08 00:39 static/components-bulma/starrater/starrater.css
+-rw-r--r--  3.0 unx     1687 tx defN 23-May-08 00:39 static/components-bulma/starrater/starrater.js
+-rw-r--r--  3.0 unx      308 tx defN 23-May-08 00:39 static/components-bulma/starrater/starrater.html
+-rw-r--r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components-bulma/mtable.html
+-rw-r--r--  3.0 unx      411 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.css
+-rw-r--r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components-bulma/grid/luxon.js
+-rw-r--r--  3.0 unx     5384 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.js
+-rw-r--r--  3.0 unx     3369 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.html
+-rw-r--r--  3.0 unx       43 tx stor 23-May-08 00:39 static/components-bulma/vueform/vueform.css
+-rw-r--r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components-bulma/vueform/luxon.js
+-rw-r--r--  3.0 unx     7257 tx defN 23-May-08 00:39 static/components-bulma/vueform/vueform.js
+-rw-r--r--  3.0 unx    70115 tx defN 23-May-08 00:39 static/components-bulma/vueform/luxon.min.js
+-rw-r--r--  3.0 unx     3400 tx defN 23-May-08 00:39 static/components-bulma/vueform/vueform.html
+-rw-r--r--  3.0 unx     8097 tx defN 23-May-08 00:39 static/components-bulma/mtable.js
+-rw-r--r--  3.0 unx       12 tx stor 23-May-08 00:39 static/hello.txt
+-rw-r--r--  3.0 unx     1913 tx defN 23-May-08 00:39 templates/socketio/socketio_index.html
+-rw-r--r--  3.0 unx     2156 tx defN 23-May-08 00:39 templates/layout_bulma.html
+-rw-r--r--  3.0 unx      488 tx defN 23-May-08 00:39 templates/vue/insert_form.html
+-rw-r--r--  3.0 unx      392 tx defN 23-May-08 00:39 templates/vue/vuegrid_bulma.html
+-rw-r--r--  3.0 unx      372 tx defN 23-May-08 00:39 templates/vue/file_uploader.html
+-rw-r--r--  3.0 unx      544 tx defN 23-May-08 00:39 templates/vue/star_rater_vue_bulma.html
+-rw-r--r--  3.0 unx      502 tx defN 23-May-08 00:39 templates/vue/star_rater_vue.html
+-rw-r--r--  3.0 unx      374 tx defN 23-May-08 00:39 templates/vue/vuegrid.html
+-rw-r--r--  3.0 unx      448 tx defN 23-May-08 00:39 templates/vue/starrating.html
+-rw-r--r--  3.0 unx      683 tx defN 23-May-08 00:39 templates/vue/vue_grid_and_forms.html
+-rw-r--r--  3.0 unx      486 tx defN 23-May-08 00:39 templates/vue/edit_form.html
+-rw-r--r--  3.0 unx      486 tx defN 23-May-08 00:39 templates/vue/view_form.html
+-rw-r--r--  3.0 unx     2172 tx defN 23-May-08 00:39 templates/ws/ws_index.html
+-rw-r--r--  3.0 unx     6788 tx defN 23-May-08 00:39 templates/index.html
+-rw-r--r--  3.0 unx      430 tx defN 23-Aug-06 14:14 templates/show.html
+-rw-r--r--  3.0 unx       26 tx stor 23-May-08 00:39 templates/examples/flash_example_next.html
+-rw-r--r--  3.0 unx      551 tx defN 23-May-08 00:39 templates/examples/auth_custom_login.html
+-rw-r--r--  3.0 unx      189 tx defN 23-May-08 00:39 templates/examples/hcaptcha_form.html
+-rw-r--r--  3.0 unx     1025 tx defN 23-May-08 00:39 templates/examples/rest_info.html
+-rw-r--r--  3.0 unx      242 tx defN 23-May-08 00:39 templates/examples/flash_example.html
+-rw-r--r--  3.0 unx       69 tx defN 23-May-08 00:39 templates/examples/ajax_grid.html
+-rw-r--r--  3.0 unx      263 tx defN 23-May-08 00:39 templates/examples/session_counter.html
+-rw-r--r--  3.0 unx      646 tx defN 23-May-08 00:39 templates/examples/auth_forms.html
+-rw-r--r--  3.0 unx      305 tx defN 23-May-08 00:39 templates/examples/form.html
+-rw-r--r--  3.0 unx      869 tx defN 23-May-08 00:39 templates/examples/custom_form.html
+-rw-r--r--  3.0 unx     1711 tx defN 23-May-08 00:39 templates/examples/tagsinput_form.html
+-rw-r--r--  3.0 unx       82 tx defN 23-May-08 00:39 templates/examples/page_with_template.html
+-rw-r--r--  3.0 unx      242 tx defN 23-May-08 00:39 templates/examples/forms.html
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/html_grid.html
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/component_loader.html
+-rw-r--r--  3.0 unx      228 tx defN 23-May-08 00:39 templates/examples/generic.html
+-rw-r--r--  3.0 unx      193 tx defN 23-May-08 00:39 templates/examples/auth_form.html
+-rw-r--r--  3.0 unx     2778 tx defN 23-May-08 00:39 templates/layout.html
+-rw-r--r--  3.0 unx      278 tx defN 23-May-08 00:39 templates/auth.html
+143 files, 9348902 bytes uncompressed, 1365612 bytes compressed:  85.4%
```

#### zipnote {}

```diff
@@ -1,430 +1,430 @@
-Filename: __init__.py
+Filename: uploads/README.md
 Comment: 
 
-Filename: uploads/README.md
+Filename: __init__.py
 Comment: 
 
-Filename: templates/layout.html
+Filename: examples/count.py
 Comment: 
 
-Filename: templates/layout_bulma.html
+Filename: examples/ws_client_example.py
 Comment: 
 
-Filename: templates/vue/vue_grid_and_forms.html
+Filename: examples/page_with_error.py
 Comment: 
 
-Filename: templates/vue/star_rater_vue_bulma.html
+Filename: examples/page_with_raise.py
 Comment: 
 
-Filename: templates/vue/star_rater_vue.html
+Filename: examples/hello_world_msg.py
 Comment: 
 
-Filename: templates/vue/view_form.html
+Filename: examples/test_expose.py
 Comment: 
 
-Filename: templates/vue/insert_form.html
+Filename: examples/page_with_parameters.py
 Comment: 
 
-Filename: templates/vue/vuegrid_bulma.html
+Filename: examples/hello_world.py
 Comment: 
 
-Filename: templates/vue/starrating.html
+Filename: examples/page_with_query.py
 Comment: 
 
-Filename: templates/vue/file_uploader.html
+Filename: examples/example_html_grid.py
 Comment: 
 
-Filename: templates/vue/vuegrid.html
+Filename: examples/page_with_redirect.py
 Comment: 
 
-Filename: templates/vue/edit_form.html
+Filename: examples/session_clear.py
 Comment: 
 
-Filename: templates/ws/ws_index.html
+Filename: examples/models.py
 Comment: 
 
-Filename: templates/socketio/socketio_index.html
+Filename: examples/flash_example_fixture.py
 Comment: 
 
-Filename: templates/examples/flash_example.html
+Filename: examples/custom_form.py
 Comment: 
 
-Filename: templates/examples/custom_form.html
+Filename: examples/rpc.py
 Comment: 
 
-Filename: templates/examples/forms.html
+Filename: examples/session_counter.py
 Comment: 
 
-Filename: templates/examples/page_with_template.html
+Filename: examples/socketio.py
 Comment: 
 
-Filename: templates/examples/tagsinput_form.html
+Filename: examples/auth_forms.py
 Comment: 
 
-Filename: templates/examples/html_grid.html
+Filename: examples/rest.py
 Comment: 
 
-Filename: templates/examples/hcaptcha_form.html
+Filename: examples/common.py
 Comment: 
 
-Filename: templates/examples/auth_custom_login.html
+Filename: examples/page_with_template.py
 Comment: 
 
-Filename: templates/examples/auth_form.html
+Filename: examples/auth_form.py
 Comment: 
 
-Filename: templates/examples/flash_example_next.html
+Filename: examples/create_form.py
 Comment: 
 
-Filename: templates/examples/form.html
+Filename: examples/ws.py
 Comment: 
 
-Filename: templates/examples/component_loader.html
+Filename: examples/show_a_button.py
 Comment: 
 
-Filename: templates/examples/generic.html
+Filename: examples/page_without_template.py
 Comment: 
 
-Filename: templates/examples/rest_info.html
+Filename: examples/settings.py
 Comment: 
 
-Filename: templates/examples/ajax_grid.html
+Filename: examples/page_with_postback.py
 Comment: 
 
-Filename: templates/examples/session_counter.html
+Filename: examples/update_form.py
 Comment: 
 
-Filename: templates/examples/auth_forms.html
+Filename: examples/example_multiple_forms.py
 Comment: 
 
-Filename: templates/auth.html
+Filename: examples/component_loader.py
 Comment: 
 
-Filename: templates/index.html
+Filename: examples/hello.py
 Comment: 
 
-Filename: templates/show.html
+Filename: examples/tagsinput_form.py
 Comment: 
 
-Filename: examples/models.py
+Filename: examples/example_helpers.py
 Comment: 
 
-Filename: examples/auth_form.py
+Filename: examples/example_ajax_grid.py
 Comment: 
 
-Filename: examples/flash_example_naive.py
+Filename: examples/hcaptcha_form.py
 Comment: 
 
-Filename: examples/rest.py
+Filename: examples/flash_example_naive.py
 Comment: 
 
-Filename: examples/create_form.py
+Filename: vue_components_examples/vue_insert_form.py
 Comment: 
 
-Filename: examples/hello_world_msg.py
+Filename: vue_components_examples/vue_grid_and_forms.py
 Comment: 
 
-Filename: examples/example_html_grid.py
+Filename: vue_components_examples/models.py
 Comment: 
 
-Filename: examples/update_form.py
+Filename: vue_components_examples/vue_file_uploader.py
 Comment: 
 
-Filename: examples/ws.py
+Filename: vue_components_examples/common.py
 Comment: 
 
-Filename: examples/session_counter.py
+Filename: vue_components_examples/vue_grid.py
 Comment: 
 
-Filename: examples/component_loader.py
+Filename: vue_components_examples/components/fileupload.py
 Comment: 
 
-Filename: examples/show_a_button.py
+Filename: vue_components_examples/components/starrater.py
 Comment: 
 
-Filename: examples/hello.py
+Filename: vue_components_examples/components/vueform.py
 Comment: 
 
-Filename: examples/ws_client_example.py
+Filename: vue_components_examples/components/grid.py
 Comment: 
 
-Filename: examples/example_helpers.py
+Filename: vue_components_examples/components/README.md
 Comment: 
 
-Filename: examples/page_with_raise.py
+Filename: vue_components_examples/settings.py
 Comment: 
 
-Filename: examples/example_multiple_forms.py
+Filename: vue_components_examples/vue_view_form.py
 Comment: 
 
-Filename: examples/page_with_template.py
+Filename: vue_components_examples/vue_edit_form.py
 Comment: 
 
-Filename: examples/custom_form.py
+Filename: vue_components_examples/vue_star_rater.py
 Comment: 
 
-Filename: examples/count.py
+Filename: translations/it.json
 Comment: 
 
-Filename: examples/socketio.py
+Filename: translations/en.json
 Comment: 
 
-Filename: examples/page_with_query.py
+Filename: static/socketio/README.md
 Comment: 
 
-Filename: examples/auth_forms.py
+Filename: static/favicon.ico
 Comment: 
 
-Filename: examples/common.py
+Filename: static/error.html
 Comment: 
 
-Filename: examples/page_with_postback.py
+Filename: static/ws/README.md
 Comment: 
 
-Filename: examples/test_expose.py
+Filename: static/data/uscities.json
 Comment: 
 
-Filename: examples/hello_world.py
+Filename: static/data/zip_codes.json
 Comment: 
 
-Filename: examples/settings.py
+Filename: static/firebase-push.html
 Comment: 
 
-Filename: examples/rpc.py
+Filename: static/css/no.css
 Comment: 
 
-Filename: examples/page_with_error.py
+Filename: static/css/prism.css
 Comment: 
 
-Filename: examples/example_ajax_grid.py
+Filename: static/components/fileupload/fileupload.css
 Comment: 
 
-Filename: examples/flash_example_fixture.py
+Filename: static/components/fileupload/fileupload.js
 Comment: 
 
-Filename: examples/page_without_template.py
+Filename: static/components/fileupload/fileupload.html
 Comment: 
 
-Filename: examples/page_with_parameters.py
+Filename: static/components/starrater/starrater.css
 Comment: 
 
-Filename: examples/page_with_redirect.py
+Filename: static/components/starrater/starrater.js
 Comment: 
 
-Filename: examples/session_clear.py
+Filename: static/components/starrater/starrater.html
 Comment: 
 
-Filename: examples/hcaptcha_form.py
+Filename: static/components/mtable.html
 Comment: 
 
-Filename: examples/tagsinput_form.py
+Filename: static/components/grid/grid.css
 Comment: 
 
-Filename: vue_components_examples/models.py
+Filename: static/components/grid/grid.js
 Comment: 
 
-Filename: vue_components_examples/vue_edit_form.py
+Filename: static/components/grid/grid.html
 Comment: 
 
-Filename: vue_components_examples/vue_view_form.py
+Filename: static/components/vueform/vueform.css
 Comment: 
 
-Filename: vue_components_examples/components/fileupload.py
+Filename: static/components/vueform/luxon.js
 Comment: 
 
-Filename: vue_components_examples/components/grid.py
+Filename: static/components/vueform/vueform.js
 Comment: 
 
-Filename: vue_components_examples/components/starrater.py
+Filename: static/components/vueform/luxon.min.js
 Comment: 
 
-Filename: vue_components_examples/components/vueform.py
+Filename: static/components/vueform/vueform.html
 Comment: 
 
-Filename: vue_components_examples/components/README.md
+Filename: static/components/mtable.js
 Comment: 
 
-Filename: vue_components_examples/vue_star_rater.py
+Filename: static/js/vue.min.js
 Comment: 
 
-Filename: vue_components_examples/vue_insert_form.py
+Filename: static/js/prism.js
 Comment: 
 
-Filename: vue_components_examples/common.py
+Filename: static/js/firebase-push.js
 Comment: 
 
-Filename: vue_components_examples/vue_grid_and_forms.py
+Filename: static/js/utils.min.js
 Comment: 
 
-Filename: vue_components_examples/settings.py
+Filename: static/js/utils.js
 Comment: 
 
-Filename: vue_components_examples/vue_file_uploader.py
+Filename: static/js/sugar.min.js
 Comment: 
 
-Filename: vue_components_examples/vue_grid.py
+Filename: static/js/axios.min.js
 Comment: 
 
-Filename: translations/it.json
+Filename: static/js/vue.js
 Comment: 
 
-Filename: translations/en.json
+Filename: static/js/star_rater_vue.js
 Comment: 
 
-Filename: static/js/utils.js
+Filename: static/components-bulma/fileupload/fileupload.css
 Comment: 
 
-Filename: static/js/star_rater_vue.js
+Filename: static/components-bulma/fileupload/fileupload.js
 Comment: 
 
-Filename: static/js/firebase-push.js
+Filename: static/components-bulma/fileupload/fileupload.html
 Comment: 
 
-Filename: static/js/vue.js
+Filename: static/components-bulma/starrater/starrater.css
 Comment: 
 
-Filename: static/js/sugar.min.js
+Filename: static/components-bulma/starrater/starrater.js
 Comment: 
 
-Filename: static/js/prism.js
+Filename: static/components-bulma/starrater/starrater.html
 Comment: 
 
-Filename: static/js/axios.min.js
+Filename: static/components-bulma/mtable.html
 Comment: 
 
-Filename: static/js/utils.min.js
+Filename: static/components-bulma/grid/grid.css
 Comment: 
 
-Filename: static/js/vue.min.js
+Filename: static/components-bulma/grid/luxon.js
 Comment: 
 
-Filename: static/ws/README.md
+Filename: static/components-bulma/grid/grid.js
 Comment: 
 
-Filename: static/hello.txt
+Filename: static/components-bulma/grid/grid.html
 Comment: 
 
-Filename: static/socketio/README.md
+Filename: static/components-bulma/vueform/vueform.css
 Comment: 
 
-Filename: static/components/mtable.js
+Filename: static/components-bulma/vueform/luxon.js
 Comment: 
 
-Filename: static/components/starrater/starrater.html
+Filename: static/components-bulma/vueform/vueform.js
 Comment: 
 
-Filename: static/components/starrater/starrater.css
+Filename: static/components-bulma/vueform/luxon.min.js
 Comment: 
 
-Filename: static/components/starrater/starrater.js
+Filename: static/components-bulma/vueform/vueform.html
 Comment: 
 
-Filename: static/components/mtable.html
+Filename: static/components-bulma/mtable.js
 Comment: 
 
-Filename: static/components/vueform/vueform.css
+Filename: static/hello.txt
 Comment: 
 
-Filename: static/components/vueform/luxon.js
+Filename: templates/socketio/socketio_index.html
 Comment: 
 
-Filename: static/components/vueform/vueform.js
+Filename: templates/layout_bulma.html
 Comment: 
 
-Filename: static/components/vueform/vueform.html
+Filename: templates/vue/insert_form.html
 Comment: 
 
-Filename: static/components/vueform/luxon.min.js
+Filename: templates/vue/vuegrid_bulma.html
 Comment: 
 
-Filename: static/components/fileupload/fileupload.html
+Filename: templates/vue/file_uploader.html
 Comment: 
 
-Filename: static/components/fileupload/fileupload.js
+Filename: templates/vue/star_rater_vue_bulma.html
 Comment: 
 
-Filename: static/components/fileupload/fileupload.css
+Filename: templates/vue/star_rater_vue.html
 Comment: 
 
-Filename: static/components/grid/grid.js
+Filename: templates/vue/vuegrid.html
 Comment: 
 
-Filename: static/components/grid/grid.css
+Filename: templates/vue/starrating.html
 Comment: 
 
-Filename: static/components/grid/grid.html
+Filename: templates/vue/vue_grid_and_forms.html
 Comment: 
 
-Filename: static/css/no.css
+Filename: templates/vue/edit_form.html
 Comment: 
 
-Filename: static/css/prism.css
+Filename: templates/vue/view_form.html
 Comment: 
 
-Filename: static/data/uscities.json
+Filename: templates/ws/ws_index.html
 Comment: 
 
-Filename: static/data/zip_codes.json
+Filename: templates/index.html
 Comment: 
 
-Filename: static/components-bulma/mtable.js
+Filename: templates/show.html
 Comment: 
 
-Filename: static/components-bulma/starrater/starrater.html
+Filename: templates/examples/flash_example_next.html
 Comment: 
 
-Filename: static/components-bulma/starrater/starrater.css
+Filename: templates/examples/auth_custom_login.html
 Comment: 
 
-Filename: static/components-bulma/starrater/starrater.js
+Filename: templates/examples/hcaptcha_form.html
 Comment: 
 
-Filename: static/components-bulma/mtable.html
+Filename: templates/examples/rest_info.html
 Comment: 
 
-Filename: static/components-bulma/vueform/vueform.css
+Filename: templates/examples/flash_example.html
 Comment: 
 
-Filename: static/components-bulma/vueform/luxon.js
+Filename: templates/examples/ajax_grid.html
 Comment: 
 
-Filename: static/components-bulma/vueform/vueform.js
+Filename: templates/examples/session_counter.html
 Comment: 
 
-Filename: static/components-bulma/vueform/vueform.html
+Filename: templates/examples/auth_forms.html
 Comment: 
 
-Filename: static/components-bulma/vueform/luxon.min.js
+Filename: templates/examples/form.html
 Comment: 
 
-Filename: static/components-bulma/fileupload/fileupload.html
+Filename: templates/examples/custom_form.html
 Comment: 
 
-Filename: static/components-bulma/fileupload/fileupload.js
+Filename: templates/examples/tagsinput_form.html
 Comment: 
 
-Filename: static/components-bulma/fileupload/fileupload.css
+Filename: templates/examples/page_with_template.html
 Comment: 
 
-Filename: static/components-bulma/grid/grid.js
+Filename: templates/examples/forms.html
 Comment: 
 
-Filename: static/components-bulma/grid/grid.css
+Filename: templates/examples/html_grid.html
 Comment: 
 
-Filename: static/components-bulma/grid/luxon.js
+Filename: templates/examples/component_loader.html
 Comment: 
 
-Filename: static/components-bulma/grid/grid.html
+Filename: templates/examples/generic.html
 Comment: 
 
-Filename: static/favicon.ico
+Filename: templates/examples/auth_form.html
 Comment: 
 
-Filename: static/error.html
+Filename: templates/layout.html
 Comment: 
 
-Filename: static/firebase-push.html
+Filename: templates/auth.html
 Comment: 
 
 Zip file comment:
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

#### __init__.py

```diff
@@ -69,15 +69,15 @@
         data.append({"name": f"{name}.md", "content": metadata, "language": "markdown"})
     filename = f"apps/showcase/{name}.py"
     if not os.path.exists(filename):
         raise HTTP(404)
     with open(filename) as stream:
         controller = stream.read().strip()
     data.append({"name": f"{name}.py", "content": controller, "language": "python"})
-    templates = re.compile("[/\w]+\.html").findall(controller)
+    templates = re.compile(r"[/\w]+\.html").findall(controller)
     for template in templates:
         with open(f"apps/showcase/templates/{template}") as stream:
             content = stream.read().strip()
             data.append(
                 {
                     "name": f"templates/{template}",
                     "content": content,
```

#### static/js/vue.js

##### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /*!
- * Vue.js v2.6.10
- * (c) 2014-2019 Evan You
+ * Vue.js v2.6.12
+ * (c) 2014-2020 Evan You
  * Released under the MIT License.
  */
 (function(global, factory) {
     typeof exports === 'object' && typeof module !== 'undefined' ? module.exports = factory() :
         typeof define === 'function' && define.amd ? define(factory) :
         (global = global || self, global.Vue = factory());
 }(this, function() {
@@ -2052,15 +2052,15 @@
         timerFunc = function() {
             counter = (counter + 1) % 2;
             textNode.data = String(counter);
         };
         isUsingMicroTask = true;
     } else if (typeof setImmediate !== 'undefined' && isNative(setImmediate)) {
         // Fallback to setImmediate.
-        // Techinically it leverages the (macro) task queue,
+        // Technically it leverages the (macro) task queue,
         // but it is still a better choice than setTimeout.
         timerFunc = function() {
             setImmediate(flushCallbacks);
         };
     } else {
         // Fallback to setTimeout.
         timerFunc = function() {
@@ -2143,15 +2143,15 @@
             );
         };
 
         var warnReservedPrefix = function(target, key) {
             warn(
                 "Property \"" + key + "\" must be accessed with \"$data." + key + "\" because " +
                 'properties starting with "$" or "_" are not proxied in the Vue instance to ' +
-                'prevent conflicts with Vue internals' +
+                'prevent conflicts with Vue internals. ' +
                 'See: https://vuejs.org/v2/api/#data',
                 target
             );
         };
 
         var hasProxy =
             typeof Proxy !== 'undefined' && isNative(Proxy);
@@ -3024,15 +3024,15 @@
 
     function bindDynamicKeys(baseObj, values) {
         for (var i = 0; i < values.length; i += 2) {
             var key = values[i];
             if (typeof key === 'string' && key) {
                 baseObj[values[i]] = values[i + 1];
             } else if (key !== '' && key !== null) {
-                // null is a speical value for explicitly removing a binding
+                // null is a special value for explicitly removing a binding
                 warn(
                     ("Invalid value for dynamic directive argument (expected string or null): " + key),
                     this
                 );
             }
         }
         return baseObj
@@ -3531,14 +3531,20 @@
         }
         var vnode, ns;
         if (typeof tag === 'string') {
             var Ctor;
             ns = (context.$vnode && context.$vnode.ns) || config.getTagNamespace(tag);
             if (config.isReservedTag(tag)) {
                 // platform built-in elements
+                if (isDef(data) && isDef(data.nativeOn)) {
+                    warn(
+                        ("The .native modifier for v-on is only valid on components but it was used on <" + tag + ">."),
+                        context
+                    );
+                }
                 vnode = new VNode(
                     config.parsePlatformTagName(tag), data, children,
                     undefined, undefined, context
                 );
             } else if ((!data || !data.pre) && isDef(Ctor = resolveAsset(context.$options, 'components', tag))) {
                 // component
                 vnode = createComponent(Ctor, data, context, children, tag);
@@ -3664,15 +3670,15 @@
 
             // set parent vnode. this allows render functions to have access
             // to the data on the placeholder node.
             vm.$vnode = _parentVnode;
             // render self
             var vnode;
             try {
-                // There's no need to maintain a stack becaues all render fns are called
+                // There's no need to maintain a stack because all render fns are called
                 // separately from one another. Nested component's render fns are called
                 // when parent component is patched.
                 currentRenderingInstance = vm;
                 vnode = render.call(vm._renderProxy, vm.$createElement);
             } catch (e) {
                 handleError(e, vm, "render");
                 // return error render result,
@@ -5601,15 +5607,15 @@
     });
 
     // expose FunctionalRenderContext for ssr runtime helper installation
     Object.defineProperty(Vue, 'FunctionalRenderContext', {
         value: FunctionalRenderContext
     });
 
-    Vue.version = '2.6.10';
+    Vue.version = '2.6.12';
 
     /*  */
 
     // these are reserved for web because they are directly compiled away
     // during template compilation
     var isReservedAttr = makeMap('style,class');
 
@@ -6296,15 +6302,15 @@
             if (isDef(i = vnode.children)) {
                 for (j = 0; j < vnode.children.length; ++j) {
                     invokeDestroyHook(vnode.children[j]);
                 }
             }
         }
 
-        function removeVnodes(parentElm, vnodes, startIdx, endIdx) {
+        function removeVnodes(vnodes, startIdx, endIdx) {
             for (; startIdx <= endIdx; ++startIdx) {
                 var ch = vnodes[startIdx];
                 if (isDef(ch)) {
                     if (isDef(ch.tag)) {
                         removeAndInvokeRemoveHook(ch);
                         invokeDestroyHook(ch);
                     } else { // Text node
@@ -6409,15 +6415,15 @@
                     newStartVnode = newCh[++newStartIdx];
                 }
             }
             if (oldStartIdx > oldEndIdx) {
                 refElm = isUndef(newCh[newEndIdx + 1]) ? null : newCh[newEndIdx + 1].elm;
                 addVnodes(parentElm, refElm, newCh, newStartIdx, newEndIdx, insertedVnodeQueue);
             } else if (newStartIdx > newEndIdx) {
-                removeVnodes(parentElm, oldCh, oldStartIdx, oldEndIdx);
+                removeVnodes(oldCh, oldStartIdx, oldEndIdx);
             }
         }
 
         function checkDuplicateKeys(children) {
             var seenKeys = {};
             for (var i = 0; i < children.length; i++) {
                 var vnode = children[i];
@@ -6511,15 +6517,15 @@
                         checkDuplicateKeys(ch);
                     }
                     if (isDef(oldVnode.text)) {
                         nodeOps.setTextContent(elm, '');
                     }
                     addVnodes(elm, null, ch, 0, ch.length - 1, insertedVnodeQueue);
                 } else if (isDef(oldCh)) {
-                    removeVnodes(elm, oldCh, 0, oldCh.length - 1);
+                    removeVnodes(oldCh, 0, oldCh.length - 1);
                 } else if (isDef(oldVnode.text)) {
                     nodeOps.setTextContent(elm, '');
                 }
             } else if (oldVnode.text !== vnode.text) {
                 nodeOps.setTextContent(elm, vnode.text);
             }
             if (isDef(data)) {
@@ -6746,15 +6752,15 @@
                             }
                             ancestor = ancestor.parent;
                         }
                     }
 
                     // destroy old node
                     if (isDef(parentElm)) {
-                        removeVnodes(parentElm, [oldVnode], 0, 0);
+                        removeVnodes([oldVnode], 0, 0);
                     } else if (isDef(oldVnode.tag)) {
                         invokeDestroyHook(oldVnode);
                     }
                 }
             }
 
             invokeInsertHook(vnode, insertedVnodeQueue, isInitialPatch);
@@ -7904,15 +7910,15 @@
                 while (svg.firstChild) {
                     elm.appendChild(svg.firstChild);
                 }
             } else if (
                 // skip the update if old and new VDOM state is the same.
                 // `value` is handled separately because the DOM value may be temporarily
                 // out of sync with VDOM state due to focus, composition and modifiers.
-                // This  #4521 by skipping the unnecesarry `checked` update.
+                // This  #4521 by skipping the unnecessary `checked` update.
                 cur !== oldProps[key]
             ) {
                 // some property updates can throw
                 // e.g. `value` on <progress> w/ non-finite value
                 try {
                     elm[key] = cur;
                 } catch (e) {}
@@ -9543,15 +9549,15 @@
     var dynamicArgAttribute = /^\s*((?:v-[\w-]+:|@|:|#)\[[^=]+\][^\s"'<>\/=]*)(?:\s*(=)\s*(?:"([^"]*)"+|'([^']*)'+|([^\s"'=<>`]+)))?/;
     var ncname = "[a-zA-Z_][\\-\\.0-9_a-zA-Z" + (unicodeRegExp.source) + "]*";
     var qnameCapture = "((?:" + ncname + "\\:)?" + ncname + ")";
     var startTagOpen = new RegExp(("^<" + qnameCapture));
     var startTagClose = /^\s*(\/?)>/;
     var endTag = new RegExp(("^<\\/" + qnameCapture + "[^>]*>"));
     var doctype = /^<!DOCTYPE [^>]+>/i;
-    // #7298: escape - to avoid being pased as HTML comment when inlined in page
+    // #7298: escape - to avoid being passed as HTML comment when inlined in page
     var comment = /^<!\--/;
     var conditionalComment = /^<!\[/;
 
     // Special Elements (can contain anything)
     var isPlainTextElement = makeMap('script,style,textarea', true);
     var reCache = {};
 
@@ -9850,15 +9856,15 @@
             }
         }
     }
 
     /*  */
 
     var onRE = /^@|^v-on:/;
-    var dirRE = /^v-|^@|^:/;
+    var dirRE = /^v-|^@|^:|^#/;
     var forAliasRE = /([\s\S]*?)\s+(?:in|of)\s+([\s\S]*)/;
     var forIteratorRE = /,([^,\}\]]*)(?:,([^,\}\]]*))?$/;
     var stripParensRE = /^\(|\)$/g;
     var dynamicArgRE = /^\[.*\]$/;
 
     var argRE = /:(.*)$/;
     var bindRE = /^:|^\.|^v-bind:/;
@@ -10213,15 +10219,15 @@
                             child.end = end;
                         }
                         children.push(child);
                     }
                 }
             },
             comment: function comment(text, start, end) {
-                // adding anyting as a sibling to the root node is forbidden
+                // adding anything as a sibling to the root node is forbidden
                 // comments should still be allowed, but ignored
                 if (currentParent) {
                     var child = {
                         type: 3,
                         text: text,
                         isComment: true
                     };
@@ -10484,15 +10490,15 @@
                                 "Unexpected mixed usage of different slot syntaxes.",
                                 el
                             );
                         }
                         if (el.parent && !maybeComponent(el.parent)) {
                             warn$2(
                                 "<template v-slot> can only appear at the root level inside " +
-                                "the receiving the component",
+                                "the receiving component",
                                 el
                             );
                         }
                     }
                     var ref = getSlotName(slotBinding);
                     var name = ref.name;
                     var dynamic = ref.dynamic;
@@ -11061,15 +11067,15 @@
             }
         }
         return false
     }
 
     /*  */
 
-    var fnExpRE = /^([\w$_]+|\([^)]*?\))\s*=>|^function\s*(?:[\w$]+)?\s*\(/;
+    var fnExpRE = /^([\w$_]+|\([^)]*?\))\s*=>|^function(?:\s+[\w$]+)?\s*\(/;
     var fnInvokeRE = /\([^)]*?\);*$/;
     var simplePathRE = /^[A-Za-z_$][\w$]*(?:\.[A-Za-z_$][\w$]*|\['[^']*?']|\["[^"]*?"]|\[\d+]|\[[A-Za-z_$][\w$]*])*$/;
 
     // KeyboardEvent.keyCode aliases
     var keyCodes = {
         esc: 27,
         tab: 9,
@@ -11860,14 +11866,16 @@
             for (var name in node.attrsMap) {
                 if (dirRE.test(name)) {
                     var value = node.attrsMap[name];
                     if (value) {
                         var range = node.rawAttrsMap[name];
                         if (name === 'v-for') {
                             checkFor(node, ("v-for=\"" + value + "\""), warn, range);
+                        } else if (name === 'v-slot' || name[0] === '#') {
+                            checkFunctionParameterExpression(value, (name + "=\"" + value + "\""), warn, range);
                         } else if (onRE.test(name)) {
                             checkEvent(value, (name + "=\"" + value + "\""), warn, range);
                         } else {
                             checkExpression(value, (name + "=\"" + value + "\""), warn, range);
                         }
                     }
                 }
@@ -11879,17 +11887,17 @@
             }
         } else if (node.type === 2) {
             checkExpression(node.expression, node.text, warn, node);
         }
     }
 
     function checkEvent(exp, text, warn, range) {
-        var stipped = exp.replace(stripStringRE, '');
-        var keywordMatch = stipped.match(unaryOperatorsRE);
-        if (keywordMatch && stipped.charAt(keywordMatch.index - 1) !== '$') {
+        var stripped = exp.replace(stripStringRE, '');
+        var keywordMatch = stripped.match(unaryOperatorsRE);
+        if (keywordMatch && stripped.charAt(keywordMatch.index - 1) !== '$') {
             warn(
                 "avoid using JavaScript unary operator as property name: " +
                 "\"" + (keywordMatch[0]) + "\" in expression " + (text.trim()),
                 range
             );
         }
         checkExpression(exp, text, warn, range);
@@ -11936,14 +11944,27 @@
                     "  Raw expression: " + (text.trim()) + "\n",
                     range
                 );
             }
         }
     }
 
+    function checkFunctionParameterExpression(exp, text, warn, range) {
+        try {
+            new Function(exp, '');
+        } catch (e) {
+            warn(
+                "invalid function parameter expression: " + (e.message) + " in\n\n" +
+                "    " + exp + "\n\n" +
+                "  Raw expression: " + (text.trim()) + "\n",
+                range
+            );
+        }
+    }
+
     /*  */
 
     var range = 2;
 
     function generateCodeFrame(
         source,
         start,
```

### Comparing `py4web-1.20231115.1/py4web/core.py` & `py4web-1.20240420.1/py4web/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import http.client
 import http.cookies
 import importlib.machinery
 import importlib.util
 import inspect
 import io
 import json
-import linecache
 import logging
 import numbers
 import os
 import pathlib
 import platform
 import re
 import signal
@@ -31,14 +30,15 @@
 import traceback
 import types
 import urllib.parse
 import uuid
 import zipfile
 from collections import OrderedDict
 from contextlib import redirect_stderr, redirect_stdout
+import html as sanitize_html
 
 import portalocker
 from watchgod import awatch
 
 from . import server_adapters
 
 # Optional web servers for speed
@@ -339,16 +339,17 @@
 
     @_safe_local.setter
     def _safe_local(self, storage):
         self.__mount_local__(self, storage)
 
     def is_valid(self):
         """check if the fixture is valid in context"""
-        ctx = self.__request_master_ctx__.request_ctx
-        if self not in ctx:
+
+        ctx = getattr(self.__request_master_ctx__, "request_ctx", None)
+        if not ctx or self not in ctx:
             logging.warn(
                 "attempted access to fixture %s from outside a request",
                 self.__class__.__name__,
             )
             return False
         return True
 
@@ -458,15 +459,15 @@
         return self._safe_local
 
     def on_request(self, context):
         self._safe_local = types.SimpleNamespace()
         # when a new request arrives we look for a flash message in the cookie
         flash = request.get_cookie("py4web-flash")
         if flash:
-            self.local.flash = json.loads(flash)
+            self.local.flash = safely(lambda: json.loads(flash), default=None)
         else:
             self.local.flash = None
 
     def on_success(self, context):
         # if we redirect and have a flash message we move it to the session
         status = context["status"]
         if status == 303 and self.local.flash:
@@ -507,20 +508,20 @@
     def _escape_data(self, data):
         """Allows Renoir to convert yatl helpers to strings"""
         return safely(
             lambda: data.xml(), default=lambda: self._to_html(self._to_unicode(data))
         )
 
 
-class RenoirCustomWriter(RenoirXMLEscapeMixin, renoir.writers.Writer):
-    ...
+class RenoirCustomWriter(RenoirXMLEscapeMixin, renoir.writers.Writer): ...
 
 
-class RenoirCustomEscapeAllWriter(RenoirXMLEscapeMixin, renoir.writers.EscapeAllWriter):
-    ...
+class RenoirCustomEscapeAllWriter(
+    RenoirXMLEscapeMixin, renoir.writers.EscapeAllWriter
+): ...
 
 
 class Renoir(renoir.Renoir):
     """Custom Renoir Engine that understands yatl helpers"""
 
     _writers = {
         renoir.constants.ESCAPES.common: RenoirCustomWriter,
@@ -694,14 +695,15 @@
             logging.debug("Session stored %s", cookie_data)
         response.set_cookie(
             self_local.session_cookie_name,
             cookie_data,
             path="/",
             secure=self_local.secure,
             same_site=self.same_site,
+            httponly=True,
         )
 
     def get(self, key, default=None):
         return self.get_data().get(key, default)
 
     def __getitem__(self, key):
         return self.get_data()[key]
@@ -831,15 +833,14 @@
 
 #########################################################################################
 # The Action Decorator
 #########################################################################################
 
 
 class HTTP(BaseException):
-
     """An exception that is considered success"""
 
     def __init__(self, status, body="", headers={}):
         self.status = status
         self.body = body
         self.headers = headers
 
@@ -1089,25 +1090,14 @@
 
     for frame, file, lnum, func, lines, idx in items:
         file = file and os.path.abspath(file) or "?"
         args, varargs, varkw, locals = inspect.getargvalues(frame)
         # Basic frame information
         f = {"file": file, "func": func, "lnum": lnum}
         f["code"] = lines
-        # FIXME: disable this for now until we understand why this goes into infinite loop
-        if False:
-            line_vars = cgitb.scanvars(
-                lambda: linecache.getline(file, lnum), frame, locals
-            )
-            # Dump local variables (referenced in current line only)
-            f["vars"] = {
-                key: repr(value)
-                for key, value in locals.items()
-                if not key.startswith("__")
-            }
         stackframes.append(f)
 
     return data
 
 
 class SimpleErrorLogger:
     def log(self, app_name, snapshot):
@@ -1185,15 +1175,14 @@
         """erase all tickets from database"""
         db = self.db
         db(db.py4web_error).delete()
         self.db.commit()
 
 
 class ErrorLogger:
-
     """
     To create your own custom logger for an app:
 
     class MyLogger:
         def log(app_name, error_snap_shop):
             ...
             return ticket_uuid
@@ -1246,15 +1235,15 @@
     ERRORS = {}
 
     @staticmethod
     def install_reloader_hook():
         # used by watcher
         def hook(*a, **k):
             app_name = request.path.split("/")[1]
-            if not app_name in Reloader.ROUTES:
+            if app_name not in Reloader.ROUTES:
                 app_name = "_default"
             if DIRTY_APPS.get(app_name):
                 Reloader.import_app(app_name)
                 DIRTY_APPS[app_name] = False
             ## APP_WATCH tasks, if used by any app
             try_app_watch_tasks()
 
@@ -1274,15 +1263,15 @@
     def import_apps():
         """Import or reimport modules and exposed static files"""
         Reloader.clear_routes()
         folder = os.environ["PY4WEB_APPS_FOLDER"]
         # if first time reload dummy top module
         if not Reloader.MODULES:
             path = os.path.join(folder, "__init__.py")
-            module = load_module("apps", path)
+            module = load_module("apps", path)  # noqa: F841
         # Then load all the apps as submodules
         if os.environ.get("PY4WEB_APP_NAMES"):
             app_names = os.environ.get("PY4WEB_APP_NAMES").split(",")
         else:
             app_names = os.listdir(folder)
         for app_name in app_names:
             Reloader.import_app(app_name, clear_before_import=False)
@@ -1402,14 +1391,17 @@
         "a:hover{background:rgba(0,0,0,0.1);padding:10px 30px}</style></head>"
         '<body><h1>[[=code]]</h1><h2>[[=message]]</h2>[[if button_text:]]<a href="[[=href]]">[[=button_text]]</a>[[pass]]</body></html>'
     ),
 }
 
 
 def error_page(code, button_text=None, href="#", color=None, message=None):
+    if button_text:
+        button_text = sanitize_html.escape(button_text)
+    href = sanitize_html.escape(href)
     message = http.client.responses[code].upper() if message is None else message
     color = (
         {"4": "#F44336", "5": "#607D8B"}.get(str(code)[0], "#2196F3")
         if not color
         else color
     )
     context = dict(
@@ -1820,15 +1812,15 @@
     help="No prompt, assume yes to questions",
     show_default=True,
 )
 def shell(**kwargs):
     """Open a python shell with apps_folder's parent added to the path"""
     if getattr(sys, "frozen", False) and hasattr(sys, "_MEIPASS"):
         # running in the PyInstaller binary bundle
-        import site
+        import site  # noqa: F401
     install_args(kwargs)
     code.interact(local=dict(globals(), **locals()))
 
 
 @cli.command()
 @click.argument("apps_folder", type=click.Path(exists=True))
 @click.argument("func")
@@ -1932,15 +1924,15 @@
 @click.option(
     "-P", "--port", default=8000, type=int, help="Port number", show_default=True
 )
 @click.option(
     "-A",
     "--app_names",
     default="",
-    help="List of apps to run (all if omitted or empty)",
+    help="List of apps to run, comma separated (all if omitted or empty)",
 )
 @click.option(
     "-p",
     "--password_file",
     default="password.txt",
     help="File for the encrypted password",
     show_default=True,
@@ -1965,16 +1957,16 @@
     "-s",
     "--server",
     default="default",
     type=click.Choice(
         ["default", "wsgiref", "tornado", "gunicorn", "gevent", "waitress"]
         + server_adapters.__all__
     ),
-    help="server to use",
-    show_default=True,
+    help="Web server to use",
+    show_default=False,
 )
 @click.option(
     "-w",
     "--number_workers",
     default=0,
     type=int,
     help="Number of workers",
@@ -2023,15 +2015,15 @@
     "-U",
     "--url_prefix",
     default="",
     help="Prefix to add to all URLs in and out",
     show_default=True,
 )
 def run(**kwargs):
-    """Run all the applications on apps_folder"""
+    """Run the applications on apps_folder"""
     install_args(kwargs)
 
     from py4web import __version__
 
     click.secho(ART, fg="blue")
     click.echo("Py4web: %s on Python %s\n\n" % (__version__, sys.version))
 
@@ -2043,15 +2035,17 @@
         if kwargs["dashboard_mode"] not in ("demo", "none") and not os.path.exists(
             kwargs["password_file"]
         ):
             click.echo(
                 'You have not set a dashboard password. Run "%s set_password" to do so.'
                 % PY4WEB_CMD
             )
-        elif "_dashboard" in Reloader.ROUTES:
+        elif "_dashboard" in Reloader.ROUTES and (
+            not kwargs["host"].startswith("unix:/")
+        ):
             click.echo(
                 f"Dashboard is at: http{'s' if kwargs.get('ssl_cert', None) else ''}://{kwargs['host']}:{kwargs['port']}/_dashboard"
             )
 
     start_server(kwargs)
```

### Comparing `py4web-1.20231115.1/py4web/server_adapters.py` & `py4web-1.20240420.1/py4web/server_adapters.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "wsgirefThreadingServer",
     "wsgiTh",  # short_name
     "rocketServer",
 ] + wsservers_list
 
 # ---------------------- utils -----------------------------------------------
 
+
 # export PY4WEB_LOGS=/tmp # export PY4WEB_LOGS=
 def get_log_file(out_banner=True):
     log_dir = os.environ.get("PY4WEB_LOGS", None)
     if log_dir and os.path.isdir(log_dir):
         log_file = os.path.join(log_dir, "server-py4web.log")
         if out_banner:
             print(f"log_file: {log_file}")
@@ -83,21 +84,25 @@
     # long_msg = short_msg + " > %(funcName)s > %(filename)s:%(lineno)d > %(levelname)s"
 
     time_msg = "%H:%M:%S"
     # date_time_msg = '%Y-%m-%d %H:%M:%S'
 
     try:
         logging.basicConfig(
-            format=short_msg, datefmt=time_msg, level=check_level(level), **log_to,
+            format=short_msg,
+            datefmt=time_msg,
+            level=check_level(level),
+            **log_to,
         )
     except (OSError, LookupError, KeyError, ValueError) as ex:
         print(f"{ex}, {__file__}")
         print(f"cannot open {log_file}")
         logging.basicConfig(
-            format="%(message)s", level=check_level(level),
+            format="%(message)s",
+            level=check_level(level),
         )
 
     if logger_name is None:
         return None
 
     log = logging.getLogger("SA:" + logger_name)
     log.propagate = True
@@ -118,37 +123,97 @@
 def get_workers(opts, default=10):
     try:
         return opts["workers"] if opts["workers"] else default
     except KeyError:
         return default
 
 
+def check_port(host="127.0.0.1", port=8000):
+    import socket
+    import errno
+    import subprocess
+
+    def os_cmd(run_cmd):
+        try:
+            subprocess.run(
+                run_cmd,
+                shell=True,
+                check=True,
+                text=True,
+            )
+        except subprocess.CalledProcessError:
+            pass
+
+    if host.startswith("unix:/"):
+        socket_path = host[5:]
+        if os.path.exists(socket_path):
+            if port == 0:
+                os_cmd(f"ls -alFi {socket_path}")
+                sys.exit(f"can't run gunicorn: {socket_path} exists")
+            elif port == 1:
+                os_cmd("ps -ef | head -1; ps -ef | grep py4web | grep -v grep")
+                os_cmd(f"ls -alFi {socket_path}")
+                os_cmd(f"lsof -w {socket_path}")
+            elif port == 8000:
+                pass
+        print(f"gunicorn listening at: {host}")
+        return
+
+    s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    try:
+        s.bind((host, int(port)))
+    except socket.error as e:
+        if e.errno == errno.EADDRINUSE:
+            os_cmd(
+                f"command -v lsof >/dev/null 2>&1 && ps -ef | head -1; ps -ef |"
+                f" grep py4web | grep -v grep && lsof -nPi:{port}"
+            )
+            sys.exit(f"{host}:{port} is already in use")
+        else:
+            sys.exit(f"{e}\n{host}:{port} cannot be acessed")
+    s.close()
+
+
 # ---------------------- servers -----------------------------------------------
 
+
 def gunicorn():
-    from gevent import local  # pip install gevent gunicorn
+    from gevent import local  # pip install gevent gunicorn setproctitle
     import threading
 
     if isinstance(threading.local(), local.local):
         print("gunicorn: monkey.patch_all() applied")
 
     class GunicornServer(ServerAdapter):
-        def run(self, py4web_apps_handler):
-            from gunicorn.app.base import Application
-            import re
+        def run(self, app_handler):
+            try:
+                from gunicorn.app.base import Application
+            except ImportError as ex:
+                sys.exit(f"{ex}\nTry: pip install gunicorn gevent setproctitle")
+
+            from ast import literal_eval
+
+            check_port(self.host, self.port)
 
             logger = None
 
+            sa_bind = (
+                self.host
+                if self.host.startswith("unix:/")
+                else f"{self.host}:{self.port}"
+            )
+
             sa_config = {
-                "bind": f"{self.host}:{self.port}",
+                "bind": sa_bind,  # f"{self.host}:{self.port}",
                 "workers": get_workers(self.options),
                 "certfile": self.options.get("certfile", None),
                 "keyfile": self.options.get("keyfile", None),
                 "accesslog": None,
                 "errorlog": None,
+                "proc_name": "sa_py4web",  # ps a | grep py4web
                 "config": "sa_config",
                 # ( 'sa_config',  'GUNICORN_', 'gunicorn.saenv', 'gunicorn.conf.py' )
             }
 
             if not self.quiet:
                 level = check_level(self.options["logging_level"])
                 log_file = get_log_file(out_banner=False)
@@ -162,36 +227,41 @@
                         "access_log_format": '%(h)s %(l)s %(u)s %(t)s "%(r)s" %(s)s %(b)s "%(f)s" "%(a)s"',
                         "accesslog": log_to,
                         "errorlog": log_to,
                     }
                 )
 
             class GunicornApplication(Application):
-                def logger_info(self, msg="its logger_info"):
-                    logger and logger.info(str(msg))
-
                 def get_gunicorn_options(
                     self,
-                    default="gunicorn.conf.py",
+                    gu_default="gunicorn.conf.py",
                     env_file="gunicorn.saenv",
                     env_key="GUNICORN_",
                 ):
                     def check_kv(kx, vx):
-                        if kx and vx and ( kx not in ( "bind", "config",) ) :
+                        if (
+                            kx
+                            and vx
+                            and (
+                                kx
+                                not in (
+                                    "bind",
+                                    "config",
+                                )
+                            )
+                        ):
                             if vx.startswith("{") and vx.endswith("}"):
-                                vt = re.sub( r'\,\s*\}', "}", vx)
-                                vx = json.loads(vt.replace("'", '"'))
+                                vx = literal_eval(vx)
                             if vx == "None":
                                 vx = None
                             return kx, vx
-                        self.logger_info(f"gunicorn: Ignored {kx}={vx}")
                         return None, None
 
-                    if os.path.isfile(default):
-                        return {"use_python_config": default, "config": default}
+                    if os.path.isfile(gu_default):
+                        return {"use_python_config": gu_default, "config": gu_default}
 
                     res_opts = dict()
 
                     if os.path.isfile(env_file):
                         try:
                             with open(env_file, "r") as f:
                                 lines = f.read().splitlines()
@@ -207,52 +277,54 @@
                                         k, v = k.strip().lower(), v.strip()
                                     except (ValueError, AttributeError):
                                         continue
                                     k, v = check_kv(k, v)
                                     if k is None:
                                         continue
                                     res_opts[k] = v
+
                                 if res_opts:
                                     res_opts["config"] = env_file
                                     return res_opts
-                        except (IOError, OSError):
-                            self.logger_info(f"gunicorn: Bad {env_file}")
+
+                        except (IOError, OSError) as ex:
+                            sys.exit(f"{ex}\nError: {env_file}")
 
                     for k, v in os.environ.items():
                         if k.startswith(env_key):
                             k = k.split("_", 1)[1].lower()
                             k, v = check_kv(k, v)
                             if k is None:
                                 continue
                             res_opts[k] = v
 
                     if res_opts:
                         res_opts["config"] = env_key
+
                     return res_opts
 
                 def load_config(self):
                     sa_config.update(self.get_gunicorn_options())
+                    logger and logger.debug(sa_config)
 
                     for k, v in sa_config.items():
                         if k not in self.cfg.settings:
                             continue
                         self.cfg.set(k, v)
 
-                    if "print_config" in sa_config:
-                        if sa_config["print_config"] == "True":
-                            self.logger_info(sa_config)
-                            self.logger_info(self.cfg)
-
-                    for e in ( "use_python_config", "usepy", ):
+                    for e in (
+                        "use_python_config",
+                        "usepy",
+                    ):
                         if e in sa_config:
-                            Application.load_config_from_file(self, sa_config [ e ]  )
+                            Application.load_config_from_file(self, sa_config[e])
                             break
 
                 def load(self):
-                    return py4web_apps_handler
+                    return app_handler
 
             GunicornApplication().run()
 
     return GunicornServer
 
 
 gunicornGevent = gunicorn
@@ -275,15 +347,18 @@
     # ./py4web.py run apps -s gevent --watch=off --host=192.168.1.161 --port=8443 --ssl_cert=server.pem -L 0
 
     class GeventServer(ServerAdapter):
         def run(self, app_handler):
             logger = None  # "default"
 
             if not self.quiet:
-                logger = logging_conf(self.options["logging_level"], "gevent",)
+                logger = logging_conf(
+                    self.options["logging_level"],
+                    "gevent",
+                )
                 # logger.addHandler(logging.StreamHandler())
 
             certfile = self.options.get("certfile", None)
 
             ssl_args = (
                 dict(
                     certfile=certfile,
@@ -327,20 +402,26 @@
     #   -sSv  https://192.168.1.161:9000/
 
     class GeventWebSocketServer(ServerAdapter):
         def run(self, app_handler):
             logger = None  # "default"
 
             if not self.quiet:
-                logger = logging_conf(self.options["logging_level"], "gevent-ws",)
+                logger = logging_conf(
+                    self.options["logging_level"],
+                    "gevent-ws",
+                )
 
             certfile = self.options.get("certfile", None)
 
             ssl_args = (
-                dict(certfile=certfile, keyfile=self.options.get("keyfile", None),)
+                dict(
+                    certfile=certfile,
+                    keyfile=self.options.get("keyfile", None),
+                )
                 if certfile
                 else dict()
             )
 
             server = pywsgi.WSGIServer(
                 (self.host, self.port),
                 app_handler,
@@ -368,15 +449,18 @@
 
     class WSGIRefThreadingServer(ServerAdapter):
         def run(self, app_handler):
 
             self.log = None
 
             if not self.quiet:
-                self.log = logging_conf(self.options["logging_level"], "wsgiref",)
+                self.log = logging_conf(
+                    self.options["logging_level"],
+                    "wsgiref",
+                )
 
             self_run = self  # used in internal classes to access options and logger
 
             class PoolMixIn(ThreadingMixIn):
                 def process_request(self, request, client_address):
                     self.pool.submit(
                         self.process_request_thread, request, client_address
@@ -476,15 +560,17 @@
         from .rocket3 import Rocket3 as Rocket
 
     class RocketServer(ServerAdapter):
         def run(self, app_handler):
 
             if not self.quiet:
 
-                logging_conf(self.options["logging_level"],)
+                logging_conf(
+                    self.options["logging_level"],
+                )
 
             interface = (
                 (
                     self.host,
                     self.port,
                     self.options["keyfile"],
                     self.options["certfile"],
```

### Comparing `py4web-1.20231115.1/py4web/utils/auth.py` & `py4web-1.20240420.1/py4web/utils/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 import calendar
 import copy
 import datetime
 import hashlib
 import random
 import re
 import time
-import urllib
 import uuid
 
 from pydal.validators import (
     CRYPT,
     IS_EMAIL,
     IS_EQUAL_TO,
     IS_MATCH,
     IS_NOT_EMPTY,
     IS_NOT_IN_DB,
     IS_STRONG,
 )
 from yatl.helpers import DIV, A
 
 from py4web import HTTP, URL, Field, action, redirect, request, response
-from py4web.core import REGEX_APPJSON, Fixture, Flash, Template, Translator
+from py4web.core import REGEX_APPJSON, Fixture, Flash, Translator
 from py4web.utils.form import Form, FormStyleDefault
 from py4web.utils.param import Param
 
 """
 [X] Enable and disable plugins
 [X] Enable and disable actions
 [X] Require passwords of various complexity
@@ -243,17 +242,19 @@
     ):
         # configuration parameters
         self.param = Param(
             registration_requires_confirmation=registration_requires_confirmation,
             registration_requires_approval=registration_requires_approval,
             login_after_registration=False,
             login_expiration_time=login_expiration_time,  # seconds
-            password_complexity={"entropy": 50}
-            if password_complexity == "default"
-            else password_complexity,
+            password_complexity=(
+                {"entropy": 50}
+                if password_complexity == "default"
+                else password_complexity
+            ),
             block_previous_password_num=block_previous_password_num,
             allowed_actions=allowed_actions or ["all"],
             use_appname_in_redirects=use_appname_in_redirects,
             formstyle=FormStyleDefault,
             messages=copy.deepcopy(self.MESSAGES),
             button_classes=copy.deepcopy(self.BUTTON_CLASSES),
             default_login_enabled=True,
@@ -511,15 +512,15 @@
                 }
         return user
 
     @property
     def is_logged_in(self):
         if not self.session.is_valid():
             return False
-        return self.session.get("user", {}).get("id", None) != None
+        return self.session.get("user", {}).get("id", None) is not None
 
     @property
     def user_id(self):
         if not self.session.is_valid():
             return None
         user = self.session.get("user")
         if not user:
@@ -544,15 +545,15 @@
         self.session.clear()
         self.store_user_in_session(impersonated_id)
         self.session["user"]["impersonator_id"] = user["id"]
         redirect(next_url)
 
     def is_impersonating(self):
         """checks if we are impersonating a user"""
-        return self.session.get("user", {}).get("impersonator_id", None) != None
+        return self.session.get("user", {}).get("impersonator_id", None) is not None
 
     def stop_impersonating(self, next_url):
         """stops impersonating a user, assuming we are impersonating one"""
         user = self.session.get("user")
         impersonator_id = (user or {}).get("impersonator_id")
         if impersonator_id is None:
             raise RuntimeError(
@@ -633,15 +634,15 @@
             if not hasattr(plugin, "get_login_url"):
                 prevent_db_lookup = True
                 if plugin.check_credentials(email, password):
                     # if the creadentials are independently validated
                     # get of create the user (if does not exist)
                     user_info = {}
                     user_info["sso_id"] = plugin.name + ":" + email
-                    if self.use_username or not "@" in email:
+                    if self.use_username or "@" not in email:
                         user_info["username"] = email
                     if "@" in email:
                         user_info["email"] = email
                     else:
                         user_info["email"] = email + "@example.com"
                     user = self.get_or_register_user(user_info)
                     break
@@ -851,40 +852,44 @@
         ):
             row.delete_record()
             return None
         return row
 
     def get_or_register_user(self, user):
         db = self.db
-        # if the we have an email for the user
-        if "email" in user:
-            # return a user if exists and has a verified email
-            row = self.get_or_delete_existing_unverified_account(user["email"])
-        # else retrieve the user from the sso_id
-        else:
+        # if we have an sso_id we use it to id the user
+        if user.get("sso_id"):
+            keyid = "sso_id"
             row = (
                 db(db.auth_user.sso_id == user["sso_id"]).select(limitby=(0, 1)).first()
             )
-        # if we have found a candidate user
-        if row:
-            # we expect the email to match if provided
-            if "email" in user and row.email != user["email"]:
-                return None
-            # we can update all the other information provided by the SSO
-            if any(user[key] != row[key] for key in user if not key == "username"):
+            # the sso source is always more authoritative so update the record
+            if row:
                 row.update_record(**user)
-            user["id"] = row["id"]
-        # if we do not have a candidate user we need to create one
+                # pass the full user
+                user = row.as_dict()
+        # othrewise we id the user via email
+        elif user.get("email"):
+            keyid = "email"
+            # return a user if exists and has a verified email
+            row = self.get_or_delete_existing_unverified_account(user["email"])
+            # the database is more authoritative
+            if row:
+                user.update(**row.as_dict())
         else:
-            # we expect an email to be able to create account
-            if not "email" in user:
-                return None
-            # if we expect a username but not provided, user email as username
-            if self.use_username and "username" not in user:
-                user["username"] = user["email"]
+            return None
+        # if we do not have a candidate user we create one
+        if not row:
+            # if we expect a username but not provided, use keyid as username
+            if self.use_username:
+                if "username" not in user:
+                    user["username"] = user[keyid]
+                    # make sure the username is unique
+                    if db(db.auth_user.username == user["username"]).count():
+                        raise HTTP(401, body=f"Conficting {user['username']} accounts")
             # create the user
             user["id"] = db.auth_user.insert(**db.auth_user._filter_fields(user))
         return user
 
     # Private methods
 
     def _query_from_token(self, token):
@@ -1080,15 +1085,15 @@
 
 
 def api_wrapper(func):
     """Validates API calls"""
 
     def func_wrapper(auth, func=func):
         data = func(auth) or {}
-        if not "status" in data and data.get("errors"):
+        if "status" not in data and data.get("errors"):
             data.update(status="error", message="validation errors", code=401)
         elif "errors" in data and not data["errors"]:
             del data["errors"]
         data["status"] = data.get("status", "success")
         response.status = data["code"] = data.get("code", 200)
         return data
 
@@ -1165,17 +1170,19 @@
                             name=field.name,
                             type=field.type,
                             label=field.label,
                             readable=field.readable,
                             writable=field.writable if field.type != "id" else False,
                             required=field.required,
                             regex=field.regex if hasattr(field, "regex") else None,
-                            default=field.default()
-                            if callable(field.default)
-                            else field.default,
+                            default=(
+                                field.default()
+                                if callable(field.default)
+                                else field.default
+                            ),
                             options=field.options,
                         )
                     )
 
                 model[key] = formatted_fields
                 break
 
@@ -1555,17 +1562,19 @@
             if model:
                 return top_buttons["buttons"]
             return top_buttons["combined_div"]
 
         fields = [
             Field(
                 "email",
-                label=self.auth.db.auth_user.username.label
-                if self.auth.use_username
-                else self.auth.db.auth_user.email.label,
+                label=(
+                    self.auth.db.auth_user.username.label
+                    if self.auth.use_username
+                    else self.auth.db.auth_user.email.label
+                ),
             ),
             Field(
                 "password",
                 type="password",
                 label=self.auth.param.messages["labels"].get("password"),
             ),
         ]
```

### Comparing `py4web-1.20231115.1/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20240420.1/py4web/utils/auth_plugins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,28 +60,36 @@
             else:
                 code = error.get("code", 401)
                 msg = error.get("message", "Unknown error")
             raise HTTP(code, msg)
         if auth.db:
             # map returned fields into auth_user fields
             user = {}
-            for key, value in self.maps.items():
-                value, parts = data, value.split(".")
+            for key, orig_key in self.maps.items():
+                value = data
+                parts = orig_key.split(".")
                 for part in parts:
-                    value = value[int(part) if part.isdigit() else part]
+                    try:
+                        value = value[int(part) if part.isdigit() else part]
+                    except Exception:
+                        break
+                else:
                     user[key] = value
             user["sso_id"] = "%s:%s" % (self.name, user["sso_id"])
-            if not "username" in user:
+            if "username" not in user:
                 user["username"] = user["sso_id"]
             # store or retrieve the user
             data = auth.get_or_register_user(user)
+            user_id = data["id"]
         else:
             # WIP Allow login without DB
-            if not "id" in data:
-                data["id"] = data.get("username") or data.get("email")
+            if "id" not in data:
+                data["id"] = (
+                    data.get("sso_id") or data.get("username") or data.get("email")
+                )
         user_id = data.get("id")
         auth.store_user_in_session(user_id)
         if "_next" in auth.session:
             next = auth.session.get("_next")
             del auth.session["_next"]
         else:
             next = URL("index")
```

### Comparing `py4web-1.20231115.1/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20240420.1/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     name = "basic"
     label = "Basic"
 
     def __init__(self, server="127.0.0.1", table=None):
         self.server = server
 
     def check_credentials(self, username, password):
-
         """
         to use basic login with a different server
         from gluon.contrib.login_methods.basic_auth import basic_auth
         auth.settings.login_methods.append(basic_auth('http://server'))
         """
         key = base64.b64encode(username + ":" + password)
         headers = {"Authorization": "Basic " + key}
```

### Comparing `py4web-1.20231115.1/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20240420.1/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,16 @@
             server.ehlo()
             if tls_mode:
                 server.starttls()
                 server.ehlo()
             server.login(email, password)
             server.quit()
             return True
-        except:
+        except Exception:
             logging.exception("email_auth() failed")
             if server:
                 try:
                     server.quit()
-                except:  # server might already close connection after error
+                except Exception:
+                    # server might already close connection after error
                     pass
             return False
```

### Comparing `py4web-1.20231115.1/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20240420.1/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,15 +421,15 @@
                         result = con.search_s(basedn, ldap.SCOPE_SUBTREE, filter)
                         if result:
                             user_dn = result[0][0]
                             # Check the password
                             con.simple_bind_s(user_dn, password)
                             found = True
                             break
-                    except ldap.LDAPError as detail:
+                    except ldap.LDAPError:
                         (exc_type, exc_value) = sys.exc_info()[:2]
                         logger.warning(
                             "ldap_auth: searching %s for %s resulted in %s: %s\n"
                             % (basedn, filter, exc_type, exc_value)
                         )
                 if not found:
                     logger.warning("User [%s] not found!" % username)
@@ -459,15 +459,15 @@
                         result = con.search_s(basedn, scope, filter)
                         if result:
                             user_dn = result[0][0]
                             # Check the password
                             con.simple_bind_s(user_dn, password)
                             found = True
                             break
-                    except ldap.LDAPError as detail:
+                    except ldap.LDAPError:
                         (exc_type, exc_value) = sys.exc_info()[:2]
                         logger.warning(
                             "ldap_auth: searching %s for %s resulted in %s: %s\n"
                             % (basedn, filter, exc_type, exc_value)
                         )
                 if not found:
                     logger.warning("User [%s] not found!" % username)
@@ -480,29 +480,29 @@
                     user_firstname = result[user_firstname_attrib][0]
                     if user_firstname_part is not None:
                         store_user_firstname = user_firstname.split(
                             b" " if isinstance(user_firstname, bytes) else " ", 1
                         )[user_firstname_part]
                     else:
                         store_user_firstname = user_firstname
-                except KeyError as e:
+                except KeyError:
                     store_user_firstname = None
                 try:
                     user_lastname = result[user_lastname_attrib][0]
                     if user_lastname_part is not None:
                         store_user_lastname = user_lastname.split(
                             b" " if isinstance(user_lastname, bytes) else " ", 1
                         )[user_lastname_part]
                     else:
                         store_user_lastname = user_lastname
-                except KeyError as e:
+                except KeyError:
                     store_user_lastname = None
                 try:
                     store_user_mail = result[user_mail_attrib][0]
-                except KeyError as e:
+                except KeyError:
                     store_user_mail = None
                 update_or_insert_values = {
                     "first_name": store_user_firstname,
                     "last_name": store_user_lastname,
                     "email": store_user_mail,
                     "username": username,
                     "sso_id": store_sso_id,
@@ -536,24 +536,24 @@
 
                 if manage_groups:
                     if not self.do_manage_groups(con, username, group_mapping):
                         return False
 
             con.unbind()
             return True
-        except ldap.INVALID_CREDENTIALS as e:
+        except ldap.INVALID_CREDENTIALS:
             return False
-        except ldap.LDAPError as e:
+        except ldap.LDAPError:
             import traceback
 
             logger.warning("[%s] Error in ldap processing" % str(username))
             logger.debug(traceback.format_exc())
             print(traceback.format_exc())
             return False
-        except IndexError as ex:  # for AD membership test
+        except IndexError:  # for AD membership test
             import traceback
 
             logger.warning("[%s] Ldap result indexing error" % str(username))
             logger.debug(traceback.format_exc())
             return False
 
     def is_user_in_allowed_groups(self, username, password=None):
@@ -679,24 +679,24 @@
                 try:
                     db_user_id = (
                         db(db.auth_user.email == username)
                         .select(db.auth_user.id)
                         .first()
                         .id
                     )
-                except AttributeError as e:
+                except AttributeError:
                     #
                     # There is no user in local db
                     # We create one
                     # ##############################
                     try:
                         db_user_id = db.auth_user.insert(
                             username=username, first_name=username
                         )
-                    except AttributeError as e:
+                    except AttributeError:
                         db_user_id = db.auth_user.insert(
                             email=username, first_name=username
                         )
             if not db_user_id:
                 logger.error("There is no username or email for %s!" % username)
                 raise
             db_groups_of_the_user = groups.get(db_user_id)
```

### Comparing `py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from . import OAuth2
+import requests
 
 
 class OAuth2Facebook(OAuth2):
     name = "oauth2facebook"
     label = "Facebook"
 
     login_url = "https://www.facebook.com/v3.3/dialog/oauth"
```

### Comparing `py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2google_scoped.py` & `py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2google_scoped.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,51 +13,70 @@
 
 import google.oauth2.credentials
 import google_auth_oauthlib.flow
 from google.auth.exceptions import RefreshError
 from googleapiclient.discovery import build
 from pydal import Field
 
-from py4web import HTTP, URL, redirect, request
+from py4web import HTTP, URL, redirect, request, response
 from py4web.utils.auth import REGEX_APPJSON, AuthEnforcer
 
 
 class AuthEnforcerGoogleScoped(AuthEnforcer):
     """This class catches certain invalid access errors Google generates
     when credentials get stale, and forces the user to login again.
     Pass it to Auth as param.auth_enfoercer, as in:
-    auth.param.auth_enforcer = AuthEnforcerGoogleScoped(auth)
+    auth.param.auth_enforcer = MyAuthEnforcerGoogleScoped(auth, db)
     """
 
-    def __init__(self, auth, condition=None, error_page=None):
+    def __init__(self, auth, db, condition=None, error_page=None):
         super().__init__(auth, condition=condition)
+        self.db = db
         self.error_page = error_page
         assert (
             error_page is not None
         ), "You need to specify an error page; can't use login."
 
     def on_error(self, context):
         if isinstance(context.get("exception"), RefreshError):
             del context["exception"]
-            self.auth.session.clear()
-            if re.search(REGEX_APPJSON, request.headers.get("accept", "")) and (
-                request.headers.get("json-redirects", "") != "on"
-            ):
-                raise HTTP(403)
-            redirect_next = request.fullpath
-            if request.query_string:
-                redirect_next = redirect_next + "?{}".format(request.query_string)
-            self.auth.flash.set("Invalid credentials")
-            redirect(
-                URL(
-                    self.error_page,
-                    vars=dict(next=redirect_next),
-                    use_appname=self.auth.param.use_appname_in_redirects,
-                )
+            self._handle_error()
+
+    def _handle_error(self):
+        # Removes this Google cookie, trying to enforce loggin in again.
+        response.delete_cookie("G_ENABLED_IDPS")
+        self.auth.session.clear()
+        if re.search(REGEX_APPJSON, request.headers.get("accept", "")) and (
+            request.headers.get("json-redirects", "") != "on"
+        ):
+            raise HTTP(403)
+        redirect_next = request.fullpath
+        if request.query_string:
+            redirect_next = redirect_next + "?{}".format(request.query_string)
+        self.auth.flash.set("Invalid credentials")
+        redirect(
+            URL(
+                self.error_page,
+                vars=dict(next=redirect_next),
+                use_appname=self.auth.param.use_appname_in_redirects,
             )
+        )
+
+    def on_request(self, context):
+        super().on_request(context)
+        user = self.auth.session.get("user")
+        user_info = (
+            self.db(self.db.auth_credentials.email == user["email"]).select().first()
+        )
+        if not user_info:
+            self._handle_error()
+        credentials_dict = json.loads(user_info.credentials)
+        if not credentials_dict.get("refresh_token"):
+            print("Missing credentials:", user["email"], credentials_dict)
+            self._handle_error()
 
 
 class OAuth2GoogleScoped(object):
     """Class that enables google login via oauth2 with additional scopes.
     The authorization info is saved so the scopes can be used later on.
 
     NOTE: if you use this plugin, it is also recommended that you set:
@@ -193,15 +212,15 @@
         if error:
             if isinstance(error, str):
                 code, msg = 401, error
             else:
                 code = error.get("code", 401)
                 msg = error.get("message", "Unknown error")
             raise HTTP(code, msg)
-        if not "code" in get_vars:
+        if "code" not in get_vars:
             raise HTTP(401, "Missing code parameter in response.")
         code = get_vars.get("code")
         flow.fetch_token(code=code)
         # We got the credentials!
         credentials = flow.credentials
         # Now we must use the credentials to check the user identity.
         # see https://github.com/googleapis/google-api-python-client/pull/1088/files
@@ -232,15 +251,15 @@
                 "last_name": user_info.get("family_name"),
             }
             data = auth.get_or_register_user(user)
             user["id"] = data.get("id")
         else:
             # WIP Allow login without DB
             user = dict(user_info)
-            if not "id" in user:
+            if "id" not in user:
                 user["id"] = user.get("username") or user.get("email")
         # Stores the user in the session.  We do it here, so we store
         # the complete details, and not just the user_id.
         auth.session["user"] = user
         auth.session["recent_activity"] = calendar.timegm(time.gmtime())
         auth.session["uuid"] = str(uuid.uuid1())
         # Finally, redirects to next.
```

### Comparing `py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import hashlib
 import uuid
 
 import jwt
 
-from py4web.core import DAL, HTTP, Field, request
+from py4web.core import HTTP, Field, request
 
 
 class OAuthServer(object):
 
     algorithms = ["HS256", "RS256"]
 
     def __init__(self, auth, secret):
```

### Comparing `py4web-1.20231115.1/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20240420.1/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     # token_url = "https://.../wp-json/moserver/token"
     # userinfo_url = "https://.../wp-json/moserver/resource"
 
     default_scope = "profile openid"
     default_maps = {
         # "email": "email",
         "sso_id": "ID",
-        "username": "username"
+        "username": "username",
         # "first_name": "firstname",
         # "last_name": "lastname",
     }
 
     def __init__(
         self,
         client_id,
@@ -107,30 +107,30 @@
             # not unique
 
             sso_id = user["sso_id"]
             user["sso_id"] = "%s:%s" % (
                 self.name,
                 sso_id,
             )
-            if not "username" in user:
+            if "username" not in user:
                 user["username"] = "%s:%s" % (
                     self.name,
                     sso_id,
                 )
             else:
                 user["username"] = "%s:%s" % (
                     self.name,
                     user["username"],
                 )
             # store or retrieve the user
             data = auth.get_or_register_user(user)
 
         else:
             # WIP Allow login without DB
-            if not "id" in data:
+            if "id" not in data:
                 data["id"] = data.get("username") or data.get("email")
         user_id = data.get("id")
         auth.store_user_in_session(user_id)
         redirect(URL("index"))
 
     # -# This method is an exact copy of the one from original class
     # without this subsequent error is raised from the jwt library (don't know why)
```

### Comparing `py4web-1.20231115.1/py4web/utils/auth_plugins/pam.py` & `py4web-1.20240420.1/py4web/utils/auth_plugins/pam.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,28 @@
 Provides an authenticate function that will allow the caller to authenticate
 a user against the Pluggable Authentication Modules (PAM) on the system.
 Implemented using ctypes, so no compilation is necessary.
 """
 __all__ = ["authenticate"]
 
 import sys
-from ctypes import (CDLL, CFUNCTYPE, POINTER, Structure, byref, c_char,
-                    c_char_p, c_int, c_uint, c_void_p, cast, sizeof)
+from ctypes import (
+    CDLL,
+    CFUNCTYPE,
+    POINTER,
+    Structure,
+    byref,
+    c_char,
+    c_char_p,
+    c_int,
+    c_uint,
+    c_void_p,
+    cast,
+    sizeof,
+)
 from ctypes.util import find_library
 
 libpam = CDLL(find_library("pam"))
 libc = CDLL(find_library("c"))
 
 calloc = libc.calloc
 calloc.restype = c_void_p
```

### Comparing `py4web-1.20231115.1/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20240420.1/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 
 """
 THIS FILE IS A WORK IN PROGRESS AND PROBALY DOES NOT WORK
 """
 
 from saml2 import BINDING_HTTP_POST, BINDING_HTTP_REDIRECT
 from saml2.client import Saml2Client
-from saml2.config import Config as Saml2Config
 
 
 def obj2dict(obj, processed=None):
     """
     converts any object into a dict, recursively
     """
-    processed = processed if not processed is None else set()
+    processed = processed if processed is not None else set()
     if obj is None:
         return None
     if isinstance(obj, (int, long, str, unicode, float, bool)):
         return obj
     if id(obj) in processed:
         return "<reference>"
     processed.add(id(obj))
@@ -28,16 +27,16 @@
         obj = obj.__dict__
     else:
         return repr(obj)
     return dict(
         (key, obj2dict(value, processed))
         for key, value in obj.items()
         if not key.startswith("_")
-        and not type(value)
-        in (
+        and type(value)
+        not in (
             types.FunctionType,
             types.LambdaType,
             types.BuiltinFunctionType,
             types.BuiltinMethodType,
         )
     )
 
@@ -75,15 +74,15 @@
         unquoted_response = request.vars.SAMLResponse
         res = {}
         try:
             data = client.parse_authn_request_response(
                 unquoted_response, binding, session.saml_outstanding_queries
             )
             res["response"] = data if data else {}
-        except Exception as e:
+        except Exception:
             import traceback
 
             res["error"] = traceback.format_exc()
         return res
 
 
 class Saml2Plugin:
```

### Comparing `py4web-1.20231115.1/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20240420.1/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 Ported from web2py - Work in Pogress
 """
 
 from functools import reduce
 
 from gluon.globals import current
-from gluon.http import HTTP, redirect
 from gluon.storage import Storage
+
 # requires M2Crypto
 from M2Crypto import X509
 
 
 class x509Plugin:
 
     name = "x509"
```

### Comparing `py4web-1.20231115.1/py4web/utils/cors.py` & `py4web-1.20240420.1/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/py4web/utils/dbstore.py` & `py4web-1.20240420.1/py4web/utils/dbstore.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class DBStore:
     def __init__(self, db, name="py4web_session"):
         self.__prerequisites__ = [db]
         Field = db.Field
         self.db = db
-        if not name in db.tables:
+        if name not in db.tables:
             db.define_table(
                 name,
                 Field("rkey", "string"),
                 Field("rvalue", "text"),
                 Field("expiration", "integer"),
                 Field("created_on", "datetime"),
                 Field("expires_on", "datetime"),
```

### Comparing `py4web-1.20231115.1/py4web/utils/downloader.py` & `py4web-1.20240420.1/py4web/utils/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import os
 import re
 import shutil
-import urllib
 
 from pydal.exceptions import NotAuthorizedException, NotFoundException
 from pydal.helpers.regex import REGEX_UPLOAD_PATTERN
 
 from py4web import HTTP, request
 from py4web.core import bottle
 
 
 def downloader(db, path, filename, download_filename=None):
-
     """
     Given a db, and filesystem path, and the filename of an uploaded file,
     it retrieves the file, checks permission, and returns or stream its.
     Optionally as an attachment if the URL contains attachment=true
     If the file is not in the filesystem, it gets copied into the path folder
     before being returned for speed.
```

### Comparing `py4web-1.20231115.1/py4web/utils/factories.py` & `py4web-1.20240420.1/py4web/utils/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import copy
 import json
-import os
-from functools import wraps
 
 import jwt
 from yatl.helpers import TAG
 
 from py4web import URL, action, request
-from py4web.core import Fixture, Session, dumps
+from py4web.core import Fixture, Session
 
 
 class Inject(Fixture):
     def __init__(self, **variables):
         self.variables = variables
 
     def on_success(self, context):
```

### Comparing `py4web-1.20231115.1/py4web/utils/form.py` & `py4web-1.20240420.1/py4web/utils/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,28 @@
 import os
 import time
 import uuid
 
 import jwt
 from pydal._compat import to_native
 from pydal.objects import FieldVirtual
-from pydal.validators import Validator
-from yatl.helpers import (CAT, DIV, FORM, INPUT, LABEL, OPTION, SELECT, SPAN,
-                          TABLE, TD, TEXTAREA, TR, XML, A, P)
+from yatl.helpers import (
+    CAT,
+    DIV,
+    FORM,
+    INPUT,
+    LABEL,
+    OPTION,
+    SELECT,
+    SPAN,
+    TEXTAREA,
+    XML,
+    A,
+    P,
+)
 
 from py4web import HTTP, request, response
 from py4web.utils.param import Param
 
 
 def to_id(field):
     """get an identified for a field"""
@@ -50,15 +61,14 @@
     classes = set(
         cls.strip() for classlist in lists for cls in classlist if cls.strip()
     )
     return " ".join(sorted(classes))
 
 
 class Widget:
-
     """Prototype widget object for all form widgets"""
 
     type_map = {
         "string": "text",
         "date": "date",
         "time": "time",
     }
@@ -112,15 +122,15 @@
         return INPUT(
             _type="checkbox",
             _id=to_id(field),
             _name=field.name,
             _value="ON",
             _checked=value,
             _readonly=readonly,
-            **attrs
+            **attrs,
         )
 
 
 class ListWidget:
     def make(self, field, value, error, title, placeholder="", readonly=False):
         if field.type == "list:string":
             _class = "type-list-string"
@@ -157,41 +167,41 @@
 
 class SelectWidget:
     def make(self, field, value, error, title, placeholder="", readonly=False):
         multiple = field.type.startswith("list:")
         value = list(map(str, value if isinstance(value, list) else [value]))
 
         field_options = [
-            [k, v, (not k is None and k in value)]
+            [k, v, (k is not None and k in value)]
             for k, v in get_options(field.requires)
         ]
         option_tags = [
             OPTION(v, _value=k, _selected=_selected)
             for (k, v, _selected) in field_options
         ]
 
         control = SELECT(
             *option_tags,
             _id=to_id(field),
             _name=field.name,
             _multiple=multiple,
             _title=title,
-            _readonly=readonly
+            _readonly=readonly,
         )
 
         return control
 
 
 class RadioWidget:
     def make(self, field, value, error, title, placeholder="", readonly=False):
         control = CAT()
         field_id = to_id(field)
         value = list(map(str, value if isinstance(value, list) else [value]))
         field_options = [
-            [k, v, (not k is None and k in value)]
+            [k, v, (k is not None and k in value)]
             for k, v in get_options(field.requires)
             if k != ""
         ]
         for k, v, selected in field_options:
             _id = "%s%s" % (field_id, k)
             control.append(
                 INPUT(
@@ -316,15 +326,15 @@
         json_controls = dict(
             form_fields=[],
             form_values=dict(),
             form_buttons=[],
             form_method=form_method,
             form_action=form_action,
             form_enctype=form_enctype,
-            **kwargs
+            **kwargs,
         )
 
         class_label = self.classes["label"]
         class_outer = self.classes["outer"]
         class_inner = self.classes["inner"]
         class_error = self.classes["error"]
         class_info = self.classes["info"]
@@ -369,19 +379,20 @@
                 continue
 
             # Reset the json control fields.
             field_attributes = dict()
             field_value = None
 
             field_name = field.name
-            field_type = field.type
             field_comment = field.comment if field.comment else ""
             field_label = field.label
             input_id = to_id(field)
-            default = field.default() if callable(field.default) else field.default
+            default = getattr(field, "default", None)
+            if callable(default):
+                default = default()
             value = vars.get(field.name, default) if not is_virtual else None
 
             error = errors.get(field.name)
             field_class = "type-" + field.type.split()[0].replace(":", "-")
             placeholder = (
                 field._placeholder if "_placeholder" in field.__dict__ else None
             )
@@ -399,15 +410,14 @@
                     )
                 # for all othe readonly fields we use represent or a string
                 else:
                     if is_virtual:
                         field_value = field.f(vars)
                     else:
                         field_value = compat_represent(field, value, vars)
-                    field_type = "represent"
                     control = DIV(field_value)
 
                 field_disabled = True
 
             # if we have a field.widget for the field use it but this logic is deprecated
             elif field.widget:
                 control = field.widget(table, vars)
@@ -462,22 +472,24 @@
             # Set the form controls.
             controls["labels"][field_name] = field_label
             controls["widgets"][field_name] = control
             controls["comments"][field_name] = field_comment
             controls["titles"][field_name] = title
             controls["placeholders"][field_name] = placeholder
 
+            field_type = str(field.type).replace(" ", "-")
+
             # Set the remain json field attributes.
             field_attributes["_title"] = title
             field_attributes["_label"] = field_label
             field_attributes["_comment"] = field_comment
             field_attributes["_id"] = to_id(field)
             field_attributes["_class"] = field_class
             field_attributes["_name"] = field.name
-            field_attributes["_type"] = field.type
+            field_attributes["_type"] = field_type
             field_attributes["_placeholder"] = placeholder
             field_attributes["_error"] = error
             field_attributes["_disabled"] = field_disabled
 
             # Add to the json controls.
             json_controls["form_fields"] += [field_attributes]
             json_controls["form_values"][field_name] = field_value
@@ -696,15 +708,15 @@
         validation=None,
         csrf_session=None,
         csrf_protection=True,
         lifespan=None,
         signing_info=None,
         submit_value="Submit",
         show_id=True,
-        **kwargs
+        **kwargs,
     ):
         self.param = Param(
             formstyle=formstyle,
             hidden=hidden,
             submit_value=submit_value,
             sidecar=[],
         )
@@ -817,18 +829,18 @@
                                 self.errors[field.name] = error
                     if self.errors:
                         for field_name in uploaded_fields:
                             validated_vars[field_name] = (
                                 self.record and self.record.get(field_name) or None
                             )
                     self.vars.update(validated_vars)
-                    if validation:
-                        validation(self)
                     if self.record and dbio:
                         self.vars["id"] = self.record.id
+                    if validation:
+                        validation(self)
                     if not self.errors:
                         for file in uploaded_files:
                             field, value = file
                             value = field.store(
                                 value.file, value.filename, field.uploadfolder
                             )
                             if value is not None:
@@ -889,15 +901,15 @@
         token = post_vars.get("_formkey")
         key = self._get_key()
         if not key:
             return False
         try:
             jwt.decode(token, key, algorithms=["HS256"])
             return True
-        except:
+        except Exception:
             return False
 
     def update_or_insert(self, validated_vars):
         if self.record:
             self.record.update_record(**validated_vars)
         else:
             # warning, should we really insert if record
```

### Comparing `py4web-1.20231115.1/py4web/utils/grid.py` & `py4web-1.20240420.1/py4web/utils/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,34 @@
 #
 #
 import base64
 import copy
 import datetime
 from urllib.parse import urlparse
 
-import ombott
 from pydal.objects import Expression, Field, FieldVirtual
-from yatl.helpers import (CAT, DIV, FORM, INPUT, OPTION, SELECT, SPAN, TABLE,
-                          TAG, TBODY, TD, TH, THEAD, TR, XML, A, I)
+from yatl.helpers import (
+    CAT,
+    DIV,
+    FORM,
+    INPUT,
+    OPTION,
+    SELECT,
+    SPAN,
+    TABLE,
+    TAG,
+    TBODY,
+    TD,
+    TH,
+    THEAD,
+    TR,
+    XML,
+    A,
+    I,
+)
 
 from py4web import HTTP, URL, redirect, request
 from py4web.utils.form import Form, FormStyleDefault, join_classes
 from py4web.utils.param import Param
 
 NAV = TAG.nav
 HEADER = TAG.header
@@ -39,15 +55,14 @@
 
 def clean_sc(**kwargs):
     """returns a clean dict with _class and _style only if value"""
     return {key: value for key, value in kwargs.items() if value}
 
 
 class GridClassStyle:
-
     """
     Default grid style
     Internal element names match default class name, other classes can be added
     Style use should be minimized since it cannot be overridden by CSS
     """
 
     classes = {
@@ -387,54 +402,54 @@
         """renders a row al position index (optional)"""
         return self.represent(row)
 
 
 class Grid:
 
     FORMATTERS_BY_TYPE = {
-        "boolean": lambda value: INPUT(
-            _type="checkbox", _checked=value, _disabled="disabled"
-        )
-        if value
-        else "",
-        "datetime": lambda value: XML(
-            "<script>document.write((new Date(%s,%s,%s,%s,%s,%s)).toLocaleString())</script>"
-            % (
-                value.year,
-                value.month - 1,
-                value.day,
-                value.hour,
-                value.minute,
-                value.second,
+        "boolean": lambda value: (
+            INPUT(_type="checkbox", _checked=value, _disabled="disabled")
+            if value
+            else ""
+        ),
+        "datetime": lambda value: (
+            XML(
+                "<script>document.write((new Date(%s,%s,%s,%s,%s,%s)).toLocaleString())</script>"
+                % (
+                    value.year,
+                    value.month - 1,
+                    value.day,
+                    value.hour,
+                    value.minute,
+                    value.second,
+                )
             )
-        )
-        if value and isinstance(value, datetime.datetime)
-        else value
-        if value
-        else "",
-        "time": lambda value: XML(
-            "<script>document.write((new Date(0, 0, 0,%s,%s,%s)).toLocaleString().split(', ')[1])</script>"
-            % (value.hour, value.minute, value.second)
-        )
-        if value and isinstance(value, datetime.time)
-        else value
-        if value
-        else "",
-        "date": lambda value: XML(
-            '<script>document.write((new Date(%s,%s,%s)).toLocaleString().split(",")[0])</script>'
-            % (
-                value.year,
-                value.month - 1,
-                value.day,
+            if value and isinstance(value, datetime.datetime)
+            else value if value else ""
+        ),
+        "time": lambda value: (
+            XML(
+                "<script>document.write((new Date(0, 0, 0,%s,%s,%s)).toLocaleString().split(', ')[1])</script>"
+                % (value.hour, value.minute, value.second)
+            )
+            if value and isinstance(value, datetime.time)
+            else value if value else ""
+        ),
+        "date": lambda value: (
+            XML(
+                '<script>document.write((new Date(%s,%s,%s)).toLocaleString().split(",")[0])</script>'
+                % (
+                    value.year,
+                    value.month - 1,
+                    value.day,
+                )
             )
-        )
-        if value and isinstance(value, datetime.date)
-        else value
-        if value
-        else "",
+            if value and isinstance(value, datetime.date)
+            else value if value else ""
+        ),
         "list:string": lambda value: ", ".join(str(x) for x in value) if value else "",
         "list:integer": lambda value: ", ".join(x for x in value) if value else "",
         "default": lambda value: str(value) if value is not None else "",
     }
 
     def __init__(
         self,
@@ -498,15 +513,15 @@
             redirect(
                 f"{fullpath}/select"
                 + (f"?{request.query_string}" if request.query_string else "")
             )
 
         # in case the query is a Table insteance
         if isinstance(query, query._db.Table):
-            query = query._id != None
+            query = query._id is not None
 
         self.path = path
         self.db = query._db
         self.T = T
         self.param = Param(
             query=query,
             columns=columns or fields,
@@ -604,15 +619,15 @@
         if not self.param.search_form and self.param.search_queries:
             search_type = safe_int(request.query.get("search_type", 0), default=0)
             search_string = request.query.get("search_string")
             if search_type < len(self.param.search_queries) and search_string:
                 query_lambda = self.param.search_queries[search_type][1]
                 try:
                     query = query_lambda(search_string)
-                except:
+                except Exception:
                     pass  # flash a message here
 
         if not query:
             query = self.param.query
         else:
             query &= self.param.query
 
@@ -954,15 +969,15 @@
         options = [
             OPTION(items[0], _value=k, _selected=(k == search_type))
             for k, items in enumerate(self.param.search_queries)
         ]
         hidden_fields = [
             INPUT(_name=key, _value=request.query.get(key), _type="hidden")
             for key in request.query
-            if not key in ("search_type", "search_string")
+            if key not in ("search_type", "search_string")
         ]
         attrs = self.attributes_plugin.link(url=self.endpoint)
         form = FORM(*hidden_fields, **attrs)
         sc = self.param.grid_class_style.get("grid-search-form-select")
         select = SELECT(
             *options,
             **dict(
@@ -1041,15 +1056,18 @@
                     **self.param.grid_class_style.get("grid-search-form-td"),
                 )
             )
         div.append(
             TABLE(tr, **self.param.grid_class_style.get("grid-search-form-table"))
         )
         for hidden_widget in self.param.search_form.custom["hidden_widgets"].keys():
-            div.append(self.param.search_form.custom["hidden_widgets"][hidden_widget])
+            if hidden_widget not in ("formname", "formkey"):
+                div.append(
+                    self.param.search_form.custom["hidden_widgets"][hidden_widget]
+                )
 
         div.append(self.param.search_form.custom["end"])
 
         return div
 
     def _make_table_header(self):
         sort_order = request.query.get("orderby", "")
@@ -1170,18 +1188,15 @@
 
         return td
 
     def _make_table_body(self):
         tbody = TBODY()
         for row in self.rows:
             #  find the row id - there may be nested tables....
-            if self.use_tablename and self.tablename in row and "id" not in row:
-                row_id = row[self.tablename]["id"]
-            else:
-                row_id = row["id"]
+            if not (self.use_tablename and self.tablename in row and "id" not in row):
                 self.use_tablename = False
 
             key = "%s.%s" % (self.tablename, "__row")
             if self.formatters.get(key):
                 extra_class = self.formatters.get(key)(row)["_class"]
                 extra_style = self.formatters.get(key)(row)["_style"]
             else:
@@ -1216,29 +1231,28 @@
                     tr.append(
                         TD(
                             column.render(row, index),
                             **clean_sc(_class=classes, _style=style),
                         )
                     )
 
-            td = None
             tbody.append(tr)
 
         return tbody
 
     def make_action_buttons(self, row):
         cat = CAT()
         row_id = row[self.param.field_id] if self.param.field_id else row.id
         if self.param.pre_action_buttons and len(self.param.pre_action_buttons) > 0:
             for btn in self.param.pre_action_buttons:
                 if callable(btn):
                     # a button can be a callable, to indicate whether or not a button should
                     # be displayed. call the function with the row object
                     btn = btn(row)
-                    if btn == None:
+                    if btn is None:
                         # if None was returned, no button is available for this row: ignore this value in the
                         # list
                         continue
                 attrs = (
                     self.attributes_plugin.confirm(message=self.T(btn.message))
                     if btn.message and btn.message != ""
                     else btn.__dict__.get("attrs", dict())
@@ -1253,17 +1267,19 @@
                         additional_styles=btn.__dict__.get("additional_styles"),
                         override_classes=btn.__dict__.get("override_classes"),
                         override_styles=btn.__dict__.get("override_styles"),
                         message=btn.message,
                         row_id=row_id if btn.append_id else None,
                         name=btn.__dict__.get("name"),
                         row=row,
-                        ignore_attribute_plugin=btn.ignore_attribute_plugin
-                        if "ignore_attribute_plugin" in btn.__dict__
-                        else False,
+                        ignore_attribute_plugin=(
+                            btn.ignore_attribute_plugin
+                            if "ignore_attribute_plugin" in btn.__dict__
+                            else False
+                        ),
                         **attrs,
                     )
                 )
 
         if self.is_readable(row):
             if isinstance(self.param.details, str):
                 details_url = self.param.details
@@ -1317,15 +1333,15 @@
 
         if self.param.post_action_buttons and len(self.param.post_action_buttons) > 0:
             for btn in self.param.post_action_buttons:
                 if callable(btn):
                     # a button can be a callable, to indicate whether or not a button should
                     # be displayed. call the function with the row object
                     btn = btn(row)
-                    if btn == None:
+                    if btn is None:
                         # if None was returned, no button is available for this row: ignore this value in the
                         # list
                         continue
                 attrs = (
                     self.attributes_plugin.confirm(message=self.T(btn.message))
                     if btn.message and btn.message != ""
                     else btn.__dict__.get("attrs", dict())
@@ -1339,17 +1355,19 @@
                         additional_styles=btn.__dict__.get("override_styles"),
                         override_classes=btn.__dict__.get("override_classes"),
                         override_styles=btn.__dict__.get("override_styles"),
                         message=btn.message,
                         row_id=row_id if btn.append_id else None,
                         name=btn.__dict__.get("name"),
                         row=row,
-                        ignore_attribute_plugin=btn.ignore_attribute_plugin
-                        if "ignore_attribute_plugin" in btn.__dict__
-                        else False,
+                        ignore_attribute_plugin=(
+                            btn.ignore_attribute_plugin
+                            if "ignore_attribute_plugin" in btn.__dict__
+                            else False
+                        ),
                         **attrs,
                     )
                 )
 
         return cat
 
     def _make_table_pager(self):
@@ -1470,25 +1488,29 @@
         #  add the table to the html
         html.append(DIV(table, **self.param.grid_class_style.get("grid-table-wrapper")))
 
         #  add the row counter information
         footer = DIV(**self.param.grid_class_style.get("grid-footer"))
 
         row_count = DIV(**self.param.grid_class_style.get("grid-info"))
-        row_count.append(
-            str(self.T("Displaying rows %s thru %s of %s"))
-            % (
-                self.page_start + 1 if self.number_of_pages > 1 else 1,
-                self.page_end
-                if self.page_end < self.total_number_of_rows
-                else self.total_number_of_rows,
-                self.total_number_of_rows,
+        (
+            row_count.append(
+                str(self.T("Displaying rows %s thru %s of %s"))
+                % (
+                    self.page_start + 1 if self.number_of_pages > 1 else 1,
+                    (
+                        self.page_end
+                        if self.page_end < self.total_number_of_rows
+                        else self.total_number_of_rows
+                    ),
+                    self.total_number_of_rows,
+                )
             )
-        ) if self.number_of_pages > 0 else row_count.append(
-            self.T("No rows to display")
+            if self.number_of_pages > 0
+            else row_count.append(self.T("No rows to display"))
         )
         footer.append(row_count)
 
         #  build the pager
         if self.number_of_pages > 1:
             footer.append(self._make_table_pager())
 
@@ -1644,15 +1666,15 @@
         if referrer:
             kvp = base64.b16decode(referrer.encode("utf8")).decode("utf8")
             if "parent_id" in kvp:
                 parent_id = kvp.split("parent_id=")[1]
 
     try:
         parent_id = parent_id.split("&")[0]
-    except:
+    except Exception:
         pass
 
     return parent_id
 
 
 class AttributesPlugin:
     def __init__(self, target_element=None):
```

### Comparing `py4web-1.20231115.1/py4web/utils/jsonrpc.py` & `py4web-1.20240420.1/py4web/utils/jsonrpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,13 @@
                 "rid": None,
                 "jsonrpc": "2.0",
                 "error": {"code": -32601, "message": "Method not found"},
             }
         try:
             result = func(*params) if isinstance(params, list) else func(**params)
             return {"result": result, "id": rid, "jsonrpc": "2.0"}
-        except Exception as e:
-            error = e
+        except Exception as err:
             return {
                 "rid": None,
                 "jsonrpc": "2.0",
-                "error": {"code": -32603, "message": "Internal error", "data": e},
+                "error": {"code": -32603, "message": "Internal error", "data": err},
             }
```

### Comparing `py4web-1.20231115.1/py4web/utils/mailer.py` & `py4web-1.20240420.1/py4web/utils/mailer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 """
 | This file is part of the py4web Web Framework
 | Copyrighted by Massimo Di Pierro <mdipierro@cs.depaul.edu>
 | License: "BSDv3" (https://opensource.org/licenses/BSD-3-Clause)
 """
 
 import email.utils
-import json
 import logging
 import mimetypes
 import os
+import re
 import smtplib
 from email import message_from_string
 from email.encoders import encode_base64
 
 from pydal._compat import *
 
 try:
@@ -501,15 +501,14 @@
                 )
             if not pyme:
                 raise RuntimeError("pyme not installed")
             ############################################
             #                   sign                   #
             ############################################
             if sign:
-                import string
 
                 core.check_version(None)
                 pin = payload_in.as_string().replace("\n", "\r\n")
                 plain = core.Data(pin)
                 sig = core.Data()
                 c = core.Context()
                 c.set_armor(1)
@@ -733,15 +732,15 @@
         if cc:
             payload["Cc"] = encoded_or_raw(to_unicode(", ".join(cc), encoding))
             to.extend(cc)
         if bcc:
             to.extend(bcc)
         payload["Subject"] = encoded_or_raw(to_unicode(subject, encoding))
         payload["Date"] = email.utils.formatdate()
-        for k, v in iteritems(headers):
+        for k, v in headers.items():
             payload[k] = encoded_or_raw(to_unicode(v, encoding))
 
         list_unsubscribe = list_unsubscribe or self.settings.list_unsubscribe
         if list_unsubscribe:
             payload["List-Unsubscribe"] = "<mailto:%s>" % list_unsubscribe
 
         dkim = dkim or self.settings.dkim
@@ -810,16 +809,17 @@
             elif self.settings.server == "aws" and boto3:
                 client = boto3.client("ses")
                 try:
                     raw = {"Data": payload.as_string()}
                     response = client.send_raw_email(
                         RawMessage=raw, Source=sender, Destinations=to
                     )
+                    print("Message send:", response)
                     return True
-                except ClientError as e:
+                except ClientError:
                     raise RuntimeError()
             else:
                 smtp_args = self.settings.server.split(":")
                 kwargs = dict(timeout=self.settings.timeout)
                 func = smtplib.SMTP_SSL if self.settings.ssl else smtplib.SMTP
                 server = func(*smtp_args, **kwargs)
                 try:
@@ -830,20 +830,20 @@
                     if self.settings.login:
                         server.login(*self.settings.login.split(":", 1))
                     result = server.sendmail(sender, to, payload.as_string())
                 finally:
                     # do not want to hide errors raising some exception here
                     try:
                         server.quit()
-                    except:
+                    except Exception:
                         pass
                     # ensure to close any socket with SMTP server
                     try:
                         server.close()
-                    except:
+                    except Exception:
                         pass
         except Exception as e:
             self.settings.logger.warning("Mailer.send failure:%s" % e)
             self.result = result
             raise
         self.result = result
         self.error = None
```

### Comparing `py4web-1.20231115.1/py4web/utils/misc.py` & `py4web-1.20240420.1/py4web/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,32 +10,31 @@
 This file specifically includes utilities for security.
 --------------------------------------------------------
 """
 
 import base64
 import hashlib
 import hmac
-import inspect
 import json
 import logging
 import os
 import random
 import re
 import socket
 import struct
 import sys
 import threading
 import time
 import uuid
 import zlib
 
-_struct_2_long_long = struct.Struct("=QQ")
-
 from Crypto.Cipher import AES
 
+_struct_2_long_long = struct.Struct("=QQ")
+
 HAVE_COMPARE_DIGEST = False
 if hasattr(hmac, "compare_digest"):
     HAVE_COMPARE_DIGEST = True
 
 
 def AES_new(key, IV=None):
     """Return an AES cipher object and random IV if None specified."""
```

### Comparing `py4web-1.20231115.1/py4web/utils/populate.py` & `py4web-1.20240420.1/py4web/utils/populate.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,18 +88,18 @@
 
 class Learner:
     def __init__(self):
         self.db = {}
 
     def learn(self, text):
         replacements1 = {
-            "[^a-zA-Z0-9\.;:\-]": " ",
-            "\s+": " ",
+            r"[^a-zA-Z0-9\.;:\-]": " ",
+            r"\s+": " ",
             ", ": " , ",
-            "\. ": " . ",
+            r"\. ": " . ",
             ": ": " : ",
             "; ": " ; ",
         }
         for key, value in replacements1.items():
             text = re.sub(key, value, text)
         items = [item.lower() for item in text.split(" ")]
         for i in range(len(items) - 1):
@@ -120,23 +120,23 @@
         with open(filename, "rb") as fp:
             self.loadd(pickle.load(fp))
 
     def loadd(self, db):
         self.db = db
 
     def generate(self, length=10000, prefix=False):
-        replacements2 = {" ,": ",", " \.": ".\n", " :": ":", " ;": ";", "\n\s+": "\n"}
+        replacements2 = {" ,": ",", " \\.": ".\n", " :": ":", " ;": ";", "\n\\s+": "\n"}
         keys = list(self.db.keys())
         key = keys[random.randint(0, len(keys) - 1)]
         words = key
         words = words.capitalize()
         regex = re.compile("[a-z]+")
         for i in range(length):
             okey = key
-            if not key in self.db:
+            if key not in self.db:
                 break  # should not happen
             db = self.db[key]
             s = sum(db.values())
             i = random.randint(0, s - 1)
             for key, value in db.items():
                 if i < value:
                     break
@@ -227,15 +227,15 @@
                 continue
             elif field.type == "id":
                 continue
             elif field.type == "upload":
                 continue
             elif field.compute is not None:
                 continue
-            elif default and not field.default in (None, ""):
+            elif default and field.default not in (None, ""):
                 record[fieldname] = field.default
             elif compute and field.compute:
                 continue
             elif field.type == "boolean":
                 record[fieldname] = random.random() > 0.5
             elif field.type == "date":
                 record[fieldname] = datetime.date(2009, 1, 1) - datetime.timedelta(
@@ -267,15 +267,15 @@
                         )
                     ]
             elif field.type == "integer":
                 try:
                     record[fieldname] = random.randint(
                         field.requires.minimum, field.requires.maximum - 1
                     )
-                except:
+                except Exception:
                     if "day" in fieldname:
                         record[fieldname] = random.randint(1, 28)
                     elif "month" in fieldname:
                         record[fieldname] = random.randint(1, 12)
                     elif "year" in fieldname:
                         record[fieldname] = random.randint(2000, 2013)
                     else:
@@ -291,28 +291,28 @@
                         field.requires.maximum - field.requires.minimum
                     )
                 else:
                     record[fieldname] = random.random() * 1000
             elif field.type[:10] == "reference ":
                 tablename = field.type[10:]
                 rtable = db[tablename]
-                if not tablename in ids:
+                if tablename not in ids:
                     if db._dbname == "gql":
                         ids[tablename] = [x.id for x in db(rtable).select(rtable.id)]
                     else:
                         ids[tablename] = [x.id for x in db(rtable).select(rtable.id)]
                 n = len(ids[tablename])
                 if n:
                     record[fieldname] = ids[tablename][random.randint(0, n - 1)]
                 else:
                     record[fieldname] = 0
             elif field.type[:15] == "list:reference ":
                 tablename = field.type[15:]
                 rtable = db[tablename]
-                if not tablename in ids:
+                if tablename not in ids:
                     if db._dbname == "gql":
                         ids[tablename] = [x.id for x in db(rtable).select(rtable.id)]
                     else:
                         ids[tablename] = [x.id for x in db(rtable).select(rtable.id)]
                 n = len(ids[tablename])
                 if n:
                     record[fieldname] = [
```

### Comparing `py4web-1.20231115.1/py4web/utils/publisher.py` & `py4web-1.20240420.1/py4web/utils/publisher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import uuid
 
-from pydal.restapi import ALLOW_ALL_POLICY, DENY_ALL_POLICY, RestAPI
+from pydal.restapi import RestAPI
 from yatl.helpers import DIV, TAG, XML
 
 from py4web import URL, action, request, response
 
 MTABLE = '<mtable url="{url}" filter="" order="" :editable="true" :deletable="true" :create="true" :render="{render}"></mtable>'
 
 
 class Publisher:
-
     """this is a work in progress - API subject to change"""
 
     def __init__(self, db, policy=None, auth=None, path="service/{uuid}/<tablename>"):
         self.db = db
         self.policy = policy
         self.restapi = RestAPI(self.db, policy)
         self.path = path.format(uuid=str(uuid.uuid4()))
         args = [db, auth] if auth else [db]
         f = action.uses(*args)(self.api)
         f = action(self.path, method=["GET", "POST"])(f)
         f = action(self.path + "/<id:int>", method=["PUT", "DELETE"])(f)
 
     def api(self, tablename, id=None):
-        policy = self.policy
         data = self.restapi(request.method, tablename, id, request.query, request.json)
         response.status = data["code"]
         return data
 
     def mtable(self, table):
         path = self.path.replace("<tablename>", table._tablename)
         return XML(MTABLE.format(url=URL(path), render={}))
```

### Comparing `py4web-1.20231115.1/py4web/utils/recaptcha.py` & `py4web-1.20240420.1/py4web/utils/recaptcha.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,22 +54,18 @@
     def fixture(self):
         return recaptcha_fixture(self.api_key)
 
     @property
     def field(self):
         return Field("g_recaptcha_response", "hidden", requires=self.validator)
 
-    @property
-    def script(self):
-        return recaptcha_script(self.api_key)
-
     def validator(self, value, _):
         data = {"secret": self.api_secret, "response": value}
         res = requests.post(
             "https://www.google.com/recaptcha/api/siteverify", data=data
         )
         try:
             if res.json()["success"]:
                 return (True, None)
             return (False, "Invalid ReCaptcha response")
-        except exc:
+        except Exception as exc:
             return (False, str(exc))
```

### Comparing `py4web-1.20231115.1/py4web/utils/security.py` & `py4web-1.20240420.1/py4web/utils/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import fnmatch
 import ipaddress
 
 from py4web.core import HTTP, Fixture, request, response
 
 
 def listify(item):
     """if item is not None and Not a list returns [item] else returns item"""
@@ -15,15 +14,14 @@
     """checks s an ip ('127.0.0.1') is a list of networks (['127.0.0.1/16'])"""
     ip = ipaddress.ip_address(ip)
     print("networks", networks)
     return any(ip in ipaddress.ip_network(network) for network in networks)
 
 
 class CheckHeaders(Fixture):
-
     """
     This fixture can block an action from being excuted if:
     - it does not match the specificated protocol (http, https)
     - referer field does not match the same protocol as the current url
     - referer field does not match the same domain as the current url
     - referer field does not match the same app_name as the current url
     - ip address is not in the allowed_networks
```

### Comparing `py4web-1.20231115.1/py4web/utils/url_signer.py` & `py4web-1.20240420.1/py4web/utils/url_signer.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
                 raise HTTP(403)
             # We remove the signature, not to pollute the request.
             del request.query["_signature"]
             # Checks the expiration time.
             if self.url_signer.lifespan is not None:
                 if float(ts) + self.url_signer.lifespan < time.time():
                     raise HTTP(403)
-        except:
-            raise HTTP(403)
+        except Exception as err:
+            raise HTTP(403, body=str(err))
 
     def _decode_ts(self, ts_string):
         """Decodes the timestamp, removing the salt."""
         s = base64.b16encode(ts_string.encode("utf-8")).decode("utf-8")
         return float(s.split(";")[1])
```

### Comparing `py4web-1.20231115.1/py4web.egg-info/PKG-INFO` & `py4web-1.20240420.1/py4web.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,21 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20231115.1
+Version: 1.20240420.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
-Requires-Dist: wheel
-Requires-Dist: ombott>=1.0.0
-Requires-Dist: click
-Requires-Dist: colorama
-Requires-Dist: cryptography
-Requires-Dist: portalocker
-Requires-Dist: tornado
-Requires-Dist: renoir>=1.4.0
-Requires-Dist: requests
-Requires-Dist: threadsafevariable>=20230507.1
-Requires-Dist: pyjwt>=2.0.1
-Requires-Dist: pycryptodome
-Requires-Dist: pluralize>=20231008.1
-Requires-Dist: rocket3>=20230507.1
-Requires-Dist: yatl>=20230507.3
-Requires-Dist: pydal>=20231114.3
-Requires-Dist: watchgod>=0.6
 
 What is py4web?
 ===============
 
 .. image:: https://travis-ci.com/web2py/py4web.svg?branch=master
     :target: https://travis-ci.com/web2py/py4web
 
@@ -67,23 +50,23 @@
 Editing a database in the Dashboard
 
 .. image:: docs/images/dashboard_restapi.png
 
 Installation
 ############
 
-PY4WEB runs fine on Windows, MacOS and Linux. There are many installation procedures (see the official documentation for details) but only two of them are summarized here.
+PY4WEB runs fine on Windows, MacOS and Linux. There are many installation procedures `(see the official documentation for details) <https://py4web.com/_documentation/static/en/chapter-03.html>`__ but only two of them are summarized here.
 
 The **simplest way** to install py4web is using binaries, but it's only available for Windows and MacOS. It's meant especially for newbies or students, because it does not require Python pre-installed on your system nor administrative rights. You just need to download the latest Windows or MacOS ZIP file from `this external repository <https://github.com/nicozanf/py4web-pyinstaller>`__. Unzip it on a local folder and open a command line there. Finally run the commands (omit './' if you're using Windows)
 
 
 .. code:: bash
 
-   ./py4web-start set_password
-   ./py4web-start run apps
+   ./py4web set_password
+   ./py4web run apps
 
 
 
 
 The **standard installation procedure** for py4web on Windows, MacOS and Linux  is using pip. Its only prerequisite is Python 3.7+.
 
 .. code:: bash
```

### Comparing `py4web-1.20231115.1/py4web.egg-info/SOURCES.txt` & `py4web-1.20240420.1/py4web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/pyproject.toml` & `py4web-1.20240420.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py4web"
-version = "1.20231115.1"
+version = "1.20240420.1"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "A fast, stable, comprehensive web framework"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `py4web-1.20231115.1/tests/test_action.py` & `py4web-1.20240420.1/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/tests/test_auth.py` & `py4web-1.20240420.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/tests/test_cache.py` & `py4web-1.20240420.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/tests/test_fixture.py` & `py4web-1.20240420.1/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/tests/test_form.py` & `py4web-1.20240420.1/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/tests/test_get_error_snapshot.py` & `py4web-1.20240420.1/tests/test_get_error_snapshot.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/tests/test_json.py` & `py4web-1.20240420.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/tests/test_main.py` & `py4web-1.20240420.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/tests/test_session.py` & `py4web-1.20240420.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20231115.1/tests/test_tags.py` & `py4web-1.20240420.1/tests/test_tags.py`

 * *Files identical despite different names*

