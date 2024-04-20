# Comparing `tmp/ry-0.0.3.tar.gz` & `tmp/ry-0.0.5.tar.gz`

## Comparing `ry-0.0.3.tar` & `ry-0.0.5.tar`

### file list

```diff
@@ -1,67 +1,70 @@
--rw-r--r--   0     1001      127      867 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/Cargo.toml
--rw-r--r--   0     1001      127      317 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/build.rs
--rw-r--r--   0     1001      127     1008 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/dev/anystr.rs
--rw-r--r--   0     1001      127      223 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/dev/mod.rs
--rw-r--r--   0     1001      127      709 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/dev/quick_maths.rs
--rw-r--r--   0     1001      127     3449 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/fmts.rs
--rw-r--r--   0     1001      127     1668 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/fnv.rs
--rw-r--r--   0     1001      127     2137 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/fs/fileio.rs
--rw-r--r--   0     1001      127     7403 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/fs/fspath.rs
--rw-r--r--   0     1001      127      227 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/fs/mod.rs
--rw-r--r--   0     1001      127      679 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/lib.rs
--rw-r--r--   0     1001      127     1958 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/libs/brotli.rs
--rw-r--r--   0     1001      127     1640 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/libs/jiter_ry.rs
--rw-r--r--   0     1001      127      331 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/libs/mod.rs
--rw-r--r--   0     1001      127     1928 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/sh.rs
--rw-r--r--   0     1001      127      338 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/shlex.rs
--rw-r--r--   0     1001      127      878 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/sleep.rs
--rw-r--r--   0     1001      127      496 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/sp/done.rs
--rw-r--r--   0     1001      127      234 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/sp/mod.rs
--rw-r--r--   0     1001      127      790 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/sp/pydone.rs
--rw-r--r--   0     1001      127     4220 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/sp/run.rs
--rw-r--r--   0     1001      127     5940 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/walkdir.rs
--rw-r--r--   0     1001      127     1481 2024-03-27 05:01:53.000000 ry-0.0.3/crates/ryo3/src/which.rs
--rw-r--r--   0        0        0     1868 1970-01-01 00:00:00.000000 ry-0.0.3/Cargo.toml
--rw-r--r--   0     1001      127     1364 2024-03-27 05:01:53.000000 ry-0.0.3/.editorconfig
--rw-r--r--   0     1001      127     1323 2024-03-27 05:01:53.000000 ry-0.0.3/.gitattributes
--rw-r--r--   0     1001      127      283 2024-03-27 05:01:53.000000 ry-0.0.3/.github/dependabot.yml
--rw-r--r--   0     1001      127     5334 2024-03-27 05:01:53.000000 ry-0.0.3/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      975 2024-03-27 05:01:53.000000 ry-0.0.3/.github/workflows/dev.yml
--rw-r--r--   0     1001      127      697 2024-03-27 05:01:53.000000 ry-0.0.3/.gitignore
--rw-r--r--   0     1001      127      526 2024-03-27 05:01:53.000000 ry-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      424 2024-03-27 05:01:53.000000 ry-0.0.3/README.md
--rw-r--r--   0     1001      127      717 2024-03-27 05:01:53.000000 ry-0.0.3/bench/test_build_profile.py
--rw-r--r--   0     1001      127     1201 2024-03-27 05:01:53.000000 ry-0.0.3/bench/test_jiter.py
--rw-r--r--   0     1001      127      357 2024-03-27 05:01:53.000000 ry-0.0.3/build.rs
--rw-r--r--   0     1001      127      622 2024-03-27 05:01:53.000000 ry-0.0.3/justfile
--rw-r--r--   0     1001      127      308 2024-03-27 05:01:53.000000 ry-0.0.3/package.json
--rw-r--r--   0     1001      127      420 2024-03-27 05:01:53.000000 ry-0.0.3/python/ry/__about__.py
--rw-r--r--   0     1001      127      292 2024-03-27 05:01:53.000000 ry-0.0.3/python/ry/__init__.py
--rw-r--r--   0     1001      127      920 2024-03-27 05:01:53.000000 ry-0.0.3/python/ry/__main__.py
--rw-r--r--   0     1001      127     3499 2024-03-27 05:01:53.000000 ry-0.0.3/python/ry/_ry.pyi
--rw-r--r--   0     1001      127        0 2024-03-27 05:01:53.000000 ry-0.0.3/python/ry/py.typed
--rw-r--r--   0     1001      127       64 2024-03-27 05:01:53.000000 ry-0.0.3/requirements.dev.in
--rw-r--r--   0     1001      127      618 2024-03-27 05:01:53.000000 ry-0.0.3/requirements.dev.txt
--rw-r--r--   0     1001      127     1266 2024-03-27 05:01:53.000000 ry-0.0.3/scripts/gen.py
--rw-r--r--   0     1001      127     2273 2024-03-27 05:01:53.000000 ry-0.0.3/src/lager.rs
--rw-r--r--   0     1001      127     1079 2024-03-27 05:01:53.000000 ry-0.0.3/src/lib.rs
--rw-r--r--   0     1001      127      103 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test__template.py
--rw-r--r--   0     1001      127      272 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_anystr.py
--rw-r--r--   0     1001      127     1305 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_brotli.py
--rw-r--r--   0     1001      127      270 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_build_profile.py
--rw-r--r--   0     1001      127      242 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_exports.py
--rw-r--r--   0     1001      127     6307 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_fnv.py
--rw-r--r--   0     1001      127     1400 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_fs.py
--rw-r--r--   0     1001      127     1589 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_fspath.py
--rw-r--r--   0     1001      127      526 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_jiter.py
--rw-r--r--   0     1001      127     1067 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_pwd_cd.py
--rw-r--r--   0     1001      127      862 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_run.py
--rw-r--r--   0     1001      127      421 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_sh.py
--rw-r--r--   0     1001      127     4969 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_shplit.py
--rw-r--r--   0     1001      127      454 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_sleep.py
--rw-r--r--   0     1001      127     1501 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_version.py
--rw-r--r--   0     1001      127     2673 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_walkdir.py
--rw-r--r--   0     1001      127     4194 2024-03-27 05:01:53.000000 ry-0.0.3/tests/test_which.py
--rw-r--r--   0     1001      127    38694 2024-03-27 05:01:53.000000 ry-0.0.3/Cargo.lock
--rw-r--r--   0     1001      127     3458 2024-03-27 05:01:53.000000 ry-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 ry-0.0.3/PKG-INFO
+-rw-r--r--   0     1001      127     1187 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/Cargo.toml
+-rw-r--r--   0     1001      127      317 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/build.rs
+-rw-r--r--   0     1001      127     1162 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/dev/anystr.rs
+-rw-r--r--   0     1001      127      225 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/dev/mod.rs
+-rw-r--r--   0     1001      127      699 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/dev/quick_maths.rs
+-rw-r--r--   0     1001      127     3463 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/fmts.rs
+-rw-r--r--   0     1001      127     2148 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/fs/fileio.rs
+-rw-r--r--   0     1001      127     7446 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/fs/fspath.rs
+-rw-r--r--   0     1001      127      215 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/fs/mod.rs
+-rw-r--r--   0     1001      127      578 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/lib.rs
+-rw-r--r--   0     1001      127     1923 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/libs/brotli.rs
+-rw-r--r--   0     1001      127     1658 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/libs/fnv.rs
+-rw-r--r--   0     1001      127     2540 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/libs/jiter_ry.rs
+-rw-r--r--   0     1001      127      566 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/libs/mod.rs
+-rw-r--r--   0     1001      127     1480 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/libs/which.rs
+-rw-r--r--   0     1001      127    11407 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/libs/xxhash.rs
+-rw-r--r--   0     1001      127     1940 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/sh.rs
+-rw-r--r--   0     1001      127      336 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/shlex.rs
+-rw-r--r--   0     1001      127      909 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/sleep.rs
+-rw-r--r--   0     1001      127      496 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/sp/done.rs
+-rw-r--r--   0     1001      127      246 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/sp/mod.rs
+-rw-r--r--   0     1001      127      804 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/sp/pydone.rs
+-rw-r--r--   0     1001      127     4232 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/sp/run.rs
+-rw-r--r--   0     1001      127     5939 2024-04-20 00:58:25.000000 ry-0.0.5/crates/ryo3/src/walkdir.rs
+-rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 ry-0.0.5/Cargo.toml
+-rw-r--r--   0     1001      127     1364 2024-04-20 00:58:25.000000 ry-0.0.5/.editorconfig
+-rw-r--r--   0     1001      127     1323 2024-04-20 00:58:25.000000 ry-0.0.5/.gitattributes
+-rw-r--r--   0     1001      127      283 2024-04-20 00:58:25.000000 ry-0.0.5/.github/dependabot.yml
+-rw-r--r--   0     1001      127     5145 2024-04-20 00:58:25.000000 ry-0.0.5/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127     1250 2024-04-20 00:58:25.000000 ry-0.0.5/.github/workflows/dev.yml
+-rw-r--r--   0     1001      127      706 2024-04-20 00:58:25.000000 ry-0.0.5/.gitignore
+-rw-r--r--   0     1001      127      526 2024-04-20 00:58:25.000000 ry-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127       77 2024-04-20 00:58:25.000000 ry-0.0.5/CHANGELOG.md
+-rw-r--r--   0     1001      127      424 2024-04-20 00:58:25.000000 ry-0.0.5/README.md
+-rw-r--r--   0     1001      127      717 2024-04-20 00:58:25.000000 ry-0.0.5/bench/test_build_profile.py
+-rw-r--r--   0     1001      127     1201 2024-04-20 00:58:25.000000 ry-0.0.5/bench/test_jiter.py
+-rw-r--r--   0     1001      127      357 2024-04-20 00:58:25.000000 ry-0.0.5/build.rs
+-rw-r--r--   0     1001      127     2334 2024-04-20 00:58:25.000000 ry-0.0.5/justfile
+-rw-r--r--   0     1001      127      308 2024-04-20 00:58:25.000000 ry-0.0.5/package.json
+-rw-r--r--   0     1001      127      420 2024-04-20 00:58:25.000000 ry-0.0.5/python/ry/__about__.py
+-rw-r--r--   0     1001      127      292 2024-04-20 00:58:25.000000 ry-0.0.5/python/ry/__init__.py
+-rw-r--r--   0     1001      127      920 2024-04-20 00:58:25.000000 ry-0.0.5/python/ry/__main__.py
+-rw-r--r--   0     1001      127     6309 2024-04-20 00:58:25.000000 ry-0.0.5/python/ry/_ry.pyi
+-rw-r--r--   0     1001      127        0 2024-04-20 00:58:25.000000 ry-0.0.5/python/ry/py.typed
+-rw-r--r--   0     1001      127       64 2024-04-20 00:58:25.000000 ry-0.0.5/requirements.dev.in
+-rw-r--r--   0     1001      127      636 2024-04-20 00:58:25.000000 ry-0.0.5/requirements.dev.txt
+-rw-r--r--   0     1001      127     1266 2024-04-20 00:58:25.000000 ry-0.0.5/scripts/gen.py
+-rw-r--r--   0     1001      127     2273 2024-04-20 00:58:25.000000 ry-0.0.5/src/lager.rs
+-rw-r--r--   0     1001      127     1132 2024-04-20 00:58:25.000000 ry-0.0.5/src/lib.rs
+-rw-r--r--   0     1001      127      103 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test__template.py
+-rw-r--r--   0     1001      127      272 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_anystr.py
+-rw-r--r--   0     1001      127     1045 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_brotli.py
+-rw-r--r--   0     1001      127      270 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_build_profile.py
+-rw-r--r--   0     1001      127      242 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_exports.py
+-rw-r--r--   0     1001      127     6307 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_fnv.py
+-rw-r--r--   0     1001      127     1401 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_fs.py
+-rw-r--r--   0     1001      127     1590 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_fspath.py
+-rw-r--r--   0     1001      127      526 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_jiter.py
+-rw-r--r--   0     1001      127     1067 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_pwd_cd.py
+-rw-r--r--   0     1001      127      862 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_run.py
+-rw-r--r--   0     1001      127      422 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_sh.py
+-rw-r--r--   0     1001      127     4969 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_shplit.py
+-rw-r--r--   0     1001      127      457 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_sleep.py
+-rw-r--r--   0     1001      127     1501 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_version.py
+-rw-r--r--   0     1001      127     2718 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_walkdir.py
+-rw-r--r--   0     1001      127     4194 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_which.py
+-rw-r--r--   0     1001      127    62695 2024-04-20 00:58:25.000000 ry-0.0.5/tests/test_xxhash.py
+-rw-r--r--   0     1001      127    34178 2024-04-20 00:58:25.000000 ry-0.0.5/Cargo.lock
+-rw-r--r--   0     1001      127     4158 2024-04-20 00:58:25.000000 ry-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 ry-0.0.5/PKG-INFO
```

