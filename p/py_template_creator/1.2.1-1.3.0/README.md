# Comparing `tmp/py_template_creator-1.2.1.tar.gz` & `tmp/py_template_creator-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_template_creator-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_template_creator-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_template_creator-1.2.1.tar` & `py_template_creator-1.3.0.tar`

### file list

```diff
@@ -1,57 +1,69 @@
--rw-r--r--   0        0        0     1800 2024-04-11 06:33:56.852609 py_template_creator-1.2.1/.gitignore
--rw-r--r--   0        0        0    11325 2024-04-11 06:33:56.852609 py_template_creator-1.2.1/LICENSE
--rw-r--r--   0        0        0      578 2024-04-11 06:33:56.852609 py_template_creator-1.2.1/README.md
--rw-r--r--   0        0        0       80 2024-04-12 08:53:33.789077 py_template_creator-1.2.1/py_template_creator/__init__.py
--rw-r--r--   0        0        0      150 2024-04-11 09:45:18.402626 py_template_creator-1.2.1/py_template_creator/api-scelet/cookiecutter.json
--rw-r--r--   0        0        0      283 2024-04-11 09:41:09.043742 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.env
--rw-r--r--   0        0        0      283 2024-04-11 09:41:05.991707 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.env.example
--rw-r--r--   0        0        0       91 2024-04-11 09:43:40.833493 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.flake8
--rw-r--r--   0        0        0     2529 2024-04-11 06:33:56.852609 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.gitignore
--rw-r--r--   0        0        0      366 2024-04-11 09:43:40.853493 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      997 2024-04-11 09:38:08.997694 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/Dockerfile
--rwxr-xr-x   0        0        0       93 2024-04-11 09:45:55.975064 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/config/run.sh
--rwxr-xr-x   0        0        0      319 2024-04-11 09:43:18.245231 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/config/test.sh
--rw-r--r--   0        0        0     1628 2024-04-11 09:57:32.247652 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/docker-compose.yaml
--rw-r--r--   0        0        0     1108 2024-04-11 09:59:47.345341 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/Makefile
--rw-r--r--   0        0        0        0 2024-04-11 09:43:18.265231 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/__init__.py
--rw-r--r--   0        0        0     1976 2024-04-11 09:43:18.265231 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/alembic.ini
--rw-r--r--   0        0        0        0 2024-04-11 09:43:18.265231 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/__init__.py
--rw-r--r--   0        0        0       38 2024-04-11 09:43:18.269231 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/alembic/README
--rw-r--r--   0        0        0        0 2024-04-11 09:43:18.269231 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/alembic/__init__.py
--rw-r--r--   0        0        0     2106 2024-04-11 09:47:06.647890 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/alembic/env.py
--rw-r--r--   0        0        0      510 2024-04-11 09:43:18.269231 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/alembic/script.py.mako
--rw-r--r--   0        0        0        0 2024-04-11 09:43:18.273231 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/alembic/versions/.gitkeep
--rw-r--r--   0        0        0       57 2024-04-11 09:47:37.496251 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/api/__init__.py
--rw-r--r--   0        0        0      312 2024-04-11 09:43:18.277232 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/api/base.py
--rw-r--r--   0        0        0     2975 2024-04-11 09:50:59.374624 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/main.py
--rw-r--r--   0        0        0      173 2024-04-11 09:47:52.012421 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/models/__init__.py
--rw-r--r--   0        0        0     2107 2024-04-11 09:48:06.660593 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/models/base.py
--rw-r--r--   0        0        0        0 2024-04-11 09:48:43.805029 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/schemas/__init__.py
--rw-r--r--   0        0        0       73 2024-04-11 09:48:59.809217 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/utilities/__init__.py
--rw-r--r--   0        0        0      209 2024-04-11 09:43:18.293232 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/utilities/dependecies.py
--rw-r--r--   0        0        0      591 2024-04-11 09:45:15.954598 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/pyproject.toml
--rw-r--r--   0        0        0      148 2024-04-12 08:53:21.044863 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/requirements/common.txt
--rw-r--r--   0        0        0       67 2024-04-11 09:52:40.387933 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/requirements/local.txt
--rw-r--r--   0        0        0       15 2024-04-11 09:43:18.321232 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/requirements/prod.txt
--rw-r--r--   0        0        0      176 2024-04-11 09:52:45.115994 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/requirements/test.txt
--rw-r--r--   0        0        0        0 2024-04-11 09:43:18.321232 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/tests/__init__.py
--rw-r--r--   0        0        0     3524 2024-04-11 10:01:16.526449 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/tests/conftest.py
--rw-r--r--   0        0        0      412 2024-04-11 09:43:18.333232 py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/tests/test_health.py
--rw-r--r--   0        0        0      792 2024-04-11 09:55:32.622141 py_template_creator-1.2.1/py_template_creator/main.py
--rw-r--r--   0        0        0      115 2024-04-11 09:19:18.370929 py_template_creator-1.2.1/py_template_creator/service-scelet/cookiecutter.json
--rw-r--r--   0        0        0      850 2024-04-11 09:21:01.623602 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/Dockerfile
--rw-r--r--   0        0        0      563 2024-04-11 09:17:01.426235 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/Makefile
--rw-r--r--   0        0        0      909 2024-04-11 09:21:18.751724 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/README.md
--rwxr-xr-x   0        0        0       52 2024-04-11 06:33:56.856609 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/config/run.sh
--rw-r--r--   0        0        0        0 2024-04-11 09:17:53.922471 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/package/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 09:22:01.116037 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/package/app/__init__.py
--rw-r--r--   0        0        0       80 2024-04-11 06:33:56.856609 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/package/app/handlers/__init__.py
--rw-r--r--   0        0        0      460 2024-04-11 09:22:29.040252 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/package/app/handlers/example_handler.py
--rw-r--r--   0        0        0     1533 2024-04-11 06:33:56.856609 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/package/run.py
--rw-r--r--   0        0        0      446 2024-04-11 09:09:57.548739 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/pyproject.toml
--rw-r--r--   0        0        0       34 2024-04-12 08:53:18.196815 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/requirements/common.txt
--rw-r--r--   0        0        0       48 2024-04-11 06:33:56.856609 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/requirements/local.txt
--rw-r--r--   0        0        0       13 2024-04-11 06:33:56.856609 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/requirements/prod.txt
--rw-r--r--   0        0        0       44 2024-04-11 09:21:39.187873 py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/requirements/test.txt
--rw-r--r--   0        0        0      448 2024-04-11 09:55:59.354480 py_template_creator-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 py_template_creator-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1800 2024-04-11 06:33:56.852609 py_template_creator-1.3.0/.gitignore
+-rw-r--r--   0        0        0    11325 2024-04-11 06:33:56.852609 py_template_creator-1.3.0/LICENSE
+-rw-r--r--   0        0        0      578 2024-04-11 06:33:56.852609 py_template_creator-1.3.0/README.md
+-rw-r--r--   0        0        0       80 2024-04-20 20:05:37.345086 py_template_creator-1.3.0/py_template_creator/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-11 09:45:18.402626 py_template_creator-1.3.0/py_template_creator/api-scelet/cookiecutter.json
+-rw-r--r--   0        0        0      543 2024-04-20 18:42:57.898424 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.env
+-rw-r--r--   0        0        0      543 2024-04-20 18:42:55.026391 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.env.example
+-rw-r--r--   0        0        0       91 2024-04-20 17:37:49.032906 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.flake8
+-rw-r--r--   0        0        0     2533 2024-04-20 17:36:22.772304 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.gitignore
+-rw-r--r--   0        0        0      366 2024-04-20 17:37:37.756828 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2255 2024-04-20 18:44:33.763522 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/docker-compose.yaml
+-rw-r--r--   0        0        0      966 2024-04-20 17:33:24.699025 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/Dockerfile
+-rw-r--r--   0        0        0     1224 2024-04-20 19:14:38.680183 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/Makefile
+-rw-r--r--   0        0        0        0 2024-04-20 17:39:18.117516 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/README.md
+-rwxr-xr-x   0        0        0      122 2024-04-20 17:41:14.786304 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/config/run.sh
+-rwxr-xr-x   0        0        0      301 2024-04-20 19:30:07.007483 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/config/test.sh
+-rw-r--r--   0        0        0        0 2024-04-20 17:28:35.404787 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/__init__.py
+-rw-r--r--   0        0        0     1984 2024-04-20 17:28:35.404787 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/alembic.ini
+-rw-r--r--   0        0        0        0 2024-04-20 17:28:35.404787 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-20 17:28:35.408788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/README
+-rw-r--r--   0        0        0        0 2024-04-20 17:28:35.408788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/__init__.py
+-rw-r--r--   0        0        0     2247 2024-04-20 20:02:42.583219 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/env.py
+-rw-r--r--   0        0        0      510 2024-04-20 17:28:35.408788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/script.py.mako
+-rw-r--r--   0        0        0        0 2024-04-20 17:28:35.408788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/versions/.gitkeep
+-rw-r--r--   0        0        0       57 2024-04-20 17:28:35.412788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/api/__init__.py
+-rw-r--r--   0        0        0      312 2024-04-20 17:28:35.412788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/api/base.py
+-rw-r--r--   0        0        0     3007 2024-04-20 17:28:35.412788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/main.py
+-rw-r--r--   0        0        0      173 2024-04-20 17:28:35.412788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/models/__init__.py
+-rw-r--r--   0        0        0     2107 2024-04-20 17:28:35.416787 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/models/base.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:28:35.416787 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/schemas/__init__.py
+-rw-r--r--   0        0        0       73 2024-04-20 17:28:35.416787 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/utilities/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-20 17:28:35.416787 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/utilities/dependecies.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:28:35.416787 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/tests/__init__.py
+-rw-r--r--   0        0        0     3560 2024-04-20 17:28:35.420788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/tests/conftest.py
+-rw-r--r--   0        0        0      412 2024-04-20 17:28:35.420788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/tests/test_health.py
+-rw-r--r--   0        0        0      662 2024-04-20 18:21:55.965797 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/pyproject.toml
+-rw-r--r--   0        0        0      148 2024-04-20 17:28:35.420788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/requirements/common.txt
+-rw-r--r--   0        0        0       67 2024-04-20 17:28:35.420788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/requirements/local.txt
+-rw-r--r--   0        0        0       15 2024-04-20 17:28:35.424788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/requirements/prod.txt
+-rw-r--r--   0        0        0      176 2024-04-20 17:28:35.424788 py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/requirements/test.txt
+-rw-r--r--   0        0        0      792 2024-04-11 09:55:32.622141 py_template_creator-1.3.0/py_template_creator/main.py
+-rw-r--r--   0        0        0      115 2024-04-20 20:04:06.404111 py_template_creator-1.3.0/py_template_creator/service-scelet/cookiecutter.json
+-rw-r--r--   0        0        0      917 2024-04-20 18:19:42.727439 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/Dockerfile
+-rw-r--r--   0        0        0     1256 2024-04-20 19:31:37.044792 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/Makefile
+-rw-r--r--   0        0        0      909 2024-04-20 20:04:06.412110 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/README.md
+-rwxr-xr-x   0        0        0       52 2024-04-20 20:04:06.412110 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/config/run.sh
+-rw-r--r--   0        0        0      328 2024-04-20 19:30:50.488121 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/config/test.sh
+-rw-r--r--   0        0        0        0 2024-04-11 09:17:53.922471 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/__init__.py
+-rw-r--r--   0        0        0     1984 2024-04-20 18:06:41.933333 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/alembic.ini
+-rw-r--r--   0        0        0        1 2024-04-11 09:22:01.116037 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-20 17:57:52.311352 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/README
+-rw-r--r--   0        0        0        0 2024-04-20 17:57:52.311352 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/__init__.py
+-rw-r--r--   0        0        0     2124 2024-04-20 20:02:01.538787 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/env.py
+-rw-r--r--   0        0        0      510 2024-04-20 17:57:52.311352 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/script.py.mako
+-rw-r--r--   0        0        0        0 2024-04-20 17:57:52.315352 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/versions/.gitkeep
+-rw-r--r--   0        0        0       80 2024-04-11 06:33:56.856609 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/handlers/__init__.py
+-rw-r--r--   0        0        0      460 2024-04-11 09:22:29.040252 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/handlers/example_handler.py
+-rw-r--r--   0        0        0      135 2024-04-20 18:59:12.391435 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/models/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-20 18:57:53.390768 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/models/base.py
+-rw-r--r--   0        0        0     1533 2024-04-20 20:04:06.412110 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/run.py
+-rw-r--r--   0        0        0        0 2024-04-20 18:12:49.849111 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/tests/__init__.py
+-rw-r--r--   0        0        0     1847 2024-04-20 19:29:16.362724 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/tests/conftest.py
+-rw-r--r--   0        0        0      642 2024-04-20 20:04:06.412110 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-04-20 18:30:22.101248 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/requirements/common.txt
+-rw-r--r--   0        0        0       48 2024-04-11 06:33:56.856609 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/requirements/local.txt
+-rw-r--r--   0        0        0       13 2024-04-11 06:33:56.856609 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/requirements/prod.txt
+-rw-r--r--   0        0        0      138 2024-04-20 18:30:03.917007 py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/requirements/test.txt
+-rw-r--r--   0        0        0      448 2024-04-11 09:55:59.354480 py_template_creator-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 py_template_creator-1.3.0/PKG-INFO
```

