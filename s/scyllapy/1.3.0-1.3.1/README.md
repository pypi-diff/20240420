# Comparing `tmp/scyllapy-1.3.0.tar.gz` & `tmp/scyllapy-1.3.1.tar.gz`

## Comparing `scyllapy-1.3.0.tar` & `scyllapy-1.3.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0      875 1970-01-01 00:00:00.000000 scyllapy-1.3.0/Cargo.toml
--rw-r--r--   0     1001      127     5151 2023-11-03 20:14:28.000000 scyllapy-1.3.0/.github/workflows/release.yaml
--rw-r--r--   0     1001      127     2579 2023-11-03 20:14:28.000000 scyllapy-1.3.0/.github/workflows/test.yaml
--rw-r--r--   0     1001      127     3113 2023-11-03 20:14:28.000000 scyllapy-1.3.0/.gitignore
--rw-r--r--   0     1001      127     1767 2023-11-03 20:14:28.000000 scyllapy-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      127       29 2023-11-03 20:14:28.000000 scyllapy-1.3.0/.python-version
--rw-r--r--   0     1001      127     1067 2023-11-03 20:14:28.000000 scyllapy-1.3.0/LICENSE
--rw-r--r--   0     1001      127    13058 2023-11-03 20:14:28.000000 scyllapy-1.3.0/README.md
--rw-r--r--   0     1001      127      503 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/scyllapy/__init__.py
--rw-r--r--   0     1001      127     8829 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/scyllapy/_internal/__init__.pyi
--rw-r--r--   0     1001      127     1324 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/scyllapy/_internal/exceptions.pyi
--rw-r--r--   0     1001      127      682 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/scyllapy/_internal/extra_types.pyi
--rw-r--r--   0     1001      127     2054 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/scyllapy/_internal/load_balancing.pyi
--rw-r--r--   0     1001      127     4494 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/scyllapy/_internal/query_builder.pyi
--rw-r--r--   0     1001      127      369 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/scyllapy/exceptions.py
--rw-r--r--   0     1001      127     1521 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/scyllapy/extra_types.py
--rw-r--r--   0     1001      127      131 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/scyllapy/load_balancing.py
--rw-r--r--   0     1001      127        0 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/scyllapy/py.typed
--rw-r--r--   0     1001      127      120 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/scyllapy/query_builder.py
--rw-r--r--   0     1001      127        0 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/__init__.py
--rw-r--r--   0     1001      127     1168 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/conftest.py
--rw-r--r--   0     1001      127        0 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/query_builders/__init__.py
--rw-r--r--   0     1001      127     2056 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/query_builders/test_delete.py
--rw-r--r--   0     1001      127     1540 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/query_builders/test_inserts.py
--rw-r--r--   0     1001      127     3910 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/query_builders/test_select.py
--rw-r--r--   0     1001      127     1583 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/query_builders/test_update.py
--rw-r--r--   0     1001      127      602 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/test_batches.py
--rw-r--r--   0     1001      127     4327 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/test_bindings.py
--rw-r--r--   0     1001      127     4306 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/test_extra_types.py
--rw-r--r--   0     1001      127     2390 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/test_pagination.py
--rw-r--r--   0     1001      127      666 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/test_parsing.py
--rw-r--r--   0     1001      127      558 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/test_prepared.py
--rw-r--r--   0     1001      127      672 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/test_profiles.py
--rw-r--r--   0     1001      127     1769 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/test_queries.py
--rw-r--r--   0     1001      127      456 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/test_query_res.py
--rw-r--r--   0     1001      127      154 2023-11-03 20:14:28.000000 scyllapy-1.3.0/python/tests/utils.py
--rw-r--r--   0     1001      127     3755 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/batches.rs
--rw-r--r--   0     1001      127     1913 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/consistencies.rs
--rw-r--r--   0     1001      127       34 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/exceptions/mod.rs
--rw-r--r--   0     1001      127     1424 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/exceptions/py_err.rs
--rw-r--r--   0     1001      127     3281 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/exceptions/rust_err.rs
--rw-r--r--   0     1001      127     1883 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/execution_profiles.rs
--rw-r--r--   0     1001      127     1546 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/extra_types.rs
--rw-r--r--   0     1001      127     1827 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/inputs.rs
--rw-r--r--   0     1001      127     1401 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/lib.rs
--rw-r--r--   0     1001      127     4312 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/load_balancing.rs
--rw-r--r--   0     1001      127      483 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/prepared_queries.rs
--rw-r--r--   0     1001      127     6196 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/queries.rs
--rw-r--r--   0     1001      127     7501 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/query_builder/delete.rs
--rw-r--r--   0     1001      127     5820 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/query_builder/insert.rs
--rw-r--r--   0     1001      127      649 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/query_builder/mod.rs
--rw-r--r--   0     1001      127     8074 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/query_builder/select.rs
--rw-r--r--   0     1001      127     9840 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/query_builder/update.rs
--rw-r--r--   0     1001      127     1090 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/query_builder/utils.rs
--rw-r--r--   0     1001      127     9485 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/query_results.rs
--rw-r--r--   0     1001      127    16230 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/scylla_cls.rs
--rw-r--r--   0     1001      127    25633 2023-11-03 20:14:28.000000 scyllapy-1.3.0/src/utils.rs
--rw-r--r--   0     1001      127      369 2023-11-03 20:14:28.000000 scyllapy-1.3.0/tox.ini
--rw-r--r--   0     1001      127    32442 2023-11-03 20:14:33.000000 scyllapy-1.3.0/Cargo.lock
--rw-r--r--   0     1001      127     3168 2023-11-03 20:14:28.000000 scyllapy-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    13680 1970-01-01 00:00:00.000000 scyllapy-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 scyllapy-1.3.1/Cargo.toml
+-rw-r--r--   0     1001      127     5151 2024-04-20 09:29:46.000000 scyllapy-1.3.1/.github/workflows/release.yaml
+-rw-r--r--   0     1001      127     2579 2024-04-20 09:29:46.000000 scyllapy-1.3.1/.github/workflows/test.yaml
+-rw-r--r--   0     1001      127     3113 2024-04-20 09:29:46.000000 scyllapy-1.3.1/.gitignore
+-rw-r--r--   0     1001      127     1836 2024-04-20 09:29:46.000000 scyllapy-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127       29 2024-04-20 09:29:46.000000 scyllapy-1.3.1/.python-version
+-rw-r--r--   0     1001      127     1067 2024-04-20 09:29:46.000000 scyllapy-1.3.1/LICENSE
+-rw-r--r--   0     1001      127    14472 2024-04-20 09:29:46.000000 scyllapy-1.3.1/README.md
+-rw-r--r--   0     1001      127      503 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/scyllapy/__init__.py
+-rw-r--r--   0     1001      127     8829 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/scyllapy/_internal/__init__.pyi
+-rw-r--r--   0     1001      127     1324 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/scyllapy/_internal/exceptions.pyi
+-rw-r--r--   0     1001      127      682 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/scyllapy/_internal/extra_types.pyi
+-rw-r--r--   0     1001      127     2054 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/scyllapy/_internal/load_balancing.pyi
+-rw-r--r--   0     1001      127     4494 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/scyllapy/_internal/query_builder.pyi
+-rw-r--r--   0     1001      127      369 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/scyllapy/exceptions.py
+-rw-r--r--   0     1001      127     1521 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/scyllapy/extra_types.py
+-rw-r--r--   0     1001      127      131 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/scyllapy/load_balancing.py
+-rw-r--r--   0     1001      127        0 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/scyllapy/py.typed
+-rw-r--r--   0     1001      127      120 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/scyllapy/query_builder.py
+-rw-r--r--   0     1001      127        0 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/__init__.py
+-rw-r--r--   0     1001      127     1168 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/conftest.py
+-rw-r--r--   0     1001      127        0 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/query_builders/__init__.py
+-rw-r--r--   0     1001      127     2056 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/query_builders/test_delete.py
+-rw-r--r--   0     1001      127     1540 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/query_builders/test_inserts.py
+-rw-r--r--   0     1001      127     3910 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/query_builders/test_select.py
+-rw-r--r--   0     1001      127     1583 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/query_builders/test_update.py
+-rw-r--r--   0     1001      127      602 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/test_batches.py
+-rw-r--r--   0     1001      127     4590 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/test_bindings.py
+-rw-r--r--   0     1001      127     4988 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/test_extra_types.py
+-rw-r--r--   0     1001      127     2390 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/test_pagination.py
+-rw-r--r--   0     1001      127      666 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/test_parsing.py
+-rw-r--r--   0     1001      127      558 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/test_prepared.py
+-rw-r--r--   0     1001      127      672 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/test_profiles.py
+-rw-r--r--   0     1001      127     1769 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/test_queries.py
+-rw-r--r--   0     1001      127      456 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/test_query_res.py
+-rw-r--r--   0     1001      127      154 2024-04-20 09:29:46.000000 scyllapy-1.3.1/python/tests/utils.py
+-rw-r--r--   0     1001      127     3786 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/batches.rs
+-rw-r--r--   0     1001      127     1913 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/consistencies.rs
+-rw-r--r--   0     1001      127       34 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/exceptions/mod.rs
+-rw-r--r--   0     1001      127     1424 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/exceptions/py_err.rs
+-rw-r--r--   0     1001      127     3302 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/exceptions/rust_err.rs
+-rw-r--r--   0     1001      127     1883 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/execution_profiles.rs
+-rw-r--r--   0     1001      127     1546 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/extra_types.rs
+-rw-r--r--   0     1001      127     1827 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/inputs.rs
+-rw-r--r--   0     1001      127     1401 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/lib.rs
+-rw-r--r--   0     1001      127     4312 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/load_balancing.rs
+-rw-r--r--   0     1001      127      483 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/prepared_queries.rs
+-rw-r--r--   0     1001      127     6203 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/queries.rs
+-rw-r--r--   0     1001      127     7500 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/query_builder/delete.rs
+-rw-r--r--   0     1001      127     5819 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/query_builder/insert.rs
+-rw-r--r--   0     1001      127      649 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/query_builder/mod.rs
+-rw-r--r--   0     1001      127     8087 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/query_builder/select.rs
+-rw-r--r--   0     1001      127     9840 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/query_builder/update.rs
+-rw-r--r--   0     1001      127     1090 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/query_builder/utils.rs
+-rw-r--r--   0     1001      127     9717 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/query_results.rs
+-rw-r--r--   0     1001      127    16603 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/scylla_cls.rs
+-rw-r--r--   0     1001      127    29115 2024-04-20 09:29:46.000000 scyllapy-1.3.1/src/utils.rs
+-rw-r--r--   0     1001      127      369 2024-04-20 09:29:46.000000 scyllapy-1.3.1/tox.ini
+-rw-r--r--   0     1001      127    39595 2024-04-20 09:29:51.000000 scyllapy-1.3.1/Cargo.lock
+-rw-r--r--   0     1001      127     3193 2024-04-20 09:29:46.000000 scyllapy-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    15125 1970-01-01 00:00:00.000000 scyllapy-1.3.1/PKG-INFO
```

### Comparing `scyllapy-1.3.0/Cargo.toml` & `scyllapy-1.3.1/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [package]
 name = "scyllapy"