### Comparing `ry-0.0.3/crates/ryo3/src/dev/quick_maths.rs` & `ry-0.0.5/crates/ryo3/src/dev/quick_maths.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 //! Quick maths - template module
 use pyo3::prelude::*;
 use pyo3::types::PyModule;
-use pyo3::{wrap_pyfunction, PyResult, Python};
+use pyo3::{wrap_pyfunction, PyResult};
 
 /// 2 + 2 that's 4, minus 1 that's 3, quick maths
 ///
 /// Based on the Big Shaq's thesis "Man's Not Hot"
 ///
 /// Ref: https://youtu.be/3M_5oYU-IsU?t=60
 ///
@@ -21,11 +21,11 @@
 pub fn quick_maths() -> i32 {
     // 2 + 2 that's 4, minus 1 that's 3, quick maths
     let mut qm = 2 + 2;
     qm -= 1;
     qm
 }
 
-pub fn madd(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn madd(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(quick_maths, m)?)?;
     Ok(())
 }
```

### Comparing `ry-0.0.3/crates/ryo3/src/fmts.rs` & `ry-0.0.5/crates/ryo3/src/fmts.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+use pyo3::prelude::*;
 use pyo3::types::PyModule;
-use pyo3::{pyfunction, wrap_pyfunction, PyResult, Python};
+use pyo3::{pyfunction, wrap_pyfunction, PyResult};
 
 const KILOBYTE: f64 = 1024.0;
 const MEGABYTE: f64 = KILOBYTE * 1024.0;
 const GIGABYTE: f64 = MEGABYTE * 1024.0;
 const TERABYTE: f64 = GIGABYTE * 1024.0;
 const PETABYTE: f64 = TERABYTE * 1024.0;
 const EXABYTE: f64 = PETABYTE * 1024.0;