### Comparing `py_template_creator-1.2.1/.gitignore` & `py_template_creator-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.2.1/LICENSE` & `py_template_creator-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.2.1/README.md` & `py_template_creator-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.gitignore` & `py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -194,9 +194,9 @@
 
 # dev
 .vscode
 
 
 # Sublime files
 *.sublime*
-!.env
-!env.sh
+# !.env
+# !env.sh
```

### Comparing `py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/Dockerfile` & `py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/Dockerfile`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ARG PYTHON_VERSION=3.12-slim
 
 # Stage 0, instaling dev packages
 FROM python:${PYTHON_VERSION} as builder
-LABEL maintainer="{{ cookiecutter.author_name }} <{{ cookiecutter.author_email }}>"
+LABEL maintainer="{{cookiecutter.author_name}} <{{cookiecutter.author_email}}>"
 ENV PYTHONUNBUFFERED 1
 
 RUN apt-get update && apt-get -y install build-essential libpq-dev
 WORKDIR /wheels
-COPY ./package/requirements/ /wheels/requirements/
+COPY ./$APP_DIR/requirements/ /wheels/requirements/
 RUN pip install -U pip && pip wheel -r ./requirements/prod.txt
 
 # Stage 1, no dev packages on wheels
 FROM python:${PYTHON_VERSION}
 ENV PYTHONUNBUFFERED=1
 
 COPY --from=builder /wheels /wheels
@@ -19,21 +19,15 @@
        && pip install -r /wheels/requirements/prod.txt \
                       -f /wheels \
        && rm -rf /wheels \
        && rm -rf /root/.cache/pip/*
 
 
 # Copy code to docker
-WORKDIR /opt/app/package
-
 COPY ./ /opt/app/
-COPY ./config /opt/app/config
-
-# Ensuring script permissions
-RUN chmod +x /opt/app/config/run.sh
-
-RUN pip install -e .
-
-EXPOSE 80
+COPY ./config/ /opt/app/config/
+WORKDIR /opt/app
+RUN python -m pip install .
 
 # Specify the command to run when the image is run.
-CMD "/opt/app/config/run.sh"
+CMD "/opt/app/config/run.sh"
+
```

