# Comparing `tmp/django-statici18n-2.4.0.tar.gz` & `tmp/django_statici18n-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-statici18n-2.4.0.tar", last modified: Sat Jul 29 13:10:26 2023, max compression
+gzip compressed data, was "django_statici18n-2.5.0.tar", last modified: Sat Apr 20 13:22:05 2024, max compression
```

## Comparing `django-statici18n-2.4.0.tar` & `django_statici18n-2.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.389206 django-statici18n-2.4.0/
--rw-r--r--   0 zyegfryed   (501) staff       (20)     2792 2020-09-18 12:18:49.000000 django-statici18n-2.4.0/LICENSE
--rw-r--r--   0 zyegfryed   (501) staff       (20)       88 2020-09-18 12:18:49.000000 django-statici18n-2.4.0/MANIFEST.in
--rw-r--r--   0 zyegfryed   (501) staff       (20)     6131 2023-07-29 13:10:26.389451 django-statici18n-2.4.0/PKG-INFO
--rw-r--r--   0 zyegfryed   (501) staff       (20)     4165 2023-07-29 12:41:23.000000 django-statici18n-2.4.0/README.rst
--rw-r--r--   0 zyegfryed   (501) staff       (20)      358 2023-07-29 13:10:26.390427 django-statici18n-2.4.0/setup.cfg
--rw-r--r--   0 zyegfryed   (501) staff       (20)     1376 2023-07-29 13:05:41.000000 django-statici18n-2.4.0/setup.py
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.375795 django-statici18n-2.4.0/src/
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.384480 django-statici18n-2.4.0/src/django_statici18n.egg-info/
--rw-r--r--   0 zyegfryed   (501) staff       (20)     6131 2023-07-29 13:10:26.000000 django-statici18n-2.4.0/src/django_statici18n.egg-info/PKG-INFO
--rw-r--r--   0 zyegfryed   (501) staff       (20)      633 2023-07-29 13:10:26.000000 django-statici18n-2.4.0/src/django_statici18n.egg-info/SOURCES.txt
--rw-r--r--   0 zyegfryed   (501) staff       (20)        1 2023-07-29 13:10:26.000000 django-statici18n-2.4.0/src/django_statici18n.egg-info/dependency_links.txt
--rw-r--r--   0 zyegfryed   (501) staff       (20)        1 2020-09-18 12:32:22.000000 django-statici18n-2.4.0/src/django_statici18n.egg-info/not-zip-safe
--rw-r--r--   0 zyegfryed   (501) staff       (20)       32 2023-07-29 13:10:26.000000 django-statici18n-2.4.0/src/django_statici18n.egg-info/requires.txt
--rw-r--r--   0 zyegfryed   (501) staff       (20)       11 2023-07-29 13:10:26.000000 django-statici18n-2.4.0/src/django_statici18n.egg-info/top_level.txt
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.386589 django-statici18n-2.4.0/src/statici18n/
--rw-r--r--   0 zyegfryed   (501) staff       (20)      146 2023-07-29 13:05:41.000000 django-statici18n-2.4.0/src/statici18n/__init__.py
--rw-r--r--   0 zyegfryed   (501) staff       (20)      152 2020-10-04 11:35:11.000000 django-statici18n-2.4.0/src/statici18n/apps.py
--rw-r--r--   0 zyegfryed   (501) staff       (20)      697 2020-10-04 11:35:11.000000 django-statici18n-2.4.0/src/statici18n/conf.py
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.387133 django-statici18n-2.4.0/src/statici18n/management/
--rw-r--r--   0 zyegfryed   (501) staff       (20)        0 2020-09-18 12:18:49.000000 django-statici18n-2.4.0/src/statici18n/management/__init__.py
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.387882 django-statici18n-2.4.0/src/statici18n/management/commands/
--rw-r--r--   0 zyegfryed   (501) staff       (20)        0 2020-09-18 12:18:49.000000 django-statici18n-2.4.0/src/statici18n/management/commands/__init__.py
--rw-r--r--   0 zyegfryed   (501) staff       (20)     5354 2022-08-14 19:57:22.000000 django-statici18n-2.4.0/src/statici18n/management/commands/compilejsi18n.py
-drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2023-07-29 13:10:26.388683 django-statici18n-2.4.0/src/statici18n/templatetags/
--rw-r--r--   0 zyegfryed   (501) staff       (20)        0 2020-09-18 12:18:49.000000 django-statici18n-2.4.0/src/statici18n/templatetags/__init__.py
--rw-r--r--   0 zyegfryed   (501) staff       (20)     1107 2020-10-04 11:35:11.000000 django-statici18n-2.4.0/src/statici18n/templatetags/statici18n.py
--rw-r--r--   0 zyegfryed   (501) staff       (20)     1414 2022-08-14 19:57:22.000000 django-statici18n-2.4.0/src/statici18n/utils.py
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2024-04-20 13:22:05.220246 django_statici18n-2.5.0/
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     2792 2020-09-18 12:18:49.000000 django_statici18n-2.5.0/LICENSE
+-rw-r--r--   0 zyegfryed   (501) staff       (20)       88 2020-09-18 12:18:49.000000 django_statici18n-2.5.0/MANIFEST.in
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     5248 2024-04-20 13:22:05.219807 django_statici18n-2.5.0/PKG-INFO
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     4165 2023-09-10 15:05:14.000000 django_statici18n-2.5.0/README.rst
+-rw-r--r--   0 zyegfryed   (501) staff       (20)      358 2024-04-20 13:22:05.221676 django_statici18n-2.5.0/setup.cfg
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     1376 2024-04-20 12:57:21.000000 django_statici18n-2.5.0/setup.py
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2024-04-20 13:22:05.183776 django_statici18n-2.5.0/src/
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2024-04-20 13:22:05.218313 django_statici18n-2.5.0/src/django_statici18n.egg-info/
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     5248 2024-04-20 13:22:05.000000 django_statici18n-2.5.0/src/django_statici18n.egg-info/PKG-INFO
+-rw-r--r--   0 zyegfryed   (501) staff       (20)      633 2024-04-20 13:22:05.000000 django_statici18n-2.5.0/src/django_statici18n.egg-info/SOURCES.txt
+-rw-r--r--   0 zyegfryed   (501) staff       (20)        1 2024-04-20 13:22:05.000000 django_statici18n-2.5.0/src/django_statici18n.egg-info/dependency_links.txt
+-rw-r--r--   0 zyegfryed   (501) staff       (20)        1 2020-09-18 12:32:22.000000 django_statici18n-2.5.0/src/django_statici18n.egg-info/not-zip-safe
+-rw-r--r--   0 zyegfryed   (501) staff       (20)       32 2024-04-20 13:22:05.000000 django_statici18n-2.5.0/src/django_statici18n.egg-info/requires.txt
+-rw-r--r--   0 zyegfryed   (501) staff       (20)       11 2024-04-20 13:22:05.000000 django_statici18n-2.5.0/src/django_statici18n.egg-info/top_level.txt
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2024-04-20 13:22:05.194592 django_statici18n-2.5.0/src/statici18n/
+-rw-r--r--   0 zyegfryed   (501) staff       (20)      146 2024-04-20 12:57:21.000000 django_statici18n-2.5.0/src/statici18n/__init__.py
+-rw-r--r--   0 zyegfryed   (501) staff       (20)      152 2020-10-04 11:35:11.000000 django_statici18n-2.5.0/src/statici18n/apps.py
+-rw-r--r--   0 zyegfryed   (501) staff       (20)      697 2020-10-04 11:35:11.000000 django_statici18n-2.5.0/src/statici18n/conf.py
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2024-04-20 13:22:05.195341 django_statici18n-2.5.0/src/statici18n/management/
+-rw-r--r--   0 zyegfryed   (501) staff       (20)        0 2020-09-18 12:18:49.000000 django_statici18n-2.5.0/src/statici18n/management/__init__.py
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2024-04-20 13:22:05.197386 django_statici18n-2.5.0/src/statici18n/management/commands/
+-rw-r--r--   0 zyegfryed   (501) staff       (20)        0 2020-09-18 12:18:49.000000 django_statici18n-2.5.0/src/statici18n/management/commands/__init__.py
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     5505 2024-04-20 12:56:23.000000 django_statici18n-2.5.0/src/statici18n/management/commands/compilejsi18n.py
+drwxr-xr-x   0 zyegfryed   (501) staff       (20)        0 2024-04-20 13:22:05.217235 django_statici18n-2.5.0/src/statici18n/templatetags/
+-rw-r--r--   0 zyegfryed   (501) staff       (20)        0 2020-09-18 12:18:49.000000 django_statici18n-2.5.0/src/statici18n/templatetags/__init__.py
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     1107 2020-10-04 11:35:11.000000 django_statici18n-2.5.0/src/statici18n/templatetags/statici18n.py
+-rw-r--r--   0 zyegfryed   (501) staff       (20)     1529 2024-04-20 12:56:23.000000 django_statici18n-2.5.0/src/statici18n/utils.py
```

### Comparing `django-statici18n-2.4.0/LICENSE` & `django_statici18n-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-statici18n-2.4.0/PKG-INFO` & `django_statici18n-2.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,142 +1,144 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-statici18n
-Version: 2.4.0
+Version: 2.5.0
 Summary: A Django app that compiles i18n JavaScript catalogs to static files.
 Home-page: http://django-statici18n.readthedocs.org/
 Author: Sebastien Fievet
 Author-email: zyegfryed@gmail.com
 License: BSD
 Project-URL: Source, https://github.com/zyegfryed/django-statici18n
