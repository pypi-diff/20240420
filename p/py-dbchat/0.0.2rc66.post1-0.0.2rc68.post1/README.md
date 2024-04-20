# Comparing `tmp/py_dbchat-0.0.2rc66.post1.tar.gz` & `tmp/py_dbchat-0.0.2rc68.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_dbchat-0.0.2rc66.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_dbchat-0.0.2rc68.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_dbchat-0.0.2rc66.post1.tar` & `py_dbchat-0.0.2rc68.post1.tar`

### file list

```diff
@@ -1,63 +1,66 @@
--rw-r--r--   0        0        0      333 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1156 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1009 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.devcontainer/docker-compose.yml
--rw-r--r--   0        0        0      417 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.github/template-sync.yml
--rw-r--r--   0        0        0      476 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.gitignore
--rw-r--r--   0        0        0     1381 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.pypirc
--rw-r--r--   0        0        0      459 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1211 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/.vscode/settings.json
--rw-r--r--   0        0        0      444 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/LICENSE
--rw-r--r--   0        0        0       41 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/README.md
--rw-r--r--   0        0        0     2780 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/SECURITY.md
--rw-r--r--   0        0        0     1308 2024-03-27 01:58:29.548328 py_dbchat-0.0.2rc66.post1/SUPPORT.md
--rw-r--r--   0        0        0      655 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/Test.session.sql
--rw-r--r--   0        0        0      634 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/developer.md
--rw-r--r--   0        0        0      468 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/make.bat
--rw-r--r--   0        0        0       50 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/pyproject.md
--rw-r--r--   0        0        0      423 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      406 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/python_package.rst
--rw-r--r--   0        0        0       65 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/docs/workflows.md
--rw-r--r--   0        0        0      199 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/playground.py
--rw-r--r--   0        0        0     6679 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/pyproject.toml
--rw-r--r--   0        0        0       41 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/README.md
--rw-r--r--   0        0        0     6148 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/.DS_Store
--rw-r--r--   0        0        0      374 2024-03-27 01:58:42.436303 py_dbchat-0.0.2rc66.post1/src/db_chat/__init__.py
--rw-r--r--   0        0        0      725 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/ask.py
--rw-r--r--   0        0        0      662 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/hello_world.py
--rw-r--r--   0        0        0     3308 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/llm/classic_prompt.py
--rw-r--r--   0        0        0     3518 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/llm/function_calling.py
--rw-r--r--   0        0        0     6791 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/llm/llm.py
--rw-r--r--   0        0        0     1135 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/llm/llm_langchain_sample.py
--rw-r--r--   0        0        0      250 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/sql_builder/Filter.py
--rw-r--r--   0        0        0      236 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/sql_builder/FilterOperator.py
--rw-r--r--   0        0        0     2498 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/sql_builder/Query.py
--rw-r--r--   0        0        0      159 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/sql_builder/SortOrder.py
--rw-r--r--   0        0        0        0 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/sql_builder/__init__.py
--rw-r--r--   0        0        0      453 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/sql_builder/mappings.py
--rw-r--r--   0        0        0     5193 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/sql_builder/schema.py
--rw-r--r--   0        0        0     8781 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/sql_builder/sql_builder.py
--rw-r--r--   0        0        0    15247 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py
--rw-r--r--   0        0        0      989 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/tests/conftest.py
--rw-r--r--   0        0        0     1210 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/tests/test_methods.py
--rw-r--r--   0        0        0      269 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/tests/test_schema_builder.py
--rw-r--r--   0        0        0    12288 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/tests/test_sql_builder.py
--rw-r--r--   0        0        0     7124 2024-03-27 01:58:29.552328 py_dbchat-0.0.2rc66.post1/tests/test_sqlalchemy.py
--rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 py_dbchat-0.0.2rc66.post1/PKG-INFO
+-rw-r--r--   0        0        0      333 2024-04-20 04:59:14.084689 py_dbchat-0.0.2rc68.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1156 2024-04-20 04:59:14.084689 py_dbchat-0.0.2rc68.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1084 2024-04-20 04:59:14.084689 py_dbchat-0.0.2rc68.post1/.devcontainer/docker-compose.yml
+-rw-r--r--   0        0        0      417 2024-04-20 04:59:14.084689 py_dbchat-0.0.2rc68.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-20 04:59:14.084689 py_dbchat-0.0.2rc68.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      476 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/.gitignore
+-rw-r--r--   0        0        0     1381 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1211 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/.vscode/settings.json
+-rw-r--r--   0        0        0      444 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/LICENSE
+-rw-r--r--   0        0        0       41 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/README.md
+-rw-r--r--   0        0        0     2780 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/SECURITY.md
+-rw-r--r--   0        0        0     1308 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/SUPPORT.md
+-rw-r--r--   0        0        0      655 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/Test.session.sql
+-rw-r--r--   0        0        0      634 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/make.bat
+-rw-r--r--   0        0        0       50 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      423 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      406 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       65 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/docs/workflows.md
+-rw-r--r--   0        0        0      203 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/playground.py
+-rw-r--r--   0        0        0     6679 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/pyproject.toml
+-rw-r--r--   0        0        0      109 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/README.md
+-rw-r--r--   0        0        0      161 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/Roadmap.md
+-rw-r--r--   0        0        0     6148 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/.DS_Store
+-rw-r--r--   0        0        0      374 2024-04-20 04:59:26.208761 py_dbchat-0.0.2rc68.post1/src/db_chat/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/ask.py
+-rw-r--r--   0        0        0      662 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/hello_world.py
+-rw-r--r--   0        0        0     3308 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/llm/classic_prompt.py
+-rw-r--r--   0        0        0     3518 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/llm/function_calling.py
+-rw-r--r--   0        0        0     6791 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/llm/llm.py
+-rw-r--r--   0        0        0     1135 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/llm/llm_langchain_sample.py
+-rw-r--r--   0        0        0      250 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/sql_builder/Filter.py
+-rw-r--r--   0        0        0      236 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/sql_builder/FilterOperator.py
+-rw-r--r--   0        0        0     2478 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/sql_builder/Query.py
+-rw-r--r--   0        0        0      159 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/sql_builder/SortOrder.py
+-rw-r--r--   0        0        0        0 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/sql_builder/__init__.py
+-rw-r--r--   0        0        0      453 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/sql_builder/mappings.py
+-rw-r--r--   0        0        0     5193 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/sql_builder/schema.py
+-rw-r--r--   0        0        0     8781 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/sql_builder/sql_builder.py
+-rw-r--r--   0        0        0    16036 2024-04-20 04:59:14.088689 py_dbchat-0.0.2rc68.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py
+-rw-r--r--   0        0        0   600200 2024-04-20 04:59:14.092689 py_dbchat-0.0.2rc68.post1/test/Chinook_PostgreSql.sql
+-rw-r--r--   0        0        0      989 2024-04-20 04:59:14.092689 py_dbchat-0.0.2rc68.post1/tests/conftest.py
+-rw-r--r--   0        0        0     2922 2024-04-20 04:59:14.092689 py_dbchat-0.0.2rc68.post1/tests/test_explicit_joins.py
+-rw-r--r--   0        0        0     1210 2024-04-20 04:59:14.092689 py_dbchat-0.0.2rc68.post1/tests/test_methods.py
+-rw-r--r--   0        0        0      269 2024-04-20 04:59:14.092689 py_dbchat-0.0.2rc68.post1/tests/test_schema_builder.py
+-rw-r--r--   0        0        0    12288 2024-04-20 04:59:14.092689 py_dbchat-0.0.2rc68.post1/tests/test_sql_builder.py
+-rw-r--r--   0        0        0     7124 2024-04-20 04:59:14.092689 py_dbchat-0.0.2rc68.post1/tests/test_sqlalchemy.py
+-rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 py_dbchat-0.0.2rc68.post1/PKG-INFO
```

