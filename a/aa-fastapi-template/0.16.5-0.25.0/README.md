# Comparing `tmp/aa-fastapi-template-0.16.5.tar.gz` & `tmp/aa_fastapi_template-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-fastapi-template-0.16.5.tar", last modified: Wed Feb 28 20:16:17 2024, max compression
+gzip compressed data, was "aa_fastapi_template-0.25.0.tar", last modified: Sat Apr 20 03:07:11 2024, max compression
```

## Comparing `aa-fastapi-template-0.16.5.tar` & `aa_fastapi_template-0.25.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aimbrock  (1000) aimbrock  (1000)        0 2024-02-28 20:16:17.936114 aa-fastapi-template-0.16.5/
--rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)     1053 2024-02-22 06:00:53.000000 aa-fastapi-template-0.16.5/LICENSE
--rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)     6136 2024-02-28 20:16:17.936114 aa-fastapi-template-0.16.5/PKG-INFO
--rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)     2601 2024-02-28 13:50:27.000000 aa-fastapi-template-0.16.5/PYPI-README.md
--rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)      578 2024-02-22 06:00:53.000000 aa-fastapi-template-0.16.5/README.md
-drwxr-xr-x   0 aimbrock  (1000) aimbrock  (1000)        0 2024-02-28 20:16:17.932780 aa-fastapi-template-0.16.5/aa_fastapi_template.egg-info/
--rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)     6136 2024-02-28 20:16:17.000000 aa-fastapi-template-0.16.5/aa_fastapi_template.egg-info/PKG-INFO
--rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)      319 2024-02-28 20:16:17.000000 aa-fastapi-template-0.16.5/aa_fastapi_template.egg-info/SOURCES.txt
--rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)        1 2024-02-28 20:16:17.000000 aa-fastapi-template-0.16.5/aa_fastapi_template.egg-info/dependency_links.txt
--rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)      478 2024-02-28 20:16:17.000000 aa-fastapi-template-0.16.5/aa_fastapi_template.egg-info/requires.txt
--rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)       17 2024-02-28 20:16:17.000000 aa-fastapi-template-0.16.5/aa_fastapi_template.egg-info/top_level.txt
-drwxr-xr-x   0 aimbrock  (1000) aimbrock  (1000)        0 2024-02-28 20:16:17.932780 aa-fastapi-template-0.16.5/fastapi_template/
--rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)        0 2024-02-21 01:49:57.000000 aa-fastapi-template-0.16.5/fastapi_template/__init__.py
--rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)     2400 2024-02-28 20:15:46.000000 aa-fastapi-template-0.16.5/pyproject.toml
--rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)       38 2024-02-28 20:16:17.936114 aa-fastapi-template-0.16.5/setup.cfg
-drwxr-xr-x   0 aimbrock  (1000) aimbrock  (1000)        0 2024-02-28 20:16:17.932780 aa-fastapi-template-0.16.5/tests/
--rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)     1242 2024-02-28 20:02:08.000000 aa-fastapi-template-0.16.5/tests/test_pyproject_toml.py
+drwxr-xr-x   0 aimbrock  (1000) aimbrock  (1000)        0 2024-04-20 03:07:11.002636 aa_fastapi_template-0.25.0/
+-rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)     1053 2024-02-25 00:34:34.000000 aa_fastapi_template-0.25.0/LICENSE
+-rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)     6136 2024-04-20 03:07:11.002636 aa_fastapi_template-0.25.0/PKG-INFO
+-rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)     2601 2024-04-20 03:03:00.000000 aa_fastapi_template-0.25.0/PYPI-README.md
+-rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)      577 2024-04-20 03:03:00.000000 aa_fastapi_template-0.25.0/README.md
+drwxr-xr-x   0 aimbrock  (1000) aimbrock  (1000)        0 2024-04-20 03:07:10.999302 aa_fastapi_template-0.25.0/aa_fastapi_template.egg-info/
+-rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)     6136 2024-04-20 03:07:10.000000 aa_fastapi_template-0.25.0/aa_fastapi_template.egg-info/PKG-INFO
+-rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)      319 2024-04-20 03:07:10.000000 aa_fastapi_template-0.25.0/aa_fastapi_template.egg-info/SOURCES.txt
+-rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)        1 2024-04-20 03:07:10.000000 aa_fastapi_template-0.25.0/aa_fastapi_template.egg-info/dependency_links.txt
+-rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)      478 2024-04-20 03:07:10.000000 aa_fastapi_template-0.25.0/aa_fastapi_template.egg-info/requires.txt
+-rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)       17 2024-04-20 03:07:10.000000 aa_fastapi_template-0.25.0/aa_fastapi_template.egg-info/top_level.txt
+drwxr-xr-x   0 aimbrock  (1000) aimbrock  (1000)        0 2024-04-20 03:07:10.999302 aa_fastapi_template-0.25.0/fastapi_template/
+-rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)        0 2024-02-25 00:34:34.000000 aa_fastapi_template-0.25.0/fastapi_template/__init__.py
+-rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)     2400 2024-04-20 03:03:16.000000 aa_fastapi_template-0.25.0/pyproject.toml
+-rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)       38 2024-04-20 03:07:11.002636 aa_fastapi_template-0.25.0/setup.cfg
+drwxr-xr-x   0 aimbrock  (1000) aimbrock  (1000)        0 2024-04-20 03:07:10.999302 aa_fastapi_template-0.25.0/tests/
+-rw-r--r--   0 aimbrock  (1000) aimbrock  (1000)     1242 2024-04-20 03:03:00.000000 aa_fastapi_template-0.25.0/tests/test_pyproject_toml.py
```

### Comparing `aa-fastapi-template-0.16.5/LICENSE` & `aa_fastapi_template-0.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-fastapi-template-0.16.5/PKG-INFO` & `aa_fastapi_template-0.25.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-fastapi-template
-Version: 0.16.5
+Version: 0.25.0
 Summary: A robust and sensible baseline for kick-starting any new FastAPI application.
 Author-email: Aaron Imbrock <aaron@sizza.net>
 Maintainer-email: Aaron Imbrock <aaron@sizza.net>
 License: Copyright Aaron Imbrock 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -40,36 +40,36 @@
 Classifier: Framework :: FastAPI
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncpg==0.29.0
 Requires-Dist: environs==10.3.0
 Requires-Dist: fastapi==0.110.0