-Description: django-statici18n
-        =================
-        
-        .. image:: https://github.com/zyegfryed/django-statici18n/actions/workflows/build.yml/badge.svg?branch=main
-           :alt: Build Status
-           :target: https://github.com/zyegfryed/django-statici18n/actions
-        
-        .. image:: https://codecov.io/gh/zyegfryed/django-statici18n/branch/main/graph/badge.svg?token=xiaDYAr30F
-           :target: https://codecov.io/gh/zyegfryed/django-statici18n
-        
-        Overview
-        --------
-        
-        When dealing with internationalization in JavaScript code, Django provides
-        the `JSONCatalog view`_ which sends out a JavaScript code library with
-        functions that mimic the gettext interface, plus an array of translation
-        strings.
-        
-        At first glance, it works well and everything is fine. But, because
-        `JSONCatalog view`_ is generating JavaScript catalog dynamically on each
-        and every request, it's `adding an overhead`_ that can be an issue with
-        site growth.
-        
-        That's what ``django-statici18n`` is for:
-        
-            Collecting JavaScript catalogs from each of your Django apps (and any
-            other place you specify) into a single location that can easily be
-            served in production.
-        
-        The main website for ``django-statici18n`` is
-        `github.com/zyegfryed/django-statici18n`_ where you can also file tickets.
-        
-        .. _JSONCatalog view: https://docs.djangoproject.com/en/3.2/topics/i18n/translation/#the-jsoncatalog-view
-        .. _adding an overhead: https://docs.djangoproject.com/en/3.2/topics/i18n/translation/#note-on-performance
-        .. _github.com/zyegfryed/django-statici18n: https://github.com/zyegfryed/django-statici18n
-        
-        Supported Django Versions
-        -------------------------
-        
-        ``django-statici18n`` works with all the Django versions officially
-        supported by the Django project. At this time of writing, these are the
-        3.2 (LTS), 4.1, 4.2 series.
-        
-        Installation
-        ------------
-        
-        1. Use your favorite Python packaging tool to install ``django-statici18n``
-           from `PyPI`_, e.g.::
-        
-            pip install django-statici18n
-        
-        2. Add ``'statici18n'`` to your ``INSTALLED_APPS`` setting::
-        
-            INSTALLED_APPS = [
-                # ...
-                'statici18n',
-            ]
-        
-        3. Once you have `translated`_ and `compiled`_ your messages, use the
-           ``compilejsi18n`` management command::
-        
-            python manage.py compilejsi18n
-        
-        4. Add the `django.core.context_processors.i18n`_ context processor to the
-           ``context_processors`` section for your backend in the ``TEMPLATES``
-           setting - it should have already been set by Django::
-        
-            TEMPLATES = [
-              {
-                # ...
-                'OPTIONS': {
-                  'context_processors': {
-                    # ...
-                    'django.template.context_processors.i18n',
-                  },
-                },
-              },
-            ]
-        
-        5. Edit your template(s) and replace the `dynamically generated script`_ by the
-           statically generated one:
-        
-          .. code-block:: html+django
-        
-            <script src="{{ STATIC_URL }}jsi18n/{{ LANGUAGE_CODE }}/djangojs.js"></script>
-        
-        .. note::
-        
-            By default, the generated catalogs are stored to ``STATIC_ROOT/jsi18n``.
-            You can modify the output path and more options by tweaking
-            ``django-statici18n`` settings.
-        
-        **(Optional)**
-        
-        The following step assumes you're using `django.contrib.staticfiles`_.
-        
-        5. Edit your template(s) and use the provided template tag:
-        
-          .. code-block:: html+django
-        
-            {% load statici18n %}
-            <script src="{% statici18n LANGUAGE_CODE %}"></script>
-        
-        6. Or inline the JavaScript directly in your template:
-        
-          .. code-block:: html+django
-        
-            {% load statici18n %}
-            <script>{% inlinei18n LANGUAGE_CODE %}</script>
-        
-        .. _PyPI: http://pypi.python.org/pypi/django-statici18n
-        .. _translated: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#message-files
-        .. _compiled: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#compiling-message-files
-        .. _django.core.context_processors.i18n: https://docs.djangoproject.com/en/4.2/ref/templates/api/#django-template-context-processors-i18n
-        .. _Upgrading templates to Django 1.8: https://docs.djangoproject.com/en/2.2/ref/templates/upgrading/
-        .. _dynamically generated script: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#using-the-javascript-translation-catalog
-        .. _django.contrib.staticfiles: https://docs.djangoproject.com/en/4.2/ref/contrib/staticfiles/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+Requires-Dist: Django>=3.2
+Requires-Dist: django-appconf>=1.0
+
+django-statici18n
+=================
+
+.. image:: https://github.com/zyegfryed/django-statici18n/actions/workflows/build.yml/badge.svg?branch=main
+   :alt: Build Status
+   :target: https://github.com/zyegfryed/django-statici18n/actions
+
+.. image:: https://codecov.io/gh/zyegfryed/django-statici18n/branch/main/graph/badge.svg?token=xiaDYAr30F
+   :target: https://codecov.io/gh/zyegfryed/django-statici18n
+
+Overview
+--------
+
+When dealing with internationalization in JavaScript code, Django provides
+the `JSONCatalog view`_ which sends out a JavaScript code library with
+functions that mimic the gettext interface, plus an array of translation
+strings.
+
+At first glance, it works well and everything is fine. But, because
+`JSONCatalog view`_ is generating JavaScript catalog dynamically on each
+and every request, it's `adding an overhead`_ that can be an issue with
+site growth.
+
+That's what ``django-statici18n`` is for:
+
+    Collecting JavaScript catalogs from each of your Django apps (and any
+    other place you specify) into a single location that can easily be
+    served in production.
+
+The main website for ``django-statici18n`` is
+`github.com/zyegfryed/django-statici18n`_ where you can also file tickets.
+
+.. _JSONCatalog view: https://docs.djangoproject.com/en/3.2/topics/i18n/translation/#the-jsoncatalog-view
+.. _adding an overhead: https://docs.djangoproject.com/en/3.2/topics/i18n/translation/#note-on-performance
+.. _github.com/zyegfryed/django-statici18n: https://github.com/zyegfryed/django-statici18n
+
+Supported Django Versions
+-------------------------
+
+``django-statici18n`` works with all the Django versions officially
+supported by the Django project. At this time of writing, these are the
+3.2 (LTS), 4.1, 4.2 series.
+
+Installation
+------------
+
+1. Use your favorite Python packaging tool to install ``django-statici18n``
+   from `PyPI`_, e.g.::
+
+    pip install django-statici18n
+
+2. Add ``'statici18n'`` to your ``INSTALLED_APPS`` setting::
+
+    INSTALLED_APPS = [
+        # ...
+        'statici18n',
+    ]
+
+3. Once you have `translated`_ and `compiled`_ your messages, use the
+   ``compilejsi18n`` management command::
+
+    python manage.py compilejsi18n
+
+4. Add the `django.core.context_processors.i18n`_ context processor to the
+   ``context_processors`` section for your backend in the ``TEMPLATES``
+   setting - it should have already been set by Django::
+
+    TEMPLATES = [
+      {
+        # ...
+        'OPTIONS': {
+          'context_processors': {
+            # ...
+            'django.template.context_processors.i18n',
+          },
+        },
+      },
+    ]
+
+5. Edit your template(s) and replace the `dynamically generated script`_ by the
+   statically generated one:
+
+  .. code-block:: html+django
+
+    <script src="{{ STATIC_URL }}jsi18n/{{ LANGUAGE_CODE }}/djangojs.js"></script>
+
+.. note::
+
+    By default, the generated catalogs are stored to ``STATIC_ROOT/jsi18n``.
+    You can modify the output path and more options by tweaking
+    ``django-statici18n`` settings.
+
+**(Optional)**
+
+The following step assumes you're using `django.contrib.staticfiles`_.
+
+5. Edit your template(s) and use the provided template tag:
+
+  .. code-block:: html+django
+
+    {% load statici18n %}
+    <script src="{% statici18n LANGUAGE_CODE %}"></script>
+
+6. Or inline the JavaScript directly in your template:
+
+  .. code-block:: html+django
+
+    {% load statici18n %}
+    <script>{% inlinei18n LANGUAGE_CODE %}</script>
+
+.. _PyPI: http://pypi.python.org/pypi/django-statici18n
+.. _translated: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#message-files
+.. _compiled: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#compiling-message-files
+.. _django.core.context_processors.i18n: https://docs.djangoproject.com/en/4.2/ref/templates/api/#django-template-context-processors-i18n
+.. _Upgrading templates to Django 1.8: https://docs.djangoproject.com/en/2.2/ref/templates/upgrading/
+.. _dynamically generated script: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#using-the-javascript-translation-catalog
+.. _django.contrib.staticfiles: https://docs.djangoproject.com/en/4.2/ref/contrib/staticfiles/
```

#### html2text {}

```diff
@@ -1,17 +1,27 @@
-Metadata-Version: 1.2 Name: django-statici18n Version: 2.4.0 Summary: A Django
+Metadata-Version: 2.1 Name: django-statici18n Version: 2.5.0 Summary: A Django
 app that compiles i18n JavaScript catalogs to static files. Home-page: http://
 django-statici18n.readthedocs.org/ Author: Sebastien Fievet Author-email:
 zyegfryed@gmail.com License: BSD Project-URL: Source, https://github.com/