### Comparing `py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/docker-compose.yaml` & `py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/docker-compose.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,100 @@
 networks:
-  {{cookiecutter.project_name}}:
-    name:  {{cookiecutter.project_name}}
-
+  {{ cookiecutter.project_name }}:
+    name: {{ cookiecutter.project_name }}
 
 services:
-  {{cookiecutter.project_name}}:
-    image: ${REGISTRY}/{{cookiecutter.project_name}}:${APP_VERSION}
-    container_name: {{cookiecutter.project_name}}_${DOCKER_CONTAINER_SUFFIX}
+  rest_api:
+    build:
+      context: rest_api
+    image: ${REGISTRY}/rest_api:${APP_VERSION}
+    container_name: rest_api_${DOCKER_CONTAINER_SUFFIX}
     environment:
       - DEVELOP
       - APP_VERSION
       - LOG_LEVEL
       - POSTGRES_PASSWORD
       - POSTGRES_USER
       - POSTGRES_DB
+      - POSTGRES_PORT
       - REDIS_HOST=${REDIS_DOCKER_HOST}
       - POSTGRES_HOST=${POSTGRES_DOCKER_HOST}
     networks:
-      {{cookiecutter.project_name}}:
+      {{ cookiecutter.project_name }}:
         aliases:
-          - {{cookiecutter.project_name}}
+          - rest_api
     ports:
       - "8080:80"
     depends_on:
       postgresDB:
         condition: service_healthy
       redisDB:
         condition: service_healthy