-version = "1.3.0"
+version = "1.3.1"
 edition = "2021"
 
 [lib]
 name = "scyllapy"
 crate-type = ["cdylib"]
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 chrono = "0.4.31"
 eq-float = "0.1.0"
 futures = "0.3.28"
 log = "0.4.20"
 openssl = { version = "0.10.57", features = ["vendored"] }
-pyo3 = { version = "0.19.2", features = [
+pyo3 = { version = "0.20.0", features = [
     "auto-initialize",
     "abi3-py38",
     "extension-module",
     "chrono",
 ] }
-pyo3-asyncio = { version = "0.19.0", features = ["tokio-runtime"] }
-pyo3-log = "0.8.3"
+pyo3-asyncio = { version = "0.20.0", features = ["tokio-runtime"] }
+pyo3-log = "0.9.0"
 rustc-hash = "1.1.0"
-scylla = { version = "0.10.1", features = ["ssl"] }
-scylla-cql = "0.0.9"
+scylla = { version = "0.12.0", features = ["ssl", "full-serialization"] }
+bigdecimal-04 = { package = "bigdecimal", version = "0.4" }
 thiserror = "1.0.48"
 tokio = { version = "1.32.0", features = ["bytes"] }
 uuid = { version = "1.4.1", features = ["v4"] }
+time = { version = "*", features = ["formatting", "macros"] }
 
 [profile.release]
 lto = "fat"
 codegen-units = 1
 opt-level = 3
 debug = false
 panic = "abort"
```

### Comparing `scyllapy-1.3.0/.github/workflows/release.yaml` & `scyllapy-1.3.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/.github/workflows/test.yaml` & `scyllapy-1.3.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/.gitignore` & `scyllapy-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/.pre-commit-config.yaml` & `scyllapy-1.3.1/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,21 @@
     hooks:
       - id: black
         name: python black
         pass_filenames: false
         always_run: true
         args: ["python"]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.5.1
+    rev: v1.9.0
     hooks:
       - id: mypy
         name: python mypy
         always_run: true
+        additional_dependencies:
+          - "types-python-dateutil"
         pass_filenames: false
         args: ["python"]
   - repo: https://github.com/astral-sh/ruff-pre-commit
     rev: v0.0.291
     hooks:
       - id: ruff
         name: ruff
```

### Comparing `scyllapy-1.3.0/LICENSE` & `scyllapy-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/README.md` & `scyllapy-1.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -85,14 +85,43 @@
 query = Query("SELECT * FROM table")
 
 new_query = query.with_consistency(Consistency.ALL)
 ```
 
 All `with_` methods create new query, copying all other parameters.
 
+Here's the list of scylla types and corresponding python types that you should use while passing parameters to queries:
+
+| Scylla type | Python type            |
+| ----------- | ---------------------- |
+| int         | int                    |
+| tinyint     | extra_types.TinyInt    |
+| bigint      | extra_types.BigInt     |
+| varint      | any int type           |
+| float       | float                  |
+| double      | extra_types.Double     |
+| decimal     | decimal.Decimal        |
+| ascii       | str                    |
+| text        | str                    |
+| varchar     | str                    |
+| blob        | bytes                  |
+| boolean     | bool                   |
+| counter     | extra_types.Counter    |
+| date        | datetime.date          |
+| uuid        | uuid.UUID              |
+| inet        | ipaddress              |
+| time        | datetime.time          |
+| timestamp   | datetime.datetime      |
+| duration    | dateutil.relativedelta |
+
+All types from `extra_types` module are used to eliminate any possible ambiguity while passing parameters to queries. You can find more information about them in `Extra types` section.
+
+We use relative delta from `dateutil` for duration, because it's the only way to represent it in python. Since scylla operates with months, days and nanosecond, there's no way we can represent it in python, becuase months are variable length.
+
+
 ## Named parameters
 
 Also, you can provide named parameters to querties, by using name
 placeholders instead of `?`.
 
 For example:
```

### Comparing `scyllapy-1.3.0/python/scyllapy/_internal/__init__.pyi` & `scyllapy-1.3.1/python/scyllapy/_internal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/scyllapy/_internal/exceptions.pyi` & `scyllapy-1.3.1/python/scyllapy/_internal/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/scyllapy/_internal/extra_types.pyi` & `scyllapy-1.3.1/python/scyllapy/_internal/extra_types.pyi`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/scyllapy/_internal/load_balancing.pyi` & `scyllapy-1.3.1/python/scyllapy/_internal/load_balancing.pyi`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/scyllapy/_internal/query_builder.pyi` & `scyllapy-1.3.1/python/scyllapy/_internal/query_builder.pyi`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/scyllapy/extra_types.py` & `scyllapy-1.3.1/python/scyllapy/extra_types.py`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/tests/conftest.py` & `scyllapy-1.3.1/python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/tests/query_builders/test_delete.py` & `scyllapy-1.3.1/python/tests/query_builders/test_delete.py`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/tests/query_builders/test_inserts.py` & `scyllapy-1.3.1/python/tests/query_builders/test_inserts.py`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/tests/query_builders/test_select.py` & `scyllapy-1.3.1/python/tests/query_builders/test_select.py`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/tests/query_builders/test_update.py` & `scyllapy-1.3.1/python/tests/query_builders/test_update.py`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/tests/test_batches.py` & `scyllapy-1.3.1/python/tests/test_batches.py`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/tests/test_bindings.py` & `scyllapy-1.3.1/python/tests/test_bindings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import datetime
 import ipaddress
 import random
 import uuid
+from decimal import Decimal
 from typing import Any, Callable
 
 import pytest
+from dateutil.relativedelta import relativedelta
 from tests.utils import random_string
 
 from scyllapy import Scylla
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
@@ -26,32 +28,35 @@
         ("TIMEUUID", uuid.uuid1()),
         ("UUID", uuid.uuid1()),
         ("UUID", uuid.uuid3(uuid.uuid4(), "name")),
         ("UUID", uuid.uuid4()),
         ("UUID", uuid.uuid5(uuid.uuid4(), "name")),
         ("INET", ipaddress.ip_address("192.168.1.1")),
         ("INET", ipaddress.ip_address("2001:db8::8a2e:370:7334")),
+        ("DECIMAL", Decimal("1.1")),
+        ("DECIMAL", Decimal("1.112e10")),
+        ("DURATION", relativedelta(months=1, days=2, microseconds=10)),
+        ("VARINT", 1000),
     ],
 )
 async def test_bindings(
     scylla: Scylla,
     type_name: str,
     test_val: Any,
 ) -> None:
     table_name = random_string(4)
     await scylla.execute(
-        f"CREATE TABLE {table_name} (id {type_name}, PRIMARY KEY (id))",
+        f"CREATE TABLE {table_name} (id INT, value {type_name}, PRIMARY KEY (id))",
     )
-    insert_query = f"INSERT INTO {table_name}(id) VALUES (?)"
-    await scylla.execute(insert_query, [test_val])
+    insert_query = f"INSERT INTO {table_name}(id, value) VALUES (?, ?)"
+    await scylla.execute(insert_query, [1, test_val])
 
     result = await scylla.execute(f"SELECT * FROM {table_name}")
     rows = result.all()
-    assert len(rows) == 1
-    assert rows[0] == {"id": test_val}
+    assert rows == [{"id": 1, "value": test_val}]
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
     ("type_name", "test_val", "cast_func"),
     [
         ("SET<TEXT>", ["one", "two"], set),
```

### Comparing `scyllapy-1.3.0/python/tests/test_extra_types.py` & `scyllapy-1.3.1/python/tests/test_extra_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import asdict, dataclass
-from typing import Any
+from typing import Any, Callable
 
 import pytest
 from tests.utils import random_string
 
 from scyllapy import Scylla, extra_types
 from scyllapy.exceptions import ScyllaPyDBError
 
@@ -143,7 +143,32 @@
 )
 @pytest.mark.anyio
 async def test_autocast_positional(scylla: Scylla, typ: str, val: Any) -> None:
     table_name = random_string(4)
     await scylla.execute(f"CREATE TABLE {table_name}(id INT PRIMARY KEY, val {typ})")
     prepared = await scylla.prepare(f"INSERT INTO {table_name}(id, val) VALUES (?, ?)")
     await scylla.execute(prepared, [1, val])