-zyegfryed/django-statici18n Description: django-statici18n ================= ..
-image:: https://github.com/zyegfryed/django-statici18n/actions/workflows/
-build.yml/badge.svg?branch=main :alt: Build Status :target: https://github.com/
-zyegfryed/django-statici18n/actions .. image:: https://codecov.io/gh/zyegfryed/
-django-statici18n/branch/main/graph/badge.svg?token=xiaDYAr30F :target: https:/
-/codecov.io/gh/zyegfryed/django-statici18n Overview -------- When dealing with
+zyegfryed/django-statici18n Classifier: Development Status :: 5 - Production/
+Stable Classifier: Environment :: Web Environment Classifier: Framework ::
+Django Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: BSD License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 License-File: LICENSE Requires-Dist: Django>=3.2 Requires-Dist:
+django-appconf>=1.0 django-statici18n ================= .. image:: https://
+github.com/zyegfryed/django-statici18n/actions/workflows/build.yml/
+badge.svg?branch=main :alt: Build Status :target: https://github.com/zyegfryed/
+django-statici18n/actions .. image:: https://codecov.io/gh/zyegfryed/django-
+statici18n/branch/main/graph/badge.svg?token=xiaDYAr30F :target: https://
+codecov.io/gh/zyegfryed/django-statici18n Overview -------- When dealing with
 internationalization in JavaScript code, Django provides the `JSONCatalog
 view`_ which sends out a JavaScript code library with functions that mimic the
 gettext interface, plus an array of translation strings. At first glance, it
 works well and everything is fine. But, because `JSONCatalog view`_ is
 generating JavaScript catalog dynamically on each and every request, it's
 `adding an overhead`_ that can be an issue with site growth. That's what
 ``django-statici18n`` is for: Collecting JavaScript catalogs from each of your