+      rabbit:
+        condition: service_healthy
 
   postgresDB:
-      image: postgres
-      container_name: postgres_${DOCKER_CONTAINER_SUFFIX}
-      ports:
-        - "5432:5432"
+    image: postgres
+    container_name: postgres_${DOCKER_CONTAINER_SUFFIX}
+    ports:
+      - "5432:5432"
     environment:
       - POSTGRES_PASSWORD
       - POSTGRES_USER
       - POSTGRES_DB
-      volumes:
-        - postgresDB:/var/lib/postgresql/data
-      networks:
-        {{cookiecutter.project_name}}:
-          aliases:
-            - ${POSTGRES_HOST}
+    volumes:
+      - postgresDB:/var/lib/postgresql/data
+    networks:
+      {{ cookiecutter.project_name }}:
+        aliases:
+          - ${POSTGRES_HOST}
+    healthcheck:
+      test: ["CMD-SHELL", "pg_isready"]
+      interval: 10s
+      timeout: 5s
+      retries: 5
 
   redisDB:
     image: redis
     container_name: redis_${DOCKER_CONTAINER_SUFFIX}
     command: redis-server --appendonly yes
     volumes:
       - redisDB:/data
     ports:
       - "6379:6379"
     networks:
-      {{cookiecutter.project_name}}:
+      {{ cookiecutter.project_name }}:
         aliases:
         - ${REDIS_HOST}
     healthcheck:
       test: ["CMD", "redis-cli", "ping"]
       interval: 15s
       timeout: 5s
       retries: 3
       start_period: 20s
 
