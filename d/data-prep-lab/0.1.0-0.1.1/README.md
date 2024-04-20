# Comparing `tmp/data_prep_lab-0.1.0.tar.gz` & `tmp/data_prep_lab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_lab-0.1.0.tar", last modified: Thu Apr 18 09:53:35 2024, max compression
+gzip compressed data, was "data_prep_lab-0.1.1.tar", last modified: Sat Apr 20 16:30:50 2024, max compression
```

## Comparing `data_prep_lab-0.1.0.tar` & `data_prep_lab-0.1.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.694190 data_prep_lab-0.1.0/
--rw-r--r--   0 boris      (501) staff       (20)      357 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/.gitignore
--rw-r--r--   0 boris      (501) staff       (20)     2229 2024-04-18 09:49:32.000000 data_prep_lab-0.1.0/Makefile
--rw-r--r--   0 boris      (501) staff       (20)     1849 2024-04-18 09:53:35.693546 data_prep_lab-0.1.0/PKG-INFO
--rw-r--r--   0 boris      (501) staff       (20)      963 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/README.md
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.647206 data_prep_lab-0.1.0/doc/
--rw-r--r--   0 boris      (501) staff       (20)    12755 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/doc/advanced-transform-tutorial.md
--rw-r--r--   0 boris      (501) staff       (20)     7617 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/doc/architecture.md
--rw-r--r--   0 boris      (501) staff       (20)     4919 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/doc/launcher-options.md
--rw-r--r--   0 boris      (501) staff       (20)     1778 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/doc/library-config.md
--rw-r--r--   0 boris      (501) staff       (20)     1609 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/doc/overview.md
--rw-r--r--   0 boris      (501) staff       (20)   137580 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/doc/processing-architecture.jpg
--rw-r--r--   0 boris      (501) staff       (20)     8708 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/doc/simplest-transform-tutorial.md
--rw-r--r--   0 boris      (501) staff       (20)      193 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/doc/testing-e2e-transform.md
--rw-r--r--   0 boris      (501) staff       (20)     5912 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/doc/testing-transforms.md
--rw-r--r--   0 boris      (501) staff       (20)    12175 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/doc/transform-external-resources.md
--rw-r--r--   0 boris      (501) staff       (20)     3666 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/doc/transform-porting.md
--rw-r--r--   0 boris      (501) staff       (20)    10818 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/doc/transform-tutorials.md
--rw-r--r--   0 boris      (501) staff       (20)     1415 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/doc/transformer-utilities.md
--rw-r--r--   0 boris      (501) staff       (20)     3481 2024-04-18 07:18:23.000000 data_prep_lab-0.1.0/doc/using_s3_transformers.md
--rw-r--r--   0 boris      (501) staff       (20)     1357 2024-04-18 09:52:03.000000 data_prep_lab-0.1.0/pyproject.toml
--rw-r--r--   0 boris      (501) staff       (20)       38 2024-04-18 09:53:35.694322 data_prep_lab-0.1.0/setup.cfg
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.624230 data_prep_lab-0.1.0/src/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.690771 data_prep_lab-0.1.0/src/data_prep_lab.egg-info/
--rw-r--r--   0 boris      (501) staff       (20)     1849 2024-04-18 09:53:35.000000 data_prep_lab-0.1.0/src/data_prep_lab.egg-info/PKG-INFO
--rw-r--r--   0 boris      (501) staff       (20)     3063 2024-04-18 09:53:35.000000 data_prep_lab-0.1.0/src/data_prep_lab.egg-info/SOURCES.txt
--rw-r--r--   0 boris      (501) staff       (20)        1 2024-04-18 09:53:35.000000 data_prep_lab-0.1.0/src/data_prep_lab.egg-info/dependency_links.txt
--rw-r--r--   0 boris      (501) staff       (20)      234 2024-04-18 09:53:35.000000 data_prep_lab-0.1.0/src/data_prep_lab.egg-info/requires.txt
--rw-r--r--   0 boris      (501) staff       (20)       16 2024-04-18 09:53:35.000000 data_prep_lab-0.1.0/src/data_prep_lab.egg-info/top_level.txt
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.650662 data_prep_lab-0.1.0/src/data_processing/
--rw-r--r--   0 boris      (501) staff       (20)        0 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/__init__.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.656526 data_prep_lab-0.1.0/src/data_processing/data_access/
--rw-r--r--   0 boris      (501) staff       (20)      427 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/data_access/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     8830 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/data_access/arrow_s3.py
--rw-r--r--   0 boris      (501) staff       (20)     8484 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/data_access/data_access.py
--rw-r--r--   0 boris      (501) staff       (20)    11302 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/data_access/data_access_factory.py
--rw-r--r--   0 boris      (501) staff       (20)     5647 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/data_access/data_access_factory_base.py
--rw-r--r--   0 boris      (501) staff       (20)    15024 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/data_access/data_access_local.py
--rw-r--r--   0 boris      (501) staff       (20)    13499 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/data_access/data_access_s3.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.662401 data_prep_lab-0.1.0/src/data_processing/ray/
--rw-r--r--   0 boris      (501) staff       (20)      574 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/ray/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     7404 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/ray/ray_utils.py
--rw-r--r--   0 boris      (501) staff       (20)     4760 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/ray/transform_launcher.py
--rw-r--r--   0 boris      (501) staff       (20)     6380 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/ray/transform_orchestrator.py
--rw-r--r--   0 boris      (501) staff       (20)     4981 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/ray/transform_orchestrator_configuration.py
--rw-r--r--   0 boris      (501) staff       (20)     7253 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/ray/transform_runtime.py
--rw-r--r--   0 boris      (501) staff       (20)     3073 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/ray/transform_statistics.py
--rw-r--r--   0 boris      (501) staff       (20)     9498 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/ray/transform_table_processor.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.663844 data_prep_lab-0.1.0/src/data_processing/test_support/
--rw-r--r--   0 boris      (501) staff       (20)       62 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/test_support/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     8234 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/test_support/abstract_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.665479 data_prep_lab-0.1.0/src/data_processing/test_support/ray/
--rw-r--r--   0 boris      (501) staff       (20)       58 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/test_support/ray/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     4686 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/test_support/ray/transform_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.667784 data_prep_lab-0.1.0/src/data_processing/test_support/transform/
--rw-r--r--   0 boris      (501) staff       (20)      120 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/test_support/transform/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     4050 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/test_support/transform/noop_transform.py
--rw-r--r--   0 boris      (501) staff       (20)     4476 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/test_support/transform/transform_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.669143 data_prep_lab-0.1.0/src/data_processing/transform/
--rw-r--r--   0 boris      (501) staff       (20)       77 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/transform/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     2298 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/transform/table_transform.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.672939 data_prep_lab-0.1.0/src/data_processing/utils/
--rw-r--r--   0 boris      (501) staff       (20)      354 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/utils/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     3135 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/utils/cli_utils.py
--rw-r--r--   0 boris      (501) staff       (20)     1694 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/utils/config.py
--rw-r--r--   0 boris      (501) staff       (20)     2052 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/utils/log.py
--rw-r--r--   0 boris      (501) staff       (20)     5738 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/utils/params_utils.py
--rw-r--r--   0 boris      (501) staff       (20)     6740 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/src/data_processing/utils/transform_utils.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.629170 data_prep_lab-0.1.0/test/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.630413 data_prep_lab-0.1.0/test/data_processing_tests/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.685362 data_prep_lab-0.1.0/test/data_processing_tests/data_access/
--rw-r--r--   0 boris      (501) staff       (20)    24548 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test/data_processing_tests/data_access/data_access_local_test.py
--rw-r--r--   0 boris      (501) staff       (20)     5734 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test/data_processing_tests/data_access/data_access_s3_test.py
--rw-r--r--   0 boris      (501) staff       (20)     1579 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test/data_processing_tests/data_access/sample_input_data_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.688480 data_prep_lab-0.1.0/test/data_processing_tests/ray/
--rw-r--r--   0 boris      (501) staff       (20)     9659 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test/data_processing_tests/ray/launcher_test.py
--rw-r--r--   0 boris      (501) staff       (20)     3282 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test/data_processing_tests/ray/ray_util_test.py
--rw-r--r--   0 boris      (501) staff       (20)     1685 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test/data_processing_tests/ray/test_noop_launch.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.689083 data_prep_lab-0.1.0/test/data_processing_tests/transform/
--rw-r--r--   0 boris      (501) staff       (20)     1678 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test/data_processing_tests/transform/test_noop.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.689681 data_prep_lab-0.1.0/test/data_processing_tests/util/
--rw-r--r--   0 boris      (501) staff       (20)     1386 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test/data_processing_tests/util/transform_utils_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.626487 data_prep_lab-0.1.0/test-data/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.627154 data_prep_lab-0.1.0/test-data/data_processing/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.673699 data_prep_lab-0.1.0/test-data/data_processing/input/
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test-data/data_processing/input/sample1.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.677402 data_prep_lab-0.1.0/test-data/data_processing/input_multiple/
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test-data/data_processing/input_multiple/sample1.parquet
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test-data/data_processing/input_multiple/sample2.parquet
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test-data/data_processing/input_multiple/sample3.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.627397 data_prep_lab-0.1.0/test-data/data_processing/ray/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.628217 data_prep_lab-0.1.0/test-data/data_processing/ray/noop/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.679625 data_prep_lab-0.1.0/test-data/data_processing/ray/noop/expected/
--rw-r--r--   0 boris      (501) staff       (20)     1128 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test-data/data_processing/ray/noop/expected/metadata.json
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test-data/data_processing/ray/noop/expected/sample1.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.680686 data_prep_lab-0.1.0/test-data/data_processing/ray/noop/expected/subdir/
--rw-r--r--   0 boris      (501) staff       (20)      753 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test-data/data_processing/ray/noop/expected/subdir/test1.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.681500 data_prep_lab-0.1.0/test-data/data_processing/ray/noop/input/
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test-data/data_processing/ray/noop/input/sample1.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-18 09:53:35.682547 data_prep_lab-0.1.0/test-data/data_processing/ray/noop/input/subdir/
--rw-r--r--   0 boris      (501) staff       (20)      753 2024-04-17 17:15:46.000000 data_prep_lab-0.1.0/test-data/data_processing/ray/noop/input/subdir/test1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.647600 data_prep_lab-0.1.1/
+-rw-r--r--   0 boris      (501) staff       (20)      357 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/.gitignore
+-rw-r--r--   0 boris      (501) staff       (20)     2290 2024-04-20 16:17:44.000000 data_prep_lab-0.1.1/Makefile
+-rw-r--r--   0 boris      (501) staff       (20)     1849 2024-04-20 16:30:50.647140 data_prep_lab-0.1.1/PKG-INFO
+-rw-r--r--   0 boris      (501) staff       (20)      963 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/README.md
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.611706 data_prep_lab-0.1.1/doc/
+-rw-r--r--   0 boris      (501) staff       (20)    12755 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/advanced-transform-tutorial.md
+-rw-r--r--   0 boris      (501) staff       (20)     7617 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/architecture.md
+-rw-r--r--   0 boris      (501) staff       (20)     4940 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/launcher-options.md
+-rw-r--r--   0 boris      (501) staff       (20)     1778 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/library-config.md
+-rw-r--r--   0 boris      (501) staff       (20)     1607 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/overview.md
+-rw-r--r--   0 boris      (501) staff       (20)   137580 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/processing-architecture.jpg
+-rw-r--r--   0 boris      (501) staff       (20)     8708 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/simplest-transform-tutorial.md
+-rw-r--r--   0 boris      (501) staff       (20)      193 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/testing-e2e-transform.md
+-rw-r--r--   0 boris      (501) staff       (20)     5912 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/testing-transforms.md
+-rw-r--r--   0 boris      (501) staff       (20)    12175 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/transform-external-resources.md
+-rw-r--r--   0 boris      (501) staff       (20)     3666 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/transform-porting.md
+-rw-r--r--   0 boris      (501) staff       (20)    10818 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/transform-tutorials.md
+-rw-r--r--   0 boris      (501) staff       (20)     1415 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/transformer-utilities.md
+-rw-r--r--   0 boris      (501) staff       (20)     3570 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/doc/using_s3_transformers.md
+-rw-r--r--   0 boris      (501) staff       (20)     1357 2024-04-20 16:30:28.000000 data_prep_lab-0.1.1/pyproject.toml
+-rw-r--r--   0 boris      (501) staff       (20)       38 2024-04-20 16:30:50.647697 data_prep_lab-0.1.1/setup.cfg
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.593289 data_prep_lab-0.1.1/src/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.644735 data_prep_lab-0.1.1/src/data_prep_lab.egg-info/
+-rw-r--r--   0 boris      (501) staff       (20)     1849 2024-04-20 16:30:50.000000 data_prep_lab-0.1.1/src/data_prep_lab.egg-info/PKG-INFO
+-rw-r--r--   0 boris      (501) staff       (20)     3063 2024-04-20 16:30:50.000000 data_prep_lab-0.1.1/src/data_prep_lab.egg-info/SOURCES.txt
+-rw-r--r--   0 boris      (501) staff       (20)        1 2024-04-20 16:30:50.000000 data_prep_lab-0.1.1/src/data_prep_lab.egg-info/dependency_links.txt
+-rw-r--r--   0 boris      (501) staff       (20)      234 2024-04-20 16:30:50.000000 data_prep_lab-0.1.1/src/data_prep_lab.egg-info/requires.txt
+-rw-r--r--   0 boris      (501) staff       (20)       16 2024-04-20 16:30:50.000000 data_prep_lab-0.1.1/src/data_prep_lab.egg-info/top_level.txt
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.614843 data_prep_lab-0.1.1/src/data_processing/
+-rw-r--r--   0 boris      (501) staff       (20)        0 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/__init__.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.619222 data_prep_lab-0.1.1/src/data_processing/data_access/
+-rw-r--r--   0 boris      (501) staff       (20)      427 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/data_access/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     8830 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/data_access/arrow_s3.py
+-rw-r--r--   0 boris      (501) staff       (20)     8484 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/data_access/data_access.py
+-rw-r--r--   0 boris      (501) staff       (20)    11316 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/data_access/data_access_factory.py
+-rw-r--r--   0 boris      (501) staff       (20)     5647 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/data_access/data_access_factory_base.py
+-rw-r--r--   0 boris      (501) staff       (20)    15024 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/data_access/data_access_local.py
+-rw-r--r--   0 boris      (501) staff       (20)    13499 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/data_access/data_access_s3.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.625152 data_prep_lab-0.1.1/src/data_processing/ray/
+-rw-r--r--   0 boris      (501) staff       (20)      574 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/ray/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     7404 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/ray/ray_utils.py
+-rw-r--r--   0 boris      (501) staff       (20)     4760 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/ray/transform_launcher.py
+-rw-r--r--   0 boris      (501) staff       (20)     6380 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/ray/transform_orchestrator.py
+-rw-r--r--   0 boris      (501) staff       (20)     4981 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/ray/transform_orchestrator_configuration.py
+-rw-r--r--   0 boris      (501) staff       (20)     7253 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/ray/transform_runtime.py
+-rw-r--r--   0 boris      (501) staff       (20)     3073 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/ray/transform_statistics.py
+-rw-r--r--   0 boris      (501) staff       (20)     9498 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/ray/transform_table_processor.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.626321 data_prep_lab-0.1.1/src/data_processing/test_support/
+-rw-r--r--   0 boris      (501) staff       (20)       62 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/test_support/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     8234 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/test_support/abstract_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.627535 data_prep_lab-0.1.1/src/data_processing/test_support/ray/
+-rw-r--r--   0 boris      (501) staff       (20)       58 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/test_support/ray/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     4686 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/test_support/ray/transform_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.629094 data_prep_lab-0.1.1/src/data_processing/test_support/transform/
+-rw-r--r--   0 boris      (501) staff       (20)      120 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/test_support/transform/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     4050 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/test_support/transform/noop_transform.py
+-rw-r--r--   0 boris      (501) staff       (20)     4476 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/test_support/transform/transform_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.630426 data_prep_lab-0.1.1/src/data_processing/transform/
+-rw-r--r--   0 boris      (501) staff       (20)       77 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/transform/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     2298 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/transform/table_transform.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.633585 data_prep_lab-0.1.1/src/data_processing/utils/
+-rw-r--r--   0 boris      (501) staff       (20)      354 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/utils/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     3135 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/utils/cli_utils.py
+-rw-r--r--   0 boris      (501) staff       (20)     1695 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/utils/config.py
+-rw-r--r--   0 boris      (501) staff       (20)     2052 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/utils/log.py
+-rw-r--r--   0 boris      (501) staff       (20)     6029 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/utils/params_utils.py
+-rw-r--r--   0 boris      (501) staff       (20)     6740 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/src/data_processing/utils/transform_utils.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.597819 data_prep_lab-0.1.1/test/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.598580 data_prep_lab-0.1.1/test/data_processing_tests/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.641087 data_prep_lab-0.1.1/test/data_processing_tests/data_access/
+-rw-r--r--   0 boris      (501) staff       (20)    24548 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test/data_processing_tests/data_access/data_access_local_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     5734 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test/data_processing_tests/data_access/data_access_s3_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     1545 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test/data_processing_tests/data_access/sample_input_data_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.642633 data_prep_lab-0.1.1/test/data_processing_tests/ray/
+-rw-r--r--   0 boris      (501) staff       (20)     9659 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test/data_processing_tests/ray/launcher_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     3282 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test/data_processing_tests/ray/ray_util_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     1685 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test/data_processing_tests/ray/test_noop_launch.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.643113 data_prep_lab-0.1.1/test/data_processing_tests/transform/
+-rw-r--r--   0 boris      (501) staff       (20)     1678 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test/data_processing_tests/transform/test_noop.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.643434 data_prep_lab-0.1.1/test/data_processing_tests/util/
+-rw-r--r--   0 boris      (501) staff       (20)     1386 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test/data_processing_tests/util/transform_utils_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.595799 data_prep_lab-0.1.1/test-data/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.596323 data_prep_lab-0.1.1/test-data/data_processing/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.633985 data_prep_lab-0.1.1/test-data/data_processing/input/
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test-data/data_processing/input/sample1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.635997 data_prep_lab-0.1.1/test-data/data_processing/input_multiple/
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test-data/data_processing/input_multiple/sample1.parquet
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test-data/data_processing/input_multiple/sample2.parquet
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test-data/data_processing/input_multiple/sample3.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.596468 data_prep_lab-0.1.1/test-data/data_processing/ray/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.597300 data_prep_lab-0.1.1/test-data/data_processing/ray/noop/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.637516 data_prep_lab-0.1.1/test-data/data_processing/ray/noop/expected/
+-rw-r--r--   0 boris      (501) staff       (20)     1128 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test-data/data_processing/ray/noop/expected/metadata.json
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test-data/data_processing/ray/noop/expected/sample1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.638254 data_prep_lab-0.1.1/test-data/data_processing/ray/noop/expected/subdir/
+-rw-r--r--   0 boris      (501) staff       (20)      753 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test-data/data_processing/ray/noop/expected/subdir/test1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.638612 data_prep_lab-0.1.1/test-data/data_processing/ray/noop/input/
+-rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test-data/data_processing/ray/noop/input/sample1.parquet
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-20 16:30:50.639407 data_prep_lab-0.1.1/test-data/data_processing/ray/noop/input/subdir/
+-rw-r--r--   0 boris      (501) staff       (20)      753 2024-04-20 08:49:10.000000 data_prep_lab-0.1.1/test-data/data_processing/ray/noop/input/subdir/test1.parquet
```

### Comparing `data_prep_lab-0.1.0/Makefile` & `data_prep_lab-0.1.1/Makefile`

 * *Files 11% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 	${PYTHON} -m twine upload --verbose --non-interactive dist/*
 	#@echo "create a git tag to reference published version"
 	#@git tag ${TAG}
 	#@git push origin ${TAG}
 
 venv::	pyproject.toml
 	@# Help: Create the virtual environment using pyproject.toml 
-	rm -rf venv	
+	rm -r dist venv || true
+	rm -rf src/*egg-info || true
+	rm makeenv || true
 	$(PYTHON) -m venv venv
 	source venv/bin/activate; 	\
 	pip install --upgrade pip;	\
 	pip install -e .;		\
 	pip install pytest pytest-cov moto==5.0.5
```