### Comparing `py_dbchat-0.0.2rc66.post1/.devcontainer/devcontainer.json` & `py_dbchat-0.0.2rc68.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/.devcontainer/docker-compose.yml` & `py_dbchat-0.0.2rc68.post1/.devcontainer/docker-compose.yml`

 * *Files 16% similar despite different names*

```diff
@@ -10,26 +10,25 @@
       - ../..:/workspaces:cached
 
     # Overrides default command so things don't shut down after the process ends.
     command: sleep infinity
 
     # Runs app on the same network as the database container, allows "forwardPorts" in devcontainer.json function.
     network_mode: service:db
-
     # Use "forwardPorts" in **devcontainer.json** to forward an app port locally.
     # (Adding the "ports" property to this file will not forward from a Codespace.)
 
   db:
     image: postgres:latest
     restart: unless-stopped
     volumes:
       - postgres-data:/var/lib/postgresql/data
+      - .test/Chinook_PostgreSql.sql:/docker-entrypoint-initdb.d/Chinook.sql
     environment:
       POSTGRES_USER: postgres
       POSTGRES_DB: postgres
       POSTGRES_PASSWORD: postgres
-
     # Add "forwardPorts": ["5432"] to **devcontainer.json** to forward PostgreSQL locally.
     # (Adding the "ports" property to this file will not forward from a Codespace.)
 
 volumes:
   postgres-data:
```