@@ -50,17 +60,8 @@
 #compiling-message-files .. _django.core.context_processors.i18n: https://
 docs.djangoproject.com/en/4.2/ref/templates/api/#django-template-context-
 processors-i18n .. _Upgrading templates to Django 1.8: https://
 docs.djangoproject.com/en/2.2/ref/templates/upgrading/ .. _dynamically
 generated script: https://docs.djangoproject.com/en/4.2/topics/i18n/
 translation/#using-the-javascript-translation-catalog ..
 _django.contrib.staticfiles: https://docs.djangoproject.com/en/4.2/ref/contrib/
-staticfiles/ Platform: UNKNOWN Classifier: Development Status :: 5 -
-Production/Stable Classifier: Environment :: Web Environment Classifier:
-Framework :: Django Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: BSD License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11
+staticfiles/
```

### Comparing `django-statici18n-2.4.0/README.rst` & `django_statici18n-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-statici18n-2.4.0/setup.py` & `django_statici18n-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="django-statici18n",
-    version="2.4.0",
+    version="2.5.0",
     author="Sebastien Fievet",
     author_email="zyegfryed@gmail.com",
     url="http://django-statici18n.readthedocs.org/",
     description=("A Django app that compiles i18n JavaScript catalogs "
                  "to static files."),
     long_description=open("README.rst").read(),
     package_dir={"": "src"},