### Comparing `data_prep_lab-0.1.0/PKG-INFO` & `data_prep_lab-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: data_prep_lab
-Version: 0.1.0
+Version: 0.1.1
 Summary: Data Preparation Laboratory Library
 Author-email: David Wood <dawood@us.ibm.com>, Boris Lublinsky <blublinsky@ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ray[default]==2.9.3
-Requires-Dist: pyarrow==14.0.2
-Requires-Dist: boto3==1.28.60
+Requires-Dist: pyarrow==15.0.2
+Requires-Dist: boto3==1.34.88
 Requires-Dist: urllib3>=1.26.18
 Requires-Dist: argparse
 Requires-Dist: mmh3
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest>=7.3.2; extra == "dev"
 Requires-Dist: pytest-dotenv>=0.5.2; extra == "dev"
```

### Comparing `data_prep_lab-0.1.0/README.md` & `data_prep_lab-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/doc/advanced-transform-tutorial.md` & `data_prep_lab-0.1.1/doc/advanced-transform-tutorial.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/doc/architecture.md` & `data_prep_lab-0.1.1/doc/architecture.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/doc/launcher-options.md` & `data_prep_lab-0.1.1/doc/launcher-options.md`

 * *Files 7% similar despite different names*

```diff
@@ -35,17 +35,17 @@
                         AST string of options for cos credentials. Only required for COS or Lakehouse.
                         access_key: access key help text
                         secret_key: secret key help text
                         cos_url: COS url
                         Example: { 'access_key': 'access', 'secret_key': 'secret', 's3_url': 'https://s3.us-east.cloud-object-storage.appdomain.cloud' }
   --data_s3_config S3_CONFIG
                         AST string containing input/output paths.