+
+
+@pytest.mark.parametrize(
+    ["cast_func", "val"],
+    [
+        (extra_types.BigInt, 1000000),
+        (extra_types.SmallInt, 10),
+        (extra_types.TinyInt, 1),
+        (int, 1),
+    ],
+)
+@pytest.mark.anyio
+async def test_varint(
+    scylla: Scylla,
+    cast_func: Callable[[Any], Any],
+    val: Any,
+) -> None:
+    table_name = random_string(4)
+    await scylla.execute(f"CREATE TABLE {table_name}(id INT PRIMARY KEY, val VARINT)")
+    await scylla.execute(
+        f"INSERT INTO {table_name}(id, val) VALUES (?, ?)",
+        (1, cast_func(val)),
+    )
+    res = await scylla.execute(f"SELECT * FROM {table_name}")
+    assert res.all() == [{"id": 1, "val": val}]
```

### Comparing `scyllapy-1.3.0/python/tests/test_pagination.py` & `scyllapy-1.3.1/python/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/tests/test_parsing.py` & `scyllapy-1.3.1/python/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/tests/test_prepared.py` & `scyllapy-1.3.1/python/tests/test_prepared.py`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/tests/test_profiles.py` & `scyllapy-1.3.1/python/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/python/tests/test_queries.py` & `scyllapy-1.3.1/python/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/src/batches.rs` & `scyllapy-1.3.1/src/batches.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 use pyo3::{pyclass, pymethods, types::PyDict, PyAny};
-use scylla::batch::{Batch, BatchStatement, BatchType};
+use scylla::{
+    batch::{Batch, BatchStatement, BatchType},
+    frame::value::LegacySerializedValues,
+};
 
 use crate::{
     exceptions::rust_err::ScyllaPyResult, inputs::BatchQueryInput, queries::ScyllaPyRequestParams,
     utils::parse_python_query_params,
 };
-use scylla::frame::value::SerializedValues;
 
 #[pyclass(name = "BatchType")]
 #[derive(Clone, Copy, Debug, PartialEq, Eq)]
 pub enum ScyllaPyBatchType {
     COUNTER,
     LOGGED,
     UNLOGGED,
@@ -23,26 +25,26 @@
 }
 
 #[pyclass(name = "InlineBatch")]
 #[derive(Clone)]
 pub struct ScyllaPyInlineBatch {
     inner: Batch,
     request_params: ScyllaPyRequestParams,
-    values: Vec<SerializedValues>,
+    values: Vec<LegacySerializedValues>,
 }
 
 impl From<ScyllaPyBatch> for Batch {
     fn from(value: ScyllaPyBatch) -> Self {
         let mut inner = value.inner;
         value.request_params.apply_to_batch(&mut inner);
         inner
     }
 }
 
-impl From<ScyllaPyInlineBatch> for (Batch, Vec<SerializedValues>) {
+impl From<ScyllaPyInlineBatch> for (Batch, Vec<LegacySerializedValues>) {
     fn from(mut value: ScyllaPyInlineBatch) -> Self {
         value.request_params.apply_to_batch(&mut value.inner);
         (value.inner, value.values)
     }
 }
 
 #[pymethods]
@@ -70,15 +72,15 @@
     }
 }
 
 impl ScyllaPyInlineBatch {
     pub fn add_query_inner(
         &mut self,
         query: impl Into<BatchStatement>,
-        values: impl Into<SerializedValues>,
+        values: impl Into<LegacySerializedValues>,
     ) {
         self.inner.append_statement(query);
         self.values.push(values.into());
     }
 }
 
 #[pymethods]
@@ -119,15 +121,15 @@
         values: Option<&PyAny>,
     ) -> ScyllaPyResult<()> {
         self.inner.append_statement(query);
         if let Some(passed_params) = values {
             self.values
                 .push(parse_python_query_params(Some(passed_params), false, None)?);
         } else {
-            self.values.push(SerializedValues::new());
+            self.values.push(LegacySerializedValues::new());
         }
         Ok(())
     }
 }
 
 impl From<ScyllaPyBatchType> for BatchType {
     fn from(value: ScyllaPyBatchType) -> Self {
```

### Comparing `scyllapy-1.3.0/src/consistencies.rs` & `scyllapy-1.3.1/src/consistencies.rs`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/src/exceptions/py_err.rs` & `scyllapy-1.3.1/src/exceptions/py_err.rs`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/src/exceptions/rust_err.rs` & `scyllapy-1.3.1/src/exceptions/rust_err.rs`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     #[error("Session error: {0}.")]
     SessionError(String),
     #[error("Binding error. Cause: {0}.")]
     BindingError(String),
 
     // Derived exception.
     #[error("{0}")]