```

### Comparing `django-statici18n-2.4.0/src/django_statici18n.egg-info/PKG-INFO` & `django_statici18n-2.5.0/src/django_statici18n.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,142 +1,144 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-statici18n
-Version: 2.4.0
+Version: 2.5.0
 Summary: A Django app that compiles i18n JavaScript catalogs to static files.
 Home-page: http://django-statici18n.readthedocs.org/
 Author: Sebastien Fievet
 Author-email: zyegfryed@gmail.com
 License: BSD
 Project-URL: Source, https://github.com/zyegfryed/django-statici18n
-Description: django-statici18n
-        =================
-        
-        .. image:: https://github.com/zyegfryed/django-statici18n/actions/workflows/build.yml/badge.svg?branch=main
-           :alt: Build Status
-           :target: https://github.com/zyegfryed/django-statici18n/actions
-        
-        .. image:: https://codecov.io/gh/zyegfryed/django-statici18n/branch/main/graph/badge.svg?token=xiaDYAr30F
-           :target: https://codecov.io/gh/zyegfryed/django-statici18n
-        
-        Overview
-        --------
-        
-        When dealing with internationalization in JavaScript code, Django provides
-        the `JSONCatalog view`_ which sends out a JavaScript code library with
-        functions that mimic the gettext interface, plus an array of translation
-        strings.
-        
-        At first glance, it works well and everything is fine. But, because
-        `JSONCatalog view`_ is generating JavaScript catalog dynamically on each
-        and every request, it's `adding an overhead`_ that can be an issue with
-        site growth.
-        
-        That's what ``django-statici18n`` is for:
-        
-            Collecting JavaScript catalogs from each of your Django apps (and any
-            other place you specify) into a single location that can easily be
-            served in production.
-        
-        The main website for ``django-statici18n`` is
-        `github.com/zyegfryed/django-statici18n`_ where you can also file tickets.
-        
-        .. _JSONCatalog view: https://docs.djangoproject.com/en/3.2/topics/i18n/translation/#the-jsoncatalog-view
-        .. _adding an overhead: https://docs.djangoproject.com/en/3.2/topics/i18n/translation/#note-on-performance
-        .. _github.com/zyegfryed/django-statici18n: https://github.com/zyegfryed/django-statici18n
-        
-        Supported Django Versions
-        -------------------------
-        
-        ``django-statici18n`` works with all the Django versions officially
-        supported by the Django project. At this time of writing, these are the
-        3.2 (LTS), 4.1, 4.2 series.
-        
-        Installation
-        ------------
-        
-        1. Use your favorite Python packaging tool to install ``django-statici18n``
-           from `PyPI`_, e.g.::
-        
-            pip install django-statici18n
-        
-        2. Add ``'statici18n'`` to your ``INSTALLED_APPS`` setting::
-        
-            INSTALLED_APPS = [
-                # ...
-                'statici18n',
-            ]
-        
-        3. Once you have `translated`_ and `compiled`_ your messages, use the
-           ``compilejsi18n`` management command::
-        
-            python manage.py compilejsi18n
-        
-        4. Add the `django.core.context_processors.i18n`_ context processor to the
-           ``context_processors`` section for your backend in the ``TEMPLATES``
-           setting - it should have already been set by Django::
-        
-            TEMPLATES = [
-              {
-                # ...
-                'OPTIONS': {
-                  'context_processors': {
-                    # ...
-                    'django.template.context_processors.i18n',
-                  },
-                },
-              },
-            ]
-        
-        5. Edit your template(s) and replace the `dynamically generated script`_ by the
-           statically generated one:
-        
-          .. code-block:: html+django
-        
-            <script src="{{ STATIC_URL }}jsi18n/{{ LANGUAGE_CODE }}/djangojs.js"></script>
-        
-        .. note::
-        
-            By default, the generated catalogs are stored to ``STATIC_ROOT/jsi18n``.
-            You can modify the output path and more options by tweaking
-            ``django-statici18n`` settings.
-        
-        **(Optional)**
-        
-        The following step assumes you're using `django.contrib.staticfiles`_.
-        
-        5. Edit your template(s) and use the provided template tag:
-        
-          .. code-block:: html+django
-        
-            {% load statici18n %}
-            <script src="{% statici18n LANGUAGE_CODE %}"></script>
-        
-        6. Or inline the JavaScript directly in your template:
-        
-          .. code-block:: html+django
-        
-            {% load statici18n %}
-            <script>{% inlinei18n LANGUAGE_CODE %}</script>
-        
-        .. _PyPI: http://pypi.python.org/pypi/django-statici18n
-        .. _translated: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#message-files
-        .. _compiled: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#compiling-message-files
-        .. _django.core.context_processors.i18n: https://docs.djangoproject.com/en/4.2/ref/templates/api/#django-template-context-processors-i18n
-        .. _Upgrading templates to Django 1.8: https://docs.djangoproject.com/en/2.2/ref/templates/upgrading/
-        .. _dynamically generated script: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#using-the-javascript-translation-catalog
-        .. _django.contrib.staticfiles: https://docs.djangoproject.com/en/4.2/ref/contrib/staticfiles/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+Requires-Dist: Django>=3.2
+Requires-Dist: django-appconf>=1.0
+
+django-statici18n
+=================
+
+.. image:: https://github.com/zyegfryed/django-statici18n/actions/workflows/build.yml/badge.svg?branch=main
+   :alt: Build Status
+   :target: https://github.com/zyegfryed/django-statici18n/actions
+
+.. image:: https://codecov.io/gh/zyegfryed/django-statici18n/branch/main/graph/badge.svg?token=xiaDYAr30F
+   :target: https://codecov.io/gh/zyegfryed/django-statici18n
+
+Overview
+--------
+
+When dealing with internationalization in JavaScript code, Django provides
+the `JSONCatalog view`_ which sends out a JavaScript code library with
+functions that mimic the gettext interface, plus an array of translation
+strings.
+
+At first glance, it works well and everything is fine. But, because
+`JSONCatalog view`_ is generating JavaScript catalog dynamically on each
+and every request, it's `adding an overhead`_ that can be an issue with
+site growth.
+
+That's what ``django-statici18n`` is for:
+
+    Collecting JavaScript catalogs from each of your Django apps (and any
+    other place you specify) into a single location that can easily be
+    served in production.
+
+The main website for ``django-statici18n`` is
+`github.com/zyegfryed/django-statici18n`_ where you can also file tickets.
+
+.. _JSONCatalog view: https://docs.djangoproject.com/en/3.2/topics/i18n/translation/#the-jsoncatalog-view
+.. _adding an overhead: https://docs.djangoproject.com/en/3.2/topics/i18n/translation/#note-on-performance
+.. _github.com/zyegfryed/django-statici18n: https://github.com/zyegfryed/django-statici18n
+
+Supported Django Versions
+-------------------------
+
+``django-statici18n`` works with all the Django versions officially
+supported by the Django project. At this time of writing, these are the
+3.2 (LTS), 4.1, 4.2 series.
+
+Installation
+------------
+
+1. Use your favorite Python packaging tool to install ``django-statici18n``
+   from `PyPI`_, e.g.::
+
+    pip install django-statici18n
+
+2. Add ``'statici18n'`` to your ``INSTALLED_APPS`` setting::
+
+    INSTALLED_APPS = [
+        # ...
+        'statici18n',
+    ]
+
+3. Once you have `translated`_ and `compiled`_ your messages, use the
+   ``compilejsi18n`` management command::
+
+    python manage.py compilejsi18n
+
+4. Add the `django.core.context_processors.i18n`_ context processor to the
+   ``context_processors`` section for your backend in the ``TEMPLATES``
+   setting - it should have already been set by Django::
+
+    TEMPLATES = [
+      {
+        # ...
+        'OPTIONS': {
+          'context_processors': {
+            # ...
+            'django.template.context_processors.i18n',
+          },
+        },
+      },
+    ]
+
+5. Edit your template(s) and replace the `dynamically generated script`_ by the
+   statically generated one:
+
+  .. code-block:: html+django
+
+    <script src="{{ STATIC_URL }}jsi18n/{{ LANGUAGE_CODE }}/djangojs.js"></script>
+
+.. note::
+
+    By default, the generated catalogs are stored to ``STATIC_ROOT/jsi18n``.
+    You can modify the output path and more options by tweaking
+    ``django-statici18n`` settings.
+
+**(Optional)**
+
+The following step assumes you're using `django.contrib.staticfiles`_.
+
+5. Edit your template(s) and use the provided template tag:
+
+  .. code-block:: html+django
+
+    {% load statici18n %}
+    <script src="{% statici18n LANGUAGE_CODE %}"></script>
+
+6. Or inline the JavaScript directly in your template:
+
+  .. code-block:: html+django
+
+    {% load statici18n %}
+    <script>{% inlinei18n LANGUAGE_CODE %}</script>
+
+.. _PyPI: http://pypi.python.org/pypi/django-statici18n
+.. _translated: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#message-files
+.. _compiled: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#compiling-message-files
+.. _django.core.context_processors.i18n: https://docs.djangoproject.com/en/4.2/ref/templates/api/#django-template-context-processors-i18n
+.. _Upgrading templates to Django 1.8: https://docs.djangoproject.com/en/2.2/ref/templates/upgrading/
+.. _dynamically generated script: https://docs.djangoproject.com/en/4.2/topics/i18n/translation/#using-the-javascript-translation-catalog
+.. _django.contrib.staticfiles: https://docs.djangoproject.com/en/4.2/ref/contrib/staticfiles/
```

#### html2text {}

```diff
@@ -1,17 +1,27 @@
-Metadata-Version: 1.2 Name: django-statici18n Version: 2.4.0 Summary: A Django
+Metadata-Version: 2.1 Name: django-statici18n Version: 2.5.0 Summary: A Django
 app that compiles i18n JavaScript catalogs to static files. Home-page: http://
 django-statici18n.readthedocs.org/ Author: Sebastien Fievet Author-email:
 zyegfryed@gmail.com License: BSD Project-URL: Source, https://github.com/