@@ -29,26 +30,28 @@
 
     if nbytes >= 0.0 {
         Ok(formatted_size)
     } else {
         Err(format!("Invalid number of bytes: {}", nbytes))
     }
 }
+
 fn nbytes_i64(nbytes: i64, precision: Option<usize>) -> Result<String, String> {
     let nabs = if nbytes < 0 { -nbytes } else { nbytes };
     nbytes_u64(nabs as u64, precision)
 }
+
 // TODO: Fix to handle negative numbers
 #[pyfunction]
 #[pyo3(name = "fmt_nbytes")]
 pub fn fmt_nbytes(nbytes: i64) -> PyResult<String> {
     Ok(nbytes_i64(nbytes, Option::from(1)).unwrap())
 }
 
-pub fn madd(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn madd(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(fmt_nbytes, m)?)?;
     Ok(())
 }
 
 #[cfg(test)]
 mod tests {
     #[test]
```

### Comparing `ry-0.0.3/crates/ryo3/src/fnv.rs` & `ry-0.0.5/crates/ryo3/src/libs/fnv.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::hash::Hasher;
 
 use ::fnv as fnv_rs;
 use pyo3::prelude::*;
 use pyo3::types::PyModule;
-use pyo3::{wrap_pyfunction, PyResult, Python};
+use pyo3::{wrap_pyfunction, PyResult};
 
 #[pyclass(name = "FnvHasher")]
 pub struct PyFnvHasher {
     pub hasher: fnv_rs::FnvHasher,
 }
 
 #[pymethods]
@@ -61,12 +61,12 @@
 }
 
 #[pyfunction]
 pub fn fnv1a(s: &[u8]) -> PyResult<PyFnvHasher> {
     Ok(PyFnvHasher::new(Some(s)))
 }
 
-pub fn madd(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn madd(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<PyFnvHasher>()?;
     m.add_function(wrap_pyfunction!(self::fnv1a, m)?)?;
     Ok(())
 }
```

### Comparing `ry-0.0.3/crates/ryo3/src/fs/fileio.rs` & `ry-0.0.5/crates/ryo3/src/fs/fileio.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+use std::path::Path;
+
 use pyo3::exceptions::{PyFileNotFoundError, PyUnicodeDecodeError};
 use pyo3::prelude::*;
 use pyo3::types::{PyBytes, PyModule};
 use pyo3::{pyfunction, wrap_pyfunction, PyResult};
-use std::path::Path;
 
 #[pyfunction]
 pub fn read_vec_u8(s: &str) -> PyResult<Vec<u8>> {
     let p = Path::new(s);
     let b = std::fs::read(p);
     match b {
         Ok(b) => Ok(b),
@@ -16,25 +17,25 @@
         }
     }
 }
 
 #[pyfunction]
 pub fn read_bytes(py: Python<'_>, s: &str) -> PyResult<PyObject> {
     let bvec = read_vec_u8(s)?;
-    Ok(PyBytes::new(py, &bvec).into())
+    Ok(PyBytes::new_bound(py, &bvec).into())
 }
 
 #[pyfunction]
 pub fn read_text(py: Python<'_>, s: &str) -> PyResult<String> {
     let bvec = read_vec_u8(s)?;
     let r = std::str::from_utf8(&bvec);
     match r {
         Ok(s) => Ok(s.to_string()),
         Err(e) => {
-            let decode_err = PyUnicodeDecodeError::new_utf8(py, &bvec, e).unwrap();
+            let decode_err = PyUnicodeDecodeError::new_utf8_bound(py, &bvec, e).unwrap();
             Err(decode_err.into())
         }
     }
 }
 
 #[pyfunction]
 pub fn write_bytes(s: &str, b: Vec<u8>) -> PyResult<()> {
@@ -59,14 +60,14 @@
             let emsg = format!("{}: {} - {:?}", p.to_str().unwrap(), e, p.to_str().unwrap());
             Err(PyFileNotFoundError::new_err(emsg))
         }
     }
 }
 
 // #[instrument(level = "warn", err, fields(s = module_path!()), ret, skip(_py))]
-pub fn madd(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn madd(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(read_text, m)?)?;
     m.add_function(wrap_pyfunction!(read_bytes, m)?)?;
     m.add_function(wrap_pyfunction!(write_text, m)?)?;
     m.add_function(wrap_pyfunction!(write_bytes, m)?)?;
     Ok(())
 }
```

### Comparing `ry-0.0.3/crates/ryo3/src/fs/fspath.rs` & `ry-0.0.5/crates/ryo3/src/fs/fspath.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+use std::path::{Path, PathBuf};
+
+use pyo3::prelude::*;
 use pyo3::types::{PyModule, PyType};
 use pyo3::{pyclass, pymethods, FromPyObject, PyObject, PyResult, Python};
-use std::path::{Path, PathBuf};
 
 use crate::fs::fileio::{read_bytes, read_text};
 
 #[pyclass(name = "FsPath")]
 #[derive(Debug, Clone, PartialEq, Eq)]
 pub struct PyFsPath {
     pth: PathBuf,
@@ -180,21 +182,21 @@
     #[getter]
     fn stem(&self) -> PyResult<String> {
         let s = self.pth.file_stem().unwrap().to_str().unwrap().to_string();
         Ok(s)
     }
 
     #[classmethod]
-    fn home(_cls: &PyType) -> PyResult<PyFsPath> {
+    fn home(_cls: &Bound<'_, PyType>) -> PyResult<PyFsPath> {
         let p = dirs::home_dir().unwrap();
         Ok(p.into())
     }
 
     #[classmethod]
-    fn cwd(_cls: &PyType) -> PyResult<PyFsPath> {
+    fn cwd(_cls: &Bound<'_, PyType>) -> PyResult<PyFsPath> {
         let p = std::env::current_dir().unwrap();
         Ok(p.into())
     }
 
     fn read_bytes(&self, py: Python<'_>) -> PyResult<PyObject> {
         read_bytes(py, &self.string())
     }
@@ -285,11 +287,11 @@
         match self {
             PathLike::PathBuf(p) => write!(f, "{}", p.to_str().unwrap()),
             PathLike::Str(s) => write!(f, "{}", s),
         }
     }
 }
 
-pub fn madd(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn madd(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<PyFsPath>()?;
     Ok(())
 }
```

### Comparing `ry-0.0.3/crates/ryo3/src/libs/brotli.rs` & `ry-0.0.5/crates/ryo3/src/libs/brotli.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+use std::io::{Read, Write};
+
 use ::brotli as br;
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
-use std::io::{Read, Write};
 
 #[pyfunction]
 pub fn brotli_encode(
     py: Python<'_>,
     data: &[u8],
     quality: Option<u32>,
     magic_number: Option<bool>,
@@ -19,37 +20,35 @@
                 ..Default::default()
             };
             let mut encoder = br::CompressorWriter::with_params(Vec::new(), 4 * 1024, &params);
             // let mut encoder = br::CompressorWriter::new(Vec::new(), 4 * 1024, 11, 22);
             encoder.write_all(data).map_err(|e| {
                 PyErr::new::<pyo3::exceptions::PyValueError, _>(format!("Error: {:?}", e))
             })?;
-            let t = encoder.into_inner();
-            t
+            encoder.into_inner()
         }
         _ => {
             let quality = if let Some(param) = quality { param } else { 11 };
             let mut encoder = br::CompressorWriter::new(Vec::new(), 4 * 1024, quality, 22);
             encoder.write_all(data).map_err(|e| {
                 PyErr::new::<pyo3::exceptions::PyValueError, _>(format!("Error: {:?}", e))
             })?;
-            let t = encoder.into_inner();
-            t
+            encoder.into_inner()
         }
     };