+  rabbit:
+    image: rabbitmq:3.13.1-management
+    container_name: rabbit_${DOCKER_CONTAINER_SUFFIX}
+    environment:
+      - RABBITMQ_DEFAULT_USER
+      - RABBITMQ_DEFAULT_PASS
+      - RABBITMQ_DEFAULT_VHOST
+    ports:
+      - "5672:5672"
+      - "15672:15672"
+    networks:
+      {{ cookiecutter.project_name }}:
+        aliases:
+          - ${RABBIT_DOCKER_HOST}
+    healthcheck:
+      test: rabbitmq-diagnostics -q ping
+      interval: 15s
+      timeout: 5s
+      retries: 3
+      start_period: 60s
+
 volumes:
   postgresDB:
     driver: local
   redisDB:
     driver: local
```

### Comparing `py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/Makefile` & `py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/Makefile`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 SHELL := /bin/bash
 include ../.env
 export
 
 env:
-	pip install -r requirements/local.txt
+	pip install -r requirements/local.txt  > /dev/null
 
 run:
 	@echo "Running service..."
-	python app/main.py
+	python package/run.py
 
 test:
 	@echo "Running unit tests..."
-	env TEST_DB=True coverage run -m pytest ${module} && \
+	env POSTGRES_DB=test_db coverage run -m pytest ${module} && \
 	coverage html && \
 	coverage report
 	@echo
 	@echo "Flake8 errors in code ----------------"
 	@echo
 	@echo "--------------------------------------"
 	@python -m flake8 --max-line-length=88 --exclude .git,__pycache__,.eggs,build
@@ -23,28 +23,28 @@
 	@echo "--------------------------------------"
 
 lint:
 	@python -m flake8 --max-line-length=88 --exclude .git,__pycache__,.eggs,build
 
 migrations:
 	@echo "Generating migrations ..."
-	alembic revision --autogenerate -m "${message}"
+	alembic -c ./package/alembic.ini revision --autogenerate -m "${message}"
 
 migrate:
 	@echo "Running migrations ..."
-	alembic upgrade head
+	alembic -c ./package/alembic.ini upgrade head
 	@echo "Migrations finished."
 
 downgrade:
 	@echo "Running downgrade ..."
-	alembic downgrade ${level}
+	alembic -c ./package/alembic.ini downgrade ${level}
 	@echo "Migrations finished."
 
 init_db:
 	@echo "Initing database ..."
-	alembic ensure_version
+	alembic -c ./package/alembic.ini ensure_version
 	@echo "Migrations finished."
 
 check_db:
 	@echo "Checking migrations ..."
-	alembic check
+	alembic -c ./package/alembic.ini check
 	@echo "Migrations finished."
```

