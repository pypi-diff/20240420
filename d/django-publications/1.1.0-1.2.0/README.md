# Comparing `tmp/django-publications-1.1.0.tar.gz` & `tmp/django_publications-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/theis/Downloads/django-publications/dist/tmp6lgjt3wd/django-publications-1.1.0.tar", last modified: Tue Sep 28 10:41:15 2021, max compression
+gzip compressed data, was "django_publications-1.2.0.tar", last modified: Sat Apr 20 17:20:30 2024, max compression
```

## Comparing `django-publications-1.1.0.tar` & `django_publications-1.2.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/
--rw-r--r--   0 theis    (760877) primarygroup (89939)      705 2021-09-28 10:41:15.000000 django-publications-1.1.0/PKG-INFO
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1060 2021-09-28 10:39:19.000000 django-publications-1.1.0/LICENSE
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/django_publications.egg-info/
--rw-r--r--   0 theis    (760877) primarygroup (89939)      705 2021-09-28 10:41:15.000000 django-publications-1.1.0/django_publications.egg-info/PKG-INFO
--rw-r--r--   0 theis    (760877) primarygroup (89939)        1 2021-09-28 10:41:14.000000 django-publications-1.1.0/django_publications.egg-info/not-zip-safe
--rw-r--r--   0 theis    (760877) primarygroup (89939)     2639 2021-09-28 10:41:15.000000 django-publications-1.1.0/django_publications.egg-info/SOURCES.txt
--rw-r--r--   0 theis    (760877) primarygroup (89939)       28 2021-09-28 10:41:15.000000 django-publications-1.1.0/django_publications.egg-info/requires.txt
--rw-r--r--   0 theis    (760877) primarygroup (89939)       13 2021-09-28 10:41:15.000000 django-publications-1.1.0/django_publications.egg-info/top_level.txt
--rw-r--r--   0 theis    (760877) primarygroup (89939)        1 2021-09-28 10:41:15.000000 django-publications-1.1.0/django_publications.egg-info/dependency_links.txt
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/templatetags/
--rw-r--r--   0 theis    (760877) primarygroup (89939)     3043 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templatetags/publication_extras.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)      151 2021-09-28 10:30:39.000000 django-publications-1.1.0/publications/templatetags/__init__.py
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/migrations/
--rw-r--r--   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/migrations/__init__.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     5844 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/migrations/0001_initial.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)      429 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/migrations/0002_initial_data.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1720 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/fields.py
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/tests/
--rw-r--r--   0 theis    (760877) primarygroup (89939)       57 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/tests/__init__.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1919 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/tests/tests_live.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)    12057 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/tests/tests.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)      415 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/tests/urls.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1887 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/tests/__main__.py
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/admin/
--rw-r--r--   0 theis    (760877) primarygroup (89939)      529 2021-09-28 10:30:39.000000 django-publications-1.1.0/publications/admin/__init__.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)      310 2021-09-28 10:30:39.000000 django-publications-1.1.0/publications/admin/typeadmin.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)      261 2021-09-28 10:30:39.000000 django-publications-1.1.0/publications/admin/listadmin.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1550 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/admin/publicationadmin.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     4975 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/admin/orderedmodeladmin.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)      173 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/__init__.py
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/models/
--rw-r--r--   0 theis    (760877) primarygroup (89939)      562 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/models/customlink.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)      534 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/models/list.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     7712 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/models/orderedmodel.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)      344 2021-09-28 10:30:39.000000 django-publications-1.1.0/publications/models/__init__.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     2043 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/models/type.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)      571 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/models/customfile.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)    10504 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/models/publication.py
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/admin_views/
--rw-r--r--   0 theis    (760877) primarygroup (89939)      193 2021-09-28 10:30:39.000000 django-publications-1.1.0/publications/admin_views/__init__.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     4611 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/admin_views/import_bibtex.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)      624 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/utils.py
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/static/
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/static/ordered_model/
--rw-r--r--   0 theis    (760877) primarygroup (89939)      838 2021-09-28 10:30:39.000000 django-publications-1.1.0/publications/static/ordered_model/arrow-up.gif
--rw-r--r--   0 theis    (760877) primarygroup (89939)       80 2021-09-28 10:30:39.000000 django-publications-1.1.0/publications/static/ordered_model/arrow-down.gif
--rw-r--r--   0 theis    (760877) primarygroup (89939)    23462 2021-09-28 10:30:39.000000 django-publications-1.1.0/publications/six.py
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/templates/
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1722 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/base.html
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/templates/publications/
--rw-r--r--   0 theis    (760877) primarygroup (89939)      135 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/publications/publications.bib
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1072 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/publications/publications.ris
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1954 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/publications/id.html
--rw-r--r--   0 theis    (760877) primarygroup (89939)     2955 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/publications/publication.html
--rw-r--r--   0 theis    (760877) primarygroup (89939)     2022 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/publications/publications.mods
--rw-r--r--   0 theis    (760877) primarygroup (89939)      687 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/publications/list.html
--rw-r--r--   0 theis    (760877) primarygroup (89939)      940 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/publications/author.html
--rw-r--r--   0 theis    (760877) primarygroup (89939)      946 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/publications/person.html
--rw-r--r--   0 theis    (760877) primarygroup (89939)      780 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/publications/publications.txt
--rw-r--r--   0 theis    (760877) primarygroup (89939)      732 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/publications/publications_with_thumbnails.html
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1303 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/publications/publication.bib
--rw-r--r--   0 theis    (760877) primarygroup (89939)      825 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/publications/years.html
--rw-r--r--   0 theis    (760877) primarygroup (89939)      749 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/publications/keyword.html
--rw-r--r--   0 theis    (760877) primarygroup (89939)      179 2021-09-28 10:30:39.000000 django-publications-1.1.0/publications/templates/publications/publications.html
--rw-r--r--   0 theis    (760877) primarygroup (89939)      724 2021-09-28 10:30:39.000000 django-publications-1.1.0/publications/templates/publications/publications.rss
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/templates/admin/
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/templates/admin/publications/
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1489 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/admin/publications/import_bibtex.html
--rw-r--r--   0 theis    (760877) primarygroup (89939)      392 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/templates/admin/publications/publication_change_list.html
--rw-r--r--   0 theis    (760877) primarygroup (89939)      228 2021-09-28 10:30:39.000000 django-publications-1.1.0/publications/templates/admin/publications/order_controls.html
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/fixtures/
--rw-r--r--   0 theis    (760877) primarygroup (89939)     2467 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/fixtures/test_data.json
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1845 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/fixtures/initial_data.json
--rw-r--r--   0 theis    (760877) primarygroup (89939)     3462 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/bibtex.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)      733 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/urls.py
-drwxr-xr-x   0 theis    (760877) primarygroup (89939)        0 2021-09-28 10:41:15.000000 django-publications-1.1.0/publications/views/
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1966 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/views/year.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1678 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/views/list.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1279 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/views/id.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     2316 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/views/unapi.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     3989 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/views/author.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)      298 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/views/__init__.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1547 2021-09-28 10:39:19.000000 django-publications-1.1.0/publications/views/keyword.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)      143 2021-09-28 10:30:39.000000 django-publications-1.1.0/MANIFEST.in
--rw-r--r--   0 theis    (760877) primarygroup (89939)     1555 2021-09-28 10:39:19.000000 django-publications-1.1.0/README.md
--rw-r--r--   0 theis    (760877) primarygroup (89939)      852 2021-09-28 10:39:19.000000 django-publications-1.1.0/setup.py
--rw-r--r--   0 theis    (760877) primarygroup (89939)       38 2021-09-28 10:41:15.000000 django-publications-1.1.0/setup.cfg
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.911792 django_publications-1.2.0/
+-rw-r--r--   0 lucas      (502) staff       (20)     1060 2016-08-29 10:21:09.000000 django_publications-1.2.0/LICENSE
+-rw-r--r--   0 lucas      (502) staff       (20)      143 2024-04-20 16:40:59.000000 django_publications-1.2.0/MANIFEST.in
+-rw-r--r--   0 lucas      (502) staff       (20)      735 2024-04-20 17:20:30.911047 django_publications-1.2.0/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     1555 2024-04-20 16:47:49.000000 django_publications-1.2.0/README.md
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.910266 django_publications-1.2.0/django_publications.egg-info/
+-rw-r--r--   0 lucas      (502) staff       (20)      735 2024-04-20 17:20:30.000000 django_publications-1.2.0/django_publications.egg-info/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     2639 2024-04-20 17:20:30.000000 django_publications-1.2.0/django_publications.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        1 2024-04-20 17:20:30.000000 django_publications-1.2.0/django_publications.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        1 2024-04-20 17:17:22.000000 django_publications-1.2.0/django_publications.egg-info/not-zip-safe
+-rw-r--r--   0 lucas      (502) staff       (20)       28 2024-04-20 17:20:30.000000 django_publications-1.2.0/django_publications.egg-info/requires.txt
+-rw-r--r--   0 lucas      (502) staff       (20)       13 2024-04-20 17:20:30.000000 django_publications-1.2.0/django_publications.egg-info/top_level.txt
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.877627 django_publications-1.2.0/publications/
+-rw-r--r--   0 lucas      (502) staff       (20)      173 2024-04-20 17:19:27.000000 django_publications-1.2.0/publications/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.880248 django_publications-1.2.0/publications/admin/
+-rw-r--r--   0 lucas      (502) staff       (20)      529 2016-08-21 18:18:31.000000 django_publications-1.2.0/publications/admin/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)      261 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/admin/listadmin.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5141 2024-04-20 16:47:54.000000 django_publications-1.2.0/publications/admin/orderedmodeladmin.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1484 2024-04-20 16:47:54.000000 django_publications-1.2.0/publications/admin/publicationadmin.py
+-rw-r--r--   0 lucas      (502) staff       (20)      310 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/admin/typeadmin.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.881211 django_publications-1.2.0/publications/admin_views/
+-rw-r--r--   0 lucas      (502) staff       (20)      193 2016-08-21 18:18:31.000000 django_publications-1.2.0/publications/admin_views/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4611 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/admin_views/import_bibtex.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3462 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/bibtex.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1720 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/fields.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.882253 django_publications-1.2.0/publications/fixtures/
+-rw-r--r--   0 lucas      (502) staff       (20)     1845 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/fixtures/initial_data.json
+-rw-r--r--   0 lucas      (502) staff       (20)     2467 2016-08-29 10:21:09.000000 django_publications-1.2.0/publications/fixtures/test_data.json
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.883855 django_publications-1.2.0/publications/migrations/
+-rw-r--r--   0 lucas      (502) staff       (20)     5844 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/migrations/0001_initial.py
+-rw-r--r--   0 lucas      (502) staff       (20)      429 2017-01-10 22:04:56.000000 django_publications-1.2.0/publications/migrations/0002_initial_data.py
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2016-08-29 10:21:09.000000 django_publications-1.2.0/publications/migrations/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.887933 django_publications-1.2.0/publications/models/
+-rw-r--r--   0 lucas      (502) staff       (20)      344 2016-08-21 18:18:31.000000 django_publications-1.2.0/publications/models/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)      571 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/models/customfile.py
+-rw-r--r--   0 lucas      (502) staff       (20)      562 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/models/customlink.py
+-rw-r--r--   0 lucas      (502) staff       (20)      534 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/models/list.py
+-rw-r--r--   0 lucas      (502) staff       (20)     7711 2024-04-20 16:47:54.000000 django_publications-1.2.0/publications/models/orderedmodel.py
+-rw-r--r--   0 lucas      (502) staff       (20)    10513 2024-04-20 16:47:54.000000 django_publications-1.2.0/publications/models/publication.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2043 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/models/type.py
+-rw-r--r--   0 lucas      (502) staff       (20)    23462 2016-08-21 18:18:31.000000 django_publications-1.2.0/publications/six.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.869423 django_publications-1.2.0/publications/static/
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.889141 django_publications-1.2.0/publications/static/ordered_model/
+-rw-r--r--   0 lucas      (502) staff       (20)       80 2016-08-21 18:18:32.000000 django_publications-1.2.0/publications/static/ordered_model/arrow-down.gif
+-rw-r--r--   0 lucas      (502) staff       (20)      838 2016-08-21 18:18:32.000000 django_publications-1.2.0/publications/static/ordered_model/arrow-up.gif
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.889699 django_publications-1.2.0/publications/templates/
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.869817 django_publications-1.2.0/publications/templates/admin/
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.891526 django_publications-1.2.0/publications/templates/admin/publications/
+-rw-r--r--   0 lucas      (502) staff       (20)     1489 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/templates/admin/publications/import_bibtex.html
+-rw-r--r--   0 lucas      (502) staff       (20)      228 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/templates/admin/publications/order_controls.html
+-rw-r--r--   0 lucas      (502) staff       (20)      392 2016-08-29 10:21:09.000000 django_publications-1.2.0/publications/templates/admin/publications/publication_change_list.html
+-rw-r--r--   0 lucas      (502) staff       (20)     1722 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/templates/base.html
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.900089 django_publications-1.2.0/publications/templates/publications/
+-rw-r--r--   0 lucas      (502) staff       (20)      940 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/templates/publications/author.html
+-rw-r--r--   0 lucas      (502) staff       (20)     1954 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/templates/publications/id.html
+-rw-r--r--   0 lucas      (502) staff       (20)      749 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/templates/publications/keyword.html
+-rw-r--r--   0 lucas      (502) staff       (20)      687 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/templates/publications/list.html
+-rw-r--r--   0 lucas      (502) staff       (20)      946 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/templates/publications/person.html
+-rw-r--r--   0 lucas      (502) staff       (20)     1303 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/templates/publications/publication.bib
+-rw-r--r--   0 lucas      (502) staff       (20)     2953 2024-04-20 16:47:54.000000 django_publications-1.2.0/publications/templates/publications/publication.html
+-rw-r--r--   0 lucas      (502) staff       (20)      135 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/templates/publications/publications.bib
+-rw-r--r--   0 lucas      (502) staff       (20)      179 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/templates/publications/publications.html
+-rw-r--r--   0 lucas      (502) staff       (20)     2022 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/templates/publications/publications.mods
+-rw-r--r--   0 lucas      (502) staff       (20)     1072 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/templates/publications/publications.ris
+-rw-r--r--   0 lucas      (502) staff       (20)      724 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/templates/publications/publications.rss
+-rw-r--r--   0 lucas      (502) staff       (20)      780 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/templates/publications/publications.txt
+-rw-r--r--   0 lucas      (502) staff       (20)      732 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/templates/publications/publications_with_thumbnails.html
+-rw-r--r--   0 lucas      (502) staff       (20)      825 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/templates/publications/years.html
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.901113 django_publications-1.2.0/publications/templatetags/
+-rw-r--r--   0 lucas      (502) staff       (20)      151 2016-08-21 18:18:32.000000 django_publications-1.2.0/publications/templatetags/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3043 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/templatetags/publication_extras.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.904307 django_publications-1.2.0/publications/tests/
+-rw-r--r--   0 lucas      (502) staff       (20)       57 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/tests/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1887 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/tests/__main__.py
+-rw-r--r--   0 lucas      (502) staff       (20)    12057 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/tests/tests.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1919 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/tests/tests_live.py
+-rw-r--r--   0 lucas      (502) staff       (20)      393 2024-04-20 16:47:54.000000 django_publications-1.2.0/publications/tests/urls.py
+-rw-r--r--   0 lucas      (502) staff       (20)      685 2024-04-20 16:47:54.000000 django_publications-1.2.0/publications/urls.py
+-rw-r--r--   0 lucas      (502) staff       (20)      624 2017-01-10 22:04:56.000000 django_publications-1.2.0/publications/utils.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-04-20 17:20:30.909619 django_publications-1.2.0/publications/views/
+-rw-r--r--   0 lucas      (502) staff       (20)      298 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/views/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3989 2024-04-20 16:47:49.000000 django_publications-1.2.0/publications/views/author.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1279 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/views/id.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1547 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/views/keyword.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1678 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/views/list.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2316 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/views/unapi.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1966 2024-04-20 16:40:59.000000 django_publications-1.2.0/publications/views/year.py
+-rw-r--r--   0 lucas      (502) staff       (20)       38 2024-04-20 17:20:30.911943 django_publications-1.2.0/setup.cfg
+-rw-r--r--   0 lucas      (502) staff       (20)      852 2024-04-20 16:47:49.000000 django_publications-1.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-publications-1.1.0/LICENSE` & `django_publications-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/django_publications.egg-info/SOURCES.txt` & `django_publications-1.2.0/django_publications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templatetags/publication_extras.py` & `django_publications-1.2.0/publications/templatetags/publication_extras.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/migrations/0001_initial.py` & `django_publications-1.2.0/publications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/fields.py` & `django_publications-1.2.0/publications/fields.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/tests/tests_live.py` & `django_publications-1.2.0/publications/tests/tests_live.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/tests/tests.py` & `django_publications-1.2.0/publications/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/tests/__main__.py` & `django_publications-1.2.0/publications/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/admin/__init__.py` & `django_publications-1.2.0/publications/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/admin/publicationadmin.py` & `django_publications-1.2.0/publications/admin/publicationadmin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 __license__ = 'MIT License <http://www.opensource.org/licenses/mit-license.php>'
 __author__ = 'Lucas Theis <lucas@theis.io>'
 __docformat__ = 'epytext'
 
 from django.contrib import admin