-    Ok(PyBytes::new(py, &encoded).into())
+    Ok(PyBytes::new_bound(py, &encoded).into())
 }
 
 #[pyfunction]
 pub fn brotli_decode(py: Python<'_>, data: &[u8]) -> PyResult<PyObject> {
     let mut decompressed = Vec::new();
     br::Decompressor::new(data, 4 * 1024)
         .read_to_end(&mut decompressed)
         .map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(format!("Error: {:?}", e)))?;
-    Ok(PyBytes::new(py, &decompressed).into())
+    Ok(PyBytes::new_bound(py, &decompressed).into())
 }
 
-pub fn madd(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn madd(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(brotli_decode, m)?)?;
     m.add_function(wrap_pyfunction!(brotli_encode, m)?)?;
     Ok(())
 }
```

### Comparing `ry-0.0.3/crates/ryo3/src/libs/jiter_ry.rs` & `ry-0.0.5/crates/ryo3/src/libs/jiter_ry.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,83 @@
 use ::jiter::map_json_error;
 use ::jiter::python_parse;
-use std::fmt::Debug;
-
+use ::jiter::StringCacheMode;
 use pyo3::prelude::*;
+use pyo3::pybacked::{PyBackedBytes, PyBackedStr};
 
-#[derive(Debug, FromPyObject)]
-pub enum BytesOrString<'a> {
-    Str(&'a str),
-    Bytes(&'a [u8]),
+#[derive(FromPyObject)]
+pub enum BytesOrString {
+    Str(PyBackedStr),
+    Bytes(PyBackedBytes),
 }
 
-#[pyfunction(signature = (data, *, allow_inf_nan = true, cache_strings = true))]
-pub fn parse_json_bytes(
-    py: Python,
+#[pyfunction(signature = (data, *, allow_inf_nan = true, cache_strings = true, allow_partial = false))]
+pub fn parse_json_bytes<'py>(
+    py: Python<'py>,
     data: &[u8],
     allow_inf_nan: bool,
     cache_strings: bool,
-) -> PyResult<PyObject> {
+    allow_partial: bool,
+) -> PyResult<Bound<'py, PyAny>> {
     let json_bytes = data;
-    python_parse(py, json_bytes, allow_inf_nan, cache_strings)
+    let cache_mode = if cache_strings {
+        StringCacheMode::All
+    } else {
+        StringCacheMode::None
+    };
+    python_parse(py, json_bytes, allow_inf_nan, cache_mode, allow_partial)
         .map_err(|e| map_json_error(json_bytes, &e))
 }
 
 #[pyfunction(signature = (data, *, allow_inf_nan = true, cache_strings = true))]
 pub fn parse_json_str(
     py: Python,
     data: &str,
     allow_inf_nan: bool,
     cache_strings: bool,
 ) -> PyResult<PyObject> {
     let json_bytes = data.as_bytes();
-    python_parse(py, json_bytes, allow_inf_nan, cache_strings)
+    let cache_mode = if cache_strings {
+        StringCacheMode::All
+    } else {
+        StringCacheMode::None
+    };
+    python_parse(py, json_bytes, allow_inf_nan, cache_mode, false)
         .map_err(|e| map_json_error(json_bytes, &e))
+        .map(|v| v.into_py(py))
 }
 
-#[pyfunction(signature = (data, *, allow_inf_nan = true, cache_strings = true))]
+#[pyfunction(signature = (data, *, allow_inf_nan = true, cache_strings = true, allow_partial = false))]
 pub fn parse_json(
-    py: Python,
+    py: Python<'_>,
     data: BytesOrString,
     allow_inf_nan: bool,
     cache_strings: bool,
-) -> PyResult<PyObject> {
-    let json_bytes = match data {
-        BytesOrString::Str(s) => s.as_bytes(),
-        BytesOrString::Bytes(b) => b,
+    allow_partial: bool,
+) -> PyResult<Bound<'_, PyAny>> {
+    let cache_mode = if cache_strings {
+        StringCacheMode::All
+    } else {
+        StringCacheMode::None
     };
-    python_parse(py, json_bytes, allow_inf_nan, cache_strings)
-        .map_err(|e| map_json_error(json_bytes, &e))
+
+    // Directly call python_parse within the match arms
+    match data {
+        BytesOrString::Str(s) => {
+            let json_bytes: &[u8] = s.as_ref();
+            python_parse(py, json_bytes, allow_inf_nan, cache_mode, allow_partial)
+                .map_err(|e| map_json_error(json_bytes, &e))
+        }
+        BytesOrString::Bytes(b) => {
+            let json_bytes: &[u8] = b.as_ref();
+            python_parse(py, json_bytes, allow_inf_nan, cache_mode, allow_partial)
+                .map_err(|e| map_json_error(json_bytes, &e))
+        }
+    }
 }
 
-pub fn madd(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn madd(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(parse_json_bytes, m)?)?;
     m.add_function(wrap_pyfunction!(parse_json_str, m)?)?;
     m.add_function(wrap_pyfunction!(parse_json, m)?)?;
     Ok(())
 }
```

### Comparing `ry-0.0.3/crates/ryo3/src/sh.rs` & `ry-0.0.5/crates/ryo3/src/sh.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 use dirs;
 use pyo3::exceptions::PyFileNotFoundError;
+use pyo3::prelude::*;
 use pyo3::types::PyModule;
-use pyo3::{pyfunction, wrap_pyfunction, PyResult, Python};
+use pyo3::{pyfunction, wrap_pyfunction, PyResult};
 
 use crate::fs::fspath::PathLike;
 
 #[pyfunction]
 #[must_use]
 pub fn home() -> String {
     dirs::home_dir().unwrap().to_str().unwrap().to_string()
@@ -55,14 +56,14 @@
             let emsg = format!("{}: {:?}", e, p_string);
             let pye = PyFileNotFoundError::new_err(format!("ls: {}", emsg));
             Err(pye)
         }
     }
 }
 
-pub fn madd(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn madd(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(pwd, m)?)?;
     m.add_function(wrap_pyfunction!(cd, m)?)?;
     m.add_function(wrap_pyfunction!(home, m)?)?;
     m.add_function(wrap_pyfunction!(ls, m)?)?;
     Ok(())
 }
