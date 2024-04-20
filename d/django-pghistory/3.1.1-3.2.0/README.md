# Comparing `tmp/django_pghistory-3.1.1.tar.gz` & `tmp/django_pghistory-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pghistory-3.1.1.tar", max compression
+gzip compressed data, was "django_pghistory-3.2.0.tar", max compression
```

## Comparing `django_pghistory-3.1.1.tar` & `django_pghistory-3.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1456 2024-04-06 16:51:43.335715 django_pghistory-3.1.1/LICENSE
--rw-r--r--   0        0        0     3131 2024-04-06 16:51:43.335715 django_pghistory-3.1.1/README.md
--rw-r--r--   0        0        0     3503 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/__init__.py
--rw-r--r--   0        0        0      277 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/admin/__init__.py
--rw-r--r--   0        0        0      297 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/admin/apps.py
--rw-r--r--   0        0        0     6806 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/admin/core.py
--rw-r--r--   0        0        0      952 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/admin/templates/admin/change_form_object_tools.html
--rw-r--r--   0        0        0      548 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/admin/templates/admin/change_list_object_tools.html
--rw-r--r--   0        0        0      219 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/admin/templates/pghistory_admin/events_change_list.html
--rw-r--r--   0        0        0        0 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/admin/templates/pghistory_admin/hidden_filter.html
--rw-r--r--   0        0        0     1464 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/admin/templatetags/pghistory_admin.py
--rw-r--r--   0        0        0      756 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/apps.py
--rw-r--r--   0        0        0      448 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/checks.py
--rw-r--r--   0        0        0    12966 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/config.py
--rw-r--r--   0        0        0      105 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/constants.py
--rw-r--r--   0        0        0    26288 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/core.py
--rw-r--r--   0        0        0     1419 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/middleware.py
--rw-r--r--   0        0        0      945 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/migrations/0001_initial.py
--rw-r--r--   0        0        0     1430 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/migrations/0002_aggregateevent.py
--rw-r--r--   0        0        0      421 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/migrations/0003_auto_20201023_1636.py
--rw-r--r--   0        0        0      531 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/migrations/0004_auto_20220906_1625.py
--rw-r--r--   0        0        0     2924 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/migrations/0005_events_middlewareevents.py
--rw-r--r--   0        0        0      309 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/migrations/0006_delete_aggregateevent.py
--rw-r--r--   0        0        0        0 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/migrations/__init__.py
--rw-r--r--   0        0        0    25066 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/models.py
--rw-r--r--   0        0        0     5356 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/runtime.py
--rw-r--r--   0        0        0     3758 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/trigger.py
--rw-r--r--   0        0        0     1302 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/utils.py
--rw-r--r--   0        0        0       83 2024-04-06 16:51:43.367715 django_pghistory-3.1.1/pghistory/version.py
--rw-r--r--   0        0        0     2347 2024-04-06 16:52:27.571778 django_pghistory-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     4382 1970-01-01 00:00:00.000000 django_pghistory-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-20 19:17:11.078903 django_pghistory-3.2.0/LICENSE
+-rw-r--r--   0        0        0     3131 2024-04-20 19:17:11.078903 django_pghistory-3.2.0/README.md
+-rw-r--r--   0        0        0     3503 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/admin/__init__.py
+-rw-r--r--   0        0        0      297 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/admin/apps.py
+-rw-r--r--   0        0        0     6806 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/admin/core.py
+-rw-r--r--   0        0        0      952 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/admin/templates/admin/change_form_object_tools.html
+-rw-r--r--   0        0        0      548 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/admin/templates/admin/change_list_object_tools.html
+-rw-r--r--   0        0        0      219 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/admin/templates/pghistory_admin/events_change_list.html
+-rw-r--r--   0        0        0        0 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/admin/templates/pghistory_admin/hidden_filter.html
+-rw-r--r--   0        0        0     1464 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/admin/templatetags/pghistory_admin.py
+-rw-r--r--   0        0        0      756 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/apps.py
+-rw-r--r--   0        0        0      448 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/checks.py
+-rw-r--r--   0        0        0    12966 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/config.py
+-rw-r--r--   0        0        0      105 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/constants.py
+-rw-r--r--   0        0        0    26345 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/core.py
+-rw-r--r--   0        0        0     1419 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/middleware.py
+-rw-r--r--   0        0        0      945 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1430 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/migrations/0002_aggregateevent.py
+-rw-r--r--   0        0        0      421 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/migrations/0003_auto_20201023_1636.py
+-rw-r--r--   0        0        0      531 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/migrations/0004_auto_20220906_1625.py
+-rw-r--r--   0        0        0     2924 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/migrations/0005_events_middlewareevents.py
+-rw-r--r--   0        0        0      309 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/migrations/0006_delete_aggregateevent.py
+-rw-r--r--   0        0        0        0 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/migrations/__init__.py
+-rw-r--r--   0        0        0    25066 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/models.py
+-rw-r--r--   0        0        0     5356 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/runtime.py
+-rw-r--r--   0        0        0     3758 2024-04-20 19:17:11.110903 django_pghistory-3.2.0/pghistory/trigger.py
+-rw-r--r--   0        0        0     1302 2024-04-20 19:17:11.114903 django_pghistory-3.2.0/pghistory/utils.py
+-rw-r--r--   0        0        0       83 2024-04-20 19:17:11.114903 django_pghistory-3.2.0/pghistory/version.py
+-rw-r--r--   0        0        0     2347 2024-04-20 19:17:59.267188 django_pghistory-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4382 1970-01-01 00:00:00.000000 django_pghistory-3.2.0/PKG-INFO
```

### Comparing `django_pghistory-3.1.1/LICENSE` & `django_pghistory-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/README.md` & `django_pghistory-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/__init__.py` & `django_pghistory-3.2.0/pghistory/__init__.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/admin/core.py` & `django_pghistory-3.2.0/pghistory/admin/core.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/admin/templates/admin/change_form_object_tools.html` & `django_pghistory-3.2.0/pghistory/admin/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/admin/templates/admin/change_list_object_tools.html` & `django_pghistory-3.2.0/pghistory/admin/templates/admin/change_list_object_tools.html`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/admin/templatetags/pghistory_admin.py` & `django_pghistory-3.2.0/pghistory/admin/templatetags/pghistory_admin.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/apps.py` & `django_pghistory-3.2.0/pghistory/apps.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/config.py` & `django_pghistory-3.2.0/pghistory/config.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/core.py` & `django_pghistory-3.2.0/pghistory/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Core functionality and interface of pghistory"""
+
 import copy
 import re
 import sys
 from typing import TYPE_CHECKING, Any, Dict, List, Type, Union
 
 import pgtrigger
 import pgtrigger.core
@@ -430,15 +431,19 @@
     app = apps.app_configs[app_label]
     models_module = app.module.__name__ + ".models"
 
     attrs = attrs or {}
     attrs.update({"pgh_trackers": trackers})
     meta = meta or {}
     exclude = exclude or []
-    fields = fields or [f.name for f in tracked_model._meta.fields if f.name not in exclude]
+    fields = (
+        fields
+        if fields is not None
+        else [f.name for f in tracked_model._meta.fields if f.name not in exclude]
+    )
 
     if append_only:
         meta["triggers"] = [
             *meta.get("triggers", []),
             pgtrigger.Protect(name="append_only", operation=pgtrigger.Update | pgtrigger.Delete),
         ]
```