### Comparing `py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/alembic.ini` & `py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/alembic.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # A generic, single database configuration.
 
 [alembic]
 # path to migration scripts
-script_location = app/alembic
+script_location = package/app/alembic
 
 # template used to generate migration files
 # file_template = %%(rev)s_%%(slug)s
 
 # timezone to use when rendering the date
 # within the migration file as well as the filename.
 # string value is passed to dateutil.tz.gettz()
```

### Comparing `py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/alembic/env.py` & `py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/env.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 from logging.config import fileConfig
 
 from alembic import context
-from app.models.base import Base, DB_URL
+from package.app.models.base import Base, DB_URL
 from psycopg.connection_async import AsyncConnection as Connection
 from sqlalchemy import pool
 from sqlalchemy.ext.asyncio import async_engine_from_config
 
 # this is the Alembic Config object, which provides
 # access to the values within the .ini file in use.
 config = context.config
@@ -27,24 +27,29 @@
     we don't even need a DBAPI to be available.
     Calls to context.execute() here emit the given string to the
     script output.
     """
     context.configure(
         url=DB_URL,
         target_metadata=target_metadata,
+        version_table="{{cookiecutter.project_name}}",
         literal_binds=True,
         dialect_opts={"paramstyle": "named"},
     )
 
     with context.begin_transaction():
         context.run_migrations()
 
 
 def do_run_migrations(connection: Connection) -> None:
-    context.configure(connection=connection, target_metadata=target_metadata)
+    context.configure(
+        connection=connection,
+        target_metadata=target_metadata,
+        version_table="{{cookiecutter.project_name}}",
+    )
 
     with context.begin_transaction():
         context.run_migrations()
 
 
 async def run_migrations_online():
     """Run migrations in 'online' mode.