```

### Comparing `ry-0.0.3/crates/ryo3/src/sleep.rs` & `ry-0.0.5/crates/ryo3/src/sleep.rs`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,23 @@
     let start = std::time::Instant::now();
     std::thread::sleep(std::time::Duration::from_secs(secs));
     let end = std::time::Instant::now();
     let duration = end - start;
     duration.as_secs_f64()
 }
 
-#[pyfunction]
-pub fn sleep_async(py: Python<'_>, secs: u64) -> PyResult<&PyAny> {
-    pyo3_asyncio::tokio::future_into_py(py, async move {
-        let start = tokio::time::Instant::now();
-        tokio::time::sleep(std::time::Duration::from_secs(secs)).await;
-        let end = tokio::time::Instant::now();
-        let duration = end - start;
-        Ok(Python::with_gil(|_py| duration.as_secs_f64()))
-    })
-}
+// #[pyfunction]
+// pub fn sleep_async(py: Python<'_>, secs: u64) -> PyResult<&PyAny> {
+//     pyo3_asyncio::tokio::future_into_py(py, async move {
+//         let start = tokio::time::Instant::now();
+//         tokio::time::sleep(std::time::Duration::from_secs(secs)).await;
+//         let end = tokio::time::Instant::now();
+//         let duration = end - start;
+//         Ok(Python::with_gil(|_py| duration.as_secs_f64()))
+//     })
+// }
 
-pub fn madd(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn madd(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(sleep, m)?)?;
-    m.add_function(wrap_pyfunction!(sleep_async, m)?)?;
+    // m.add_function(wrap_pyfunction!(sleep_async, m)?)?;
     Ok(())
 }
```

### Comparing `ry-0.0.3/crates/ryo3/src/sp/pydone.rs` & `ry-0.0.5/crates/ryo3/src/sp/pydone.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-use crate::sp::done::Done;
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
 
+use crate::sp::done::Done;
+
 #[pyclass]
 #[derive(Debug)]
 pub struct PyDone {
     done: Done,
 }
 
 #[pymethods]
@@ -21,16 +22,16 @@
         Ok(s)
     }
     fn __str__(&self) -> PyResult<String> {
         self.__repr__()
     }
 
     #[getter]
