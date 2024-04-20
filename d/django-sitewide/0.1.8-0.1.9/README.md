# Comparing `tmp/django-sitewide-0.1.8.tar.gz` & `tmp/django-sitewide-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sitewide-0.1.8.tar", last modified: Mon Feb 19 05:45:13 2024, max compression
+gzip compressed data, was "django-sitewide-0.1.9.tar", last modified: Fri Mar  1 18:07:49 2024, max compression
```

## Comparing `django-sitewide-0.1.8.tar` & `django-sitewide-0.1.9.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-02-19 05:45:13.980001 django-sitewide-0.1.8/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    35149 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/LICENSE
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      135 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/MANIFEST.in
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1714 2024-02-19 05:45:13.980001 django-sitewide-0.1.8/PKG-INFO
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      702 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/README.rst
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-02-19 05:45:13.980001 django-sitewide-0.1.8/django_sitewide.egg-info/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1714 2024-02-19 05:45:13.000000 django-sitewide-0.1.8/django_sitewide.egg-info/PKG-INFO
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     2152 2024-02-19 05:45:13.000000 django-sitewide-0.1.8/django_sitewide.egg-info/SOURCES.txt
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        1 2024-02-19 05:45:13.000000 django-sitewide-0.1.8/django_sitewide.egg-info/dependency_links.txt
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       12 2024-02-19 05:45:13.000000 django-sitewide-0.1.8/django_sitewide.egg-info/requires.txt
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        9 2024-02-19 05:45:13.000000 django-sitewide-0.1.8/django_sitewide.egg-info/top_level.txt
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       90 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/pyproject.toml
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      984 2024-02-19 05:45:13.981001 django-sitewide-0.1.8/setup.cfg
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       38 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/setup.py
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-02-19 05:45:13.976001 django-sitewide-0.1.8/sitewide/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        0 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/__init__.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       63 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/admin.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      148 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/apps.py
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-02-19 05:45:13.976001 django-sitewide-0.1.8/sitewide/migrations/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      848 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/migrations/0001_initial.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        0 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/migrations/__init__.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      355 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/models.py
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-02-19 05:45:13.973001 django-sitewide-0.1.8/sitewide/static/
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-02-19 05:45:13.976001 django-sitewide-0.1.8/sitewide/static/css/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    16384 2024-01-28 14:35:53.000000 django-sitewide-0.1.8/sitewide/static/css/.sidebar.css.swp
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    17033 2024-02-19 05:44:14.000000 django-sitewide-0.1.8/sitewide/static/css/base.css
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1019 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/css/fonts.css
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      162 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/css/footer.css
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      955 2024-02-02 04:36:57.000000 django-sitewide-0.1.8/sitewide/static/css/header.css
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     3869 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/css/sidebar.css
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     2427 2024-02-18 14:25:24.000000 django-sitewide-0.1.8/sitewide/static/css/var.css
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-02-19 05:45:13.978001 django-sitewide-0.1.8/sitewide/static/fonts/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)   327360 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/fonts/MaterialIcons-Regular.ttf
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)   160576 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/fonts/MaterialIcons-Regular.woff
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    82438 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].codepoints
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     6487 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].ttf
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     6498 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].woff2
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    82442 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsRounded[FILL,GRAD,opsz,wght].codepoints
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     6482 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsRounded[FILL,GRAD,opsz,wght].ttf
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     6493 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsRounded[FILL,GRAD,opsz,wght].woff2
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    82420 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsSharp[FILL,GRAD,opsz,wght].codepoints
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     6469 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsSharp[FILL,GRAD,opsz,wght].ttf
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     6480 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsSharp[FILL,GRAD,opsz,wght].woff2
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-02-19 05:45:13.979001 django-sitewide-0.1.8/sitewide/static/imgs/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     5750 2023-09-27 10:45:05.000000 django-sitewide-0.1.8/sitewide/static/imgs/avatar.png
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     5766 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/imgs/no-image-1200x1200.svg
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     5746 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/imgs/no-image-800x1200.svg
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     5756 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/imgs/no-image.svg
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      858 2024-01-27 10:25:03.000000 django-sitewide-0.1.8/sitewide/static/imgs/sitewide-favicon-32x32.png
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     4205 2024-01-27 10:47:55.000000 django-sitewide-0.1.8/sitewide/static/imgs/sitewide-favicon-32x32.svg
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1269 2024-02-02 05:06:46.000000 django-sitewide-0.1.8/sitewide/static/imgs/sitewide-favicon-48x48.png
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     4203 2024-02-02 05:06:48.000000 django-sitewide-0.1.8/sitewide/static/imgs/sitewide-favicon-48x48.svg
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     4112 2024-01-27 09:50:00.000000 django-sitewide-0.1.8/sitewide/static/imgs/sitewide-logo.svg
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-02-19 05:45:13.979001 django-sitewide-0.1.8/sitewide/static/js/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      465 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/static/js/sidebar.js
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-02-19 05:45:13.974001 django-sitewide-0.1.8/sitewide/templates/
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-02-19 05:45:13.980001 django-sitewide-0.1.8/sitewide/templates/sitewide/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      147 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/templates/sitewide/authenticated.html
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       68 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/templates/sitewide/footer.html
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      509 2024-02-03 13:37:01.000000 django-sitewide-0.1.8/sitewide/templates/sitewide/header.html
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1607 2024-02-02 04:53:56.000000 django-sitewide-0.1.8/sitewide/templates/sitewide/layout.html
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      262 2024-02-08 17:16:22.000000 django-sitewide-0.1.8/sitewide/templates/sitewide/sample-starter-view-template.html
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1571 2024-02-03 13:37:54.000000 django-sitewide-0.1.8/sitewide/templates/sitewide/sidebar.html
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      639 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/templates/sitewide/stylesheets.html
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       60 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/tests.py
--rwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)      147 2023-12-13 17:44:54.000000 django-sitewide-0.1.8/sitewide/urls.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     9558 2024-02-04 06:10:40.000000 django-sitewide-0.1.8/sitewide/views.py
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-01 18:07:49.853488 django-sitewide-0.1.9/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    35149 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/LICENSE
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      135 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/MANIFEST.in
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1714 2024-03-01 18:07:49.853488 django-sitewide-0.1.9/PKG-INFO
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      702 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/README.rst
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-01 18:07:49.853488 django-sitewide-0.1.9/django_sitewide.egg-info/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1714 2024-03-01 18:07:49.000000 django-sitewide-0.1.9/django_sitewide.egg-info/PKG-INFO
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     2215 2024-03-01 18:07:49.000000 django-sitewide-0.1.9/django_sitewide.egg-info/SOURCES.txt
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        1 2024-03-01 18:07:49.000000 django-sitewide-0.1.9/django_sitewide.egg-info/dependency_links.txt
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       12 2024-03-01 18:07:49.000000 django-sitewide-0.1.9/django_sitewide.egg-info/requires.txt
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        9 2024-03-01 18:07:49.000000 django-sitewide-0.1.9/django_sitewide.egg-info/top_level.txt
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       90 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/pyproject.toml
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      984 2024-03-01 18:07:49.853488 django-sitewide-0.1.9/setup.cfg
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       38 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/setup.py
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-01 18:07:49.848488 django-sitewide-0.1.9/sitewide/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        0 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/__init__.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       63 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/admin.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      148 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/apps.py
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-01 18:07:49.848488 django-sitewide-0.1.9/sitewide/migrations/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      848 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/migrations/0001_initial.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        0 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/migrations/__init__.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      355 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/models.py
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-01 18:07:49.845488 django-sitewide-0.1.9/sitewide/static/
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-01 18:07:49.849488 django-sitewide-0.1.9/sitewide/static/css/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    36864 2024-03-01 18:07:41.000000 django-sitewide-0.1.9/sitewide/static/css/.base.css.swp
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    12288 2024-02-25 05:34:02.000000 django-sitewide-0.1.9/sitewide/static/css/.var.css.swn
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    12288 2024-02-23 20:18:20.000000 django-sitewide-0.1.9/sitewide/static/css/.var.css.swo
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    17102 2024-03-01 18:07:37.000000 django-sitewide-0.1.9/sitewide/static/css/base.css
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1019 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/css/fonts.css
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      150 2024-02-29 08:32:41.000000 django-sitewide-0.1.9/sitewide/static/css/footer.css
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      922 2024-02-29 08:30:35.000000 django-sitewide-0.1.9/sitewide/static/css/header.css
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     3821 2024-02-25 23:54:16.000000 django-sitewide-0.1.9/sitewide/static/css/sidebar.css
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     3964 2024-03-01 10:35:56.000000 django-sitewide-0.1.9/sitewide/static/css/var.css
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-01 18:07:49.851488 django-sitewide-0.1.9/sitewide/static/fonts/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)   327360 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/fonts/MaterialIcons-Regular.ttf
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)   160576 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/fonts/MaterialIcons-Regular.woff
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    82438 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].codepoints
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     6487 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].ttf
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     6498 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].woff2
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    82442 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsRounded[FILL,GRAD,opsz,wght].codepoints
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     6482 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsRounded[FILL,GRAD,opsz,wght].ttf
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     6493 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsRounded[FILL,GRAD,opsz,wght].woff2
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    82420 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsSharp[FILL,GRAD,opsz,wght].codepoints
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     6469 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsSharp[FILL,GRAD,opsz,wght].ttf
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     6480 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsSharp[FILL,GRAD,opsz,wght].woff2
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-01 18:07:49.852488 django-sitewide-0.1.9/sitewide/static/imgs/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     5750 2023-09-27 10:45:05.000000 django-sitewide-0.1.9/sitewide/static/imgs/avatar.png
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     5766 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/imgs/no-image-1200x1200.svg
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     5746 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/imgs/no-image-800x1200.svg
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     5756 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/imgs/no-image.svg
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      858 2024-01-27 10:25:03.000000 django-sitewide-0.1.9/sitewide/static/imgs/sitewide-favicon-32x32.png
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     4205 2024-01-27 10:47:55.000000 django-sitewide-0.1.9/sitewide/static/imgs/sitewide-favicon-32x32.svg
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1269 2024-02-02 05:06:46.000000 django-sitewide-0.1.9/sitewide/static/imgs/sitewide-favicon-48x48.png
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     4203 2024-02-02 05:06:48.000000 django-sitewide-0.1.9/sitewide/static/imgs/sitewide-favicon-48x48.svg
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     4112 2024-01-27 09:50:00.000000 django-sitewide-0.1.9/sitewide/static/imgs/sitewide-logo.svg
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-01 18:07:49.852488 django-sitewide-0.1.9/sitewide/static/js/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      465 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/static/js/sidebar.js
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-01 18:07:49.846488 django-sitewide-0.1.9/sitewide/templates/
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-01 18:07:49.852488 django-sitewide-0.1.9/sitewide/templates/sitewide/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      147 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/templates/sitewide/authenticated.html
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       68 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/templates/sitewide/footer.html
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      509 2024-02-03 13:37:01.000000 django-sitewide-0.1.9/sitewide/templates/sitewide/header.html
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1589 2024-02-29 08:12:13.000000 django-sitewide-0.1.9/sitewide/templates/sitewide/layout.html
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      262 2024-02-08 17:16:22.000000 django-sitewide-0.1.9/sitewide/templates/sitewide/sample-starter-view-template.html
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1571 2024-02-03 13:37:54.000000 django-sitewide-0.1.9/sitewide/templates/sitewide/sidebar.html
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      639 2024-02-29 08:12:29.000000 django-sitewide-0.1.9/sitewide/templates/sitewide/stylesheets.html
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       60 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/tests.py
+-rwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)      147 2023-12-13 17:44:54.000000 django-sitewide-0.1.9/sitewide/urls.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     9558 2024-02-04 06:10:40.000000 django-sitewide-0.1.9/sitewide/views.py
```

### Comparing `django-sitewide-0.1.8/LICENSE` & `django-sitewide-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/PKG-INFO` & `django-sitewide-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sitewide
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Django app for creating and maintaining consistent looks across a django website.
 Home-page: https://gitlab.com/twohot/django-sitewide
 Author: Onyeibo Oku
 Author-email: onyeibo@schemefusion.com
 License: GPLv3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-sitewide-0.1.8/README.rst` & `django-sitewide-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/django_sitewide.egg-info/PKG-INFO` & `django-sitewide-0.1.9/django_sitewide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sitewide
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Django app for creating and maintaining consistent looks across a django website.
 Home-page: https://gitlab.com/twohot/django-sitewide
 Author: Onyeibo Oku
 Author-email: onyeibo@schemefusion.com
 License: GPLv3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-sitewide-0.1.8/django_sitewide.egg-info/SOURCES.txt` & `django-sitewide-0.1.9/django_sitewide.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 sitewide/apps.py
 sitewide/models.py
 sitewide/tests.py
 sitewide/urls.py
 sitewide/views.py
 sitewide/migrations/0001_initial.py
 sitewide/migrations/__init__.py