```

### Comparing `py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/main.py` & `py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import inspect
 import logging
 import uvicorn
 from fastapi.middleware import Middleware
 from contextlib import asynccontextmanager
 from starlette.middleware.cors import CORSMiddleware
-from app.models import (
+from package.app.models import (
     sessionmanager,
     get_db_session,
 )
-from app import api as a_app
+from package.app import api as a_app
 from fastapi import FastAPI
 from mrkutil.logging import get_logging_config
 
 log_level = os.getenv("LOG_LEVEL", "DEBUG")
 develop = bool("true" == str(os.getenv("DEVELOP", "false")).lower())
 json_format = bool("true" == str(os.getenv("JSON_FORMAT", "false")).lower())
 
@@ -62,26 +62,26 @@
 for name, obj in inspect.getmembers(a_app):
     if "_router" in name:
         app.include_router(obj, prefix=API_STR)
 
 
 def dev():
     uvicorn.run(
-        "app.main:app",
+        "package.app.main:app",
         host="0.0.0.0",
         port=8080,
         reload=True,
         log_level=log_level.lower(),
         log_config=logging_config,
     )
 
 
 def prod():
     uvicorn.run(
-        "app.main:app",
+        "package.app.main:app",
         headers=[
             ("server", "Apache"),
             ("X-Frame-Options", "SAMEORIGIN"),
             ("X-XSS-Protection", "1; mode=block"),
             ("X-Content-Type-Options", "nosniff"),
             ("Strict-Transport-Security", "max-age=15768000; includeSubDomains"),
             ("Referrer-Policy", "no-referrer-when-downgrade"),
```

### Comparing `py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/app/models/base.py` & `py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/models/base.py`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.2.1/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/package/tests/conftest.py` & `py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from contextlib import ExitStack
 
 import pytest
 from alembic.config import Config
 from alembic.migration import MigrationContext
 from alembic.operations import Operations
 from alembic.script import ScriptDirectory
-from app.models import Base, get_db_session
-from app.models.base import DatabaseSessionManager
-from app.main import app as actual_app
+from package.app.models import Base, get_db_session
+from package.app.models.base import DatabaseSessionManager
+from package.app.main import app as actual_app
 from psycopg.connection_async import AsyncConnection as Connection
 
 from fastapi.testclient import TestClient
 from sqlalchemy.pool import NullPool
 from sqlalchemy.ext.asyncio import (
     create_async_engine,
 )
@@ -36,16 +36,16 @@
 @pytest.fixture
 def client(event_loop, app):
     with TestClient(app) as c:
         yield c
 
 
 def run_migrations(connection: Connection):
-    config = Config("app/alembic.ini")
-    config.set_main_option("script_location", "app/alembic")
+    config = Config("package/alembic.ini")
+    config.set_main_option("script_location", "package/app/alembic")
     config.set_main_option("sqlalchemy.url", DB_URL)
     script = ScriptDirectory.from_config(config)
 
     def upgrade(rev, context):
         return script._upgrade_revs("head", rev)
 
     context = MigrationContext.configure(
```

### Comparing `py_template_creator-1.2.1/py_template_creator/main.py` & `py_template_creator-1.3.0/py_template_creator/main.py`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/Dockerfile` & `py_template_creator-1.3.0/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/Dockerfile`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 ARG PYTHON_VERSION=3.12-slim
 
 # Stage 0, instaling dev packages
 FROM python:${PYTHON_VERSION} as builder
 LABEL maintainer="{{cookiecutter.author_name}} <{{cookiecutter.author_email}}>"
 ENV PYTHONUNBUFFERED 1
 
+RUN apt-get update && apt-get -y install build-essential libpq-dev
 WORKDIR /wheels
-COPY ./$APP_DIR/requirements/ /wheels/requirements/
+COPY ./requirements/ /wheels/requirements/
 RUN pip install -U pip && pip wheel -r ./requirements/prod.txt
 
 # Stage 1, no dev packages on wheels
 FROM python:${PYTHON_VERSION}
 ENV PYTHONUNBUFFERED=1
 
 COPY --from=builder /wheels /wheels
@@ -18,15 +19,19 @@
        && pip install -r /wheels/requirements/prod.txt \
                       -f /wheels \
        && rm -rf /wheels \
        && rm -rf /root/.cache/pip/*
 
 
 # Copy code to docker
-COPY ./ /opt/app/
-COPY ./config/ /opt/app/config/
 WORKDIR /opt/app
-RUN python -m pip install .
 
-# Specify the command to run when the image is run.
-CMD "/opt/app/config/run.sh"
+COPY ./ /opt/app/
+COPY ./config /opt/app/config
 
+# Ensuring script permissions
+RUN chmod +x /opt/app/config/run.sh
+
+RUN pip install -e .
+
+# Specify the command to run when the image is run.
+CMD "/opt/app/config/run.sh"
```

### Comparing `py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/README.md` & `py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-# {{ cookiecutter.service_name }} service
+# {{ cookiecutter.project_name }} service
 
 ## Setup service
 
 - create virtualenv with virtualenv wrapper
 ```
-cd {{ cookiecutter.service_name }}
+cd {{ cookiecutter.project_name }}
 mkvirtualenv <env name> --python=/path/to/python/executable/python3.12.*
 ```
 
 - install packages needed for the project
 ```
 make env
 ```
 
 
 ## Start service
 
 - stop docker container for this service
 ```
 cd <project root>
-docker-compose stop {{ cookiecutter.service_name }}
+docker-compose stop {{ cookiecutter.project_name }}
 ```
 
 - start service from virtual environment
 ```
-cd {{ cookiecutter.service_name }}
+cd {{ cookiecutter.project_name }}
 workon <env name>
 make run
 ```
 
 
 ## Run tests
 
 - tests are run on virtual environment
 ```
-cd {{ cookiecutter.service_name }}
+cd {{ cookiecutter.project_name }}
 workon <env name>
 ```
 
 - run all tests
 ```
 make test
 ```
```

### Comparing `py_template_creator-1.2.1/py_template_creator/service-scelet/{{ cookiecutter.service_name }}/package/run.py` & `py_template_creator-1.3.0/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,27 @@
     """
     App starting point
     """
     try:
         pid = str(os.getpid())
         if not os.path.isdir("/tmp/service"):
             os.makedirs("/tmp/service")
-        pidfile = "/tmp/service_{{ cookiecutter.service_name }}.pid"
+        pidfile = "/tmp/service_{{ cookiecutter.project_name }}.pid"
         if os.path.isfile(pidfile):
             logger.warning("Service is already running")
             sys.exit(1)
         with open(pidfile, 'w') as file:
             file.write(pid)
             file.write("\n")
         try:
             logger.info("Starting ...")
             listen(
-                exchange=os.getenv("EXCHANGE_{{ cookiecutter.service_name.upper() }}"),
-                exchange_type=os.getenv("EXCHANGE_TYPE_{{ cookiecutter.service_name.upper() }}"),
-                queue=os.getenv("QUEUE_{{ cookiecutter.service_name.upper() }}"),
+                exchange=os.getenv("EXCHANGE_{{ cookiecutter.project_name.upper() }}"),
+                exchange_type=os.getenv("EXCHANGE_TYPE_{{ cookiecutter.project_name.upper() }}"),
+                queue=os.getenv("QUEUE_{{ cookiecutter.project_name.upper() }}"),
             )
             sys.exit(0)
         finally:
             os.unlink(pidfile)
     except KeyboardInterrupt:
         print("Watchfiles detected changes ... reloading now")
```

### Comparing `py_template_creator-1.2.1/PKG-INFO` & `py_template_creator-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_template_creator
-Version: 1.2.1
+Version: 1.3.0
 Summary: Generate your python project template with ease.
 Author-email: Ivan Djuraki <ivan.djuraki@bridgewaterlabs.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: cookiecutter
```