-zyegfryed/django-statici18n Description: django-statici18n ================= ..
-image:: https://github.com/zyegfryed/django-statici18n/actions/workflows/
-build.yml/badge.svg?branch=main :alt: Build Status :target: https://github.com/
-zyegfryed/django-statici18n/actions .. image:: https://codecov.io/gh/zyegfryed/
-django-statici18n/branch/main/graph/badge.svg?token=xiaDYAr30F :target: https:/
-/codecov.io/gh/zyegfryed/django-statici18n Overview -------- When dealing with
+zyegfryed/django-statici18n Classifier: Development Status :: 5 - Production/
+Stable Classifier: Environment :: Web Environment Classifier: Framework ::
+Django Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: BSD License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 License-File: LICENSE Requires-Dist: Django>=3.2 Requires-Dist:
+django-appconf>=1.0 django-statici18n ================= .. image:: https://
+github.com/zyegfryed/django-statici18n/actions/workflows/build.yml/
+badge.svg?branch=main :alt: Build Status :target: https://github.com/zyegfryed/
+django-statici18n/actions .. image:: https://codecov.io/gh/zyegfryed/django-
+statici18n/branch/main/graph/badge.svg?token=xiaDYAr30F :target: https://
+codecov.io/gh/zyegfryed/django-statici18n Overview -------- When dealing with
 internationalization in JavaScript code, Django provides the `JSONCatalog
 view`_ which sends out a JavaScript code library with functions that mimic the
 gettext interface, plus an array of translation strings. At first glance, it
 works well and everything is fine. But, because `JSONCatalog view`_ is
 generating JavaScript catalog dynamically on each and every request, it's
 `adding an overhead`_ that can be an issue with site growth. That's what
 ``django-statici18n`` is for: Collecting JavaScript catalogs from each of your
