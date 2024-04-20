# Comparing `tmp/moyopy-0.1.2.tar.gz` & `tmp/moyopy-0.1.3.tar.gz`

## Comparing `moyopy-0.1.2.tar` & `moyopy-0.1.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0     1001      127      903 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/Cargo.toml
--rw-r--r--   0     1001      127      245 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/README.md
--rw-r--r--   0     1001      127      703 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/benches/dataset.rs
--rw-r--r--   0     1001      127     2493 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/benches/translation_search.rs
--rw-r--r--   0     1001      127     2926 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base/cell.rs
--rw-r--r--   0     1001      127     1123 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base/error.rs
--rw-r--r--   0     1001      127     2932 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base/lattice.rs
--rw-r--r--   0     1001      127     3820 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base/operation.rs
--rw-r--r--   0     1001      127     2146 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base/tolerance.rs
--rw-r--r--   0     1001      127     9891 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base/transformation.rs
--rw-r--r--   0     1001      127      559 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base.rs
--rw-r--r--   0     1001      127     8405 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/arithmetic_crystal_class.rs
--rw-r--r--   0     1001      127     7841 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/classification.rs
--rw-r--r--   0     1001      127    20576 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/hall_symbol.rs
--rw-r--r--   0     1001      127    81241 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/hall_symbol_database.rs
--rw-r--r--   0     1001      127     7762 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/point_group.rs
--rw-r--r--   0     1001      127     3370 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/setting.rs
--rw-r--r--   0     1001      127   201241 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/wyckoff.rs
--rw-r--r--   0     1001      127      740 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data.rs
--rw-r--r--   0     1001      127    19605 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/identify/point_group.rs
--rw-r--r--   0     1001      127    13483 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/identify/space_group.rs
--rw-r--r--   0     1001      127       68 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/identify.rs
--rw-r--r--   0     1001      127     8765 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/lib.rs
--rw-r--r--   0     1001      127      901 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/cycle_checker.rs
--rw-r--r--   0     1001      127     5124 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/delaunay.rs
--rw-r--r--   0     1001      127     2284 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/elementary.rs
--rw-r--r--   0     1001      127     3797 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/hnf.rs
--rw-r--r--   0     1001      127     2440 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/integer_system.rs
--rw-r--r--   0     1001      127     7889 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/minkowski.rs
--rw-r--r--   0     1001      127    14588 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/niggli.rs
--rw-r--r--   0     1001      127     4889 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/snf.rs
--rw-r--r--   0     1001      127      344 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math.rs
--rw-r--r--   0     1001      127    11991 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/search/primitive_cell.rs
--rw-r--r--   0     1001      127    12095 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/search/solve.rs
--rw-r--r--   0     1001      127    12714 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/search/symmetry_search.rs
--rw-r--r--   0     1001      127      250 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/search.rs
--rw-r--r--   0     1001      127    14886 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/symmetrize/standardize.rs
--rw-r--r--   0     1001      127       94 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/symmetrize.rs
--rw-r--r--   0     1001      127     5985 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-1185639.json
--rw-r--r--   0     1001      127     5374 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-1197586.json
--rw-r--r--   0     1001      127     9958 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-1201492.json
--rw-r--r--   0     1001      127      820 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-1221598.json
--rw-r--r--   0     1001      127      735 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-1277787.json
--rw-r--r--   0     1001      127     3820 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-30665.json
--rw-r--r--   0     1001      127     1370 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-550745.json
--rw-r--r--   0     1001      127     5272 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-569901.json
--rw-r--r--   0     1001      127    20173 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/test_moyo_dataset.rs
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 moyopy-0.1.2/moyopy/Cargo.toml
--rw-r--r--   0     1001      127      315 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/README.md
--rw-r--r--   0     1001      127       37 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/python/moyopy/__init__.py
--rw-r--r--   0     1001      127     2504 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/python/moyopy/_moyopy.pyi
--rw-r--r--   0     1001      127        0 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/python/moyopy/py.typed
--rw-r--r--   0     1001      127      623 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/python/tests/conftest.py
--rw-r--r--   0     1001      127      394 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/python/tests/test_moyo_dataset.py
--rw-r--r--   0     1001      127     4934 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/src/base.rs
--rw-r--r--   0     1001      127      704 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/src/data.rs
--rw-r--r--   0     1001      127     4119 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/src/lib.rs
--rw-r--r--   0     1001      127    42754 2024-04-15 03:02:38.000000 moyopy-0.1.2/Cargo.lock
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 moyopy-0.1.2/Cargo.toml
--rw-r--r--   0        0        0     1800 1970-01-01 00:00:00.000000 moyopy-0.1.2/pyproject.toml
--rw-r--r--   0     1001      127     2504 2024-04-15 03:02:38.000000 moyopy-0.1.2/python/moyopy/_moyopy.pyi
--rw-r--r--   0     1001      127       37 2024-04-15 03:02:38.000000 moyopy-0.1.2/python/moyopy/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-15 03:02:38.000000 moyopy-0.1.2/python/moyopy/py.typed
--rw-r--r--   0     1001      127      315 2024-04-15 03:02:38.000000 moyopy-0.1.2/README.md
--rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 moyopy-0.1.2/PKG-INFO
+-rw-r--r--   0     1001      127      903 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/Cargo.toml
+-rw-r--r--   0     1001      127      245 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/README.md
+-rw-r--r--   0     1001      127      703 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/benches/dataset.rs
+-rw-r--r--   0     1001      127     2493 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/benches/translation_search.rs
+-rw-r--r--   0     1001      127     2926 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/base/cell.rs
+-rw-r--r--   0     1001      127     1123 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/base/error.rs
+-rw-r--r--   0     1001      127     2932 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/base/lattice.rs
+-rw-r--r--   0     1001      127     3820 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/base/operation.rs
+-rw-r--r--   0     1001      127     2146 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/base/tolerance.rs
+-rw-r--r--   0     1001      127     9891 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/base/transformation.rs
+-rw-r--r--   0     1001      127      559 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/base.rs
+-rw-r--r--   0     1001      127     8405 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/data/arithmetic_crystal_class.rs
+-rw-r--r--   0     1001      127     7841 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/data/classification.rs
+-rw-r--r--   0     1001      127    20576 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/data/hall_symbol.rs
+-rw-r--r--   0     1001      127    81241 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/data/hall_symbol_database.rs
+-rw-r--r--   0     1001      127     7762 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/data/point_group.rs
+-rw-r--r--   0     1001      127     3370 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/data/setting.rs
+-rw-r--r--   0     1001      127   201241 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/data/wyckoff.rs
+-rw-r--r--   0     1001      127      740 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/data.rs
+-rw-r--r--   0     1001      127    19605 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/identify/point_group.rs
+-rw-r--r--   0     1001      127    13483 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/identify/space_group.rs
+-rw-r--r--   0     1001      127       68 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/identify.rs
+-rw-r--r--   0     1001      127     8765 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/lib.rs
+-rw-r--r--   0     1001      127      901 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/math/cycle_checker.rs
+-rw-r--r--   0     1001      127     5124 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/math/delaunay.rs
+-rw-r--r--   0     1001      127     2284 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/math/elementary.rs
+-rw-r--r--   0     1001      127     4148 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/math/hnf.rs
+-rw-r--r--   0     1001      127     2440 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/math/integer_system.rs
+-rw-r--r--   0     1001      127     7889 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/math/minkowski.rs
+-rw-r--r--   0     1001      127    14588 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/math/niggli.rs
+-rw-r--r--   0     1001      127     4889 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/math/snf.rs
+-rw-r--r--   0     1001      127      344 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/math.rs
+-rw-r--r--   0     1001      127    11991 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/search/primitive_cell.rs
+-rw-r--r--   0     1001      127    12095 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/search/solve.rs
+-rw-r--r--   0     1001      127    12714 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/search/symmetry_search.rs
+-rw-r--r--   0     1001      127      250 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/search.rs
+-rw-r--r--   0     1001      127    14886 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/symmetrize/standardize.rs
+-rw-r--r--   0     1001      127       94 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/src/symmetrize.rs
+-rw-r--r--   0     1001      127     5985 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/tests/assets/mp-1185639.json
+-rw-r--r--   0     1001      127     5374 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/tests/assets/mp-1197586.json
+-rw-r--r--   0     1001      127     9958 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/tests/assets/mp-1201492.json
+-rw-r--r--   0     1001      127      820 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/tests/assets/mp-1221598.json
+-rw-r--r--   0     1001      127      735 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/tests/assets/mp-1277787.json
+-rw-r--r--   0     1001      127     3820 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/tests/assets/mp-30665.json
+-rw-r--r--   0     1001      127     1370 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/tests/assets/mp-550745.json
+-rw-r--r--   0     1001      127     5272 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/tests/assets/mp-569901.json
+-rw-r--r--   0     1001      127    20173 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyo/tests/test_moyo_dataset.rs
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 moyopy-0.1.3/moyopy/Cargo.toml
+-rw-r--r--   0     1001      127      315 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyopy/README.md
+-rw-r--r--   0     1001      127       37 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyopy/python/moyopy/__init__.py
+-rw-r--r--   0     1001      127     2504 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyopy/python/moyopy/_moyopy.pyi
+-rw-r--r--   0     1001      127        0 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyopy/python/moyopy/py.typed
+-rw-r--r--   0     1001      127      623 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyopy/python/tests/conftest.py
+-rw-r--r--   0     1001      127      394 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyopy/python/tests/test_moyo_dataset.py
+-rw-r--r--   0     1001      127     4934 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyopy/src/base.rs
+-rw-r--r--   0     1001      127      704 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyopy/src/data.rs
+-rw-r--r--   0     1001      127     4119 2024-04-20 13:06:49.000000 moyopy-0.1.3/moyopy/src/lib.rs
+-rw-r--r--   0     1001      127    42754 2024-04-20 13:06:49.000000 moyopy-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 moyopy-0.1.3/Cargo.toml
+-rw-r--r--   0        0        0     1800 1970-01-01 00:00:00.000000 moyopy-0.1.3/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-04-20 13:06:49.000000 moyopy-0.1.3/python/moyopy/py.typed
+-rw-r--r--   0     1001      127       37 2024-04-20 13:06:49.000000 moyopy-0.1.3/python/moyopy/__init__.py
+-rw-r--r--   0     1001      127     2504 2024-04-20 13:06:49.000000 moyopy-0.1.3/python/moyopy/_moyopy.pyi
+-rw-r--r--   0     1001      127      315 2024-04-20 13:06:49.000000 moyopy-0.1.3/README.md
+-rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 moyopy-0.1.3/PKG-INFO
```

### Comparing `moyopy-0.1.2/moyo/Cargo.toml` & `moyopy-0.1.3/moyo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/benches/dataset.rs` & `moyopy-0.1.3/moyo/benches/dataset.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/benches/translation_search.rs` & `moyopy-0.1.3/moyo/benches/translation_search.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/base/cell.rs` & `moyopy-0.1.3/moyo/src/base/cell.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/base/error.rs` & `moyopy-0.1.3/moyo/src/base/error.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/base/lattice.rs` & `moyopy-0.1.3/moyo/src/base/lattice.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/base/operation.rs` & `moyopy-0.1.3/moyo/src/base/operation.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/base/tolerance.rs` & `moyopy-0.1.3/moyo/src/base/tolerance.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/base/transformation.rs` & `moyopy-0.1.3/moyo/src/base/transformation.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/base.rs` & `moyopy-0.1.3/moyo/src/base.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/data/arithmetic_crystal_class.rs` & `moyopy-0.1.3/moyo/src/data/arithmetic_crystal_class.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/data/classification.rs` & `moyopy-0.1.3/moyo/src/data/classification.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/data/hall_symbol.rs` & `moyopy-0.1.3/moyo/src/data/hall_symbol.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/data/hall_symbol_database.rs` & `moyopy-0.1.3/moyo/src/data/hall_symbol_database.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/data/point_group.rs` & `moyopy-0.1.3/moyo/src/data/point_group.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/data/setting.rs` & `moyopy-0.1.3/moyo/src/data/setting.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/data/wyckoff.rs` & `moyopy-0.1.3/moyo/src/data/wyckoff.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/data.rs` & `moyopy-0.1.3/moyo/src/data.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/identify/point_group.rs` & `moyopy-0.1.3/moyo/src/identify/point_group.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/identify/space_group.rs` & `moyopy-0.1.3/moyo/src/identify/space_group.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/lib.rs` & `moyopy-0.1.3/moyo/src/lib.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/math/cycle_checker.rs` & `moyopy-0.1.3/moyo/src/math/cycle_checker.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/math/delaunay.rs` & `moyopy-0.1.3/moyo/src/math/delaunay.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/math/elementary.rs` & `moyopy-0.1.3/moyo/src/math/elementary.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/math/hnf.rs` & `moyopy-0.1.3/moyo/src/math/hnf.rs`

 * *Files 7% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
                 // Add the `s`th column to the other columns
                 let mut update = false;
                 for j in 0..n.value() {
                     if j == s {
                         continue;
                     }
-                    let k = h[(s, j)] / h[(s, s)];
+                    let k = h[(s, j)].div_euclid(h[(s, s)]);
 
                     if k != 0 {
                         update = true;
                         // h[(:, j)] -= k * h[(:, s)]
                         for i in 0..m.value() {
                             h[(i, j)] -= k * h[(i, s)];
                         }
@@ -88,14 +88,28 @@
 
     use super::HNF;
 
     #[test]
     fn test_hnf_small() {
         {
             let m = matrix![
+                -1, 0, 0;
+                1, 2, 2;
+                0, -1, -2;
+            ];
+            let hnf = HNF::new(&m);
+            let expect = matrix![
+                1, 0, 0;
+                1, 2, 0;
+                0, 0, 1;
+            ];
+            assert_eq!(hnf.h, expect);
+        }
+        {
+            let m = matrix![
                 20, -6;
                 -2, 1;
             ];
             let hnf = HNF::new(&m);
             assert_eq!(hnf.h, matrix![2, 0; 1, 4]);
         }
         {
```