-    QueryError(#[from] scylla_cql::errors::QueryError),
+    QueryError(#[from] scylla::transport::errors::QueryError),
     #[error("{0}")]
-    DBError(#[from] scylla_cql::errors::DbError),
+    DBError(#[from] scylla::transport::errors::DbError),
     #[error("Python exception: {0}.")]
     PyError(#[from] pyo3::PyErr),
     #[error("OpenSSL error: {0}.")]
     SSLError(#[from] openssl::error::ErrorStack),
     #[error("Cannot construct new session: {0}.")]
-    ScyllaSessionError(#[from] scylla_cql::errors::NewSessionError),
+    ScyllaSessionError(#[from] scylla::transport::errors::NewSessionError),
 
     // Binding errors
     #[error("Binding error. Cannot build values for query: {0},")]
     ScyllaValueError(#[from] scylla::frame::value::SerializeValuesError),
     #[error("Binding error. Cannot parse time, because of: {0}.")]
     DateParseError(#[from] chrono::ParseError),
     #[error("Binding error. Cannot parse ip address, because of: {0}.")]
```

### Comparing `scyllapy-1.3.0/src/execution_profiles.rs` & `scyllapy-1.3.1/src/execution_profiles.rs`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/src/extra_types.rs` & `scyllapy-1.3.1/src/extra_types.rs`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/src/inputs.rs` & `scyllapy-1.3.1/src/inputs.rs`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/src/lib.rs` & `scyllapy-1.3.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/src/load_balancing.rs` & `scyllapy-1.3.1/src/load_balancing.rs`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/src/queries.rs` & `scyllapy-1.3.1/src/queries.rs`

 * *Files 2% similar despite different names*

```diff
@@ -62,39 +62,39 @@
     /// incorrect type passed.
     pub fn from_dict(params: Option<&PyDict>) -> ScyllaPyResult<Self> {
         let Some(params) = params else {
             return Ok(Self::default());
         };
         Ok(Self {
             consistency: params
-                .get_item("consistency")
+                .get_item("consistency")?
                 .map(pyo3::FromPyObject::extract)
                 .transpose()?,
             serial_consistency: params
-                .get_item("serial_consistency")
+                .get_item("serial_consistency")?
                 .map(pyo3::FromPyObject::extract)
                 .transpose()?,
             request_timeout: params
-                .get_item("request_timeout")
+                .get_item("request_timeout")?
                 .map(pyo3::FromPyObject::extract)
                 .transpose()?,
             timestamp: params
-                .get_item("timestamp")
+                .get_item("timestamp")?
                 .map(pyo3::FromPyObject::extract)
                 .transpose()?,
             is_idempotent: params
-                .get_item("is_idempotent")
+                .get_item("is_idempotent")?
                 .map(pyo3::FromPyObject::extract)
                 .transpose()?,
             tracing: params
-                .get_item("tracing")
+                .get_item("tracing")?
                 .map(pyo3::FromPyObject::extract)
                 .transpose()?,
             profile: params
-                .get_item("profile")
+                .get_item("profile")?
                 .map(pyo3::FromPyObject::extract)
                 .transpose()?,
         })
     }
 }
 
 #[pyclass(name = "Query")]
```

### Comparing `scyllapy-1.3.0/src/query_builder/delete.rs` & `scyllapy-1.3.1/src/query_builder/delete.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 use pyo3::{pyclass, pymethods, types::PyDict, PyAny, PyRefMut, Python};
-use scylla::query::Query;
+use scylla::{frame::value::LegacySerializedValues, query::Query};
 
 use super::utils::{pretty_build, IfCluase, Timeout};
 use crate::{
     batches::ScyllaPyInlineBatch,
     exceptions::rust_err::{ScyllaPyError, ScyllaPyResult},
     queries::ScyllaPyRequestParams,
     scylla_cls::Scylla,
     utils::{py_to_value, ScyllaPyCQLDTO},
 };
-use scylla::frame::value::SerializedValues;
 
 #[pyclass]
 #[derive(Clone, Debug, Default)]
 pub struct Delete {
     table_: String,
     columns: Option<Vec<String>>,
     timeout_: Option<Timeout>,
@@ -31,15 +30,15 @@
                 "At least one where clause should be specified.",
             ));
         }
         let columns = self
             .columns
             .as_ref()
             .map_or(String::new(), |cols| cols.join(", "));
-        let params = vec![
+        let params = [
             self.timestamp_
                 .map(|timestamp| format!("TIMESTAMP {timestamp}")),
             self.timeout_.as_ref().map(|timeout| match timeout {
                 Timeout::Int(int) => format!("TIMEOUT {int}"),
                 Timeout::Str(string) => format!("TIMEOUT {string}"),
             }),
         ];
@@ -204,28 +203,28 @@
         scylla.native_execute(py, Some(query), None, values, false)
     }
 
     /// Add to batch
     ///
     /// Adds current query to batch.
     ///
-    /// # Error
+    /// # Errors
     ///
     /// May result into error if query cannot be build.
     /// Or values cannot be passed to batch.
     pub fn add_to_batch(&self, batch: &mut ScyllaPyInlineBatch) -> ScyllaPyResult<()> {
         let mut query = Query::new(self.build_query()?);
         self.request_params_.apply_to_query(&mut query);
 
         let values = if let Some(if_clause) = &self.if_clause_ {
             if_clause.extend_values(self.values_.clone())
         } else {
             self.values_.clone()
         };
-        let mut serialized = SerializedValues::new();
+        let mut serialized = LegacySerializedValues::new();
         for val in values {
             serialized.add_value(&val)?;
         }
         batch.add_query_inner(query, serialized);
         Ok(())
     }
```

### Comparing `scyllapy-1.3.0/src/query_builder/insert.rs` & `scyllapy-1.3.1/src/query_builder/insert.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 use pyo3::{pyclass, pymethods, types::PyDict, PyAny, PyRefMut, Python};
-use scylla::query::Query;
+use scylla::{frame::value::LegacySerializedValues, query::Query};
 
 use crate::{
     batches::ScyllaPyInlineBatch,
     exceptions::rust_err::{ScyllaPyError, ScyllaPyResult},
     queries::ScyllaPyRequestParams,
     scylla_cls::Scylla,
     utils::{py_to_value, ScyllaPyCQLDTO},
 };
-use scylla::frame::value::SerializedValues;
 
 use super::utils::{pretty_build, Timeout};
 
 #[pyclass]
 #[derive(Clone, Debug, Default)]
 pub struct Insert {
     table_: String,
@@ -47,15 +46,15 @@
             .join(",");
         let names_values = format!("({names}) VALUES ({values})");
         let ifnexist = if self.if_not_exists_ {
             "IF NOT EXISTS"
         } else {
             ""
         };
-        let params = vec![
+        let params = [
             self.timestamp_
                 .map(|timestamp| format!("TIMESTAMP {timestamp}")),
             self.ttl_.map(|ttl| format!("TTL {ttl}")),
             self.timeout_.as_ref().map(|timeout| match timeout {
                 Timeout::Int(int) => format!("TIMEOUT {int}"),
                 Timeout::Str(string) => format!("TIMEOUT {string}"),
             }),
@@ -168,23 +167,23 @@
         scylla.native_execute(py, Some(query), None, self.values_.clone(), false)
     }
 
     /// Add to batch
     ///
     /// Adds current query to batch.
     ///
-    /// # Error
+    /// # Errors
     ///
     /// May result into error if query cannot be build.
     /// Or values cannot be passed to batch.
     pub fn add_to_batch(&self, batch: &mut ScyllaPyInlineBatch) -> ScyllaPyResult<()> {
         let mut query = Query::new(self.build_query()?);
         self.request_params_.apply_to_query(&mut query);
 
-        let mut serialized = SerializedValues::new();
+        let mut serialized = LegacySerializedValues::new();
         for val in self.values_.clone() {
             serialized.add_value(&val)?;
         }
         batch.add_query_inner(query, serialized);
         Ok(())
     }
```

### Comparing `scyllapy-1.3.0/src/query_builder/mod.rs` & `scyllapy-1.3.1/src/query_builder/mod.rs`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/src/query_builder/select.rs` & `scyllapy-1.3.1/src/query_builder/select.rs`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     exceptions::rust_err::ScyllaPyResult,
     queries::ScyllaPyRequestParams,
     scylla_cls::Scylla,
     utils::{py_to_value, ScyllaPyCQLDTO},
 };
 
 use super::utils::{pretty_build, Timeout};
-use scylla::frame::value::SerializedValues;
+use scylla::frame::value::LegacySerializedValues;
 
 #[pyclass]
 #[derive(Clone, Debug, Default)]
 pub struct Select {
     table_: String,
     distinct_: bool,
     allow_filtering_: bool,
@@ -251,22 +251,22 @@
         scylla.native_execute(py, Some(query), None, self.values_.clone(), paged)
     }
 
     /// Add to batch
     ///
     /// Adds current query to batch.
     ///
-    /// # Error
+    /// # Errors
     ///
     /// Returns error if values cannot be passed to batch.
     pub fn add_to_batch(&self, batch: &mut ScyllaPyInlineBatch) -> ScyllaPyResult<()> {
         let mut query = Query::new(self.build_query());
         self.request_params_.apply_to_query(&mut query);
 
-        let mut serialized = SerializedValues::new();
+        let mut serialized = LegacySerializedValues::new();
         for val in self.values_.clone() {
             serialized.add_value(&val)?;
         }
         batch.add_query_inner(query, serialized);
         Ok(())
     }
```

### Comparing `scyllapy-1.3.0/src/query_builder/update.rs` & `scyllapy-1.3.1/src/query_builder/update.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 use pyo3::{pyclass, pymethods, types::PyDict, PyAny, PyRefMut, Python};
-use scylla::query::Query;
+use scylla::{frame::value::LegacySerializedValues, query::Query};
 
 use crate::{
     batches::ScyllaPyInlineBatch,
     exceptions::rust_err::{ScyllaPyError, ScyllaPyResult},
     queries::ScyllaPyRequestParams,
     scylla_cls::Scylla,
     utils::{py_to_value, ScyllaPyCQLDTO},
 };
 
 use super::utils::{pretty_build, IfCluase, Timeout};
-use scylla::frame::value::SerializedValues;
 #[derive(Clone, Debug)]
 enum UpdateAssignment {
     Simple(String),
     Inc(String, String),
     Dec(String, String),
 }
 
@@ -54,15 +53,15 @@
             ));
         }
         if self.where_clauses_.is_empty() {
             return Err(ScyllaPyError::QueryBuilderError(
                 "Update should contain at least one where clause",
             ));
         }
-        let params = vec![
+        let params = [
             self.timestamp_
                 .map(|timestamp| format!("TIMESTAMP {timestamp}")),
             self.ttl_.map(|ttl| format!("TTL {ttl}")),
             self.timeout_.as_ref().map(|timeout| match timeout {
                 Timeout::Int(int) => format!("TIMEOUT {int}"),
                 Timeout::Str(string) => format!("TIMEOUT {string}"),
             }),
@@ -132,15 +131,15 @@
         slf.assignments_.push(UpdateAssignment::Simple(name));
         slf.values_.push(py_to_value(value, None)?);
         Ok(slf)
     }
 
     /// Increment column value.
     ///
-    /// # Error
+    /// # Errors
     ///
     /// If cannot convert python type
     /// to appropriate rust type.
     pub fn inc<'a>(
         mut slf: PyRefMut<'a, Self>,
         name: String,
         value: &'a PyAny,
@@ -288,15 +287,15 @@
         scylla.native_execute(py, Some(query), None, values, false)
     }
 
     /// Add to batch
     ///
     /// Adds current query to batch.
     ///
-    /// # Error
+    /// # Errors
     ///
     /// May result into error if query cannot be build.
     /// Or values cannot be passed to batch.
     pub fn add_to_batch(&self, batch: &mut ScyllaPyInlineBatch) -> ScyllaPyResult<()> {
         let mut query = Query::new(self.build_query()?);
         self.request_params_.apply_to_query(&mut query);
 
@@ -304,15 +303,15 @@
         values.extend(self.where_values_.clone());
         let values = if let Some(if_clause) = &self.if_clause_ {
             if_clause.extend_values(values)
         } else {
             values
         };
 
-        let mut serialized = SerializedValues::new();
+        let mut serialized = LegacySerializedValues::new();
         for val in values {
             serialized.add_value(&val)?;
         }
         batch.add_query_inner(query, serialized);
         Ok(())
     }
```

### Comparing `scyllapy-1.3.0/src/query_builder/utils.rs` & `scyllapy-1.3.1/src/query_builder/utils.rs`

 * *Files identical despite different names*

### Comparing `scyllapy-1.3.0/src/query_results.rs` & `scyllapy-1.3.1/src/query_results.rs`

 * *Files 6% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     }
 
     /// Function to get first column of every row.
     ///
     /// This function grabs rows from all function and
     /// tries to get the first column of any row.
     ///
-    /// # Erros
+    /// # Errors
     ///
     /// May result in an error if:
     /// * Query doesn't have a returns;
     /// * Results don't have any columns.
     pub fn scalars(&self, py: Python<'_>) -> ScyllaPyResult<Option<Py<PyAny>>> {
         let Some(rows) = self.get_rows(py, None)? else {
             return Err(ScyllaPyError::NoReturnsError);
@@ -154,15 +154,15 @@
     }
 
     /// Function to get first column of first row.
     ///
     /// This function grabs first row and
     /// tries to get the first column of a result.
     ///
-    /// # Erros
+    /// # Errors
     ///
     /// May result in an error if:
     /// * Query doesn't have a returns;
     /// * Results don't have any columns.
     pub fn scalar(&self, py: Python<'_>) -> ScyllaPyResult<Option<Py<PyAny>>> {
         let Some(rows) = self.get_rows(py, Some(1))? else {
             return Err(ScyllaPyError::NoReturnsError);
@@ -234,15 +234,23 @@
     #[must_use]
     pub fn __aiter__(slf: PyRef<'_, Self>) -> PyRef<'_, Self> {
         slf
     }
 
     /// Actual async iteration.
     ///
-    /// Here we define how to
+    /// Here we define how to iterate over rows.
+    ///
+    /// # Errors
+    ///
+    /// May return an error if:
+    /// * No more rows to iterate;
+    /// * No columns in a row.
+    /// * Cannot convert column to python object.
+    /// * Cannot acquire GIL.
     pub fn __anext__(&self, py: Python<'_>) -> ScyllaPyResult<Option<PyObject>> {
         let streamer = self.inner.clone();
         let map_function = self.mapper.clone();
         let scalars = self.scalars;
         // Here we create our future that actually yields row.
         let future = scyllapy_future(py, async move {
             let mut row_iterator = streamer.lock().await;
```

### Comparing `scyllapy-1.3.0/src/scylla_cls.rs` & `scyllapy-1.3.1/src/scylla_cls.rs`

 * *Files 5% similar despite different names*

```diff
@@ -63,33 +63,37 @@
             let session = session_guard.as_ref().ok_or(ScyllaPyError::SessionError(
                 "Session is not initialized.".into(),
             ))?;
             // let res = session.query(query, values).await?;
             if paged {
                 match (query, prepared) {
                     (Some(query), None) => Ok(ScyllaPyQueryReturns::IterableQueryResult(
-                        ScyllaPyIterableQueryResult::new(session.query_iter(query, values).await?),
+                        ScyllaPyIterableQueryResult::new(
+                            session.query_iter(query, values.serialized()?).await?,
+                        ),
                     )),
                     (None, Some(prepared)) => Ok(ScyllaPyQueryReturns::IterableQueryResult(
                         ScyllaPyIterableQueryResult::new(
-                            session.execute_iter(prepared, values).await?,
+                            session.execute_iter(prepared, values.serialized()?).await?,
                         ),
                     )),
                     _ => Err(ScyllaPyError::SessionError(
                         "You should pass either query or prepared query.".into(),
                     )),
                 }
             } else {
                 match (query, prepared) {
                     (Some(query), None) => Ok(ScyllaPyQueryReturns::QueryResult(
-                        ScyllaPyQueryResult::new(session.query(query, values).await?),
-                    )),
-                    (None, Some(prepared)) => Ok(ScyllaPyQueryReturns::QueryResult(
-                        ScyllaPyQueryResult::new(session.execute(&prepared, values).await?),
+                        ScyllaPyQueryResult::new(session.query(query, values.serialized()?).await?),
                     )),
+                    (None, Some(prepared)) => {
+                        Ok(ScyllaPyQueryReturns::QueryResult(ScyllaPyQueryResult::new(
+                            session.execute(&prepared, values.serialized()?).await?,
+                        )))
+                    }
                     _ => Err(ScyllaPyError::SessionError(
                         "You should pass either query or prepared query.".into(),
                     )),
                 }
             }
         })
         .map_err(Into::into)
@@ -242,15 +246,15 @@
                 session_builder = session_builder.use_keyspace(keyspace, true);
             }
             if let Some(connection_timeout) = conn_timeout {
                 session_builder =
                     session_builder.connection_timeout(Duration::from_secs(connection_timeout));
             }
             let mut session_guard = scylla_session.write().await;
-            *session_guard = Some(session_builder.build().await?);
+            *session_guard = Some(Box::pin(session_builder.build()).await?);
             Ok(())
         })
     }
 
     /// Close current session, free resources.
     ///
     /// # Errors
@@ -305,14 +309,18 @@
         };
         self.native_execute(py, query, prepared, query_params, paged)
     }
 
     /// Execute a batch statement.
     ///
     /// This function takes a batch and list of lists of params.
+    ///
+    /// # Errors
+    ///
+    /// Can result in an error in any case, when something goes wrong.
     #[pyo3(signature = (batch, params = None))]
     pub fn batch<'a>(
         &'a self,
         py: Python<'a>,
         batch: BatchInput,
         params: Option<Vec<&'a PyAny>>,
     ) -> ScyllaPyResult<&'a PyAny> {
@@ -353,14 +361,18 @@
     /// Prepare a query.
     ///
     /// This function takes a query to prepare
     /// and sends it to server.
     ///
     /// After preparation it returns a prepared
     /// query, that you can use later.
+    ///
+    /// # Errors
+    ///
+    /// May return an error, if session is not initialized.
     pub fn prepare<'a>(
         &'a self,
         python: Python<'a>,
         query: PrepareInput,
     ) -> ScyllaPyResult<&'a PyAny> {
         let session_arc = self.scylla_session.clone();
         scyllapy_future(python, async move {
```

### Comparing `scyllapy-1.3.0/src/utils.rs` & `scyllapy-1.3.1/src/utils.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 use std::{collections::HashMap, future::Future, hash::BuildHasherDefault, str::FromStr};
 
-use chrono::Duration;
 use pyo3::{
     types::{PyBool, PyBytes, PyDict, PyFloat, PyInt, PyList, PyModule, PySet, PyString, PyTuple},
     IntoPy, Py, PyAny, PyObject, PyResult, Python, ToPyObject,
 };
 use scylla::{
     frame::{
-        response::result::{ColumnType, CqlValue},
-        value::{SerializedValues, Value},
+        response::result::{ColumnSpec, ColumnType, CqlValue},
+        value::{CqlDuration, LegacySerializedValues, Value},
     },
     BufMut,
 };
-use scylla_cql::frame::response::result::ColumnSpec;
 
 use std::net::IpAddr;
 
 use crate::{
     exceptions::rust_err::{ScyllaPyError, ScyllaPyResult},
     extra_types::{BigInt, Counter, Double, ScyllaPyUnset, SmallInt, TinyInt},
 };
 
+const DATE_FORMAT: &[::time::format_description::FormatItem<'static>] =
+    ::time::macros::format_description!(version = 2, "[year]-[month]-[day]");
+
 /// Add submodule.
 ///
 /// This function is required,
 /// because by default for native libs python
 /// adds module as an attribute and
 /// doesn't add it's submodules in list
 /// of all available modules.
@@ -87,19 +88,25 @@
     BigInt(i64),
     Int(i32),
     SmallInt(i16),
     TinyInt(i8),
     Counter(i64),
     Bool(bool),
     Double(eq_float::F64),
+    Decimal(bigdecimal_04::BigDecimal),
+    Duration {
+        months: i32,
+        days: i32,
+        nanoseconds: i64,
+    },
     Float(eq_float::F32),
     Bytes(Vec<u8>),
     Date(chrono::NaiveDate),
-    Time(chrono::Duration),
-    Timestamp(chrono::Duration),
+    Time(chrono::NaiveTime),
+    Timestamp(chrono::DateTime<chrono::Utc>),
     Uuid(uuid::Uuid),
     Inet(IpAddr),
     List(Vec<ScyllaPyCQLDTO>),
     Map(Vec<(ScyllaPyCQLDTO, ScyllaPyCQLDTO)>),
     // UDT holds serialized bytes according to the protocol.
     Udt(Vec<u8>),
 }
@@ -117,29 +124,40 @@
             ScyllaPyCQLDTO::Bytes(bytes) => bytes.serialize(buf),
             ScyllaPyCQLDTO::Uuid(uuid) => uuid.serialize(buf),
             ScyllaPyCQLDTO::Inet(inet) => inet.serialize(buf),
             ScyllaPyCQLDTO::List(list) => list.serialize(buf),
             ScyllaPyCQLDTO::Counter(counter) => counter.serialize(buf),
             ScyllaPyCQLDTO::TinyInt(tinyint) => tinyint.serialize(buf),
             ScyllaPyCQLDTO::Date(date) => date.serialize(buf),
-            ScyllaPyCQLDTO::Time(time) => scylla::frame::value::Time(*time).serialize(buf),
+            ScyllaPyCQLDTO::Time(time) => time.serialize(buf),
             ScyllaPyCQLDTO::Map(map) => map
                 .iter()
                 .cloned()
                 .collect::<HashMap<_, _, BuildHasherDefault<rustc_hash::FxHasher>>>()
                 .serialize(buf),
             ScyllaPyCQLDTO::Timestamp(timestamp) => {
-                scylla::frame::value::Timestamp(*timestamp).serialize(buf)
+                scylla::frame::value::CqlTimestamp::from(*timestamp).serialize(buf)
             }
-            ScyllaPyCQLDTO::Null => Option::<i16>::None.serialize(buf),
+            ScyllaPyCQLDTO::Null => Option::<bool>::None.serialize(buf),
             ScyllaPyCQLDTO::Udt(udt) => {
                 buf.extend(udt);
                 Ok(())
             }
+            ScyllaPyCQLDTO::Decimal(decimal) => decimal.serialize(buf),
             ScyllaPyCQLDTO::Unset => scylla::frame::value::Unset.serialize(buf),
+            ScyllaPyCQLDTO::Duration {
+                months,
+                days,
+                nanoseconds,
+            } => CqlDuration {
+                months: *months,
+                days: *days,
+                nanoseconds: *nanoseconds,
+            }
+            .serialize(buf),
         }
     }
 }
 
 /// Convert Python type to CQL parameter value.
 ///
 /// It converts python object to another type,
@@ -239,29 +257,44 @@
             item.str()?.extract::<&str>()?,
         )?))
     } else if item.get_type().name()? == "date" {
         Ok(ScyllaPyCQLDTO::Date(chrono::NaiveDate::from_str(
             item.call_method0("isoformat")?.extract::<&str>()?,
         )?))
     } else if item.get_type().name()? == "time" {
-        Ok(ScyllaPyCQLDTO::Time(
-            chrono::NaiveTime::from_str(item.call_method0("isoformat")?.extract::<&str>()?)?
-                .signed_duration_since(
-                    chrono::NaiveTime::from_num_seconds_from_midnight_opt(0, 0).ok_or(
-                        ScyllaPyError::BindingError(format!(
-                            "Cannot calculate offset from midnight for value {item}"
-                        )),
-                    )?,
-                ),
+        Ok(ScyllaPyCQLDTO::Time(chrono::NaiveTime::from_str(
+            item.call_method0("isoformat")?.extract::<&str>()?,
+        )?))
+    } else if item.get_type().name()? == "Decimal" {
+        Ok(ScyllaPyCQLDTO::Decimal(
+            bigdecimal_04::BigDecimal::from_str(item.str()?.to_str()?).map_err(|err| {
+                ScyllaPyError::BindingError(format!("Cannot parse decimal {err}"))
+            })?,
         ))
     } else if item.get_type().name()? == "datetime" {
         let milliseconds = item.call_method0("timestamp")?.extract::<f64>()? * 1000f64;
         #[allow(clippy::cast_possible_truncation)]
-        let timestamp = Duration::milliseconds(milliseconds.trunc() as i64);
+        let seconds = milliseconds as i64 / 1_000;
+        #[allow(clippy::cast_possible_truncation)]
+        #[allow(clippy::cast_sign_loss)]
+        let nsecs = (milliseconds as i64 % 1_000) as u32 * 1_000_000;
+        let timestamp = chrono::DateTime::<chrono::Utc>::from_timestamp(seconds, nsecs).ok_or(
+            ScyllaPyError::BindingError("Cannot convert datetime to timestamp.".into()),
+        )?;
         Ok(ScyllaPyCQLDTO::Timestamp(timestamp))
+    } else if item.get_type().name()? == "relativedelta" {
+        let months = item.getattr("months")?.extract::<i32>()?;
+        let days = item.getattr("days")?.extract::<i32>()?;
+        let nanoseconds = item.getattr("microseconds")?.extract::<i64>()? * 1_000
+            + item.getattr("seconds")?.extract::<i64>()? * 1_000_000;
+        Ok(ScyllaPyCQLDTO::Duration {
+            months,
+            days,
+            nanoseconds,
+        })
     } else if item.is_instance_of::<PyList>()
         || item.is_instance_of::<PyTuple>()
         || item.is_instance_of::<PySet>()
     {
         let mut items = Vec::new();
         for inner in item.iter()? {
             items.push(py_to_value(inner?, column_type)?);
@@ -414,69 +447,95 @@
         ColumnType::Timeuuid => {
             let uuid_str = unwrapped_value
                 .as_timeuuid()
                 .ok_or(ScyllaPyError::ValueDowncastError(
                     col_name.into(),
                     "Timeuuid",
                 ))?
+                .as_ref()
                 .as_simple()
                 .to_string();
             Ok(py.import("uuid")?.getattr("UUID")?.call1((uuid_str,))?)
         }
         ColumnType::Duration => {
             // We loose some perscision on converting it to
             // python datetime, because in scylla,
             // durations is stored in nanoseconds.
             // But that's ok, because we assume that
             // all values were inserted using
             // same driver. Will fix it on demand.
             let duration =
                 unwrapped_value
-                    .as_duration()
+                    .as_cql_duration()
                     .ok_or(ScyllaPyError::ValueDowncastError(
                         col_name.into(),
                         "Duration",
                     ))?;
             let kwargs = PyDict::new(py);
-            kwargs.set_item("microseconds", duration.num_microseconds())?;
+            kwargs.set_item("months", duration.months)?;
+            kwargs.set_item("days", duration.days)?;
+            kwargs.set_item("microseconds", duration.nanoseconds / 1_000)?;
             Ok(py
-                .import("datetime")?
-                .getattr("timedelta")?
+                .import("dateutil")?
+                .getattr("relativedelta")?
+                .getattr("relativedelta")?
                 .call((), Some(kwargs))?)
         }
         ColumnType::Timestamp => {
             // Timestamp - num of milliseconds since unix epoch.
             let timestamp =
                 unwrapped_value
-                    .as_duration()
+                    .as_cql_timestamp()
                     .ok_or(ScyllaPyError::ValueDowncastError(
                         col_name.into(),
                         "Timestamp",
                     ))?;
+            let milliseconds = timestamp.0;
+            if milliseconds < 0 {
+                return Err(ScyllaPyError::ValueDowncastError(
+                    col_name.into(),
+                    "Timestamp cannot be less than 0",
+                ));
+            }
+            let seconds =
+                milliseconds
+                    .checked_div(1_000)
+                    .ok_or(ScyllaPyError::ValueDowncastError(
+                        col_name.into(),
+                        "Cannot get seconds out of milliseconds.",
+                    ))?;
+            #[allow(clippy::cast_possible_truncation)]
+            #[allow(clippy::cast_sign_loss)]
+            let nsecs = (milliseconds % 1_000).checked_mul(1_000_000).ok_or(
+                ScyllaPyError::ValueDowncastError(col_name.into(), "Cannot construct nanoseconds"),
+            )? as u32;
+
+            let timestamp = chrono::DateTime::<chrono::Utc>::from_timestamp(seconds, nsecs).ok_or(
+                ScyllaPyError::ValueDowncastError(
+                    col_name.into(),
+                    "Cannot construct datetime based on timestamp",
+                ),
+            )?;
             #[allow(clippy::cast_precision_loss)]
-            let seconds = timestamp.num_seconds() as f64;
-            #[allow(clippy::cast_precision_loss)]
-            let micros = (timestamp - Duration::seconds(timestamp.num_seconds())).num_milliseconds()
-                as f64
-                / 1_000f64; // Converting microseconds to seconds to construct timestamp
-            Ok(py
-                .import("datetime")?
-                .getattr("datetime")?
-                .call_method1("fromtimestamp", (seconds + micros,))?)
+            Ok(py.import("datetime")?.getattr("datetime")?.call_method1(
+                "fromtimestamp",
+                (timestamp.timestamp_millis() as f64 / 1000f64,),
+            )?)
         }
         ColumnType::Inet => Ok(unwrapped_value
             .as_inet()
             .ok_or(ScyllaPyError::ValueDowncastError(col_name.into(), "Inet"))?
             .to_object(py)
             .into_ref(py)),
         ColumnType::Date => {
             let formatted_date = unwrapped_value
                 .as_date()
                 .ok_or(ScyllaPyError::ValueDowncastError(col_name.into(), "Date"))?
-                .format("%Y-%m-%d")
+                .format(DATE_FORMAT)
+                .map_err(|_| ScyllaPyError::ValueDowncastError(col_name.into(), "Date"))?
                 .to_string();
             Ok(py
                 .import("datetime")?
                 .getattr("date")?
                 .call_method1("fromisoformat", (formatted_date,))?)
         }
         ColumnType::Tuple(types) => {
@@ -496,27 +555,26 @@
                 col_name.into(),
                 "Counter",
             ))?
             .0
             .to_object(py)
             .into_ref(py)),
         ColumnType::Time => {
-            let duration = unwrapped_value
-                .as_duration()
+            let time = unwrapped_value
+                .as_time()
                 .ok_or(ScyllaPyError::ValueDowncastError(col_name.into(), "Time"))?;
-            let time = chrono::NaiveTime::from_num_seconds_from_midnight_opt(0, 0).ok_or(
-                ScyllaPyError::ValueDowncastError(
-                    col_name.into(),
-                    "Time, because it's value is too big",
-                ),
-            )? + duration;
+            let kwargs = PyDict::new(py);
+            kwargs.set_item("hour", time.hour())?;
+            kwargs.set_item("minute", time.minute())?;
+            kwargs.set_item("second", time.second())?;
+            kwargs.set_item("microsecond", time.microsecond())?;
             Ok(py
                 .import("datetime")?
                 .getattr("time")?
-                .call_method1("fromisoformat", (time.format("%H:%M:%S%.6f").to_string(),))?)
+                .call((), Some(kwargs))?)
         }
         ColumnType::UserDefinedType {
             type_name,
             keyspace,
             field_types,
         } => {
             let mut fields: HashMap<&str, &ColumnType, _> = HashMap::with_capacity_and_hasher(
@@ -547,38 +605,66 @@
 
             let res_map = PyDict::new(py);
             for (key, value) in map_values {
                 res_map.set_item(key, value)?;
             }
             Ok(res_map)
         }
-        ColumnType::Custom(_) | ColumnType::Varint | ColumnType::Decimal => Err(
-            ScyllaPyError::ValueDowncastError(col_name.into(), "Unknown"),
-        ),
+        ColumnType::Decimal => {
+            // Because the `as_decimal` method is not implemented for `CqlValue`,
+            // will make a PR.
+            let decimal: bigdecimal_04::BigDecimal = match unwrapped_value {
+                CqlValue::Decimal(inner) => inner.clone().into(),
+                _ => {
+                    return Err(ScyllaPyError::ValueDowncastError(
+                        col_name.into(),
+                        "Decimal",
+                    ))
+                }
+            };
+            Ok(py
+                .import("decimal")?
+                .getattr("Decimal")?
+                .call1((decimal.to_scientific_notation(),))?)
+        }
+        ColumnType::Varint => {
+            let bigint: bigdecimal_04::num_bigint::BigInt = match unwrapped_value {
+                CqlValue::Varint(inner) => inner.clone().into(),
+                _ => return Err(ScyllaPyError::ValueDowncastError(col_name.into(), "Varint")),
+            };
+            Ok(py
+                .import("builtins")?
+                .getattr("int")?
+                .call1((bigint.to_string(),))?)
+        }
+        ColumnType::Custom(_) => Err(ScyllaPyError::ValueDowncastError(
+            col_name.into(),
+            "Unknown",
+        )),
     }
 }
 
