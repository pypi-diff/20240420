# Comparing `tmp/django_user_email-1.1.0.tar.gz` & `tmp/django_user_email-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_user_email-1.1.0.tar", max compression
+gzip compressed data, was "django_user_email-1.1.1.tar", max compression
```

## Comparing `django_user_email-1.1.0.tar` & `django_user_email-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-12-21 09:22:02.500810 django_user_email-1.1.0/LICENSE
--rw-r--r--   0        0        0     2070 2023-12-21 09:22:02.500810 django_user_email-1.1.0/README.md
--rw-r--r--   0        0        0     1654 2023-12-21 09:22:19.724824 django_user_email-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-21 09:22:02.500810 django_user_email-1.1.0/user_email/__init__.py
--rw-r--r--   0        0        0     1480 2023-12-21 09:22:02.500810 django_user_email-1.1.0/user_email/admin.py
--rw-r--r--   0        0        0      149 2023-12-21 09:22:02.500810 django_user_email-1.1.0/user_email/apps.py
--rw-r--r--   0        0        0      253 2023-12-21 09:22:02.500810 django_user_email-1.1.0/user_email/factory.py
--rw-r--r--   0        0        0      408 2023-12-21 09:22:02.500810 django_user_email-1.1.0/user_email/forms.py
--rw-r--r--   0        0        0     3309 2023-12-21 09:22:02.500810 django_user_email-1.1.0/user_email/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-12-21 09:22:02.500810 django_user_email-1.1.0/user_email/migrations/__init__.py
--rw-r--r--   0        0        0     2340 2023-12-21 09:22:02.500810 django_user_email-1.1.0/user_email/models.py
--rw-r--r--   0        0        0     3209 1970-01-01 00:00:00.000000 django_user_email-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-20 18:50:58.651043 django_user_email-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2080 2024-04-20 18:50:58.651043 django_user_email-1.1.1/README.md
+-rw-r--r--   0        0        0     1654 2024-04-20 18:51:13.807001 django_user_email-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-20 18:50:58.651043 django_user_email-1.1.1/user_email/__init__.py
+-rw-r--r--   0        0        0     1480 2024-04-20 18:50:58.651043 django_user_email-1.1.1/user_email/admin.py
+-rw-r--r--   0        0        0      149 2024-04-20 18:50:58.651043 django_user_email-1.1.1/user_email/apps.py
+-rw-r--r--   0        0        0      253 2024-04-20 18:50:58.651043 django_user_email-1.1.1/user_email/factory.py
+-rw-r--r--   0        0        0      408 2024-04-20 18:50:58.655043 django_user_email-1.1.1/user_email/forms.py
+-rw-r--r--   0        0        0     3309 2024-04-20 18:50:58.655043 django_user_email-1.1.1/user_email/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-20 18:50:58.655043 django_user_email-1.1.1/user_email/migrations/__init__.py
+-rw-r--r--   0        0        0     2340 2024-04-20 18:50:58.655043 django_user_email-1.1.1/user_email/models.py
+-rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 django_user_email-1.1.1/PKG-INFO
```

### Comparing `django_user_email-1.1.0/LICENSE` & `django_user_email-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_user_email-1.1.0/README.md` & `django_user_email-1.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <h1 align="center">
   django-user-email
 </h1>
 
 <p align="center">
   <a href="https://github.com/khasbilegt/django-user-email/">
-    <img src="https://img.shields.io/github/workflow/status/khasbilegt/django-user-email/test?label=CI&logo=github&style=for-the-badge" alt="ci status">
+    <img src="https://img.shields.io/github/actions/workflow/status/khasbilegt/django-user-email/ci.yml?label=CI&logo=github&style=for-the-badge" alt="ci status">
   </a>
   <a href="https://pypi.org/project/django-user-email/">
     <img src="https://img.shields.io/pypi/v/django-user-email?style=for-the-badge" alt="pypi link">
   </a>
   <a href="https://codecov.io/github/khasbilegt/django-user-email">
     <img src="https://img.shields.io/codecov/c/github/khasbilegt/django-user-email?logo=codecov&style=for-the-badge" alt="codecov">
   </a>
```

### Comparing `django_user_email-1.1.0/pyproject.toml` & `django_user_email-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 show_missing = true
 skip_covered = true
 skip_empty = true
 precision = 2
 
 [tool.poetry]
 name = "django-user-email"
-version = "1.1.0"
+version = "1.1.1"
 description = "Custom, simple Django User model with email as username"
 authors = ["Khasbilegt.TS <khasbilegt.ts@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/khasbilegt/django-user-email"
 repository = "https://github.com/khasbilegt/django-user-email"
 keywords = ["django", "model", "user", "email", "username", "custom"]
 readme = "README.md"
@@ -56,13 +56,13 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
 factory-boy = "^3.3.0"
 nox = "^2023.4.22"
-ruff = "^0.1.8"
+ruff = "^0.4.1"
 coverage = {extras = ["toml"], version = "^7.3.4"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_user_email-1.1.0/user_email/admin.py` & `django_user_email-1.1.1/user_email/admin.py`

 * *Files identical despite different names*

### Comparing `django_user_email-1.1.0/user_email/migrations/0001_initial.py` & `django_user_email-1.1.1/user_email/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_user_email-1.1.0/user_email/models.py` & `django_user_email-1.1.1/user_email/models.py`

 * *Files identical despite different names*

### Comparing `django_user_email-1.1.0/PKG-INFO` & `django_user_email-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-user-email
-Version: 1.1.0
+Version: 1.1.1
 Summary: Custom, simple Django User model with email as username
 Home-page: https://github.com/khasbilegt/django-user-email
 License: MIT
 Keywords: django,model,user,email,username,custom
 Author: Khasbilegt.TS
 Author-email: khasbilegt.ts@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -28,15 +28,15 @@
 
 <h1 align="center">
   django-user-email
 </h1>
 
 <p align="center">
   <a href="https://github.com/khasbilegt/django-user-email/">
-    <img src="https://img.shields.io/github/workflow/status/khasbilegt/django-user-email/test?label=CI&logo=github&style=for-the-badge" alt="ci status">
+    <img src="https://img.shields.io/github/actions/workflow/status/khasbilegt/django-user-email/ci.yml?label=CI&logo=github&style=for-the-badge" alt="ci status">
   </a>
   <a href="https://pypi.org/project/django-user-email/">
     <img src="https://img.shields.io/pypi/v/django-user-email?style=for-the-badge" alt="pypi link">
   </a>
   <a href="https://codecov.io/github/khasbilegt/django-user-email">
     <img src="https://img.shields.io/codecov/c/github/khasbilegt/django-user-email?logo=codecov&style=for-the-badge" alt="codecov">
   </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-user-email Version: 1.1.0 Summary: Custom,
+Metadata-Version: 2.1 Name: django-user-email Version: 1.1.1 Summary: Custom,
 simple Django User model with email as username Home-page: https://github.com/
 khasbilegt/django-user-email License: MIT Keywords:
 django,model,user,email,username,custom Author: Khasbilegt.TS Author-email:
 khasbilegt.ts@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Environment ::
 Web Environment Classifier: Framework :: Django Classifier: Framework :: Django
 :: 3.2 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Django
 :: 5.0 Classifier: Intended Audience :: Developers Classifier: License :: OSI
```