-Requires-Dist: mypy==1.8.0
+Requires-Dist: mypy==1.9.0
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: pydantic==2.6.2
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: sqlalchemy==2.0.27
 Requires-Dist: sqlmodel==0.0.16
 Requires-Dist: uvicorn==0.27.1
 Provides-Extra: tests
-Requires-Dist: pytest==8.0.2; extra == "tests"
-Requires-Dist: pytest-mock==3.12.0; extra == "tests"
+Requires-Dist: pytest==8.1.1; extra == "tests"
+Requires-Dist: pytest-mock==3.14.0; extra == "tests"
 Requires-Dist: hypothesis==6.98.11; extra == "tests"
-Requires-Dist: pytest-cov==4.1.0; extra == "tests"
-Requires-Dist: pytest-xdist==3.5.0; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0; extra == "tests"
+Requires-Dist: pytest-xdist==3.6.0; extra == "tests"
 Requires-Dist: pytest-md==0.2.0; extra == "tests"
 Requires-Dist: pytest-emoji==0.2.0; extra == "tests"
 Requires-Dist: tox==4.13.0; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: aa-fastapi-template[tests]; extra == "dev"
 Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: httpx==0.27.0; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
-Requires-Dist: ruff==0.2.2; extra == "dev"
+Requires-Dist: ruff==0.4.1; extra == "dev"
 Requires-Dist: toml==0.10.2; extra == "dev"
 Requires-Dist: types-toml==0.10.8.7; extra == "dev"
 Provides-Extra: build
 Requires-Dist: setuptools; extra == "build"
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
```

### Comparing `aa-fastapi-template-0.16.5/PYPI-README.md` & `aa_fastapi_template-0.25.0/PYPI-README.md`

 * *Files identical despite different names*

### Comparing `aa-fastapi-template-0.16.5/README.md` & `aa_fastapi_template-0.25.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Building a package to release
 
 ### Install Dependencies
 
 ```shell
 python3 -m pip install --upgrade pip
 pip install --upgrade setuptools build twine
```