### Comparing `moyopy-0.1.2/moyo/src/math/integer_system.rs` & `moyopy-0.1.3/moyo/src/math/integer_system.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/math/minkowski.rs` & `moyopy-0.1.3/moyo/src/math/minkowski.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/math/niggli.rs` & `moyopy-0.1.3/moyo/src/math/niggli.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/math/snf.rs` & `moyopy-0.1.3/moyo/src/math/snf.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/search/primitive_cell.rs` & `moyopy-0.1.3/moyo/src/search/primitive_cell.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/search/solve.rs` & `moyopy-0.1.3/moyo/src/search/solve.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/search/symmetry_search.rs` & `moyopy-0.1.3/moyo/src/search/symmetry_search.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/src/symmetrize/standardize.rs` & `moyopy-0.1.3/moyo/src/symmetrize/standardize.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/tests/assets/mp-1185639.json` & `moyopy-0.1.3/moyo/tests/assets/mp-1185639.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/tests/assets/mp-1197586.json` & `moyopy-0.1.3/moyo/tests/assets/mp-1197586.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/tests/assets/mp-1201492.json` & `moyopy-0.1.3/moyo/tests/assets/mp-1201492.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/tests/assets/mp-1221598.json` & `moyopy-0.1.3/moyo/tests/assets/mp-1221598.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/tests/assets/mp-1277787.json` & `moyopy-0.1.3/moyo/tests/assets/mp-1277787.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/tests/assets/mp-30665.json` & `moyopy-0.1.3/moyo/tests/assets/mp-30665.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/tests/assets/mp-550745.json` & `moyopy-0.1.3/moyo/tests/assets/mp-550745.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/tests/assets/mp-569901.json` & `moyopy-0.1.3/moyo/tests/assets/mp-569901.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyo/tests/test_moyo_dataset.rs` & `moyopy-0.1.3/moyo/tests/test_moyo_dataset.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyopy/Cargo.toml` & `moyopy-0.1.3/moyopy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyopy/python/moyopy/_moyopy.pyi` & `moyopy-0.1.3/moyopy/python/moyopy/_moyopy.pyi`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyopy/python/tests/conftest.py` & `moyopy-0.1.3/moyopy/python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyopy/src/base.rs` & `moyopy-0.1.3/moyopy/src/base.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyopy/src/data.rs` & `moyopy-0.1.3/moyopy/src/data.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/moyopy/src/lib.rs` & `moyopy-0.1.3/moyopy/src/lib.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/Cargo.lock` & `moyopy-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -614,15 +614,15 @@
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "moyo"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "approx",
  "criterion",
  "env_logger",
  "itertools 0.11.0",
  "kiddo",
  "log",
@@ -636,15 +636,15 @@
  "test-log",
  "thiserror",
  "union-find",
 ]
 
 [[package]]
 name = "moyopy"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "approx",
  "moyo",
  "nalgebra",
  "pyo3",
  "serde",
  "serde_json",
```

### Comparing `moyopy-0.1.2/Cargo.toml` & `moyopy-0.1.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 resolver = "2"
 
 [workspace.package]
 authors = ["Kohei Shinohara <kshinohara0508@gmail.com>"]
 description = "Library for Crystal Symmetry in Rust"
 edition = "2021"
-version = "0.1.2"
+version = "0.1.3"
 license = "MIT OR Apache-2.0"
 repository = "https://github.com/spglib/moyo"
 
 [workspace.dependencies]
 nalgebra = { version = "0.32.3", features = ["serde-serialize"] }
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
```

### Comparing `moyopy-0.1.2/pyproject.toml` & `moyopy-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/python/moyopy/_moyopy.pyi` & `moyopy-0.1.3/python/moyopy/_moyopy.pyi`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.2/PKG-INFO` & `moyopy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: moyopy
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