-/// Parse python type to `SerializedValues`.
+/// Parse python type to `LegacySerializedValues`.
 ///
 /// Serialized values are used for
 /// parameter binding. We parse python types
 /// into our own types that are capable
 /// of being bound to query and add parsed
-/// results to `SerializedValues`.
+/// results to `LegacySerializedValues`.
 ///
 /// # Errors
 ///
 /// May result in error if any of parameters cannot
 /// be parsed.
 pub fn parse_python_query_params(
     params: Option<&PyAny>,
     allow_dicts: bool,
     col_spec: Option<&[ColumnSpec]>,
-) -> ScyllaPyResult<SerializedValues> {
-    let mut values = SerializedValues::new();
+) -> ScyllaPyResult<LegacySerializedValues> {
+    let mut values = LegacySerializedValues::new();
 
     let Some(params) = params else {
         return Ok(values);
     };
 
     // If list was passed, we construct only unnamed parameters.
     // Otherwise it parses dict to named parameters.
```

### Comparing `scyllapy-1.3.0/Cargo.lock` & `scyllapy-1.3.1/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -30,125 +30,159 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "arc-swap"
-version = "1.6.0"
+version = "1.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
+checksum = "69f7f8c3906b62b754cd5326047894316021dcfe5a194c8ea52bdd94934a3457"
 
 [[package]]
 name = "async-trait"
-version = "0.1.74"
+version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a66537f1bb974b254c98ed142ff995236e81b9d0fe4db0575f46612cb15eb0f9"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "bigdecimal"
-version = "0.2.2"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1e50562e37200edf7c6c43e54a08e64a5553bfb59d9c297d5572512aa517256"
+checksum = "9324c8014cd04590682b34f1e9448d38f0674d0f7b2dc553331016ef0e4e9ebc"
 dependencies = [
- "num-bigint",
+ "autocfg",
+ "libm",
+ "num-bigint 0.4.4",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "327762f6e5a765692301e5bb513e0d9fef63be86bbc14528052b1cd3e6f03e07"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
-dependencies = [
- "libc",
-]
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.31"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f2c685bad3eb3d45a01354cedb7d5faa66194d1d58ba6e267a8de788f79db38"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
- "windows-targets",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.4"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
+
+[[package]]
+name = "darling"
+version = "0.20.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
+dependencies = [
+ "darling_core",
+ "darling_macro",
+]
+
+[[package]]
+name = "darling_core"
+version = "0.20.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
+dependencies = [
+ "fnv",
+ "ident_case",
+ "proc-macro2",
+ "quote",
+ "strsim",
+ "syn 2.0.60",
+]
+
+[[package]]
+name = "darling_macro"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
+dependencies = [
+ "darling_core",
+ "quote",
+ "syn 2.0.60",
+]
 
 [[package]]
 name = "dashmap"
 version = "5.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978747c1d849a7d2ee5e8adc0159961c48fb7e5db2f06af6723b80123bb53856"
 dependencies = [
@@ -156,32 +190,47 @@
  "hashbrown",
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
+name = "deranged"
+version = "0.3.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
+dependencies = [
+ "powerfmt",
+]
+
+[[package]]
 name = "either"
-version = "1.9.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "eq-float"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c02b5d1d1e6ba431b960d4bf971c8b0e2d2942b8cbc577d9bdf9c60fca5d41d"
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
+name = "fnv"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
+
+[[package]]
 name = "foreign-types"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f6f339eb8adc052cd2ca78910fda869aefa38d22d5cb648e6485e4d3fc06f3b1"
 dependencies = [
  "foreign-types-shared",
 ]
@@ -190,88 +239,88 @@
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
 name = "futures"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0290714b38af9b4a7b094b8a37086d1b4e61f2df9122c3cad2577669145335"
+checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff4dd66668b557604244583e3e1e1eada8c5c2e96a6d0d6653ede395b78bbacb"
+checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb1d22c66e66d9d72e1758f0bd7d4fd0bee04cad842ee34587d68c07e45d088c"
+checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f4fb8693db0cf099eadcca0efe2a5a22e4550f98ed16aba6c48700da29597bc"
+checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8bf34a163b5c4c52d0478a4d757da8fb65cabef42ba90515efee0f6f9fa45aaa"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53b153fd91e4b0147f4aced87be237c98248656bb01050b96bf3ee89220a8ddb"
+checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e36d3378ee38c2a36ad710c5d30c2911d752cb941c00c72dbabfb786a7970817"
+checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "efd193069b0ddadc69c46389b740bbccdd97203899b48d09c5f7969591d6bae2"
+checksum = "38d84fa142264698cdce1a9f9172cf383a0c82de1bddcf3092901442c4097004"
 
 [[package]]
 name = "futures-util"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a19526d624e703a3179b3d322efec918b6246ea0fa51d41124525f00f1cc8104"
+checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -279,61 +328,67 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.10"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.28.0"
+version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6fb8d784f27acf97159b40fc4db5ecd8aa23b9ad5ef69cdd136d3bc80665f0c0"
+checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "hashbrown"
-version = "0.14.2"
+version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f93e7192158dbcda357bdec5fb5788eebf8bbac027f3f33e719d29135ae84156"
+checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 
 [[package]]
 name = "heck"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d621efb26863f0e9924c6ac577e8275e5e6b77455db64ffa6c65c904e9e132c"
 dependencies = [
  "unicode-segmentation",
 ]
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "hermit-abi"
-version = "0.3.3"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d77f7ec81a6d05a3abb01ab6eb7590f6083d08449fe5a1c8b1e620283546ccb7"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "histogram"
 version = "0.6.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "12cb882ccb290b8646e554b157ab0b71e64e8d5bef775cd66b6531e52d302669"
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.58"
+version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8326b86b6cff230b97d0d312a6c40a60726df3332e721f72a1b035f451663b20"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows-core",
@@ -345,139 +400,173 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
+name = "ident_case"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
+
+[[package]]
 name = "indexmap"
-version = "2.1.0"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d530e1a18b1cb4c484e6e34556a0d948706958449fca0cab753d649f2bce3d1f"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "itertools"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itoa"
+version = "1.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
+
+[[package]]
 name = "js-sys"
-version = "0.3.65"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54c0c35952f67de54bb584e9fd912b3023117cbafc0a77d8f3dee1fb5f572fe8"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.149"
+version = "0.2.153"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+
+[[package]]
+name = "libm"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a08173bc88b7955d1b3145aa561539096c421ac8debde8cbc3612ec635fee29b"
+checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "lz4_flex"
-version = "0.11.1"
+version = "0.11.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ea9b256699eda7b0387ffbc776dd625e28bde3918446381781245b7a50349d8"
+checksum = "75761162ae2b0e580d7e7c390558127e5f01b4194debd6221fd8c207fc80e3f5"
 dependencies = [
  "twox-hash",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.6.4"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f665ee40bc4a3c5590afb1e9677db74a508659dfd71e126420da8274909a0167"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.9"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3dce281c5e46beae905d4de1870d8b1509a9142b62eedf18b443b011ca8343d0"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "wasi",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "num-bigint"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5f6f7833f2cbf2360a6cfd58cd41a53aa7a90bd4c202f5b1c7dd2ed73c57b2c3"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
-name = "num-integer"
-version = "0.1.45"
+name = "num-bigint"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
 dependencies = [
  "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
+name = "num-conv"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
+
+[[package]]
+name = "num-integer"
+version = "0.1.46"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
+dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -502,39 +591,39 @@
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96667db765a921f7b295ffee8b60472b686a51d4f21c2ee4ffdb94c7013b65a6"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "object"
-version = "0.32.1"
+version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cf5f9dd3933bd50a9e1f149ec995f39ae2c496d31fd772c1fd45ebc27e902b0"
+checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "openssl"
-version = "0.10.59"
+version = "0.10.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a257ad03cd8fb16ad4172fedf8094451e1af1c4b70097636ef2eac9a5f0cc33"
+checksum = "95a0481286a310808298130d22dd1fef0fa571e05a8f44ec801801e84b216b1f"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
@@ -543,31 +632,31 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "openssl-src"
-version = "300.1.6+3.1.4"
+version = "300.2.3+3.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "439fac53e092cd7442a3660c85dde4643ab3b5bd39040912388dcdabf6b88085"
+checksum = "5cff92b6f71555b61bb9315f7c64da3ca43d87531622120fea0195fc761b4843"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.95"
+version = "0.9.102"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "40a4130519a360279579c2053038317e40eff64d13fd3f004f9e1b72b8a6aaf9"
+checksum = "c597637d56fbc83893a35eb0dd04b2b8e7a50c91e64e9493e398b5df4fb45fa2"
 dependencies = [
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
@@ -588,34 +677,46 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.27"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
+
+[[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
+name = "powerfmt"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
@@ -627,111 +728,114 @@
 dependencies = [
  "once_cell",
  "toml_edit",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.69"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "134c189feb4956b20f6f547d2cf727d4c0fe06722b20a0eec87ed445a97f92da"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
  "chrono",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-asyncio"
-version = "0.19.0"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2cc34c1f907ca090d7add03dc523acdd91f3a4dab12286604951e2f5152edad"
+checksum = "6ea6b68e93db3622f3bb3bf363246cf948ed5375afe7abff98ccbdd50b184995"
 dependencies = [
  "futures",
  "once_cell",
  "pin-project-lite",
  "pyo3",
  "tokio",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
-version = "0.8.4"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c09c2b349b6538d8a73d436ca606dab6ce0aaab4dad9e6b7bdd57a4f556c3bc3"
+checksum = "4c10808ee7250403bedb24bc30c32493e93875fef7ba3e4292226fe924f398bd"
 dependencies = [
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
+ "heck 0.4.1",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -790,42 +894,40 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "scylla"
-version = "0.10.1"
+version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b30067d0d0313a0bbcda9c31a503678f18dacd5426dd8a63c3f581cf80f5c30"
+checksum = "03d2db76aa23f55d2ece5354e1a3778633098a3d1ea76153f494d71e92cd02d8"
 dependencies = [
  "arc-swap",
  "async-trait",
- "bigdecimal",
  "byteorder",
  "bytes",
  "chrono",
  "dashmap",
  "futures",
  "histogram",
  "itertools",
  "lz4_flex",
- "num-bigint",
  "num_enum",
  "openssl",
  "rand",
  "rand_pcg",
  "scylla-cql",
  "scylla-macros",
  "smallvec",
@@ -838,114 +940,154 @@
  "tokio-openssl",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "scylla-cql"
-version = "0.0.9"
+version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c9642864295085ef2fe62493eec405a109fbaae9f3a9b80ea087556af4a97df2"
+checksum = "345626c0dd5d9624c413daaba854685bba6a65cff4eb5ea0fb0366df16901f67"
 dependencies = [
  "async-trait",
  "bigdecimal",
  "byteorder",
  "bytes",
  "chrono",
  "lz4_flex",
- "num-bigint",
+ "num-bigint 0.3.3",
+ "num-bigint 0.4.4",
  "num_enum",
  "scylla-macros",
+ "secrecy",
  "snap",
  "thiserror",
+ "time",
  "tokio",
  "uuid",
 ]
 
 [[package]]
 name = "scylla-macros"
-version = "0.2.1"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5757ded3dfb10967ca7d1ff1084d072d565b5e10b2b21c286d5335c245425a7e"
+checksum = "eb6085ff9c3fd7e5163826901d39164ab86f11bdca16b2f766a00c528ff9cef9"
 dependencies = [
+ "darling",
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "scyllapy"
-version = "1.3.0"
+version = "1.3.1"
 dependencies = [
+ "bigdecimal",
  "chrono",
  "eq-float",
  "futures",
  "log",
  "openssl",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
  "rustc-hash",
  "scylla",
- "scylla-cql",
  "thiserror",
+ "time",
  "tokio",
  "uuid",
 ]
 
 [[package]]
+name = "secrecy"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0673d6a6449f5e7d12a1caf424fd9363e2af3a4953023ed455e3c4beef4597c0"
+dependencies = [
+ "zeroize",
+]
+
+[[package]]
+name = "serde"
+version = "1.0.198"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
+dependencies = [
+ "serde_derive",
+]
+
+[[package]]
+name = "serde_derive"
+version = "1.0.198"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.60",
+]
+
+[[package]]
 name = "slab"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "942b4a808e05215192e39f4ab80813e599068285906cc91aa64f923db842bd5a"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "snap"
-version = "1.1.0"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e9f0ab6ef7eb7353d9119c170a436d1bf248eea575ac42d19d12f4e34130831"
+checksum = "1b6b67fb9a61334225b5b790716f609cd58395f895b3fe8b328786812a40bc3b"
 
 [[package]]
 name = "socket2"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
+checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
+name = "strsim"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
+
+[[package]]
 name = "strum"
 version = "0.23.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cae14b91c7d11c9a851d3fbc80a963198998c2a64eec840477fa92d8ce9b70bb"
 
 [[package]]
 name = "strum_macros"
 version = "0.23.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5bb0dc7ee9c15cea6199cde9a127fa16a4c5819af85395457ad72d68edc85a38"
 dependencies = [
- "heck",
+ "heck 0.3.3",
  "proc-macro2",
  "quote",
  "rustversion",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -957,82 +1099,113 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.38"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e96b79aaa137db8f61e26363a0c9b47d8b4ec75da28b7d1d614c2303e232408b"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.12"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c39fd04924ca3a864207c66fc2cd7d22d7c016007f9ce846cbb9326331930a"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.50"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9a7210f5c9a7156bb50aa36aed4c95afb51df0df00713949448cf9e97d382d2"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.50"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "266b2e40bc00e5a6c09c3584011e08b06f123c00362c92b975ba9843aaaa14b8"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.60",
+]
+
+[[package]]
+name = "time"
+version = "0.3.36"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
+dependencies = [
+ "deranged",
+ "itoa",
+ "num-conv",
+ "powerfmt",
+ "serde",
+ "time-core",
+ "time-macros",
+]
+
+[[package]]
+name = "time-core"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
+
+[[package]]
+name = "time-macros"
+version = "0.2.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f252a68540fde3a3877aeea552b832b40ab9a69e318efd078774a01ddee1ccf"
+dependencies = [
+ "num-conv",
+ "time-core",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.33.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f38200e3ef7995e5ef13baec2f432a6da0aa9ac495b2c0e8f3b7eec2c92d653"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "socket2",
  "tokio-macros",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "2.1.0"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
+checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tokio-openssl"
-version = "0.6.3"
+version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08f9ffb7809f1b20c1b398d92acf4cc719874b3b2b2d9ea2f09b4a80350878a"
+checksum = "6ffab79df67727f6acf57f1ff743091873c24c579b1e2ce4d8f53e47ded4d63d"
 dependencies = [
  "futures-util",
  "openssl",
  "openssl-sys",
  "tokio",
 ]
 
@@ -1068,15 +1241,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -1098,29 +1271,29 @@
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-segmentation"
-version = "1.10.1"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
+checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "uuid"
-version = "1.5.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88ad59a7560b41a70d191093a945f0b87bc1deeda46fb237479708a1d6b6cdfc"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
@@ -1131,142 +1304,221 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.88"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7daec296f25a1bae309c0cd5c29c4b260e510e6d813c286b19eaadf409d40fce"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.88"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e397f4664c0e4e428e8313a469aaa58310d302159845980fd23b0f22a847f217"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.88"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5961017b3b08ad5f3fe39f1e79877f8ee7c23c5e5fd5eb80de95abc41f1f16b2"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.88"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5353b8dab669f5e10f5bd76df26a9360c748f054f862ff5f3f8aae0c7fb3907"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.38",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.88"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d046c5d029ba91a1ed14da14dca44b68bf2f124cfbaf741c54151fdb3e0750b"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "windows-core"
-version = "0.51.1"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1f8cf84f35d2db49a46868f947758c7a1138116f7fac3bc844f43ade1292e64"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.5",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.48.5",
+ "windows_aarch64_msvc 0.48.5",
+ "windows_i686_gnu 0.48.5",
+ "windows_i686_msvc 0.48.5",
+ "windows_x86_64_gnu 0.48.5",
+ "windows_x86_64_gnullvm 0.48.5",
+ "windows_x86_64_msvc 0.48.5",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
+dependencies = [
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
+
+[[package]]
 name = "winnow"
-version = "0.5.18"
+version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176b6138793677221d420fd2f0aeeced263f197688b36484660da767bca2fa32"
+checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
+
+[[package]]
+name = "zeroize"
+version = "1.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
```

### Comparing `scyllapy-1.3.0/pyproject.toml` & `scyllapy-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "Programming Language :: Rust",
     "Operating System :: MacOS",
     "Operating System :: Microsoft",
     "Operating System :: POSIX :: Linux",
     "Intended Audience :: Developers",
     "Topic :: Database :: Front-Ends",
 ]
-
+dependencies = ["python-dateutil"]
 
 [tool.maturin]
 python-source = "python"
 module-name = "scyllapy._internal"
 features = ["pyo3/extension-module"]
 
 [tool.isort]
@@ -101,8 +101,8 @@
 ]
 
 [tool.ruff.pydocstyle]
 convention = "pep257"
 ignore-decorators = ["typing.overload"]
 
 [tool.ruff.pylint]
-allow-magic-value-types = ["int", "str", "float", "tuple"]
+allow-magic-value-types = ["int", "str", "float"]
```

### Comparing `scyllapy-1.3.0/PKG-INFO` & `scyllapy-1.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: scyllapy
-Version: 1.3.0
+Version: 1.3.1
 Classifier: Typing :: Typed
 Classifier: Topic :: Database
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database :: Front-Ends
+Requires-Dist: python-dateutil
 License-File: LICENSE
 Summary: Async scylla driver for python
 Keywords: scylla,cassandra,async-driver,scylla-driver
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 [![PyPI](https://img.shields.io/pypi/v/scyllapy?style=for-the-badge)](https://pypi.org/project/scyllapy/)
@@ -103,14 +104,43 @@
 query = Query("SELECT * FROM table")
 
 new_query = query.with_consistency(Consistency.ALL)
 ```
 
 All `with_` methods create new query, copying all other parameters.
 
+Here's the list of scylla types and corresponding python types that you should use while passing parameters to queries:
+
+| Scylla type | Python type            |
+| ----------- | ---------------------- |
+| int         | int                    |
+| tinyint     | extra_types.TinyInt    |
+| bigint      | extra_types.BigInt     |
+| varint      | any int type           |
+| float       | float                  |
+| double      | extra_types.Double     |
+| decimal     | decimal.Decimal        |
+| ascii       | str                    |
+| text        | str                    |
+| varchar     | str                    |
+| blob        | bytes                  |
+| boolean     | bool                   |
+| counter     | extra_types.Counter    |
+| date        | datetime.date          |
+| uuid        | uuid.UUID              |
+| inet        | ipaddress              |
+| time        | datetime.time          |
+| timestamp   | datetime.datetime      |
+| duration    | dateutil.relativedelta |
+
+All types from `extra_types` module are used to eliminate any possible ambiguity while passing parameters to queries. You can find more information about them in `Extra types` section.
+
+We use relative delta from `dateutil` for duration, because it's the only way to represent it in python. Since scylla operates with months, days and nanosecond, there's no way we can represent it in python, becuase months are variable length.
+
+
 ## Named parameters
 
 Also, you can provide named parameters to querties, by using name
 placeholders instead of `?`.
 
 For example:
```