@@ -50,17 +60,8 @@
 #compiling-message-files .. _django.core.context_processors.i18n: https://
 docs.djangoproject.com/en/4.2/ref/templates/api/#django-template-context-
 processors-i18n .. _Upgrading templates to Django 1.8: https://
 docs.djangoproject.com/en/2.2/ref/templates/upgrading/ .. _dynamically
 generated script: https://docs.djangoproject.com/en/4.2/topics/i18n/
 translation/#using-the-javascript-translation-catalog ..
 _django.contrib.staticfiles: https://docs.djangoproject.com/en/4.2/ref/contrib/
-staticfiles/ Platform: UNKNOWN Classifier: Development Status :: 5 -
-Production/Stable Classifier: Environment :: Web Environment Classifier:
-Framework :: Django Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: BSD License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11
+staticfiles/
```

### Comparing `django-statici18n-2.4.0/src/django_statici18n.egg-info/SOURCES.txt` & `django_statici18n-2.5.0/src/django_statici18n.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-statici18n-2.4.0/src/statici18n/conf.py` & `django_statici18n-2.5.0/src/statici18n/conf.py`

 * *Files identical despite different names*

### Comparing `django-statici18n-2.4.0/src/statici18n/management/commands/compilejsi18n.py` & `django_statici18n-2.5.0/src/statici18n/management/commands/compilejsi18n.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,15 +101,21 @@
         # currently not used by django
         response = catalog.get(self, None, domain=domain, packages=packages)
         return force_str(response.content)
 
     def _create_output(
         self, outputdir, outputformat, locale, domain, packages, namespace
     ):