### Comparing `django_pghistory-3.1.1/pghistory/middleware.py` & `django_pghistory-3.2.0/pghistory/middleware.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/migrations/0001_initial.py` & `django_pghistory-3.2.0/pghistory/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/migrations/0002_aggregateevent.py` & `django_pghistory-3.2.0/pghistory/migrations/0002_aggregateevent.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/migrations/0004_auto_20220906_1625.py` & `django_pghistory-3.2.0/pghistory/migrations/0004_auto_20220906_1625.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/migrations/0005_events_middlewareevents.py` & `django_pghistory-3.2.0/pghistory/migrations/0005_events_middlewareevents.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/models.py` & `django_pghistory-3.2.0/pghistory/models.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/runtime.py` & `django_pghistory-3.2.0/pghistory/runtime.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/trigger.py` & `django_pghistory-3.2.0/pghistory/trigger.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pghistory/utils.py` & `django_pghistory-3.2.0/pghistory/utils.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-3.1.1/pyproject.toml` & `django_pghistory-3.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 name = "django-pghistory"
 packages = [
   { include = "pghistory" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "3.1.1"
+version = "3.2.0"
 description = "History tracking for Django and Postgres"
 authors = ["Wes Kendall"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
```

### Comparing `django_pghistory-3.1.1/PKG-INFO` & `django_pghistory-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pghistory
-Version: 3.1.1
+Version: 3.2.0
 Summary: History tracking for Django and Postgres
 Home-page: https://github.com/Opus10/django-pghistory
 License: BSD-3-Clause
 Author: Wes Kendall
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