-sitewide/static/css/.sidebar.css.swp
+sitewide/static/css/.base.css.swp
+sitewide/static/css/.var.css.swn
+sitewide/static/css/.var.css.swo
 sitewide/static/css/base.css
 sitewide/static/css/fonts.css
 sitewide/static/css/footer.css
 sitewide/static/css/header.css
 sitewide/static/css/sidebar.css
 sitewide/static/css/var.css
 sitewide/static/fonts/MaterialIcons-Regular.ttf
```

### Comparing `django-sitewide-0.1.8/setup.cfg` & `django-sitewide-0.1.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-sitewide
-version = 0.1.8
+version = 0.1.9
 description = A Django app for creating and maintaining consistent looks across a django website.
 long_description = file: README.rst
 url = https://gitlab.com/twohot/django-sitewide
 author = Onyeibo Oku
 author_email = onyeibo@schemefusion.com
 license = GPLv3
 classifiers =
```

### Comparing `django-sitewide-0.1.8/sitewide/migrations/0001_initial.py` & `django-sitewide-0.1.9/sitewide/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/css/fonts.css` & `django-sitewide-0.1.9/sitewide/static/css/fonts.css`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/css/header.css` & `django-sitewide-0.1.9/sitewide/static/css/header.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 header {
-    color: var(--color-bg);
-    min-height: var(--height-header);
-    padding-bottom: var(--margins);
-    padding-top: var(--margins);
+    color: var(--bg);
+    min-height: var(--header-height);
+    padding-bottom: var(--mgns);
+    padding-top: var(--mgns);
 } 
 
 header .container {
     display: flex;
     column-gap: 10px;
 }
 
 .header-insite {
-    background: var(--color-header-bg);
-    border-bottom: 1px solid var(--color-header-bg);
+    background: var(--header-bg);
+    border-bottom: 1px solid var(--header-bg);
 }
 
 .header-outsite {
-    background: var(--color-bg);
-    border-bottom: 1px dashed var(--color-header-bg);
+    background: var(--bg);
+    border-bottom: 1px dashed var(--header-bg);
 }
 
 #hamburger {
-    color: var(--hamburger);
+    color: var(--hamburger-fg);
     cursor: pointer;
     display: none;
     font-family: 'Material Icons';
     font-size: 24px;
     text-decoration: none;
 }
```