-    fn stdout<'py>(&'py self, py: Python<'py>) -> &'py PyBytes {
-        PyBytes::new(py, &self.done.stdout)
+    fn stdout<'py>(&'py self, py: Python<'py>) -> Bound<'py, PyBytes> {
+        PyBytes::new_bound(py, &self.done.stdout)
     }
 }
 
 impl From<Done> for PyDone {
     fn from(done: Done) -> Self {
         Self { done }
     }
```

### Comparing `ry-0.0.3/crates/ryo3/src/sp/run.rs` & `ry-0.0.5/crates/ryo3/src/sp/run.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 use std::sync::mpsc;
 use std::thread::{self};
 
 use pyo3::prelude::*;
 use pyo3::pyfunction;
 use pyo3::types::PyTuple;
 use tracing::warn;
-// use serde::{Deserialize, Serialize};
-// use tracing::instrument::WithSubscriber;
 
 use super::done::Done;
 use super::pydone::PyDone;
 
+// use serde::{Deserialize, Serialize};
+// use tracing::instrument::WithSubscriber;
+
 fn communicate_tee<W: Write + Send + 'static>(
     mut stream: impl Read,
     sender: mpsc::Sender<Vec<u8>>,
     mut writer: W,
     buf_size: usize,
     collect: bool,
 ) -> io::Result<()> {
@@ -63,15 +64,15 @@
 
     Ok(())
 }
 
 #[pyfunction]
 #[pyo3(signature = (* popenargs, tee = false, capture = true, timeout = None, check = false))]
 pub fn run(
-    popenargs: &PyTuple,
+    popenargs: &Bound<'_, PyTuple>,
     tee: Option<bool>,
     capture: Option<bool>,
     timeout: Option<u64>,
     check: Option<bool>,
 ) -> PyResult<PyDone> {
     // warn that timeout and check are not implemented
     if timeout.is_some() {
```

### Comparing `ry-0.0.3/crates/ryo3/src/walkdir.rs` & `ry-0.0.5/crates/ryo3/src/walkdir.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #![allow(clippy::too_many_arguments)]
+
 use std::path::Path;
 
 use ::walkdir as walkdir_rs;
 use pyo3::prelude::*;
 
 use crate::fs::fspath::PathLike;
 
@@ -196,15 +197,15 @@
     Ok(PyFspathsGen {
         iter: wd.into_iter(),
         files: files.unwrap_or(true),
         dirs: dirs.unwrap_or(true),
     })
 }
 
-pub fn madd(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn madd(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<PyWalkDirEntry>()?;
     m.add_class::<PyWalkdirGen>()?;
     m.add_class::<PyFspathsGen>()?;
     m.add_function(wrap_pyfunction!(self::walkdir, m)?)?;
     m.add_function(wrap_pyfunction!(self::fspaths, m)?)?;
     Ok(())
 }
```

### Comparing `ry-0.0.3/crates/ryo3/src/which.rs` & `ry-0.0.5/crates/ryo3/src/libs/which.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-use ::which as which_rs;
-use pyo3::prelude::*;
 use std::env;
 use std::ffi::OsString;
 
+use ::which as which_rs;
+use pyo3::prelude::*;
+
 #[pyfunction]
 pub fn which(cmd: &str, path: Option<&str>) -> PyResult<Option<std::path::PathBuf>> {
     match path {
         Some(p) => {
             let which_res = which_rs::which_in(cmd, Some(p), env::current_dir().unwrap());
             match which_res {
                 Ok(p) => Ok(Some(p)),
@@ -39,13 +40,13 @@
 }
 
 #[pyfunction]
 pub fn whicha(cmd: &str, path: Option<&str>) -> PyResult<Vec<String>> {
     which_all(cmd, path)
 }
 
-pub fn madd(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn madd(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(self::which, m)?)?;
     m.add_function(wrap_pyfunction!(self::which_all, m)?)?;
     m.add_function(wrap_pyfunction!(self::whicha, m)?)?;
     Ok(())
 }
```

### Comparing `ry-0.0.3/Cargo.toml` & `ry-0.0.5/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [lib]
 name = "ry"
 crate-type = ["cdylib"]
 
 [dependencies]
 ryo3 = { path = "./crates/ryo3", features = ["all"] }
 pyo3 = { workspace = true, features = ["experimental-inspect"] }
-pyo3-asyncio = {workspace = true, features = ["attributes", "tokio-runtime"] }
+# pyo3-asyncio = {workspace = true, features = ["attributes", "tokio-runtime"] }
 tokio.workspace = true
 tracing.workspace = true
 tracing-subscriber.workspace = true
 serde.workspace = true
 serde_json.workspace = true
 dirs.workspace = true
 thiserror.workspace = true
@@ -34,32 +34,32 @@
 strip = true
 
 [workspace]
 resolver = "2"
 
 [workspace.package]
 edition = "2021"
-version = "0.0.3"
+version = "0.0.5"
 homepage = "https://github.com/jessekrubin/ry-dev"
 documentation = "https://github.com/jessekrubin/ry-dev"
 repository = "https://github.com/jessekrubin/ry-dev"
 authors = ["Jesse K. Rubin <jessekrubin@gmail.com>"]
 license = "MIT OR Apache-2.0"
 
 [workspace.dependencies]
 anyhow = "1.0.75"
-chrono = "0.4.31"
+chrono = "0.4.38"
 dirs = { version = "5.0.1", features = [] }
-pyo3 = {  version = "0.20.0", features = ["experimental-inspect"] }
-pyo3-asyncio = { version = "0.20.0", features = ["attributes", "tokio-runtime"] }
-pyo3-build-config = "0.20.0"
+pyo3 = {  version = "0.21.0", features = ["experimental-inspect"] }
+pyo3-asyncio = { version = "0.21.0", features = ["attributes", "tokio-runtime"] }
+pyo3-build-config = "0.21.0"
 regex = "1.10.3"
 serde = { version = "1.0", features = ["derive"] }
 serde_bytes = "0.11.12"
 serde_json = "1.0.96"
 shlex = "1.3.0"
 thiserror = "1.0.50"
-tokio = { version = "1.33.0", features = ["full"] }
+tokio = { version = "1.37.0", features = ["full"] }
 tracing = "0.1.40"
 tracing-subscriber = { version = "0.3.17", features = ["serde", "serde_json", "env-filter", "default"] }
 walkdir = "2.4.0"
 which = { version = "6.0.0", features = ["regex"] }
```

### Comparing `ry-0.0.3/.editorconfig` & `ry-0.0.5/.editorconfig`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/.gitattributes` & `ry-0.0.5/.gitattributes`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/.github/workflows/ci.yml` & `ry-0.0.5/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,14 @@
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
           manylinux: auto
-      #      - name: Upload wheels
-      #        uses: actions/upload-artifact@v4
-      #        with:
-      #          name: wheels-linux-${{ matrix.target }}
-      #          path: dist
       - name: pytest
         if: ${{ startsWith(matrix.target, 'x86_64') }}
         shell: bash
         run: |
           set -e
           pip install ry --no-index --no-deps --find-links dist --force-reinstall
           pip install -r requirements.dev.txt
@@ -76,15 +71,15 @@
           set -e
           pip install ry --no-index --no-deps --find-links dist --force-reinstall
           pip install -r requirements.dev.txt
           pip install pytest
           pytest
       - name: pytest
         if: ${{ !startsWith(matrix.target, 'x86') && matrix.target != 'ppc64' }}
-        uses: uraimo/run-on-arch-action@v2.7.1
+        uses: uraimo/run-on-arch-action@v2.7.2
         with:
           arch: ${{ matrix.target }}
           distro: ubuntu22.04
           githubToken: ${{ github.token }}
           install: |
             apt-get update
             apt-get install -y --no-install-recommends python3 python3-pip
```

### Comparing `ry-0.0.3/.github/workflows/dev.yml` & `ry-0.0.5/.github/workflows/dev.yml`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,25 @@
   pull_request:
   workflow_dispatch:
 
 permissions:
   contents: read
 
 jobs:
+  check:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v4
+      - uses: taiki-e/install-action@v2
+        with:
+          tool: just
+      - uses: Swatinem/rust-cache@v2
+        if: github.event_name != 'release' && github.event_name != 'workflow_dispatch'
+      - run: just ci
+
   dev-test-linux-x86_64:
     runs-on: ubuntu-latest
     timeout-minutes: 15
     strategy:
       matrix:
         target: [ x86_64 ]
     steps:
@@ -30,15 +41,14 @@
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
-#          manylinux: auto
       - name: pytest
         if: ${{ startsWith(matrix.target, 'x86_64') }}
         shell: bash
         run: |
           set -e
           pip install ry --find-links dist --force-reinstall
           pip install -r requirements.dev.txt
```

### Comparing `ry-0.0.3/.gitignore` & `ry-0.0.5/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -67,7 +67,8 @@
 
 # VSCode
 .vscode/
 
 # Pyenv
 .python-version
 target/ 
+scratch/
```

### Comparing `ry-0.0.3/.pre-commit-config.yaml` & `ry-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/bench/test_build_profile.py` & `ry-0.0.5/bench/test_build_profile.py`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/bench/test_jiter.py` & `ry-0.0.5/bench/test_jiter.py`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/python/ry/__main__.py` & `ry-0.0.5/python/ry/__main__.py`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/scripts/gen.py` & `ry-0.0.5/scripts/gen.py`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/src/lager.rs` & `ry-0.0.5/src/lager.rs`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/src/lib.rs` & `ry-0.0.5/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 const BUILD_TIMESTAMP: &str = env!("BUILD_TIMESTAMP");
 
 /// ry = rust + python
 ///
 /// `ry` is a kitchen-sink of utils and wrappers around popular rust crates
 #[pymodule]
 #[pyo3(name = "_ry")]
-fn ry(py: Python, m: &PyModule) -> PyResult<()> {
+
+fn ry(m: &Bound<'_, PyModule>) -> PyResult<()> {
+    // fn ry(py: Python, m: &PyModule) -> PyResult<()> {
     lager::tracing_init();
     debug!("version: {}", VERSION);
     debug!("build_profile: {}", BUILD_PROFILE);
     debug!("build_timestamp: {}", BUILD_TIMESTAMP);
     m.add("__pkg_name__", PACKAGE)?;
     m.add("__description__", DESCRIPTION)?;
     m.add("__version__", VERSION)?;
     m.add("__build_profile__", BUILD_PROFILE)?;
     m.add("__build_timestamp__", BUILD_TIMESTAMP)?;
     m.add("__authors__", AUTHORS)?;
 
     // register/add core lib from ryo3
-    ryo3::madd(py, m)?;
+    ryo3::madd(m)?;
     Ok(())
 }
```

### Comparing `ry-0.0.3/tests/test_brotli.py` & `ry-0.0.5/tests/test_brotli.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,25 +11,19 @@
     assert decoded == input_data
 
 
 def test_10x10y_round_trip_magic_number() -> None:
     input_data = b"XXXXXXXXXXYYYYYYYYYY"
     output_data_magic_true = ry.brotli_encode(input_data, magic_number=True)
     output_data_magic_false = ry.brotli_encode(input_data, magic_number=False)
-    print(
-        f"output_data_magic_false: {output_data_magic_false}\noutput_data_magic_true: {output_data_magic_true}"
-    )
-    print(
-        f"output_data_magic_false: {len(output_data_magic_false)}\noutput_data_magic_true: {len(output_data_magic_true)}"
-    )
     assert output_data_magic_false is not None and output_data_magic_true is not None
     assert output_data_magic_false != output_data_magic_true
     assert output_data_magic_true is not None
     decoded = ry.brotli_decode(output_data_magic_true)
     assert decoded == input_data
     # ends with
 
 
-def test_decompress():
+def test_decompress() -> None:
     _10x_10y_compressed = b"\x1b\x13\x00\x00\xa4\xb0\xb2\xea\x81G\x02\x8a"
     decoded = ry.brotli_decode(_10x_10y_compressed)
     assert decoded == b"XXXXXXXXXXYYYYYYYYYY"
```

### Comparing `ry-0.0.3/tests/test_fnv.py` & `ry-0.0.5/tests/test_fnv.py`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/tests/test_fs.py` & `ry-0.0.5/tests/test_fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import pytest
 from pathlib import Path
 
+import pytest
+
 import ry
 
 
 def test_read_string(tmp_path: Path) -> None:
     p = tmp_path / "test.txt"
     p.write_text("hello")
     ry.cd(tmp_path)
```

### Comparing `ry-0.0.3/tests/test_fspath.py` & `ry-0.0.5/tests/test_fspath.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Tests for ry.FsPath"""
 
-import ry
 from pathlib import Path
-import pytest
 from typing import Type
 
+import pytest
+
+import ry
+
 
 def test_new_path() -> None:
     pypath = Path()
     rypath = ry.FsPath()
     assert rypath == pypath
 
 
@@ -23,38 +25,37 @@
         pytest.param(
             ry.FsPath,
             id="ry.FsPath",
         ),
     ],
 )
 class TestFsPath:
-
     def test_new_path(self, path_cls: Type[Path]) -> None:
         pypath = Path()
         rypath = path_cls()
         assert rypath == pypath
 
-    def test_parent(self, path_cls: Type[Path]) -> None:
+    def test_parent(self, path_cls: type[Path]) -> None:
         pypath = Path()
         rypath = path_cls()
         assert rypath.parent == pypath.parent
 
-    def test_absolute(self, path_cls: Type[Path]) -> None:
+    def test_absolute(self, path_cls: type[Path]) -> None:
         pypath = Path()
         rypath = path_cls()
         pypath_abs = pypath.absolute()
         rypath_abs = rypath.absolute()
         assert rypath_abs == pypath_abs
 
-    def test_read_text(self, path_cls: Type[Path], tmp_path: Path) -> None:
+    def test_read_text(self, path_cls: type[Path], tmp_path: Path) -> None:
         pypath = tmp_path / "test.txt"
         pypath.write_text("hello")
         rypath = path_cls(pypath)
         assert rypath.read_text() == pypath.read_text()
 
-    def test_read_bytes(self, path_cls: Type[Path], tmp_path: Path) -> None:
+    def test_read_bytes(self, path_cls: type[Path], tmp_path: Path) -> None:
         pypath = tmp_path / "test.txt"
         pypath.write_bytes(b"hello")
         rypath = path_cls(pypath)
         b = rypath.read_bytes()
         assert rypath.read_bytes() == pypath.read_bytes()
         assert rypath.read_bytes() == b
```

### Comparing `ry-0.0.3/tests/test_jiter.py` & `ry-0.0.5/tests/test_jiter.py`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/tests/test_pwd_cd.py` & `ry-0.0.5/tests/test_pwd_cd.py`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/tests/test_run.py` & `ry-0.0.5/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/tests/test_shplit.py` & `ry-0.0.5/tests/test_shplit.py`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/tests/test_version.py` & `ry-0.0.5/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/tests/test_walkdir.py` & `ry-0.0.5/tests/test_walkdir.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import ry
-from pathlib import Path
-
 import json
-
 from dataclasses import dataclass
+from pathlib import Path
+
+import ry
 
 
 @dataclass
 class MkDirTree:
     dirpaths: set[Path]
     filepaths: set[Path]
 
 
-def mk_dir_tree(tmp_path: Path | str) -> MkDirTree:
+def mk_dir_tree(tmp_path: Path) -> MkDirTree:
     tmp_path = Path(tmp_path)
     abcd = tmp_path / "a" / "b" / "c" / "d"
     abcd.mkdir(parents=True)
     efgh = tmp_path / "e" / "f" / "g" / "h"
     efgh.mkdir(parents=True)
     dirpaths = set()
     filepaths = set()
@@ -37,25 +36,24 @@
     tiles_root = tmp_path / "tiles"
     for z, x in dir_parts:
         dirpath = Path(tiles_root / str(z) / str(x))
         dirpath.mkdir(parents=True)
         dirpaths.add(dirpath)
     for x, y, z in tiles_z4:
         tile_file = tiles_root / str(z) / str(x) / f"{y}.json"
-        tile_file.write_text(
-            json.dumps(
-                {
-                    "x": x,
-                    "y": y,
-                    "z": z,
-                }
-            ),
-            encoding="utf-8",
-            newline="\n",
-        )
+        with open(tile_file, "w", encoding="utf-8", newline="\n") as phile:
+            phile.write(
+                json.dumps(
+                    {
+                        "x": x,
+                        "y": y,
+                        "z": z,
+                    }
+                )
+            )
         filepaths.add(tile_file)
     # make some empty dirs
     empty_dirs = [tmp_path / "nada", tmp_path / "nothing-in-here"]
     for d in empty_dirs:
         d.mkdir()
         dirpaths.add(d)
 
@@ -103,8 +101,8 @@
         print(f)
         paths.append(f)
     print(paths)
     # assert False
 
 
 if __name__ == "__main__":
-    mk_dir_tree(".")
+    mk_dir_tree(Path("."))
```

### Comparing `ry-0.0.3/tests/test_which.py` & `ry-0.0.5/tests/test_which.py`

 * *Files identical despite different names*

### Comparing `ry-0.0.3/Cargo.lock` & `ry-0.0.5/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -51,20 +51,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
 dependencies = [
  "alloc-no-stdlib",
 ]
 
 [[package]]
-name = "allocator-api2"
-version = "0.2.16"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
-
-[[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
 name = "android_system_properties"
@@ -106,69 +100,69 @@
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "brotli"
-version = "3.5.0"
+version = "5.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d640d25bc63c50fb1f0b545ffd80207d2e10a4c965530809b40ba3386825c391"
+checksum = "19483b140a7ac7174d34b5a581b406c64f84da5409d3e09cf4fff604f9270e67"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
  "brotli-decompressor",
 ]
 
 [[package]]
 name = "brotli-decompressor"
-version = "2.5.1"
+version = "4.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e2e4afe60d7dd600fdd3de8d0f08c2b7ec039712e3b6137ff98b7004e82de4f"
+checksum = "e6221fe77a248b9117d431ad93761222e1cf8ff282d9d1d5d9f53d6299a1cf76"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.35"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
@@ -192,17 +186,17 @@
  "option-ext",
  "redox_users",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "errno"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
@@ -213,130 +207,31 @@
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
-name = "futures"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
-dependencies = [
- "futures-channel",
- "futures-core",
- "futures-executor",
- "futures-io",
- "futures-sink",
- "futures-task",
- "futures-util",
-]
-
-[[package]]
-name = "futures-channel"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
-dependencies = [
- "futures-core",
- "futures-sink",
-]
-
-[[package]]
-name = "futures-core"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
-
-[[package]]
-name = "futures-executor"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
-dependencies = [
- "futures-core",
- "futures-task",
- "futures-util",
-]
-
-[[package]]
-name = "futures-io"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
-
-[[package]]
-name = "futures-macro"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.55",
-]
-
-[[package]]
-name = "futures-sink"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
-
-[[package]]
-name = "futures-task"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38d84fa142264698cdce1a9f9172cf383a0c82de1bddcf3092901442c4097004"
-
-[[package]]
-name = "futures-util"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
-dependencies = [
- "futures-channel",
- "futures-core",
- "futures-io",
- "futures-macro",
- "futures-sink",
- "futures-task",
- "memchr",
- "pin-project-lite",
- "pin-utils",
- "slab",
-]
-
-[[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
-name = "hashbrown"
-version = "0.14.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
-dependencies = [
- "ahash",
- "allocator-api2",
-]
-
-[[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
@@ -386,21 +281,20 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jiter"
-version = "0.0.6"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87db066a99f69382be06d02313f8ce989996b53a04a8a70cfd1a6483a56227f7"
+checksum = "2c0b7c896d2b1da897be13affb0bbf7bff95437e9c50823ede962addadae58d8"
 dependencies = [
  "ahash",
- "hashbrown",
- "lexical-core",
+ "lexical-parse-float",
  "num-bigint",
  "num-traits",
  "pyo3",
  "smallvec",
 ]
 
 [[package]]
@@ -415,27 +309,14 @@
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
-name = "lexical-core"
-version = "0.8.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2cde5de06e8d4c2faabc400238f9ae1c74d5412d03a7bd067645ccbc47070e46"
-dependencies = [
- "lexical-parse-float",
- "lexical-parse-integer",
- "lexical-util",
- "lexical-write-float",
- "lexical-write-integer",
-]
-
-[[package]]
 name = "lexical-parse-float"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "683b3a5ebd0130b8fb52ba0bdc718cc56815b6a097e28ae5a6997d0ad17dc05f"
 dependencies = [
  "lexical-parse-integer",
  "lexical-util",
@@ -458,49 +339,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5255b9ff16ff898710eb9eb63cb39248ea8a5bb036bea8085b1a767ff6c4e3fc"
 dependencies = [
  "static_assertions",
 ]
 
 [[package]]
-name = "lexical-write-float"
-version = "0.8.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "accabaa1c4581f05a3923d1b4cfd124c329352288b7b9da09e766b0668116862"
-dependencies = [
- "lexical-util",
- "lexical-write-integer",
- "static_assertions",
-]
-
-[[package]]
-name = "lexical-write-integer"
-version = "0.8.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1b6f3d1f4422866b68192d62f77bc5c700bee84f3069f2469d7bc8c77852446"
-dependencies = [
- "lexical-util",
- "static_assertions",
-]
-
-[[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libredox"
-version = "0.0.1"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85c833ca1e66078851dba29046874e38f08b2c883700aa29a03ddd3b23814ee8"
+checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
  "bitflags 2.5.0",
  "libc",
- "redox_syscall",
 ]
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
@@ -528,17 +387,17 @@
 checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
 dependencies = [
  "regex-automata 0.1.10",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
@@ -662,44 +521,38 @@
  "redox_syscall",
  "smallvec",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
-
-[[package]]
-name = "pin-utils"
-version = "0.1.0"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "num-bigint",
  "parking_lot",
@@ -707,88 +560,63 @@
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
-name = "pyo3-asyncio"
-version = "0.20.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea6b68e93db3622f3bb3bf363246cf948ed5375afe7abff98ccbdd50b184995"
-dependencies = [
- "futures",
- "once_cell",
- "pin-project-lite",
- "pyo3",
- "pyo3-asyncio-macros",
- "tokio",
-]
-
-[[package]]
-name = "pyo3-asyncio-macros"
-version = "0.20.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56c467178e1da6252c95c29ecf898b133f742e9181dca5def15dc24e19d45a39"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 1.0.109",
-]
-
-[[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.55",
+ "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.55",
+ "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.4.1"
@@ -796,17 +624,17 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_users"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a18479200779601e498ada4e8c1e1f50e3ee19deb0259c25825a98b5603b2cb4"
+checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
  "libredox",
  "thiserror",
 ]
 
 [[package]]
@@ -870,50 +698,49 @@
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ry"
-version = "0.0.3"
+version = "0.0.5"
 dependencies = [
  "chrono",
  "dirs",
  "pyo3",
- "pyo3-asyncio",
  "pyo3-build-config",
  "ryo3",
  "serde",
  "serde_json",
  "thiserror",
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "ryo3"
-version = "0.0.3"
+version = "0.0.5"
 dependencies = [
  "brotli",
  "chrono",
  "dirs",
  "fnv",
  "jiter",
  "pyo3",
- "pyo3-asyncio",
  "regex",
  "serde",
  "serde_bytes",
  "serde_json",
  "shlex",
  "tokio",
  "tracing",
  "walkdir",
  "which",
+ "xxhash-rust",
 ]
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
@@ -931,17 +758,17 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
 version = "0.11.14"
@@ -949,28 +776,28 @@
 checksum = "8b8497c313fd43ab992087548117643f6fcd935cbf36f176ffda0aacf9591734"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -994,23 +821,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
-name = "slab"
-version = "0.4.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
@@ -1026,28 +844,17 @@
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "syn"
-version = "1.0.109"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
-dependencies = [
- "proc-macro2",
- "quote",
- "unicode-ident",
-]
-
-[[package]]
-name = "syn"
-version = "2.0.55"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1069,32 +876,32 @@
 name = "thiserror-impl"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
@@ -1109,15 +916,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn",
 ]
 
 [[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
@@ -1131,15 +938,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -1236,15 +1043,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1258,15 +1065,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -1319,15 +1126,15 @@
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
@@ -1337,15 +1144,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1357,118 +1164,131 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
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
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winsafe"
 version = "0.0.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d135d17ab770252ad95e9a872d365cf3090e3be864a34ab46f48555993efc904"
 
 [[package]]
+name = "xxhash-rust"
+version = "0.8.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "927da81e25be1e1a2901d59b81b37dd2efd1fc9c9345a55007f09bf5a2d3ee03"
+
+[[package]]
 name = "zerocopy"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
 dependencies = [
  "zerocopy-derive",
 ]
@@ -1477,9 +1297,9 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn",
 ]
```

### Comparing `ry-0.0.3/pyproject.toml` & `ry-0.0.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 [build-system]
 requires = ['maturin>=0.14.16,<2']
 build-backend = "maturin"
 
 [project]
 name = "ry"
-description = "ry = rust + python kitchen sink utils (WIP -- use at your own risk!)"
-requires-python = ">=3.8"
+description = "ry = rust + python kitchen sink utils (WIP)"
+requires-python = ">=3.9"
 authors = [
     { name = 'jesse rubin', email = 'jessekrubin@gmail.com' },
 ]
 maintainers = [
     { name = 'jesse rubin', email = 'jessekrubin@gmail.com' },
 ]
 keywords = [
     "rust",
-    "python",
-    "utils",
+    "pyo3",
 ]
 license = "MIT OR Apache-2.0"
 classifiers = [
+    "Development Status :: 3 - Alpha",
+    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
+    'Programming Language :: Python',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
+    'Programming Language :: Python :: 3 :: Only',
+    "Intended Audience :: Developers",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Development Status :: 3 - Alpha",
+    "Topic :: Utilities",
+    "Typing :: Typed",
+
 ]
 dynamic = ["version", "readme"]
 
 [project.optional-dependencies]
 tests = [
     "pytest",
 ]
@@ -62,46 +75,52 @@
 ]
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
     "bench"
 ]
 
 [tool.black]
-target-version = ["py38"]
+target-version = ["py39"]
 line-length = 88
 
 [tool.ruff]
-target-version = "py38"
+target-version = "py39"
 line-length = 88
 include = [
     "python/**/*.{py,pyi}",
+    "tests/**/*.{py,pyi}",
 ]
 
-[tool.ruff.lint]
+[tool.ruff.format]
+docstring-code-format = true
 
+[tool.ruff.lint]
+# Require explicit selection of preview rules.
+explicit-preview-rules = true
+preview = true
 select = [
     "A",
     "ARG",
     "B",
     "C",
     "DTZ",
     "E",
     "EM",
     "F",
     #  "FBT",
     "I",
     "ICN",
-    "ISC",
     "N",
     "PLC",
     "PLE",
     "PLR",
     "PLW",
     "Q",
     "RUF",
+    "RUF022", # unsorted-dunder-all
     "S",
     "T",
     "TID",
     "UP",
     "W",
     "YTT",
 ]
@@ -185,8 +204,8 @@
 [[tool.mypy.overrides]]
 module = "tests.*"
 ignore_missing_imports = true
 check_untyped_defs = true
 
 [tool.pyright]
 include = ['ry', 'tests']
-reportUnnecessaryTypeIgnoreComment = true
+reportUnnecessaryTypeIgnoreComment = true
```