-try:
-	from django.conf.urls import url
-except ImportError:
-	from django.conf.urls.defaults import url
+from django.urls import re_path
 from publications.models import CustomLink, CustomFile
 
 import publications.admin_views
 
 class CustomLinkInline(admin.StackedInline):
 	model = CustomLink
 	extra = 1
@@ -42,10 +39,10 @@
 		(None, {'fields':
 			('lists',)}),
 	)
 	inlines = [CustomLinkInline, CustomFileInline]
 
 	def get_urls(self):
 		return [
-				url(r'^import_bibtex/$', publications.admin_views.import_bibtex,
+				re_path(r'^import_bibtex/$', publications.admin_views.import_bibtex,
 					name='publications_publication_import_bibtex'),
 			] + super(PublicationAdmin, self).get_urls()
```

### Comparing `django-publications-1.1.0/publications/admin/orderedmodeladmin.py` & `django_publications-1.2.0/publications/admin/orderedmodeladmin.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,65 +26,78 @@
 """
 
 from functools import update_wrapper
 
 from django.urls import reverse
 from django.http import HttpResponseRedirect
 from django.shortcuts import get_object_or_404
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.template.loader import render_to_string
 from django.contrib import admin
 try:
     from django.contrib.admin.utils import unquote
 except ImportError:
     # Django <= 1.6
     from django.contrib.admin.util import unquote
 from django.contrib.admin.views.main import ChangeList
 from django.db.models.options import Options
+from django import VERSION
 
 # Django <= 1.6
 if not getattr(Options, 'model_name', False):
     Options.model_name = lambda self: self.module_name.lower()
 if not getattr(ChangeList, 'get_queryset', False):
     ChangeList.get_queryset = ChangeList.get_query_set
 
 class OrderedModelAdmin(admin.ModelAdmin):
 
     def get_model_info(self):
         return dict(app=self.model._meta.app_label,
                     model=self.model._meta.model_name)
 
     def get_urls(self):
-        try:
-            from django.conf.urls import url
-        except ImportError:
-            from django.conf.urls.defaults import url
+        from django.urls import re_path
 
         def wrap(view):
             def wrapper(*args, **kwargs):
                 return self.admin_site.admin_view(view)(*args, **kwargs)
             return update_wrapper(wrapper, view)
         return [
-            url(r'^(.+)/move-(up)/$', wrap(self.move_view),
+            re_path(r'^(.+)/move-(up)/$', wrap(self.move_view),
                 name='{app}_{model}_order_up'.format(**self.get_model_info())),
-            url(r'^(.+)/move-(down)/$', wrap(self.move_view),
+            re_path(r'^(.+)/move-(down)/$', wrap(self.move_view),
                 name='{app}_{model}_order_down'.format(**self.get_model_info())),
         ] + super(OrderedModelAdmin, self).get_urls()
 
     def _get_changelist(self, request):
         list_display = self.get_list_display(request)
         list_display_links = self.get_list_display_links(request, list_display)
+        args = (
+            request,
+            self.model,
+            list_display,
+            list_display_links,
+            self.list_filter,
+            self.date_hierarchy,
+            self.search_fields,
+            self.list_select_related,
+            self.list_per_page,
+            self.list_max_show_all,
+            self.list_editable,
+            self,
+        )
+
+        if VERSION >= (2, 1):
+            sortable_by = self.list_display
+            args = args + (sortable_by,)
 
-        cl = ChangeList(request, self.model, list_display,
-                        list_display_links, self.list_filter, self.date_hierarchy,
-                        self.search_fields, self.list_select_related,
-                        self.list_per_page, self.list_max_show_all, self.list_editable,
-                        self, sortable_by=self.list_display)
+        if VERSION >= (4, 0):
+            args = args + (self.search_help_text,)
 
-        return cl
+        return ChangeList(*args)
 
     request_query_string = ''
 
     def changelist_view(self, request, extra_context=None):
         cl = self._get_changelist(request)
         self.request_query_string = cl.get_query_string()
         return super(OrderedModelAdmin, self).changelist_view(request, extra_context)
```

### Comparing `django-publications-1.1.0/publications/models/customlink.py` & `django_publications-1.2.0/publications/models/customlink.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/models/list.py` & `django_publications-1.2.0/publications/models/list.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/models/orderedmodel.py` & `django_publications-1.2.0/publications/models/orderedmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 import warnings
 from django.contrib.contenttypes.models import ContentType
 from django.urls import reverse
 from django.db import models
 from django.db.models import Max, Min, F
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 class OrderedModel(models.Model):
     """
     An abstract model that allows objects to be ordered relative to each other.
     Provides an ``order`` field.
     """
```

### Comparing `django-publications-1.1.0/publications/models/type.py` & `django_publications-1.2.0/publications/models/type.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/models/customfile.py` & `django_publications-1.2.0/publications/models/customfile.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/models/publication.py` & `django_publications-1.2.0/publications/models/publication.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 __license__ = 'MIT License <http://www.opensource.org/licenses/mit-license.php>'
 __author__ = 'Lucas Theis <lucas@theis.io>'
 __docformat__ = 'epytext'
 
 import os
 
 from django.db import models
-from django.utils.http import urlquote_plus
 from django.conf import settings
 from publications.fields import PagesField
 from publications.models import Type, List
 from string import ascii_uppercase
+from urllib.parse import quote_plus as urlquote_plus
 
 if 'django.contrib.sites' in settings.INSTALLED_APPS:
 	from django.contrib.sites.models import Site
 
 class Publication(models.Model):
 	"""
 	Model representing a publication.
```

### Comparing `django-publications-1.1.0/publications/admin_views/import_bibtex.py` & `django_publications-1.2.0/publications/admin_views/import_bibtex.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/utils.py` & `django_publications-1.2.0/publications/utils.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/static/ordered_model/arrow-up.gif` & `django_publications-1.2.0/publications/static/ordered_model/arrow-up.gif`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/six.py` & `django_publications-1.2.0/publications/six.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/base.html` & `django_publications-1.2.0/publications/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/publications/publications.ris` & `django_publications-1.2.0/publications/templates/publications/publications.ris`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/publications/id.html` & `django_publications-1.2.0/publications/templates/publications/id.html`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/publications/publication.html` & `django_publications-1.2.0/publications/templates/publications/publication.html`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 	{% for keyword, keyword_escaped in publication.keywords_escaped %}
 	<a class="keyword" href="{% url 'publications:keyword' keyword_escaped %}">{{ keyword }}</a>
 	{% endfor %}
 	<br />
 {% endif %}
 {% if publication.code %}<a class="link" href="{{ publication.code }}">Code</a>,{% endif %}
 {% if publication.url %}<a class="link" rel="external" href="{{ publication.url }}">URL</a>,{% endif %}
-{% if publication.doi %}<a class="link" rel="external" href="http://dx.doi.org/{{ publication.doi }}">DOI</a>,{% endif %}
+{% if publication.doi %}<a class="link" rel="external" href="https://doi.org/{{ publication.doi }}">DOI</a>,{% endif %}
 {% if not publication.journal and publication.isbn %}<a class="link" rel="external" href="http://isbndb.com/search/all?query={{ publication.isbn }}">ISBN</a>,{% endif %}
 {% if publication.pdf %}<a class="link" href="{{ MEDIA_URL }}{{ publication.pdf }}">PDF</a>,{% endif %}
 {% for file in publication.files %}
 	<a class="link" href="{{ MEDIA_URL }}{{ file.file }}">{{ file.description }}</a>,
 {% endfor %}
 {% for link in publication.links %}
 	<a class="link" rel="external" href="{{ link.url }}">{{ link.description }}</a>,
```

### Comparing `django-publications-1.1.0/publications/templates/publications/publications.mods` & `django_publications-1.2.0/publications/templates/publications/publications.mods`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/publications/list.html` & `django_publications-1.2.0/publications/templates/publications/list.html`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/publications/author.html` & `django_publications-1.2.0/publications/templates/publications/author.html`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/publications/person.html` & `django_publications-1.2.0/publications/templates/publications/person.html`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/publications/publications.txt` & `django_publications-1.2.0/publications/templates/publications/publications.txt`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/publications/publications_with_thumbnails.html` & `django_publications-1.2.0/publications/templates/publications/publications_with_thumbnails.html`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/publications/publication.bib` & `django_publications-1.2.0/publications/templates/publications/publication.bib`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/publications/years.html` & `django_publications-1.2.0/publications/templates/publications/years.html`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/publications/keyword.html` & `django_publications-1.2.0/publications/templates/publications/keyword.html`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/publications/publications.rss` & `django_publications-1.2.0/publications/templates/publications/publications.rss`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/templates/admin/publications/import_bibtex.html` & `django_publications-1.2.0/publications/templates/admin/publications/import_bibtex.html`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/fixtures/test_data.json` & `django_publications-1.2.0/publications/fixtures/test_data.json`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/fixtures/initial_data.json` & `django_publications-1.2.0/publications/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/bibtex.py` & `django_publications-1.2.0/publications/bibtex.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/urls.py` & `django_publications-1.2.0/publications/urls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 __license__ = 'MIT License <http://www.opensource.org/licenses/mit-license.php>'
 __author__ = 'Lucas Theis <lucas@theis.io>'
 __docformat__ = 'epytext'
 
-try:
-    from django.conf.urls import url
-except ImportError:
-    from django.conf.urls.defaults import url
+from django.urls import re_path
 
 from publications import views
 
 app_name = 'publications'
 urlpatterns = [
-    url(r'^$', views.year, name='index'),
-    url(r'^(?P<publication_id>\d+)/$', views.id, name='id'),
-    url(r'^year/(?P<year>\d+)/$', views.year, name='year'),
-    url(r'^tag/(?P<keyword>.+)/$', views.keyword, name='keyword'),
-    url(r'^list/(?P<list>.+)/$', views.list, name='list'),
-    url(r'^unapi/$', views.unapi, name='unapi'),
-    url(r'^(?P<name>.+)/$', views.author, name='author'),
+    re_path(r'^$', views.year, name='index'),
+    re_path(r'^(?P<publication_id>\d+)/$', views.id, name='id'),
+    re_path(r'^year/(?P<year>\d+)/$', views.year, name='year'),
+    re_path(r'^tag/(?P<keyword>.+)/$', views.keyword, name='keyword'),
+    re_path(r'^list/(?P<list>.+)/$', views.list, name='list'),
+    re_path(r'^unapi/$', views.unapi, name='unapi'),
+    re_path(r'^(?P<name>.+)/$', views.author, name='author'),
 ]
```

### Comparing `django-publications-1.1.0/publications/views/year.py` & `django_publications-1.2.0/publications/views/year.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/views/list.py` & `django_publications-1.2.0/publications/views/list.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/views/id.py` & `django_publications-1.2.0/publications/views/id.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/views/unapi.py` & `django_publications-1.2.0/publications/views/unapi.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/views/author.py` & `django_publications-1.2.0/publications/views/author.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/publications/views/keyword.py` & `django_publications-1.2.0/publications/views/keyword.py`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/README.md` & `django_publications-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django-publications-1.1.0/setup.py` & `django_publications-1.2.0/setup.py`

 * *Files identical despite different names*