-        outputfile = os.path.join(outputdir, get_filename(locale, domain, outputformat))
+        try:
+            filename = get_filename(locale, domain, outputformat)
+        except LookupError:
+            # Silence error for backward-compatibility
+            return ""
+
+        outputfile = os.path.join(outputdir, filename)
         basedir = os.path.dirname(outputfile)
         if not os.path.isdir(basedir):
             os.makedirs(basedir)
 
         if outputformat == "js":
             data = self._create_javascript_catalog(locale, domain, packages)
             if namespace:
```

### Comparing `django-statici18n-2.4.0/src/statici18n/templatetags/statici18n.py` & `django_statici18n-2.5.0/src/statici18n/templatetags/statici18n.py`

 * *Files identical despite different names*

### Comparing `django-statici18n-2.4.0/src/statici18n/utils.py` & `django_statici18n-2.5.0/src/statici18n/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,47 @@
+import os
 from collections.abc import Sequence
 from importlib import import_module
-import os
+
+from django.utils.translation import get_supported_language_variant
+from django.utils.translation.trans_real import to_language
 
 from statici18n.conf import settings
 
 
 def get_mod_func(callback):
     """
     Converts 'django.views.news.stories.story_detail' to
     ('django.views.news.stories', 'story_detail')
     """
     try:
         dot = callback.rindex(".")
     except ValueError:
         return callback, ""
-    return callback[:dot], callback[dot + 1 :]
+    return callback[:dot], callback[dot + 1:]
 
 
 def get_filename(*args, **kwargs):
     try:
         mod_name, func_name = get_mod_func(settings.STATICI18N_FILENAME_FUNCTION)
         _filename_func = getattr(import_module(mod_name), func_name)
     except (AttributeError, ImportError) as e:
         raise ImportError(
             "Couldn't import filename function %s: %s"
             % (settings.STATICI18N_FILENAME_FUNCTION, e)
         )
     return _filename_func(*args, **kwargs)
 
 
-def default_filename(language_code, domain, output_format="js"):
+def default_filename(locale, domain, output_format="js"):
+    language_code = get_supported_language_variant(locale)
     return os.path.join(language_code, "%s.%s" % (domain, output_format))
 
 
 def legacy_filename(locale, domain, output_format="js"):
-    from django.utils.translation.trans_real import to_language
-
     return os.path.join(to_language(locale), "%s.%s" % (domain, output_format))
 
 
 def get_packages(packages):
     if packages == "django.conf":
         return None
```