### Comparing `aa-fastapi-template-0.16.5/aa_fastapi_template.egg-info/PKG-INFO` & `aa_fastapi_template-0.25.0/aa_fastapi_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-fastapi-template
-Version: 0.16.5
+Version: 0.25.0
 Summary: A robust and sensible baseline for kick-starting any new FastAPI application.
 Author-email: Aaron Imbrock <aaron@sizza.net>
 Maintainer-email: Aaron Imbrock <aaron@sizza.net>
 License: Copyright Aaron Imbrock 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -40,36 +40,36 @@
 Classifier: Framework :: FastAPI
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncpg==0.29.0
 Requires-Dist: environs==10.3.0
 Requires-Dist: fastapi==0.110.0
-Requires-Dist: mypy==1.8.0
+Requires-Dist: mypy==1.9.0
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: pydantic==2.6.2
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: sqlalchemy==2.0.27
 Requires-Dist: sqlmodel==0.0.16
 Requires-Dist: uvicorn==0.27.1
 Provides-Extra: tests
-Requires-Dist: pytest==8.0.2; extra == "tests"
-Requires-Dist: pytest-mock==3.12.0; extra == "tests"
+Requires-Dist: pytest==8.1.1; extra == "tests"
+Requires-Dist: pytest-mock==3.14.0; extra == "tests"
 Requires-Dist: hypothesis==6.98.11; extra == "tests"
-Requires-Dist: pytest-cov==4.1.0; extra == "tests"
-Requires-Dist: pytest-xdist==3.5.0; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0; extra == "tests"
+Requires-Dist: pytest-xdist==3.6.0; extra == "tests"
 Requires-Dist: pytest-md==0.2.0; extra == "tests"
 Requires-Dist: pytest-emoji==0.2.0; extra == "tests"
 Requires-Dist: tox==4.13.0; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: aa-fastapi-template[tests]; extra == "dev"
 Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: httpx==0.27.0; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
-Requires-Dist: ruff==0.2.2; extra == "dev"
+Requires-Dist: ruff==0.4.1; extra == "dev"
 Requires-Dist: toml==0.10.2; extra == "dev"
 Requires-Dist: types-toml==0.10.8.7; extra == "dev"
 Provides-Extra: build
 Requires-Dist: setuptools; extra == "build"
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
```

### Comparing `aa-fastapi-template-0.16.5/pyproject.toml` & `aa_fastapi_template-0.25.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,45 +22,45 @@
   "Framework :: FastAPI"
 ]
 description = "A robust and sensible baseline for kick-starting any new FastAPI application."
 license = { file = "LICENSE" }
 keywords = ["fastapi"]
 readme = "PYPI-README.md"
 requires-python = ">=3.10"
-version = "0.16.5"
+version = "0.25.0"
 dependencies = [
   "asyncpg == 0.29.0",
   "environs == 10.3.0",
   "fastapi == 0.110.0",
-  "mypy == 1.8.0",
+  "mypy == 1.9.0",
   "psycopg2-binary == 2.9.9",
   "pydantic == 2.6.2",
   "python-dotenv == 1.0.1",
   "sqlalchemy == 2.0.27",
   "sqlmodel == 0.0.16",
   "uvicorn == 0.27.1",
 ]
 
 [project.optional-dependencies]
 tests = [
-  "pytest == 8.0.2",
-  "pytest-mock == 3.12.0",
+  "pytest == 8.1.1",
+  "pytest-mock == 3.14.0",
   "hypothesis == 6.98.11",
-  "pytest-cov == 4.1.0",
-  "pytest-xdist == 3.5.0",
+  "pytest-cov == 5.0.0",
+  "pytest-xdist == 3.6.0",
   "pytest-md == 0.2.0",
   "pytest-emoji == 0.2.0",
   "tox == 4.13.0",
 ]
 dev = [
   "aa-fastapi-template[tests]",
   "black == 24.2.0",
   "httpx == 0.27.0",
   "isort == 5.13.2",
-  "ruff == 0.2.2",
+  "ruff == 0.4.1",
   "toml == 0.10.2",
   "types-toml == 0.10.8.7",
 ]
 build = [
   "setuptools",
   "build",
   "twine",
```

### Comparing `aa-fastapi-template-0.16.5/tests/test_pyproject_toml.py` & `aa_fastapi_template-0.25.0/tests/test_pyproject_toml.py`

 * *Files identical despite different names*