### Comparing `py_dbchat-0.0.2rc66.post1/.github/workflows/schedule-update-actions.yml` & `py_dbchat-0.0.2rc68.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/.gitignore` & `py_dbchat-0.0.2rc68.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/.pre-commit-config.yaml` & `py_dbchat-0.0.2rc68.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/.vscode/settings.json` & `py_dbchat-0.0.2rc68.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/LICENSE` & `py_dbchat-0.0.2rc68.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/SECURITY.md` & `py_dbchat-0.0.2rc68.post1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/SUPPORT.md` & `py_dbchat-0.0.2rc68.post1/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/Test.session.sql` & `py_dbchat-0.0.2rc68.post1/Test.session.sql`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/docs/Makefile` & `py_dbchat-0.0.2rc68.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/docs/conf.py` & `py_dbchat-0.0.2rc68.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/docs/make.bat` & `py_dbchat-0.0.2rc68.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/docs/pylint.md` & `py_dbchat-0.0.2rc68.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/pyproject.toml` & `py_dbchat-0.0.2rc68.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/src/db_chat/.DS_Store` & `py_dbchat-0.0.2rc68.post1/src/db_chat/.DS_Store`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/src/db_chat/ask.py` & `py_dbchat-0.0.2rc68.post1/src/db_chat/ask.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/src/db_chat/hello_world.py` & `py_dbchat-0.0.2rc68.post1/src/db_chat/hello_world.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/src/db_chat/llm/classic_prompt.py` & `py_dbchat-0.0.2rc68.post1/src/db_chat/llm/classic_prompt.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/src/db_chat/llm/function_calling.py` & `py_dbchat-0.0.2rc68.post1/src/db_chat/llm/function_calling.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/src/db_chat/llm/llm.py` & `py_dbchat-0.0.2rc68.post1/src/db_chat/llm/llm.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/src/db_chat/llm/llm_langchain_sample.py` & `py_dbchat-0.0.2rc68.post1/src/db_chat/llm/llm_langchain_sample.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/src/db_chat/sql_builder/Query.py` & `py_dbchat-0.0.2rc68.post1/src/db_chat/sql_builder/Query.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,17 +68,16 @@
 
 @dataclasses.dataclass
 class Join:
     """
     Class to encapsulate a join
     """
 
-    query: Query
+    # query: Query
     table: str
-    alias: str = None
 
     # TODO: this should be a list of conditions rather than a single equality condition. But for later
     field: str = None
     related_field: str = None
     join_type: str = "JOIN"
 
     def __post_init__(self):
```

### Comparing `py_dbchat-0.0.2rc66.post1/src/db_chat/sql_builder/schema.py` & `py_dbchat-0.0.2rc68.post1/src/db_chat/sql_builder/schema.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/src/db_chat/sql_builder/sql_builder.py` & `py_dbchat-0.0.2rc68.post1/src/db_chat/sql_builder/sql_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py` & `py_dbchat-0.0.2rc68.post1/src/db_chat/sql_builder/sqlalchemy_query_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """     Query Builder that builds SQL Alchmey Query """
 
 from __future__ import annotations
 
 from db_chat.sql_builder.schema import Column, Schema, Table
-from sqlalchemy import Label, alias, and_, select, table, column, TableClause, func
+from sqlalchemy import Label, alias, and_, select, table, column, TableClause, func, ColumnClause
 from db_chat.sql_builder.Filter import Filter
 from db_chat.sql_builder.FilterOperator import FilterOperator
 
 from db_chat.sql_builder.Query import Expression, Functions, Query
 from db_chat.sql_builder.mappings import Relationship
 
 
@@ -63,15 +63,15 @@
         return sql
 
     def _build_from_clause(self):
         """
         Build the FROM clause
         """
 