-                        input_path: Path to input folder of files to be processed
-                        output_path: Path to outpu folder of processed files
-                        Example: { 'input_path': 'input_folder', 'output_path': 'output_folder' }
+                        input_folder: Path to input folder of files to be processed
+                        output_folder: Path to output folder of processed files
+                        Example: { 'input_folder': 'your input folder', 'output_folder ': 'your output folder' }
   --data_local_config LOCAL_CONFIG
                         ast string containing input/output folders using local fs.
                         input_folder: Path to input folder of files to be processed
                         output_folder: Path to output folder of processed files
                         Example: { 'input_folder': './input', 'output_folder': '/tmp/output' }
   --data_max_files MAX_FILES
                         Max amount of files to process
@@ -77,8 +77,8 @@
                         delay between actor' creation
   --code_location CODE_LOCATION
                         AST string containing code location
                         github: Github repository URL.
                         commit_hash: github commit hash
                         path: Path within the repository
                         Example: { 'github': 'https://github.com/somerepo', 'commit_hash': '13241231asdfaed', 'path': 'transforms/universal/ededup' }
-```
+```
```

### Comparing `data_prep_lab-0.1.0/doc/library-config.md` & `data_prep_lab-0.1.1/doc/library-config.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/doc/overview.md` & `data_prep_lab-0.1.1/doc/overview.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The Data Processing Framework is python-based and enables the 
 application of "transforms" to data files (currently parquet) across a distributed 
 [Ray](https://docs.ray.io/en/latest/index.html) cluster, enabling the
 scalable processing/transformation of virtually unlimited amounts of data. 
 
 The framework allows simple 1:1 transformation of parquet files, but also enables
 more complex transformations requiring coordination among transforming nodes.
-This might include operations such as de-duplification, merging, and splitting.
+This might include operations such as de-duplication, merging, and splitting.
 The framework uses a plugin-model for the primary functions.  The key ones for
 developers of data transformation are:
 * [Transformation](../src/data_processing/transform/table_transform.py) - a simple, easily-implemented interface defines
 the specifics of a given data transformation.
 * [Transform Configuration](../src/data_processing/ray/transform_runtime.py) - defines
 the transform implementation and runtime classes, the 
 command line arguments specific to transform, and the short name for the transform.
```

### Comparing `data_prep_lab-0.1.0/doc/processing-architecture.jpg` & `data_prep_lab-0.1.1/doc/processing-architecture.jpg`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/doc/simplest-transform-tutorial.md` & `data_prep_lab-0.1.1/doc/simplest-transform-tutorial.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/doc/testing-transforms.md` & `data_prep_lab-0.1.1/doc/testing-transforms.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/doc/transform-external-resources.md` & `data_prep_lab-0.1.1/doc/transform-external-resources.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/doc/transform-porting.md` & `data_prep_lab-0.1.1/doc/transform-porting.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/doc/transform-tutorials.md` & `data_prep_lab-0.1.1/doc/transform-tutorials.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/doc/transformer-utilities.md` & `data_prep_lab-0.1.1/doc/transformer-utilities.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/doc/using_s3_transformers.md` & `data_prep_lab-0.1.1/doc/using_s3_transformers.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 The default user name/password is `minioadmin|minioadmin`
 
 ## Populating Minio with testing data
 
 Populating Minio server with test data can be done using `mc`. First configure mc to work with the local
 Minio server:
 
+
 ```shell
 mc alias set local http://127.0.0.1:9000 minioadmin minioadmin
 ```
 
 This set an alias `local` to 'mc' connected to the local Minio server instance. Now we can use our
 mc instance to populate server using a set of
 [commands](https://min.io/docs/minio/linux/reference/minio-mc.html) provided by `mc`.
@@ -51,14 +52,15 @@
 ```shell
 mc mb local/test
 ```
 
 Once the bucket is created, you can copy files (assuming you are in the transforms directory), using:
 
 ```shell
+mc cp --recursive tools/ingest2parquet/test-data/input/ local/test/ingest2parquet/input
 mc cp --recursive code/code_quality/test-data/input/ local/test/code_quality/input
 mc cp --recursive code/language_annotator/test-data/input/ local/test/language_annotator/input
 mc cp --recursive code/language_annotator/test-data/languages/ local/test/lang_annotator/languages
 mc cp --recursive code/malware/test-data/input/ local/test/malware/input
 
 mc cp --recursive language/doc_quality/test-data/input/ local/test/doc_quality/input
 mc cp --recursive language/language_id/test-data/input/ local/test/language_id/input
```

### Comparing `data_prep_lab-0.1.0/pyproject.toml` & `data_prep_lab-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "data_prep_lab"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.10"
 description = "Data Preparation Laboratory Library"
 license = {text = "Apache-2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     { name = "David Wood", email = "dawood@us.ibm.com" },
     { name = "Boris Lublinsky", email = "blublinsky@ibm.com" },
 ]
 dependencies = [
     "ray[default]==2.9.3",
-    "pyarrow==14.0.2",
-    "boto3==1.28.60",
+    "pyarrow==15.0.2",
+    "boto3==1.34.88",
     # The version of urllib fixes a whitesource-identified security issue - dawood 10/19/2023,
     "urllib3>=1.26.18",
     "argparse",
     "mmh3"
 ]
 
 [build-system]
```

### Comparing `data_prep_lab-0.1.0/src/data_prep_lab.egg-info/PKG-INFO` & `data_prep_lab-0.1.1/src/data_prep_lab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: data_prep_lab
-Version: 0.1.0
+Version: 0.1.1
 Summary: Data Preparation Laboratory Library
 Author-email: David Wood <dawood@us.ibm.com>, Boris Lublinsky <blublinsky@ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ray[default]==2.9.3
-Requires-Dist: pyarrow==14.0.2
-Requires-Dist: boto3==1.28.60
+Requires-Dist: pyarrow==15.0.2
+Requires-Dist: boto3==1.34.88
 Requires-Dist: urllib3>=1.26.18
 Requires-Dist: argparse
 Requires-Dist: mmh3
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest>=7.3.2; extra == "dev"
 Requires-Dist: pytest-dotenv>=0.5.2; extra == "dev"
```

### Comparing `data_prep_lab-0.1.0/src/data_prep_lab.egg-info/SOURCES.txt` & `data_prep_lab-0.1.1/src/data_prep_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/data_access/arrow_s3.py` & `data_prep_lab-0.1.1/src/data_processing/data_access/arrow_s3.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/data_access/data_access.py` & `data_prep_lab-0.1.1/src/data_processing/data_access/data_access.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/data_access/data_access_factory.py` & `data_prep_lab-0.1.1/src/data_processing/data_access/data_access_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,20 +74,20 @@
         )
 
         if self.enable_data_navigation:
             self.__add_data_navigation_params(parser)
 
     def __add_data_navigation_params(self, parser):
         help_example_dict = {
-            "input_path": [
-                "path_to_input_folder",
+            "input_folder": [
+                "s3-path/your-input-bucket",
                 "Path to input folder of files to be processed",
             ],
-            "output_path": [
-                "path_to_output_folder",
+            "output_folder": [
+                "s3-path/your-output-bucket",
                 "Path to output folder of processed files",
             ],
         }
         parser.add_argument(
             f"--{self.cli_arg_prefix}s3_config",
             type=ast.literal_eval,
             default=None,
```

### Comparing `data_prep_lab-0.1.0/src/data_processing/data_access/data_access_factory_base.py` & `data_prep_lab-0.1.1/src/data_processing/data_access/data_access_factory_base.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/data_access/data_access_local.py` & `data_prep_lab-0.1.1/src/data_processing/data_access/data_access_local.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/data_access/data_access_s3.py` & `data_prep_lab-0.1.1/src/data_processing/data_access/data_access_s3.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/ray/__init__.py` & `data_prep_lab-0.1.1/src/data_processing/ray/__init__.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/ray/ray_utils.py` & `data_prep_lab-0.1.1/src/data_processing/ray/ray_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/ray/transform_launcher.py` & `data_prep_lab-0.1.1/src/data_processing/ray/transform_launcher.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/ray/transform_orchestrator.py` & `data_prep_lab-0.1.1/src/data_processing/ray/transform_orchestrator.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/ray/transform_orchestrator_configuration.py` & `data_prep_lab-0.1.1/src/data_processing/ray/transform_orchestrator_configuration.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/ray/transform_runtime.py` & `data_prep_lab-0.1.1/src/data_processing/ray/transform_runtime.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/ray/transform_statistics.py` & `data_prep_lab-0.1.1/src/data_processing/ray/transform_statistics.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/ray/transform_table_processor.py` & `data_prep_lab-0.1.1/src/data_processing/ray/transform_table_processor.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/test_support/abstract_test.py` & `data_prep_lab-0.1.1/src/data_processing/test_support/abstract_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/test_support/ray/transform_test.py` & `data_prep_lab-0.1.1/src/data_processing/test_support/ray/transform_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/test_support/transform/noop_transform.py` & `data_prep_lab-0.1.1/src/data_processing/test_support/transform/noop_transform.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/test_support/transform/transform_test.py` & `data_prep_lab-0.1.1/src/data_processing/test_support/transform/transform_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/transform/table_transform.py` & `data_prep_lab-0.1.1/src/data_processing/transform/table_transform.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/utils/cli_utils.py` & `data_prep_lab-0.1.1/src/data_processing/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/utils/config.py` & `data_prep_lab-0.1.1/src/data_processing/utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         return None
 
     HUGGING_FACE_TOKEN = _get_first_env_var(["DPL_HUGGING_FACE_TOKEN"])
     """ Set from DPL_HUGGING_FACE_TOKEN env var(s) """
     DEFAULT_LOG_LEVEL = os.environ.get("DPL_LOG_LEVEL", "INFO")
     """ Set from DPL_LOG_LEVEL env var(s) """
 
+
 def add_if_missing(config: dict[str, Any], key: str, dflt: Any):
     """
     Add the given default key value if there no value for the key in the dictionary.
     :param config:
     :param key:
     :param dflt:
     :return:
```

### Comparing `data_prep_lab-0.1.0/src/data_processing/utils/log.py` & `data_prep_lab-0.1.1/src/data_processing/utils/log.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/src/data_processing/utils/params_utils.py` & `data_prep_lab-0.1.1/src/data_processing/utils/params_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -59,31 +59,38 @@
 
     @staticmethod
     def __dict_to_str(dict_val: dict[str, str], initial_indent: str, indent_per_level: str, as_value: bool) -> str:
         all_text = ""
         if as_value:
             all_text = all_text + "{ "
         first = True
+        last_line = ""
         for key, value in dict_val.items():
             if isinstance(value, dict):
                 text = ParamsUtils.__dict_to_str(value, initial_indent + indent_per_level, indent_per_level, as_value)
             else:
                 if as_value:
                     key = "'" + key + "'"
                     if isinstance(value, str):
                         value = "'" + value + "'"
                 text = initial_indent + key + ": " + str(value)
             if first:
-                sep = ""
+                new_text = ""
             elif as_value:
-                sep = ", "
+                new_text = ", "
             else:
-                sep = "\n"
-            all_text = all_text + sep + text
+                new_text = "\n"
+            if as_value and len(last_line) + len(text) > 60:
+                new_text = new_text + "\n"
+                last_line = ""
+            new_text = new_text + text
+            all_text = all_text + new_text
+            last_line = last_line + new_text
             first = False
+        all_text = all_text.strip()
         if as_value:
             all_text = all_text + " }"
         return all_text
 
     @staticmethod
     def get_ast_help_and_example_text(help_dict: dict[str, str], examples: list[dict[str, Any]]):
         initial_indent = ""
```

### Comparing `data_prep_lab-0.1.0/src/data_processing/utils/transform_utils.py` & `data_prep_lab-0.1.1/src/data_processing/utils/transform_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test/data_processing_tests/data_access/data_access_local_test.py` & `data_prep_lab-0.1.1/test/data_processing_tests/data_access/data_access_local_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test/data_processing_tests/data_access/data_access_s3_test.py` & `data_prep_lab-0.1.1/test/data_processing_tests/data_access/data_access_s3_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test/data_processing_tests/data_access/sample_input_data_test.py` & `data_prep_lab-0.1.1/test/data_processing_tests/data_access/sample_input_data_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 
 def test_table_sampling_data():
     """
     Testing data sampling
     :return: None
     """
 
-    input_folder = os.path.abspath(os.path.join(os.path.dirname(__file__),
-                                                "../../../test-data/data_processing/input_multiple"))
+    input_folder = os.path.abspath(
+        os.path.join(os.path.dirname(__file__), "../../../test-data/data_processing/input_multiple")
+    )
     output_folder = "/tmp"
     print(input_folder)
     data_access = DataAccessLocal({"input_folder": input_folder, "output_folder": output_folder})
     profile = data_access.sample_input_data()
     print(f"\nprofiled directory {input_folder}")
     print(f"profile {profile}")
     assert profile["estimated number of docs"] == 15.0
```

### Comparing `data_prep_lab-0.1.0/test/data_processing_tests/ray/launcher_test.py` & `data_prep_lab-0.1.1/test/data_processing_tests/ray/launcher_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test/data_processing_tests/ray/ray_util_test.py` & `data_prep_lab-0.1.1/test/data_processing_tests/ray/ray_util_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test/data_processing_tests/ray/test_noop_launch.py` & `data_prep_lab-0.1.1/test/data_processing_tests/ray/test_noop_launch.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test/data_processing_tests/transform/test_noop.py` & `data_prep_lab-0.1.1/test/data_processing_tests/transform/test_noop.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test/data_processing_tests/util/transform_utils_test.py` & `data_prep_lab-0.1.1/test/data_processing_tests/util/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test-data/data_processing/input/sample1.parquet` & `data_prep_lab-0.1.1/test-data/data_processing/input/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test-data/data_processing/input_multiple/sample1.parquet` & `data_prep_lab-0.1.1/test-data/data_processing/input_multiple/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test-data/data_processing/input_multiple/sample2.parquet` & `data_prep_lab-0.1.1/test-data/data_processing/input_multiple/sample2.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test-data/data_processing/input_multiple/sample3.parquet` & `data_prep_lab-0.1.1/test-data/data_processing/input_multiple/sample3.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test-data/data_processing/ray/noop/expected/metadata.json` & `data_prep_lab-0.1.1/test-data/data_processing/ray/noop/expected/metadata.json`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test-data/data_processing/ray/noop/expected/sample1.parquet` & `data_prep_lab-0.1.1/test-data/data_processing/ray/noop/expected/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test-data/data_processing/ray/noop/expected/subdir/test1.parquet` & `data_prep_lab-0.1.1/test-data/data_processing/ray/noop/expected/subdir/test1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test-data/data_processing/ray/noop/input/sample1.parquet` & `data_prep_lab-0.1.1/test-data/data_processing/ray/noop/input/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.0/test-data/data_processing/ray/noop/input/subdir/test1.parquet` & `data_prep_lab-0.1.1/test-data/data_processing/ray/noop/input/subdir/test1.parquet`

 * *Files identical despite different names*