### Comparing `django-sitewide-0.1.8/sitewide/static/css/sidebar.css` & `django-sitewide-0.1.9/sitewide/static/css/sidebar.css`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #sidebar {
-    background: var(--color-sidebar-bg);
-    color: var(--color-sidebar-fg);
+    background: var(--sidebar-bg);
+    color: var(--sidebar-fg);
     font-size: unset;
     height: 100%;
     left: 0px;
     line-height: 1;
     overflow-x: hidden;
     overflow-y: auto;
     position: fixed;
@@ -82,35 +82,35 @@
 .menu, .submenu {
     list-style-type: none;
     margin: 0;
     padding: 0;
 }
 
 .submenu {
-    background: var(--color-sidebar-sub-bg);
+    background: var(--sidebar-submenu-bg);
 }
 
 .item, .subitem {
     align-items: center;
-    border-left: 2px solid var(--color-sidebar-bg);
+    border-left: 2px solid var(--sidebar-bg);
     display: flex;
-    color: var(--color-sidebar);
+    color: var(--sidebar);
     height: var(--sidebar-item-height);
     text-decoration: none;
     transition: background 0.5s ease;
 }
 
 .item:focus, .item:active {
-    border-left-color: var(--focus-indicator);
+    border-left-color: var(--indicator);
     font-weight: bold;
     outline: none;
 }
 
 .subitem:focus, .subitem:active {
-    border-left-color: var(--focus-indicator-sub);
+    border-left-color: var(--indicator-submenu);
     font-weight: bold;
     outline: none;
 }
 
 .item div:first-child,
 .subitem div:first-child {
     /*border-left: 3px solid var(side-bar);*/
@@ -134,21 +134,21 @@
 }
 
 .submenu:target {
     display: block;
 }
 
 .item:hover, .item:focus {
-    background-color: var(--color-sidebar-bg-hover);
+    background-color: var(--sidebar-bg-hover);
     color: white;
     cursor: pointer;
 }
 
 .subitem:hover, .subitem:focus {
-    background-color: var(--color-sidebar-sub-bg-hover);
+    background-color: var(--sidebar-submenu-bg-hover);
     color: white;
     cursor: pointer;
 }
 
 
 /*-----------------------------------*/
 /* SideBar Responsiveness            */
