# Comparing `tmp/django_router-1.0.7.tar.gz` & `tmp/django_router-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_router-1.0.7.tar", last modified: Fri Sep 29 13:09:48 2023, max compression
+gzip compressed data, was "django_router-1.0.8.tar", last modified: Sat Apr 20 14:00:49 2024, max compression
```

## Comparing `django_router-1.0.7.tar` & `django_router-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1525 2023-09-29 13:09:26.968718 django_router-1.0.7/LICENSE
--rw-r--r--   0        0        0     6859 2023-09-29 13:09:26.968718 django_router-1.0.7/README.md
--rw-r--r--   0        0        0     3702 2023-09-29 13:09:26.968718 django_router-1.0.7/django_router/__init__.py
--rw-r--r--   0        0        0      230 2023-09-29 13:09:26.968718 django_router-1.0.7/django_router/apps.py
--rw-r--r--   0        0        0        0 2023-09-29 13:09:26.968718 django_router-1.0.7/django_router/management/__init__.py
--rw-r--r--   0        0        0        0 2023-09-29 13:09:26.968718 django_router-1.0.7/django_router/management/commands/__init__.py
--rw-r--r--   0        0        0      694 2023-09-29 13:09:26.968718 django_router-1.0.7/django_router/management/commands/router_list.py
--rw-r--r--   0        0        0     1338 2023-09-29 13:09:26.968718 django_router-1.0.7/django_router/management/commands/router_urls.py
--rw-r--r--   0        0        0     1252 2023-09-29 13:09:26.968718 django_router-1.0.7/django_router/settings.py
--rw-r--r--   0        0        0      806 2023-09-29 13:09:26.968718 django_router-1.0.7/django_router/utils.py
--rw-r--r--   0        0        0      535 2023-09-29 13:09:48.440837 django_router-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     7134 1970-01-01 00:00:00.000000 django_router-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1525 2024-04-20 14:00:37.937528 django_router-1.0.8/LICENSE
+-rw-r--r--   0        0        0     6859 2024-04-20 14:00:37.941528 django_router-1.0.8/README.md
+-rw-r--r--   0        0        0     3702 2024-04-20 14:00:37.941528 django_router-1.0.8/django_router/__init__.py
+-rw-r--r--   0        0        0      230 2024-04-20 14:00:37.941528 django_router-1.0.8/django_router/apps.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:00:37.941528 django_router-1.0.8/django_router/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:00:37.941528 django_router-1.0.8/django_router/management/commands/__init__.py
+-rw-r--r--   0        0        0      694 2024-04-20 14:00:37.941528 django_router-1.0.8/django_router/management/commands/router_list.py
+-rw-r--r--   0        0        0     1280 2024-04-20 14:00:37.941528 django_router-1.0.8/django_router/management/commands/router_urls.py
+-rw-r--r--   0        0        0     1290 2024-04-20 14:00:37.941528 django_router-1.0.8/django_router/settings.py
+-rw-r--r--   0        0        0      806 2024-04-20 14:00:37.941528 django_router-1.0.8/django_router/utils.py
+-rw-r--r--   0        0        0      535 2024-04-20 14:00:49.081546 django_router-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7134 1970-01-01 00:00:00.000000 django_router-1.0.8/PKG-INFO
```

### Comparing `django_router-1.0.7/LICENSE` & `django_router-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django_router-1.0.7/README.md` & `django_router-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `django_router-1.0.7/django_router/__init__.py` & `django_router-1.0.8/django_router/__init__.py`

 * *Files identical despite different names*

### Comparing `django_router-1.0.7/django_router/management/commands/router_list.py` & `django_router-1.0.8/django_router/management/commands/router_list.py`

 * *Files identical despite different names*

### Comparing `django_router-1.0.7/django_router/settings.py` & `django_router-1.0.8/django_router/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,21 @@
     ADMIN_LIKE_VERBS: bool = False
     MODULE_PATH_MAP: bool = True
 
     def __init__(self):
         project_settings = getattr(settings, "ROUTER_SETTINGS", {})
         if "NAME_WORDS_SEPARATOR" in project_settings:  # pragma: no cover
             raise ImproperlyConfigured(
-                "Option NAME_WORDS_SEPARATOR for Django Router renamed to WORDS_SEPARATOR"
+                "Option NAME_WORDS_SEPARATOR for Django Router"
+                " renamed to WORDS_SEPARATOR"
             )
         if "DJANGO_ADMIN_LIKE_NAMES" in project_settings:  # pragma: no cover
             raise ImproperlyConfigured(
-                "Option DJANGO_ADMIN_LIKE_NAMES for Django Router renamed to ADMIN_LIKE_VERBS"
+                "Option DJANGO_ADMIN_LIKE_NAMES for Django Router"
+                " renamed to ADMIN_LIKE_VERBS"
             )
         if "TRY_USE_MODEL_NAMES" in project_settings:  # pragma: no cover
             raise ImproperlyConfigured(
                 "Option TRY_USE_MODEL_NAMES for Django router is deprecated"
             )
 
     def __getattribute__(self, name):
```

### Comparing `django_router-1.0.7/django_router/utils.py` & `django_router-1.0.8/django_router/utils.py`

 * *Files identical despite different names*

### Comparing `django_router-1.0.7/pyproject.toml` & `django_router-1.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "django-router"
-version = "1.0.7"
+version = "1.0.8"
 description = "Use simple decorators on views instead of maintaining lengthy urls.py"
 authors = [
     { name = "RealGecko", email = "alexandrbezenkov@gmail.com" },
 ]
 dependencies = []
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 readme = "README.md"
 
 [project.license]
 text = "BSD-3-Clause"
 
 [build-system]
 requires = [
@@ -20,9 +20,9 @@
 
 [tool.pdm.dev-dependencies]
 dev = []
 test = [
     "django>=2.2",
     "django-extensions>=3.1",
     "tox",
-    "coverage>=7.3.1",
+    "coverage>=7.2.7",
 ]
```

### Comparing `django_router-1.0.7/PKG-INFO` & `django_router-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: django-router
-Version: 1.0.7
+Version: 1.0.8
 Summary: Use simple decorators on views instead of maintaining lengthy urls.py
 Author-Email: RealGecko <alexandrbezenkov@gmail.com>
 License: BSD-3-Clause
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Django Router
 
 You have a data and you need to provide some CRUD functionality for it quickly. What do you do?
 
 1. Create model
```