-        # self._build_joins()
+        self._build_joins()
 
         from_clause = self._build_select_clause_for_fields()
 
         from_clause, filter_clauses, sa_having_clauses = self._build_filter_clause(
             self.query, self.sa_table, self.joined_paths, self.joined_tables, from_clause
         )
 
@@ -94,21 +94,21 @@
 
         return statement
 
     def _build_joins(self):
         for join_key in self.query.joins:
             join = self.query.joins[join_key]
             join_table = self._get_table_from_mapping(join.table)
-            join_to_aliased_table = alias(join_table, join.alias)
+            join_to_aliased_table = alias(join_table, join_key)
             join_condition = self.sa_table.columns.get(join.field) == join_to_aliased_table.columns.get(
                 join.related_field
             )
             self.sa_table = self.sa_table.join(join_to_aliased_table, join_condition)
-            self.joined_paths.append(join.alias)
-            self.joined_tables[join.alias] = join_to_aliased_table
+            self.joined_paths.append(join_key)
+            self.joined_tables[join_key] = join_to_aliased_table
 
     def _append_non_having_clauses_to_group_by(self, select_columns, sa_having_clauses, group_by_clauses):
         select_columns_without_aggregates = [
             select_column for select_column in select_columns if not self._is_sa_column_aggregate(select_column)
         ]
         if sa_having_clauses and len(sa_having_clauses) > 0:
             group_by_clauses += select_columns_without_aggregates
@@ -217,16 +217,24 @@
                 continue
 
             field_column = self._get_field_from_table(self.query.table, field_name)
 
             current_table_name = self.query.table
             current_alias = self.query.table
 
+            if isinstance(field_column, ColumnClause):
+                self.select_columns.append(field_column)
+                continue
+
             if not field_column.relationships:
-                self.select_columns.append(self.sa_table.columns.get(field_column.name))
+                sa_colum_to_select = self._get_sa_column_from_sa_table_clause(
+                    self.sa_table, field_column.name, self.query.table
+                )
+                self.select_columns.append(sa_colum_to_select)
+                continue
 
             if field_column.relationships:
                 from_clause, join_to_aliased_table = self._build_join_for_relationship(
                     self.sa_table,
                     from_clause,
                     self.joined_paths,
                     self.joined_tables,
@@ -234,17 +242,24 @@
                     current_table_name,
                     current_alias,
                 )
 
                 self.select_columns.append(
                     join_to_aliased_table.columns.get(field_column.related_field).label(field_column.name)
                 )
+                continue
 
         return from_clause
 
+    def _get_sa_column_from_sa_table_clause(self, sa_table: TableClause, column_name: str, sa_table_name: str):
+        for column in sa_table.columns:
+            if column.name == column_name and column.table.name == sa_table_name:
+                return column
+        return None
+
     def _build_clause_for_expression(
         self,
         query: Query,
         from_clause: TableClause,
         expression: Expression,
         sa_table: TableClause,
         joined_paths,
@@ -352,15 +367,18 @@
             current_table_name = target_table_name
             previous_table = join_to_aliased_table
         return from_clause, join_to_aliased_table
 
     def _get_relationship_by_name(self, relationship_name):
         return next((rel for rel in self.schema.relationships if rel.name == relationship_name), None)
 
-    def _get_field_from_table(self, table_name, field_name):
+    def _get_field_from_table(self, table_name, field_name: str):
+        if "." in field_name:
+            table_name, field_name = field_name.split(".")
+            return self.joined_tables[table_name].columns.get(field_name)
         return next(
             (c for c in self.schema.tables[table_name].columns if c.name == field_name),
             None,
         )
 
     def _get_table_from_mapping(self, table_name: str):
         """
```

### Comparing `py_dbchat-0.0.2rc66.post1/tests/conftest.py` & `py_dbchat-0.0.2rc68.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/tests/test_methods.py` & `py_dbchat-0.0.2rc68.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/tests/test_sql_builder.py` & `py_dbchat-0.0.2rc68.post1/tests/test_sql_builder.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/tests/test_sqlalchemy.py` & `py_dbchat-0.0.2rc68.post1/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `py_dbchat-0.0.2rc66.post1/PKG-INFO` & `py_dbchat-0.0.2rc68.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-dbchat
-Version: 0.0.2rc66.post1
+Version: 0.0.2rc68.post1
 Summary: Chat with your existing database without using vector DB.
 Author-email: Dhanilan <mail2dhanilan@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