@@ -164,15 +164,15 @@
 }
 
 /* iPads and Tablets */
 
 @media screen and (max-width: 768px) {
     #user h3, #user p {
         font-size: 0em;
-        color: var(--color-sidebar-bg);
+        color: var(--sidebar-bg);
     }
 
     #avatar {
         grid-template-columns: 1fr var(--sidebar-dock-avatar) 1fr;
         grid-template-rows: 1fr var(--sidebar-dock-avatar) 1fr;
     }
```

### Comparing `django-sitewide-0.1.8/sitewide/static/fonts/MaterialIcons-Regular.ttf` & `django-sitewide-0.1.9/sitewide/static/fonts/MaterialIcons-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/fonts/MaterialIcons-Regular.woff` & `django-sitewide-0.1.9/sitewide/static/fonts/MaterialIcons-Regular.woff`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].codepoints` & `django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].codepoints`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].ttf` & `django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].ttf`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].woff2` & `django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsOutlined[FILL,GRAD,opsz,wght].woff2`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsRounded[FILL,GRAD,opsz,wght].codepoints` & `django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsRounded[FILL,GRAD,opsz,wght].codepoints`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsRounded[FILL,GRAD,opsz,wght].ttf` & `django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsRounded[FILL,GRAD,opsz,wght].ttf`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsRounded[FILL,GRAD,opsz,wght].woff2` & `django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsRounded[FILL,GRAD,opsz,wght].woff2`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsSharp[FILL,GRAD,opsz,wght].codepoints` & `django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsSharp[FILL,GRAD,opsz,wght].codepoints`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsSharp[FILL,GRAD,opsz,wght].ttf` & `django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsSharp[FILL,GRAD,opsz,wght].ttf`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/fonts/MaterialSymbolsSharp[FILL,GRAD,opsz,wght].woff2` & `django-sitewide-0.1.9/sitewide/static/fonts/MaterialSymbolsSharp[FILL,GRAD,opsz,wght].woff2`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/imgs/avatar.png` & `django-sitewide-0.1.9/sitewide/static/imgs/avatar.png`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/imgs/no-image-1200x1200.svg` & `django-sitewide-0.1.9/sitewide/static/imgs/no-image-1200x1200.svg`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/imgs/no-image-800x1200.svg` & `django-sitewide-0.1.9/sitewide/static/imgs/no-image-800x1200.svg`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/imgs/no-image.svg` & `django-sitewide-0.1.9/sitewide/static/imgs/no-image.svg`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/imgs/sitewide-favicon-32x32.png` & `django-sitewide-0.1.9/sitewide/static/imgs/sitewide-favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/imgs/sitewide-favicon-32x32.svg` & `django-sitewide-0.1.9/sitewide/static/imgs/sitewide-favicon-32x32.svg`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/imgs/sitewide-favicon-48x48.png` & `django-sitewide-0.1.9/sitewide/static/imgs/sitewide-favicon-48x48.png`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/imgs/sitewide-favicon-48x48.svg` & `django-sitewide-0.1.9/sitewide/static/imgs/sitewide-favicon-48x48.svg`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/static/imgs/sitewide-logo.svg` & `django-sitewide-0.1.9/sitewide/static/imgs/sitewide-logo.svg`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/templates/sitewide/layout.html` & `django-sitewide-0.1.9/sitewide/templates/sitewide/layout.html`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,25 @@
     <body>
         {% if sitewide.sidebar.show %}
             {% include "sitewide/sidebar.html" %}
         {% endif %}
         {% block banner %}{% endblock %}
         {% if sitewide.header.show %}
         <header class={% if sitewide.sidebar.show %}"header-insite"{% else %}"header-outsite"{% endif %}>
-            <div class={% if sitewide.sidebar.show %}"margins-insite"{% else %}"margins-outsite"{% endif %}>
+            <div class={% if sitewide.sidebar.show %}"mgns-insite"{% else %}"mgns-outsite"{% endif %}>
                 {% include "sitewide/header.html" %}
             </div>
         </header>
         {% endif %}
         <main>
-            <div class={% if sitewide.sidebar.show %}"margins-insite"{% else %}"margins-outsite"{% endif %}>
+            <div class={% if sitewide.sidebar.show %}"mgns-insite"{% else %}"mgns-outsite"{% endif %}>
                 {% block main %}{% endblock %}
             </div>
         </main>
         <footer>
-            <div class={% if sitewide.sidebar.show %}"margins-insite"{% else %}"margins-outsite"{% endif %}>
+            <div class={% if sitewide.sidebar.show %}"mgns-insite"{% else %}"mgns-outsite"{% endif %}>
                 {% include "sitewide/footer.html" %}
             </div>
         </footer>
     </body>
     <script src="{% static 'js/sidebar.js' %}"></script>
 </html>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% load static %}
 {% include "sitewide/stylesheets.html" %} {% block 'app-css' %}{% endblock %}
 {% block head %}{% endblock %}
 {% if sitewide.sidebar.show %} {% include "sitewide/sidebar.html" %} {% endif
 %} {% block banner %}{% endblock %} {% if sitewide.header.show %}
 }"header-insite"{% else %}"header-outsite"{% endif %}>
-}"margins-insite"{% else %}"margins-outsite"{% endif %}> {% include "sitewide/
+}"mgns-insite"{% else %}"mgns-outsite"{% endif %}> {% include "sitewide/
 header.html" %}
 {% endif %}
-}"margins-insite"{% else %}"margins-outsite"{% endif %}> {% block main %}{%
-endblock %}
-}"margins-insite"{% else %}"margins-outsite"{% endif %}> {% include "sitewide/
+}"mgns-insite"{% else %}"mgns-outsite"{% endif %}> {% block main %}{% endblock
+%}
+}"mgns-insite"{% else %}"mgns-outsite"{% endif %}> {% include "sitewide/
 footer.html" %}
```

### Comparing `django-sitewide-0.1.8/sitewide/templates/sitewide/sidebar.html` & `django-sitewide-0.1.9/sitewide/templates/sitewide/sidebar.html`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/templates/sitewide/stylesheets.html` & `django-sitewide-0.1.9/sitewide/templates/sitewide/stylesheets.html`

 * *Files identical despite different names*

### Comparing `django-sitewide-0.1.8/sitewide/views.py` & `django-sitewide-0.1.9/sitewide/views.py`

 * *Files identical despite different names*

