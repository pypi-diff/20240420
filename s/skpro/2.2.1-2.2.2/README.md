# Comparing `tmp/skpro-2.2.1.tar.gz` & `tmp/skpro-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skpro-2.2.1.tar", last modified: Sun Mar  3 22:07:33 2024, max compression
+gzip compressed data, was "skpro-2.2.2.tar", last modified: Sat Apr 20 18:35:59 2024, max compression
```

## Comparing `skpro-2.2.1.tar` & `skpro-2.2.2.tar`

### file list

```diff
@@ -1,238 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.239456 skpro-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-03 22:07:29.000000 skpro-2.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-03-03 22:07:29.000000 skpro-2.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15784 2024-03-03 22:07:33.239456 skpro-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-03-03 22:07:29.000000 skpro-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.207455 skpro-2.2.1/build_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-03-03 22:07:29.000000 skpro-2.2.1/build_tools/changelog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.203455 skpro-2.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.207455 skpro-2.2.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-03-03 22:07:29.000000 skpro-2.2.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.207455 skpro-2.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-03 22:07:29.000000 skpro-2.2.1/examples/custom_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.211455 skpro-2.2.1/examples/parametric/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-03 22:07:29.000000 skpro-2.2.1/examples/parametric/bagging.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-03 22:07:29.000000 skpro-2.2.1/examples/parametric/hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-03 22:07:29.000000 skpro-2.2.1/examples/parametric/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-03 22:07:29.000000 skpro-2.2.1/examples/parametric/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-03 22:07:29.000000 skpro-2.2.1/examples/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.211455 skpro-2.2.1/examples/vendors/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-03 22:07:29.000000 skpro-2.2.1/examples/vendors/pymc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-03 22:07:29.000000 skpro-2.2.1/examples/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.211455 skpro-2.2.1/extension_templates/
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-03-03 22:07:29.000000 skpro-2.2.1/extension_templates/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-03-03 22:07:29.000000 skpro-2.2.1/extension_templates/survival.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-03 22:07:29.000000 skpro-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-03 22:07:33.239456 skpro-2.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.211455 skpro-2.2.1/skpro/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.211455 skpro-2.2.1/skpro/base/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22066 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/base/old_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.211455 skpro-2.2.1/skpro/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/benchmarking/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.211455 skpro-2.2.1/skpro/benchmarking/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/benchmarking/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/benchmarking/tests/test_evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.211455 skpro-2.2.1/skpro/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.211455 skpro-2.2.1/skpro/datatypes/_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_adapter/polars.py
--rw-r--r--   0 runner    (1001) docker     (127)    20992 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.215455 skpro-2.2.1/skpro/datatypes/_convert_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_convert_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_convert_utils/_coerce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_convert_utils/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.215455 skpro-2.2.1/skpro/datatypes/_proba/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_proba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_proba/_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_proba/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_proba/_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_proba/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.215455 skpro-2.2.1/skpro/datatypes/_table/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_table/_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_table/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_table/_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/_table/_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.215455 skpro-2.2.1/skpro/datatypes/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/tests/test_convert_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/datatypes/tests/test_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.215455 skpro-2.2.1/skpro/distributions/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.215455 skpro-2.2.1/skpro/distributions/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.219455 skpro-2.2.1/skpro/distributions/adapters/scipy/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/adapters/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/adapters/scipy/_empirical.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.219455 skpro-2.2.1/skpro/distributions/adapters/scipy/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/adapters/scipy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/adapters/scipy/tests/test_scipy_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.219455 skpro-2.2.1/skpro/distributions/adapters/statsmodels/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/adapters/statsmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/adapters/statsmodels/_empirical.py
--rw-r--r--   0 runner    (1001) docker     (127)    26978 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/empirical.py
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/laplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)    24225 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/qpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/t.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.219455 skpro-2.2.1/skpro/distributions/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/tests/test_all_distrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/tests/test_base_default_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/tests/test_proba_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/distributions/tests/test_qpd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.219455 skpro-2.2.1/skpro/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16238 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/metrics/_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/metrics/_coerce.py
--rw-r--r--   0 runner    (1001) docker     (127)    18539 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/metrics/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.219455 skpro-2.2.1/skpro/metrics/survival/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/metrics/survival/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/metrics/survival/_c_harrell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/metrics/survival/_spll.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.219455 skpro-2.2.1/skpro/metrics/survival/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/metrics/survival/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/metrics/survival/tests/test_c_harrell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.219455 skpro-2.2.1/skpro/metrics/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/metrics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/metrics/tests/test_distr_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/metrics/tests/test_probabilistic_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.219455 skpro-2.2.1/skpro/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/model_selection/_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.223455 skpro-2.2.1/skpro/registry/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/registry/_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/registry/_scitype.py
--rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/registry/_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.223455 skpro-2.2.1/skpro/registry/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/registry/tests/test_scitype.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/registry/tests/test_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.223455 skpro-2.2.1/skpro/regression/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.223455 skpro-2.2.1/skpro/regression/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.223455 skpro-2.2.1/skpro/regression/adapters/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/adapters/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/adapters/sklearn/_sklearn_proba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.223455 skpro-2.2.1/skpro/regression/base/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30706 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/base/_delegate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.223455 skpro-2.2.1/skpro/regression/base/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/base/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/base/adapters/_sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.223455 skpro-2.2.1/skpro/regression/baselines/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/baselines/density.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.223455 skpro-2.2.1/skpro/regression/compose/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/compose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21530 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/compose/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    16701 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/cyclic_boosting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/density.py
--rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.223455 skpro-2.2.1/skpro/regression/gp/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/gp/_sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.227455 skpro-2.2.1/skpro/regression/linear/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/linear/_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/mapie.py
--rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/multiquantile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.227455 skpro-2.2.1/skpro/regression/parametric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/parametric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/parametric/estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/parametric/parametric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14702 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/residual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.227455 skpro-2.2.1/skpro/regression/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/tests/test_all_regressors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/tests/test_cyclic_boosting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.227455 skpro-2.2.1/skpro/regression/vendors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/vendors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/regression/vendors/pymc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.227455 skpro-2.2.1/skpro/survival/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/survival/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/survival/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.227455 skpro-2.2.1/skpro/survival/compose/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/survival/compose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/survival/compose/_reduce_cond_unc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/survival/compose/_reduce_uncensored.py
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/survival/coxph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.227455 skpro-2.2.1/skpro/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.231455 skpro-2.2.1/skpro/tests/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/scenarios/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/scenarios/scenarios_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/scenarios/scenarios_regressor_proba.py
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/test_all_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/test_baselines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/test_class_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/test_vendors.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.231455 skpro-2.2.1/skpro/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.231455 skpro-2.2.1/skpro/utils/_maint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/_maint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/_maint/_show_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.231455 skpro-2.2.1/skpro/utils/_maint/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/_maint/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/_maint/tests/test_show_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.231455 skpro-2.2.1/skpro/utils/deep_equals/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/deep_equals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/deep_equals/_deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/git_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/index.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/random_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.231455 skpro-2.2.1/skpro/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.231455 skpro-2.2.1/skpro/utils/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14906 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/utils/validation/_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.231455 skpro-2.2.1/skpro/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/workflow/cross_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.235455 skpro-2.2.1/skpro/workflow/manager/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/workflow/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/workflow/manager/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/workflow/manager/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.235455 skpro-2.2.1/skpro/workflow/table/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/workflow/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/workflow/table/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-03 22:07:29.000000 skpro-2.2.1/skpro/workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 22:07:33.235455 skpro-2.2.1/skpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15784 2024-03-03 22:07:33.000000 skpro-2.2.1/skpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-03-03 22:07:33.000000 skpro-2.2.1/skpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 22:07:33.000000 skpro-2.2.1/skpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-03 22:07:33.000000 skpro-2.2.1/skpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-03 22:07:33.000000 skpro-2.2.1/skpro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 22:07:32.000000 skpro-2.2.1/skpro.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.235070 skpro-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-20 18:35:52.000000 skpro-2.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-20 18:35:52.000000 skpro-2.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15900 2024-04-20 18:35:59.235070 skpro-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-04-20 18:35:52.000000 skpro-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/build_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-20 18:35:52.000000 skpro-2.2.2/build_tools/changelog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.199069 skpro-2.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-04-20 18:35:52.000000 skpro-2.2.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/examples/parametric/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/parametric/bagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/parametric/hyperparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/parametric/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/parametric/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/examples/vendors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/vendors/pymc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/extension_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-04-20 18:35:52.000000 skpro-2.2.2/extension_templates/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-04-20 18:35:52.000000 skpro-2.2.2/extension_templates/survival.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-20 18:35:52.000000 skpro-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-20 18:35:59.235070 skpro-2.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/skpro/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/skpro/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22066 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/base/old_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/skpro/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/benchmarking/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/benchmarking/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/benchmarking/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/benchmarking/tests/test_evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/datatypes/_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_adapter/polars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20992 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/datatypes/_convert_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_convert_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_convert_utils/_coerce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_convert_utils/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/datatypes/_proba/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_proba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_proba/_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_proba/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_proba/_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_proba/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/datatypes/_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_table/_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_table/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_table/_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_table/_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/datatypes/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/tests/test_convert_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/tests/test_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/adapters/scipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/scipy/_empirical.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/adapters/scipy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/scipy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/scipy/tests/test_scipy_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/adapters/statsmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/statsmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/statsmodels/_empirical.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27660 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/base/_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/fisk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/laplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/logistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/qpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/qpd_empirical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/t.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/tests/test_all_distrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/tests/test_base_default_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/tests/test_proba_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/tests/test_qpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/weibull.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16917 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/_coerce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18539 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/metrics/survival/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/survival/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/survival/_c_harrell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/survival/_spll.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/metrics/survival/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/survival/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/survival/tests/test_c_harrell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/metrics/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/tests/test_distr_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/tests/test_probabilistic_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/model_selection/_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/_scitype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/tests/test_scitype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/tests/test_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/regression/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/regression/adapters/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/adapters/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/adapters/sklearn/_sklearn_proba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/regression/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30706 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/base/_delegate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/base/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/base/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/base/adapters/_sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/baselines/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/baselines/density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/compose/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21530 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/compose/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16701 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/cyclic_boosting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/gp/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/gp/_sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/linear/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/linear/_glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/linear/_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/mapie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13604 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/multiquantile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/parametric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/parametric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/parametric/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/parametric/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14702 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/residual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/tests/test_all_regressors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/tests/test_cyclic_boosting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/vendors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/vendors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/vendors/pymc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/survival/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/survival/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/adapters/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/adapters/lifelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/adapters/sksurv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/survival/additive/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/additive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/additive/_aalen_lifelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/survival/aft/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/aft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/aft/_aft_lifelines_fisk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/aft/_aft_lifelines_lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/aft/_aft_lifelines_weibull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/survival/compose/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/compose/_reduce_cond_unc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/compose/_reduce_uncensored.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/survival/coxph/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/coxph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/coxph/_coxnet_sksurv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/coxph/_coxph_lifelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/coxph/_coxph_sksurv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/coxph/_coxph_statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/survival/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/ensemble/_grad_boost_sksurv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16778 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/ensemble/_survforest_sksurv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/survival/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/tree/_tree_sksurv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/tests/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/scenarios/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/scenarios/scenarios_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/scenarios/scenarios_regressor_proba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_all_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_baselines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_class_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_vendors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/utils/_maint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/_maint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/_maint/_show_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/utils/_maint/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/_maint/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/_maint/tests/test_show_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/utils/deep_equals/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/deep_equals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/deep_equals/_deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/git_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/random_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/utils/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14906 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/validation/_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/cross_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/workflow/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/manager/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/manager/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/workflow/table/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/table/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15900 2024-04-20 18:35:59.000000 skpro-2.2.2/skpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-20 18:35:59.000000 skpro-2.2.2/skpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:35:59.000000 skpro-2.2.2/skpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-20 18:35:59.000000 skpro-2.2.2/skpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 18:35:59.000000 skpro-2.2.2/skpro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:35:56.000000 skpro-2.2.2/skpro.egg-info/zip-safe
```

### Comparing `skpro-2.2.1/LICENSE.txt` & `skpro-2.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/PKG-INFO` & `skpro-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skpro
-Version: 2.2.1
+Version: 2.2.2
 Summary: A unified framework for probability distributions and probabilistic supervised regression
 Author: Franz Király, Frithjof Gressmann, Vitaly Davydov
 Author-email: skpro developers <sktime.toolbox@gmail.com>
 Maintainer: Franz Király, Frithjof Gressmann
 Maintainer-email: skpro developers <sktime.toolbox@gmail.com>
 Project-URL: Homepage, https://github.com/sktime/skpro
 Project-URL: Repository, https://github.com/sktime/skpro
@@ -37,19 +37,21 @@
 Requires-Dist: packaging
 Requires-Dist: scikit-base<0.8.0,>=0.6.1
 Requires-Dist: scikit-learn<1.5.0,>=0.24.0
 Requires-Dist: scipy<2.0.0,>=1.2.0
 Provides-Extra: all-extras
 Requires-Dist: attrs; extra == "all-extras"
 Requires-Dist: distfit; extra == "all-extras"
+Requires-Dist: lifelines<0.29.0; extra == "all-extras"
 Requires-Dist: mapie; extra == "all-extras"
 Requires-Dist: matplotlib>=3.3.2; extra == "all-extras"
 Requires-Dist: ngboost; extra == "all-extras"
 Requires-Dist: polars<0.21.0; extra == "all-extras"
 Requires-Dist: pyarrow<14.0.0; python_version < "3.12" and extra == "all-extras"
+Requires-Dist: scikit-survival<0.23.0; extra == "all-extras"
 Requires-Dist: statsmodels>=0.12.1; extra == "all-extras"
 Requires-Dist: tabulate; extra == "all-extras"
 Requires-Dist: uncertainties; extra == "all-extras"
 Requires-Dist: cyclic-boosting>=1.2.5; python_version < "3.12" and extra == "all-extras"
 Provides-Extra: dev
 Requires-Dist: backoff; extra == "dev"
 Requires-Dist: httpx; extra == "dev"
@@ -73,15 +75,15 @@
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.16.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 
 <a href="https://skpro.readthedocs.io/en/latest"><img src="https://github.com/sktime/skpro/blob/main/docs/source/images/skpro-banner.png" width="500" align="right" /></a>
 
-:rocket: **Version 2.2.1 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
+:rocket: **Version 2.2.2 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
 
 `skpro` is a library for supervised probabilistic prediction in python.
 It provides `scikit-learn`-like, `scikit-base` compatible interfaces to:
 
 * tabular **supervised regressors for probabilistic prediction** - interval, quantile and distribution predictions
 * tabular **probabilistic time-to-event and survival prediction** - instance-individual survival distributions
 * **metrics to evaluate probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS, survival losses
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skpro Version: 2.2.1 Summary: A unified framework
+Metadata-Version: 2.1 Name: skpro Version: 2.2.2 Summary: A unified framework
 for probability distributions and probabilistic supervised regression Author:
 Franz KirÃ¡ly, Frithjof Gressmann, Vitaly Davydov Author-email: skpro
 developers
 gmail.com> Maintainer: Franz KirÃ¡ly, Frithjof Gressmann Maintainer-email:
 skpro developers
 gmail.com> Project-URL: Homepage, https://github.com/sktime/skpro Project-URL:
 Repository, https://github.com/sktime/skpro Project-URL: Documentation, https:/
@@ -21,44 +21,45 @@
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Python: <3.13,>=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.txt License-File: AUTHORS.rst Requires-Dist: numpy<1.27,>=1.21.0
 Requires-Dist: pandas<2.3.0,>=1.1.0 Requires-Dist: packaging Requires-Dist:
 scikit-base<0.8.0,>=0.6.1 Requires-Dist: scikit-learn<1.5.0,>=0.24.0 Requires-
 Dist: scipy<2.0.0,>=1.2.0 Provides-Extra: all-extras Requires-Dist: attrs;
 extra == "all-extras" Requires-Dist: distfit; extra == "all-extras" Requires-
-Dist: mapie; extra == "all-extras" Requires-Dist: matplotlib>=3.3.2; extra ==
-"all-extras" Requires-Dist: ngboost; extra == "all-extras" Requires-Dist:
-polars<0.21.0; extra == "all-extras" Requires-Dist: pyarrow<14.0.0;
-python_version < "3.12" and extra == "all-extras" Requires-Dist:
-statsmodels>=0.12.1; extra == "all-extras" Requires-Dist: tabulate; extra ==
-"all-extras" Requires-Dist: uncertainties; extra == "all-extras" Requires-Dist:
-cyclic-boosting>=1.2.5; python_version < "3.12" and extra == "all-extras"
-Provides-Extra: dev Requires-Dist: backoff; extra == "dev" Requires-Dist:
-httpx; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
-pytest; extra == "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist:
-pytest-randomly; extra == "dev" Requires-Dist: pytest-timeout; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev" Requires-Dist: wheel; extra ==
-"dev" Provides-Extra: binder Requires-Dist: jupyter; extra == "binder"
-Provides-Extra: docs Requires-Dist: jupyter; extra == "docs" Requires-Dist:
-myst-parser; extra == "docs" Requires-Dist: nbsphinx>=0.8.6; extra == "docs"
-Requires-Dist: numpydoc; extra == "docs" Requires-Dist: pydata-sphinx-theme;
-extra == "docs" Requires-Dist: sphinx!=7.2.0,<8.0.0; extra == "docs" Requires-
-Dist: sphinx-design<0.6.0; extra == "docs" Requires-Dist: sphinx-issues<5.0.0;
-extra == "docs" Requires-Dist: sphinx-gallery<0.16.0; extra == "docs" Requires-
-Dist: sphinx-panels; extra == "docs" Requires-Dist: tabulate; extra == "docs"
-_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-
-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.2.1 out now!** [Read the release notes here.]
-(https://skpro.readthedocs.io/en/latest/changelog.html). `skpro` is a library
-for supervised probabilistic prediction in python. It provides `scikit-learn`-
-like, `scikit-base` compatible interfaces to: * tabular **supervised regressors
-for probabilistic prediction** - interval, quantile and distribution
-predictions * tabular **probabilistic time-to-event and survival prediction** -
-instance-individual survival distributions * **metrics to evaluate
-probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS,
-survival losses * **reductions** to turn `scikit-learn` regressors into
+Dist: lifelines<0.29.0; extra == "all-extras" Requires-Dist: mapie; extra ==
+"all-extras" Requires-Dist: matplotlib>=3.3.2; extra == "all-extras" Requires-
+Dist: ngboost; extra == "all-extras" Requires-Dist: polars<0.21.0; extra ==
+"all-extras" Requires-Dist: pyarrow<14.0.0; python_version < "3.12" and extra
+== "all-extras" Requires-Dist: scikit-survival<0.23.0; extra == "all-extras"
+Requires-Dist: statsmodels>=0.12.1; extra == "all-extras" Requires-Dist:
+tabulate; extra == "all-extras" Requires-Dist: uncertainties; extra == "all-
+extras" Requires-Dist: cyclic-boosting>=1.2.5; python_version < "3.12" and
+extra == "all-extras" Provides-Extra: dev Requires-Dist: backoff; extra ==
+"dev" Requires-Dist: httpx; extra == "dev" Requires-Dist: pre-commit; extra ==
+"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra ==
+"dev" Requires-Dist: pytest-randomly; extra == "dev" Requires-Dist: pytest-
+timeout; extra == "dev" Requires-Dist: pytest-xdist; extra == "dev" Requires-
+Dist: wheel; extra == "dev" Provides-Extra: binder Requires-Dist: jupyter;
+extra == "binder" Provides-Extra: docs Requires-Dist: jupyter; extra == "docs"
+Requires-Dist: myst-parser; extra == "docs" Requires-Dist: nbsphinx>=0.8.6;
+extra == "docs" Requires-Dist: numpydoc; extra == "docs" Requires-Dist: pydata-
+sphinx-theme; extra == "docs" Requires-Dist: sphinx!=7.2.0,<8.0.0; extra ==
+"docs" Requires-Dist: sphinx-design<0.6.0; extra == "docs" Requires-Dist:
+sphinx-issues<5.0.0; extra == "docs" Requires-Dist: sphinx-gallery<0.16.0;
+extra == "docs" Requires-Dist: sphinx-panels; extra == "docs" Requires-Dist:
+tabulate; extra == "docs" _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/
+_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.2.2 out now!** [Read the
+release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
+`skpro` is a library for supervised probabilistic prediction in python. It
+provides `scikit-learn`-like, `scikit-base` compatible interfaces to: * tabular
+**supervised regressors for probabilistic prediction** - interval, quantile and
+distribution predictions * tabular **probabilistic time-to-event and survival
+prediction** - instance-individual survival distributions * **metrics to
+evaluate probabilistic predictions**, e.g., pinball loss, empirical coverage,
+CRPS, survival losses * **reductions** to turn `scikit-learn` regressors into
 probabilistic `skpro` regressors, such as bootstrap or conformal * building
 **pipelines and composite models**, including tuning via probabilistic
 performance metrics * symbolic **probability distributions** with value domain
 of `pandas.DataFrame`-s and `pandas`-like interface | Overview | | |---|---| |
 **Open Source** | [![BSD 3-clause](https://img.shields.io/badge/License-
 BSD%203--Clause-blue.svg)](https://github.com/sktime/sktime/blob/main/LICENSE)
 | | **Tutorials** | [![Binder](https://mybinder.org/badge_logo.svg)](https://
```

### Comparing `skpro-2.2.1/README.md` & `skpro-2.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <a href="https://skpro.readthedocs.io/en/latest"><img src="https://github.com/sktime/skpro/blob/main/docs/source/images/skpro-banner.png" width="500" align="right" /></a>
 
-:rocket: **Version 2.2.1 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
+:rocket: **Version 2.2.2 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
 
 `skpro` is a library for supervised probabilistic prediction in python.
 It provides `scikit-learn`-like, `scikit-base` compatible interfaces to:
 
 * tabular **supervised regressors for probabilistic prediction** - interval, quantile and distribution predictions
 * tabular **probabilistic time-to-event and survival prediction** - instance-individual survival distributions
 * **metrics to evaluate probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS, survival losses
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-
-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.2.1 out now!** [Read the release notes here.]
+_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.2.2 out now!** [Read the release notes here.]
 (https://skpro.readthedocs.io/en/latest/changelog.html). `skpro` is a library
 for supervised probabilistic prediction in python. It provides `scikit-learn`-
 like, `scikit-base` compatible interfaces to: * tabular **supervised regressors
 for probabilistic prediction** - interval, quantile and distribution
 predictions * tabular **probabilistic time-to-event and survival prediction** -
 instance-individual survival distributions * **metrics to evaluate
 probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS,
```

### Comparing `skpro-2.2.1/build_tools/changelog.py` & `skpro-2.2.2/build_tools/changelog.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/docs/source/conf.py` & `skpro-2.2.2/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,26 +130,30 @@
 
     if domain != "py" or not info["module"]:
         return None
     try:
         filename = "skpro/%s#L%d-L%d" % find_source()
     except Exception:
         filename = info["module"].replace(".", "/") + ".py"
-    return f"https://github.com/sktime/skpro/blob/{version_match}/{filename}"
+    if version_match == "latest":
+        version = "main"
+    else:
+        version = version_match
+    return f"https://github.com/sktime/skpro/blob/{version}/{filename}"
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
 html_theme = "pydata_sphinx_theme"
 
 # Define the json_url for our version switcher.
-json_url = "https://github.com/sktime/skpro/blob/main/docs/source/_static/switcher.json"
+json_url = "https://skpro.readthedocs.io/en/latest/_static/switcher.json"
 
 # This uses code from the py-data-sphinx theme's own conf.py
 # Define the version we use for matching in the version switcher.
 version_match = os.environ.get("READTHEDOCS_VERSION")
 
 # If READTHEDOCS_VERSION doesn't exist, we're not on RTD
 # If it is an integer, we're in a PR build and the version isn't correct.
```

### Comparing `skpro-2.2.1/examples/custom_model.py` & `skpro-2.2.2/examples/custom_model.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/examples/parametric/bagging.py` & `skpro-2.2.2/examples/parametric/bagging.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/examples/parametric/hyperparameters.py` & `skpro-2.2.2/examples/parametric/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/examples/parametric/simple.py` & `skpro-2.2.2/examples/parametric/simple.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/examples/parametric/workflow.py` & `skpro-2.2.2/examples/parametric/workflow.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/examples/simple.py` & `skpro-2.2.2/examples/simple.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/examples/vendors/pymc.py` & `skpro-2.2.2/examples/vendors/pymc.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/examples/workflow.py` & `skpro-2.2.2/examples/workflow.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/extension_templates/regression.py` & `skpro-2.2.2/extension_templates/regression.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/extension_templates/survival.py` & `skpro-2.2.2/extension_templates/survival.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/pyproject.toml` & `skpro-2.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "skpro"
-version = "2.2.1"
+version = "2.2.2"
 description = "A unified framework for probability distributions and probabilistic supervised regression"
 authors = [
     {name = "skpro developers", email = "sktime.toolbox@gmail.com"},
     {name = "Franz Király"},
     {name = "Frithjof Gressmann"},
     {name = "Vitaly Davydov"},
 ]
@@ -49,19 +49,21 @@
     "scipy<2.0.0,>=1.2.0",
 ]
 
 [project.optional-dependencies]
 all_extras = [
     "attrs",
     "distfit",
+    "lifelines<0.29.0",
     "mapie",
     "matplotlib>=3.3.2",
     "ngboost",
     "polars<0.21.0",
     "pyarrow<14.0.0; python_version < '3.12'",
+    "scikit-survival<0.23.0",
     "statsmodels>=0.12.1",
     "tabulate",
     "uncertainties",
     "cyclic-boosting>=1.2.5; python_version < '3.12'"
 ]
 
 dev = [
```

### Comparing `skpro-2.2.1/setup.cfg` & `skpro-2.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/base/_base.py` & `skpro-2.2.2/skpro/base/_base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/base/old_base.py` & `skpro-2.2.2/skpro/base/old_base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/benchmarking/evaluate.py` & `skpro-2.2.2/skpro/benchmarking/evaluate.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/benchmarking/tests/test_evaluate.py` & `skpro-2.2.2/skpro/benchmarking/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/__init__.py` & `skpro-2.2.2/skpro/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_adapter/polars.py` & `skpro-2.2.2/skpro/datatypes/_adapter/polars.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_check.py` & `skpro-2.2.2/skpro/datatypes/_check.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_common.py` & `skpro-2.2.2/skpro/datatypes/_common.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_convert.py` & `skpro-2.2.2/skpro/datatypes/_convert.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_convert_utils/_coerce.py` & `skpro-2.2.2/skpro/datatypes/_convert_utils/_coerce.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_convert_utils/_convert.py` & `skpro-2.2.2/skpro/datatypes/_convert_utils/_convert.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_examples.py` & `skpro-2.2.2/skpro/datatypes/_examples.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_proba/__init__.py` & `skpro-2.2.2/skpro/datatypes/_proba/__init__.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_proba/_check.py` & `skpro-2.2.2/skpro/datatypes/_proba/_check.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_proba/_convert.py` & `skpro-2.2.2/skpro/datatypes/_proba/_convert.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_proba/_examples.py` & `skpro-2.2.2/skpro/datatypes/_proba/_examples.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_proba/_registry.py` & `skpro-2.2.2/skpro/datatypes/_proba/_registry.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_registry.py` & `skpro-2.2.2/skpro/datatypes/_registry.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_table/__init__.py` & `skpro-2.2.2/skpro/datatypes/_table/__init__.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_table/_check.py` & `skpro-2.2.2/skpro/datatypes/_table/_check.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_table/_convert.py` & `skpro-2.2.2/skpro/datatypes/_table/_convert.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_table/_examples.py` & `skpro-2.2.2/skpro/datatypes/_table/_examples.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/_table/_registry.py` & `skpro-2.2.2/skpro/datatypes/_table/_registry.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/tests/test_check.py` & `skpro-2.2.2/skpro/datatypes/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/tests/test_convert.py` & `skpro-2.2.2/skpro/datatypes/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/tests/test_convert_to.py` & `skpro-2.2.2/skpro/datatypes/tests/test_convert_to.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/datatypes/tests/test_lookup.py` & `skpro-2.2.2/skpro/datatypes/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/distributions/__init__.py` & `skpro-2.2.2/skpro/distributions/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 """Probability distribution objects."""
 # copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
 # adapted from sktime
 
 __all__ = [
     "Empirical",
+    "Fisk",
     "Laplace",
+    "Logistic",
+    "LogNormal",
     "Mixture",
     "Normal",
-    "TDistribution",
+    "Poisson",
+    "QPD_Empirical",
     "QPD_S",
     "QPD_B",
     "QPD_U",
+    "TDistribution",
+    "Weibull",
 ]
 
 from skpro.distributions.empirical import Empirical
+from skpro.distributions.fisk import Fisk
 from skpro.distributions.laplace import Laplace
+from skpro.distributions.logistic import Logistic
+from skpro.distributions.lognormal import LogNormal
 from skpro.distributions.mixture import Mixture
 from skpro.distributions.normal import Normal
+from skpro.distributions.poisson import Poisson
 from skpro.distributions.qpd import QPD_B, QPD_S, QPD_U
+from skpro.distributions.qpd_empirical import QPD_Empirical
 from skpro.distributions.t import TDistribution
+from skpro.distributions.weibull import Weibull
```

### Comparing `skpro-2.2.1/skpro/distributions/adapters/scipy/_empirical.py` & `skpro-2.2.2/skpro/distributions/adapters/scipy/_empirical.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/distributions/adapters/scipy/tests/test_scipy_adapters.py` & `skpro-2.2.2/skpro/distributions/adapters/scipy/tests/test_scipy_adapters.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/distributions/adapters/statsmodels/_empirical.py` & `skpro-2.2.2/skpro/distributions/adapters/statsmodels/_empirical.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/distributions/base.py` & `skpro-2.2.2/skpro/distributions/base/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,18 @@
         return _Indexer(ref=self, method="_iloc")
 
     @property
     def shape(self):
         """Shape of self, a pair (2-tuple)."""
         return (len(self.index), len(self.columns))
 
+    def __len__(self):
+        """Length of self, number of rows."""
+        return len(self.index)
+
     def _loc(self, rowidx=None, colidx=None):
         if rowidx is not None:
             row_iloc = self.index.get_indexer_for(rowidx)
         else:
             row_iloc = None
         if colidx is not None:
             col_iloc = self.columns.get_indexer_for(colidx)
@@ -160,26 +164,29 @@
             f"filled in {fill_in}."
         )
         if severity == "warn":
             return msg_approx
         else:
             return msg
 
-    def _get_bc_params(self, *args, dtype=None):
+    def _get_bc_params(self, *args, dtype=None, oned_as="row"):
         """Fully broadcast tuple of parameters given param shapes and index, columns.
 
         Parameters
         ----------
         args : float, int, array of floats, or array of ints (1D or 2D)
             Distribution parameters that are to be made broadcastable. If no positional
             arguments are provided, all parameters of `self` are used except for `index`
             and `columns`.
         dtype : str, optional
             broadcasted arrays are cast to all have datatype `dtype`. If None, then no
             datatype casting is done.
+        oned_as : str, optional, "row" (default) or "col"
+            If 'row', then 1D arrays are treated as row vectors. If 'column', then 1D
+            arrays are treated as column vectors.
 
         Returns
         -------
         Tuple of float or integer arrays
             Each element of the tuple represents a different broadcastable distribution
             parameter.
         """
@@ -188,19 +195,29 @@
             # Handle case where no positional arguments are provided
             params = self.get_params()
             params.pop("index")
             params.pop("columns")
             args = tuple(params.values())
             number_of_params = len(args)
 
+        def row_to_col(arr):
+            """Convert 1D arrays to 2D col arrays, leave 2D arrays unchanged."""
+            if arr.ndim == 1:
+                return arr.reshape(-1, 1)
+            return arr
+
+        args_as_np = [np.array(arg) for arg in args]
+        if oned_as == "col":
+            args_as_np = [row_to_col(arg) for arg in args_as_np]
+
         if hasattr(self, "index") and self.index is not None:
-            args += (self.index.to_numpy().reshape(-1, 1),)
+            args_as_np += (self.index.to_numpy().reshape(-1, 1),)
         if hasattr(self, "columns") and self.columns is not None:
-            args += (self.columns.to_numpy(),)
-        bc = np.broadcast_arrays(*args)
+            args_as_np += (self.columns.to_numpy(),)
+        bc = np.broadcast_arrays(*args_as_np)
         if dtype is not None:
             bc = [array.astype(dtype) for array in bc]
         return bc[:number_of_params]
 
     def pdf(self, x):
         r"""Probability density function.
```

### Comparing `skpro-2.2.1/skpro/distributions/empirical.py` & `skpro-2.2.2/skpro/distributions/empirical.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     def __init__(self, spl, weights=None, time_indep=True, index=None, columns=None):
         self.spl = spl
         self.weights = weights
         self.time_indep = time_indep
         self.index = index
         self.columns = columns
 
-        _timestamps = spl.index.get_level_values(-1).unique()
-        _spl_instances = spl.index.droplevel(-1).unique()
+        _timestamps = spl.index.droplevel(0).unique()
+        _spl_instances = spl.index.get_level_values(0).unique()
         self._timestamps = _timestamps
         self._spl_instances = _spl_instances
         self._N = len(_spl_instances)
 
         if index is None:
             index = pd.Index(_timestamps)
 
@@ -79,29 +79,35 @@
 
         sorted = {}
         weights = {}
         for t in times:
             sorted[t] = {}
             weights[t] = {}
             for col in cols:
-                spl_t = self.spl.loc[(slice(None), t), col].values
+                sl = (slice(None),) + self._coerce_tuple(t)
+                spl_t = self.spl.loc[sl, col].values
                 sorter = np.argsort(spl_t)
                 spl_t_sorted = spl_t[sorter]
                 sorted[t][col] = spl_t_sorted
                 if self.weights is not None:
                     weights_t = self.weights.loc[(slice(None), t)].values
                     weights_t_sorted = weights_t[sorter]
                     weights[t][col] = weights_t_sorted
                 else:
                     ones = np.ones(len(spl_t_sorted))
                     weights[t][col] = ones
 
         self._sorted = sorted
         self._weights = weights
 
+    def _coerce_tuple(self, x):
+        if not isinstance(x, tuple):
+            x = (x,)
+        return x
+
     def _apply_per_ix(self, func, params, x=None):
         """Apply function per index."""
         sorted = self._sorted
         weights = self._weights
 
         if x is not None and hasattr(x, "index"):
             index = x.index
```

### Comparing `skpro-2.2.1/skpro/distributions/laplace.py` & `skpro-2.2.2/skpro/distributions/laplace.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/distributions/mixture.py` & `skpro-2.2.2/skpro/distributions/mixture.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/distributions/normal.py` & `skpro-2.2.2/skpro/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/distributions/qpd.py` & `skpro-2.2.2/skpro/distributions/qpd.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,17 @@
         quantile function value of ``alpha``
     qv_median : float or array_like[float]
         quantile function value of quantile 0.5
     qv_high : float or array_like[float]
         quantile function value of quantile ``1 - alpha``
     lower : float
         lower bound of semi-bounded range (default is 0)
-    version: str
+    version: str, optional, default="normal"
         options are ``normal`` (default) or ``logistic``
-    dist_shape: str
+    dist_shape: float, optional, default=0.0
         parameter modifying the logistic base distribution via
         sinh/arcsinh-scaling (only active in sinhlogistic version)
 
     Example
     -------
     >>> from skpro.distributions.qpd import QPD_S  # doctest: +SKIP
 
@@ -64,16 +64,16 @@
         # packaging info
         # --------------
         "authors": ["setoguchi-naoki", "felix-wick"],
         "maintainers": ["setoguchi-naoki"],
         "python_dependencies": "cyclic_boosting>=1.2.5",
         # estimator tags
         # --------------
-        "capabilities:approx": [],
-        "capabilities:exact": ["mean", "var", "cdf", "ppf"],
+        "capabilities:approx": ["pdfnorm", "energy"],
+        "capabilities:exact": ["mean", "var", "cdf", "ppf", "pdf", "log_pdf"],
         "distr:measuretype": "continuous",
     }
 
     def __init__(
         self,
         alpha: float,
         qv_low: float or object,
@@ -96,26 +96,18 @@
         self.index = index
         self.columns = columns
 
         super().__init__(index=index, columns=columns)
 
         from cyclic_boosting.quantile_matching import J_QPD_extended_S
 
-        params = [alpha, qv_low, qv_median, qv_high]
-        for idx, p in enumerate(params):
-            if isinstance(p, float):
-                params[idx] = np.array([p])
-            elif (
-                isinstance(p, tuple) or isinstance(p, list) or isinstance(p, np.ndarray)
-            ):
-                params[idx] = np.array(p)
-            else:
-                raise ValueError("data type is not float or array_like object")
+        alpha, qv_low, qv_median, qv_high = _prep_qpd_params(
+            self, alpha, qv_low, qv_median, qv_high
+        )
 
-        alpha, qv_low, qv_median, qv_high = params[:]
         if index is None:
             index = pd.RangeIndex(qv_low.shape[0])
             self.index = index
 
         if columns is None:
             columns = pd.RangeIndex(1)
             self.columns = columns
@@ -232,14 +224,16 @@
         """Return testing parameter settings for the estimator."""
         params1 = {
             "alpha": 0.2,
             "version": "normal",
             "qv_low": 0.2,
             "qv_median": 0.5,
             "qv_high": 0.8,
+            "index": pd.Index([1, 2, 5]),
+            "columns": pd.Index(["a"]),
         }
         params2 = {
             "alpha": 0.2,
             "version": "normal",
             "qv_low": [0.2, 0.2, 0.2],
             "qv_median": [0.5, 0.5, 0.5],
             "qv_high": [0.8, 0.8, 0.8],
@@ -268,17 +262,17 @@
         quantile function value of quantile 0.5
     qv_high : float or array_like[float]
         quantile function value of quantile ``1 - alpha``
     lower : float
         lower bound of semi-bounded range
     upper : float
         upper bound of supported range
-    version: str
+    version: str, optional, default="normal"
         options are ``normal`` (default) or ``logistic``
-    dist_shape: str
+    dist_shape: float, optional, default=0.0
         parameter modifying the logistic base distribution via
         sinh/arcsinh-scaling (only active in sinhlogistic version)
 
     Example
     -------
     >>> from skpro.distributions.qpd import QPD_B  # doctest: +SKIP
 
@@ -298,16 +292,16 @@
         # packaging info
         # --------------
         "authors": ["setoguchi-naoki", "felix-wick"],
         "maintainers": ["setoguchi-naoki"],
         "python_dependencies": "cyclic_boosting>=1.2.5",
         # estimator tags
         # --------------
-        "capabilities:approx": [],
-        "capabilities:exact": ["mean", "var", "cdf", "ppf"],
+        "capabilities:approx": ["pdfnorm", "energy"],
+        "capabilities:exact": ["mean", "var", "cdf", "ppf", "pdf", "log_pdf"],
         "distr:measuretype": "continuous",
     }
 
     def __init__(
         self,
         alpha: float,
         qv_low: float or object,
@@ -332,26 +326,18 @@
         self.index = index
         self.columns = columns
 
         super().__init__(index=index, columns=columns)
 
         from cyclic_boosting.quantile_matching import J_QPD_extended_B
 
-        params = [alpha, qv_low, qv_median, qv_high]
-        for idx, p in enumerate(params):
-            if isinstance(p, float):
-                params[idx] = np.array([p])
-            elif (
-                isinstance(p, tuple) or isinstance(p, list) or isinstance(p, np.ndarray)
-            ):
-                params[idx] = np.array(p)
-            else:
-                raise ValueError("data type is not float or array_like object")
+        alpha, qv_low, qv_median, qv_high = _prep_qpd_params(
+            self, alpha, qv_low, qv_median, qv_high
+        )
 
-        alpha, qv_low, qv_median, qv_high = params[:]
         if index is None:
             index = pd.RangeIndex(qv_low.shape[0])
             self.index = index
 
         if columns is None:
             columns = pd.RangeIndex(1)
             self.columns = columns
@@ -471,14 +457,16 @@
             "alpha": 0.2,
             "version": "normal",
             "qv_low": 0.2,
             "qv_median": 0.5,
             "qv_high": 0.8,
             "lower": 0.0,
             "upper": 1.0,
+            "index": pd.Index([1, 2, 5]),
+            "columns": pd.Index(["a"]),
         }
         params2 = {
             "alpha": 0.2,
             "version": "normal",
             "qv_low": [0.2, 0.2, 0.2],
             "qv_median": [0.5, 0.5, 0.5],
             "qv_high": [0.8, 0.8, 0.8],
@@ -505,17 +493,17 @@
         lower quantile of SPT (upper is ``1 - alpha``)
     qv_low : float or array_like[float]
         quantile function value of ``alpha``
     qv_median : float or array_like[float]
         quantile function value of quantile 0.5
     qv_high : float or array_like[float]
         quantile function value of quantile ``1 - alpha``
-    version: str
+    version: str, optional, default="normal"
         options are ``normal`` (default) or ``logistic``
-    dist_shape: str
+    dist_shape: float, optional, default=0.0
         parameter modifying the logistic base distribution via
         sinh/arcsinh-scaling (only active in sinhlogistic version)
 
     Example
     -------
     >>> from skpro.distributions.qpd import QPD_U  # doctest: +SKIP
 
@@ -533,16 +521,16 @@
         # packaging info
         # --------------
         "authors": ["setoguchi-naoki", "felix-wick"],
         "maintainers": ["setoguchi-naoki"],
         "python_dependencies": "cyclic_boosting>=1.2.5",
         # estimator tags
         # --------------
-        "capabilities:approx": [],
-        "capabilities:exact": ["mean", "var", "cdf", "ppf"],
+        "capabilities:approx": ["pdfnorm", "energy"],
+        "capabilities:exact": ["mean", "var", "cdf", "ppf", "pdf", "log_pdf"],
         "distr:measuretype": "continuous",
     }
 
     def __init__(
         self,
         alpha: float,
         qv_low: float or object,
@@ -563,26 +551,18 @@
         self.index = index
         self.columns = columns
 
         super().__init__(index=index, columns=columns)
 
         from cyclic_boosting.quantile_matching import J_QPD_extended_U
 
-        params = [alpha, qv_low, qv_median, qv_high]
-        for idx, p in enumerate(params):
-            if isinstance(p, float):
-                params[idx] = np.array([p])
-            elif (
-                isinstance(p, tuple) or isinstance(p, list) or isinstance(p, np.ndarray)
-            ):
-                params[idx] = np.array(p)
-            else:
-                raise ValueError("data type is not float or array_like object")
+        alpha, qv_low, qv_median, qv_high = _prep_qpd_params(
+            self, alpha, qv_low, qv_median, qv_high
+        )
 
-        alpha, qv_low, qv_median, qv_high = params[:]
         if index is None:
             index = pd.RangeIndex(qv_low.shape[0])
             self.index = index
 
         if columns is None:
             columns = pd.RangeIndex(1)
             self.columns = columns
@@ -698,14 +678,16 @@
         """Return testing parameter settings for the estimator."""
         params1 = {
             "alpha": 0.2,
             "version": "normal",
             "qv_low": 0.2,
             "qv_median": 0.5,
             "qv_high": 0.8,
+            "index": pd.Index([1, 2, 5]),
+            "columns": pd.Index(["a"]),
         }
         params2 = {
             "alpha": 0.2,
             "version": "normal",
             "qv_low": [0.2, 0.2, 0.2],
             "qv_median": [0.5, 0.5, 0.5],
             "qv_high": [0.8, 0.8, 0.8],
@@ -723,7 +705,20 @@
 
 
 def var_func(x, mu, qpd):
     """Return Variance."""
     # TODO: scipy.integrate will be removed in scipy 1.12.0
     pdf = derivative(qpd.cdf, x, dx=1e-6)
     return ((x - mu) ** 2) * pdf
+
+
+def _prep_qpd_params(self, alpha, qv_low, qv_median, qv_high):
+    """Prepare parameters for Johnson Quantile-Parameterized Distributions."""
+    if not isinstance(alpha, np.ndarray):
+        alpha = np.array([alpha])
+    qv_low, qv_median, qv_high = BaseDistribution._get_bc_params(
+        self, qv_low, qv_median, qv_high, oned_as="col"
+    )
+    qv_low = qv_low.flatten()
+    qv_median = qv_median.flatten()
+    qv_high = qv_high.flatten()
+    return alpha, qv_low, qv_median, qv_high
```

### Comparing `skpro-2.2.1/skpro/distributions/t.py` & `skpro-2.2.2/skpro/distributions/t.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/distributions/tests/test_all_distrs.py` & `skpro-2.2.2/skpro/distributions/tests/test_all_distrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,33 @@
 
 
 class TestAllDistributions(PackageConfig, DistributionFixtureGenerator, QuickTester):
     """Module level tests for all skpro parameter fitters."""
 
     # TEMPORARY skip for CyclicBoosting and QPD classes
     # due to silent failures on main, se #190
-    exclude_objects = ["QPD_S", "QPD_B", "QPD_U"]
+    exclude_objects = ["QPD_B"]
     # remove this when fixing failures to re-enable testing
 
+    def test_shape(self, object_instance):
+        """Test index, columns, len and shape of distribution."""
+        d = object_instance
+
+        assert isinstance(d.index, pd.Index)
+        assert isinstance(d.columns, pd.Index)
+
+        assert isinstance(d.shape, tuple)
+        assert len(d.shape) == 2
+
+        assert d.shape[0] == len(d.index)
+        assert d.shape[1] == len(d.columns)
+
+        assert isinstance(len(d), int)
+        assert len(d) == d.shape[0]
+
     @pytest.mark.parametrize("shuffled", [False, True])
     def test_sample(self, object_instance, shuffled):
         """Test sample expected return."""
         d = object_instance
 
         if shuffled:
             d = _shuffle_distr(d)
```

### Comparing `skpro-2.2.1/skpro/distributions/tests/test_base_default_methods.py` & `skpro-2.2.2/skpro/distributions/tests/test_base_default_methods.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/distributions/tests/test_qpd.py` & `skpro-2.2.2/skpro/distributions/tests/test_qpd.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/metrics/__init__.py` & `skpro-2.2.2/skpro/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/metrics/_classes.py` & `skpro-2.2.2/skpro/metrics/_classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -232,17 +232,17 @@
 class LogLoss(BaseDistrMetric):
     r"""Logarithmic loss for distributional predictions.
 
     For a predictive distribution :math:`d` with pdf :math:`p_d`
     and a ground truth value :math:`y`, the logarithmic loss is
     defined as :math:`L(y, d) := -\log p_d(y)`.
 
-    `evaluate` computes the average test sample loss.
-    `evaluate_by_index` produces the loss sample by test data point
-    `multivariate` controls averaging over variables.
+    * ``evaluate`` computes the average test sample loss.
+    * ``evaluate_by_index`` produces the loss sample by test data point.
+    * ``multivariate`` controls averaging over variables.
 
     Parameters
     ----------
     multioutput : {'raw_values', 'uniform_average'} or array-like of shape \
             (n_outputs,), default='uniform_average'
         Defines whether and how to aggregate metric for across variables.
         If 'uniform_average' (default), errors are mean-averaged across variables.
@@ -264,27 +264,34 @@
         # replace this by multivariate log_pdf once distr implements
         # i.e., pass multivariate on to log_pdf
         if self.multivariate:
             return pd.DataFrame(res.mean(axis=1), columns=["density"])
         else:
             return res
 
+    @classmethod
+    def get_test_params(cls, parameter_set="default"):
+        """Retrieve test parameters."""
+        params1 = {}
+        params2 = {"multivariate": True}
+        return [params1, params2]
+
 
 class LinearizedLogLoss(BaseDistrMetric):
     r"""Lineararized logarithmic loss for distributional predictions.
 
     For a predictive distribution :math:`d` with pdf :math:`p_d`
     and a ground truth value :math:`y`, the linearized logarithmic loss is
     defined as :math:`L(y, d) := -\log p_d(y)` if :math:`p_d(y) \geq r`,
     and :math:`L(y, d) := -\log p_d(r) + 1 - \frac{1}{r} p_d(r)` otherwise,
     where :math:`r` is the range of linearization parameter, `range` below.
 
-    `evaluate` computes the average test sample loss.
-    `evaluate_by_index` produces the loss sample by test data point
-    `multivariate` controls averaging over variables.
+    * ``evaluate`` computes the average test sample loss.
+    * ``evaluate_by_index`` produces the loss sample by test data point.
+    * ``multivariate`` controls averaging over variables.
 
     Parameters
     ----------
     range : positive float, optional, default=1
         range of linearization, i.e., where to linearize the log-loss
         for values smaller than range, the log-loss is linearized
     multioutput : {'raw_values', 'uniform_average'} or array-like of shape \
@@ -343,17 +350,17 @@
       point prediction loss commonly known as the mean squared error
 
     For a predictive distribution :math:`d`
     and a ground truth value :math:`y`, the squared (distribution) loss is
     defined as :math:`L(y, d) := -2 p_d(y) + \|p_d\|^2`,
     where :math:`\|p_d\|^2` is the (function) L2-norm of :math:`p_d`.
 
-    `evaluate` computes the average test sample loss.
-    `evaluate_by_index` produces the loss sample by test data point
-    `multivariate` controls averaging over variables.
+    * ``evaluate`` computes the average test sample loss.
+    * ``evaluate_by_index`` produces the loss sample by test data point.
+    * ``multivariate`` controls averaging over variables.
 
     Parameters
     ----------
     multioutput : {'raw_values', 'uniform_average'} or array-like of shape \
             (n_outputs,), default='uniform_average'
         Defines whether and how to aggregate metric for across variables.
         If 'uniform_average' (default), errors are mean-averaged across variables.
@@ -375,47 +382,61 @@
         # replace this by multivariate log_pdf once distr implements
         # i.e., pass multivariate on to log_pdf
         if self.multivariate:
             return pd.DataFrame(res.mean(axis=1), columns=["density"])
         else:
             return res
 
+    @classmethod
+    def get_test_params(cls, parameter_set="default"):
+        """Retrieve test parameters."""
+        params1 = {}
+        params2 = {"multivariate": True}
+        return [params1, params2]
+
 
 class CRPS(BaseDistrMetric):
     r"""Continuous rank probability score for distributional predictions.
 
     Also known as:
 
     * integrated squared loss (ISL)
     * integrated Brier loss (IBL)
     * energy loss
 
     For a predictive distribution :math:`d` and a ground truth value :math:`y`,
     the CRPS is defined as
-    :math:`L(y, d) := \mathbb{E}_{Y \sim d}|Y-y| - \frac{1}{2} \mathbb{E}_{X,Y \sim d}|X-Y|`.  # noqa: E501
+    :math:`L(y, d) := \mathbb{E}_{Y \sim d}|Y-y| - \frac{1}{2} \mathbb{E}_{X,Y \sim d}|X-Y|`.
 
-    `evaluate` computes the average test sample loss.
-    `evaluate_by_index` produces the loss sample by test data point
-    `multivariate` controls averaging over variables.
+    * ``evaluate`` computes the average test sample loss.
+    * ``evaluate_by_index`` produces the loss sample by test data point.
+    * ``multivariate`` controls averaging over variables.
 
     Parameters
     ----------
     multioutput : {'raw_values', 'uniform_average'} or array-like of shape \
             (n_outputs,), default='uniform_average'
         Defines whether and how to aggregate metric for across variables.
         If 'uniform_average' (default), errors are mean-averaged across variables.
         If array-like, errors are weighted averaged across variables, values as weights.
         If 'raw_values', does not average errors across variables, columns are retained.
     multivariate : bool, optional, default=False
         if True, behaves as multivariate CRPS (sum of scores)
         CRPS is computed for entire row, results one score per row
         if False, is univariate log-loss, per variable
         CRPS is computed per variable marginal, results in many scores per row
-    """
+    """  # noqa: E501
 
     def __init__(self, multioutput="uniform_average", multivariate=False):
         self.multivariate = multivariate
         super().__init__(multioutput=multioutput)
 
     def _evaluate_by_index(self, y_true, y_pred, **kwargs):
         # CRPS(d, y) = E_X,Y as d [abs(Y-y) - 0.5 abs(X-Y)]
         return y_pred.energy(y_true) - y_pred.energy() / 2
+
+    @classmethod
+    def get_test_params(cls, parameter_set="default"):
+        """Retrieve test parameters."""
+        params1 = {}
+        params2 = {"multivariate": True}
+        return [params1, params2]
```

### Comparing `skpro-2.2.1/skpro/metrics/_coerce.py` & `skpro-2.2.2/skpro/metrics/_coerce.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/metrics/base.py` & `skpro-2.2.2/skpro/metrics/base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/metrics/survival/_c_harrell.py` & `skpro-2.2.2/skpro/metrics/survival/_c_harrell.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/metrics/survival/_spll.py` & `skpro-2.2.2/skpro/metrics/survival/_spll.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/metrics/survival/tests/test_c_harrell.py` & `skpro-2.2.2/skpro/metrics/survival/tests/test_c_harrell.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/metrics/tests/test_distr_metrics.py` & `skpro-2.2.2/skpro/metrics/tests/test_distr_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from skpro.distributions import Normal
 from skpro.tests.test_all_estimators import BaseFixtureGenerator, PackageConfig
 
 TEST_DISTS = [Normal]
 
 
 class TestAllDistrMetrics(PackageConfig, BaseFixtureGenerator, QuickTester):
-    """Generic tests for all regressors in the mini package."""
+    """Generic tests for all probabilistic regression metrics in the package."""
 
     # class variables which can be overridden by descendants
     # ------------------------------------------------------
 
     # which object types are generated; None=all, or scitype string
     # passed to skpro.registry.all_objects as object_type
     object_type_filter = "metric_distr"
```

### Comparing `skpro-2.2.1/skpro/metrics/tests/test_probabilistic_metrics.py` & `skpro-2.2.2/skpro/metrics/tests/test_probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/model_selection/_tuning.py` & `skpro-2.2.2/skpro/model_selection/_tuning.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/registry/_lookup.py` & `skpro-2.2.2/skpro/registry/_lookup.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/registry/_scitype.py` & `skpro-2.2.2/skpro/registry/_scitype.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/registry/_tags.py` & `skpro-2.2.2/skpro/registry/_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,21 @@
     (
         "python_dependencies_alias",
         "object",
         "dict",
         "should be provided if import name differs from package name, \
         key-value pairs are package name, import name",
     ),
+    (
+        "license_type",
+        "object",
+        "str",
+        "license type for interfaced packages: 'copyleft', 'permissive', 'copyright'. \
+        may be incorrect, NO LIABILITY assumed for this field",
+    ),
     # ------------------
     # BaseProbaRegressor
     # ------------------
     (
         "capability:survival",
         "regressor_proba",
         "bool",
```

### Comparing `skpro-2.2.1/skpro/registry/tests/test_scitype.py` & `skpro-2.2.2/skpro/registry/tests/test_scitype.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/registry/tests/test_tags.py` & `skpro-2.2.2/skpro/registry/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/adapters/sklearn/_sklearn_proba.py` & `skpro-2.2.2/skpro/regression/adapters/sklearn/_sklearn_proba.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/base/_base.py` & `skpro-2.2.2/skpro/regression/base/_base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/base/_delegate.py` & `skpro-2.2.2/skpro/regression/base/_delegate.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/base/adapters/_sklearn.py` & `skpro-2.2.2/skpro/regression/base/adapters/_sklearn.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/baselines/density.py` & `skpro-2.2.2/skpro/regression/baselines/density.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/bootstrap.py` & `skpro-2.2.2/skpro/regression/bootstrap.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/compose/_pipeline.py` & `skpro-2.2.2/skpro/regression/compose/_pipeline.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/cyclic_boosting.py` & `skpro-2.2.2/skpro/regression/cyclic_boosting.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/density.py` & `skpro-2.2.2/skpro/regression/density.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/ensemble.py` & `skpro-2.2.2/skpro/regression/ensemble.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/gp/_sklearn.py` & `skpro-2.2.2/skpro/regression/gp/_sklearn.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/linear/_sklearn.py` & `skpro-2.2.2/skpro/regression/linear/_sklearn.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/mapie.py` & `skpro-2.2.2/skpro/regression/mapie.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/multiquantile.py` & `skpro-2.2.2/skpro/regression/multiquantile.py`

 * *Files 5% similar despite different names*

```diff
@@ -289,43 +289,28 @@
             data to predict labels for
 
         Returns
         -------
         y : skpro BaseDistribution, same length as `X`
             labels predicted for `X`
         """
-        from skpro.distributions import Empirical
+        from skpro.distributions import QPD_Empirical
 
         alpha_sorted = sorted(self.alpha)
 
         # get quantile prediction for all fitted quantile regressors
         quantile_preds = self._predict_quantiles(X, alpha_sorted)
 
         # format as emprical sample for empirical distr
         # row multiindex: (alpha, X.index)
         # column index  : as y in fit
         empirical_spl = quantile_preds.stack(level=1).swaplevel(0, 1)
 
-        # obtain alpha weights for empirical distr such that we take the nearest
-        # available quantile prob (the cum weights match the chosen quantile prob)
-        alpha_np = np.array(alpha_sorted)
-        alpha_diff = np.diff(alpha_np)
-        alpha_diff2 = np.repeat(alpha_diff, 2) / 2
-        weight_double = np.concatenate([[alpha_np[0]], alpha_diff2, [1 - alpha_np[-1]]])
-        weight_double2 = weight_double.reshape(-1, 2)
-        weights = weight_double2.sum(axis=1)
-
-        # obtain weights per emprical sample
-        empirical_spl_weights = pd.Series(index=empirical_spl.index)
-        for i, a in enumerate(alpha_sorted):
-            empirical_spl_weights.loc[a] = weights[i]
-
-        y_pred_proba = Empirical(
+        y_pred_proba = QPD_Empirical(
             empirical_spl,
-            weights=empirical_spl_weights,
             index=X.index,
             columns=[self._y_varname],
         )
 
         return y_pred_proba
 
     @classmethod
```

### Comparing `skpro-2.2.1/skpro/regression/parametric/estimators.py` & `skpro-2.2.2/skpro/regression/parametric/estimators.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/parametric/parametric.py` & `skpro-2.2.2/skpro/regression/parametric/parametric.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/residual.py` & `skpro-2.2.2/skpro/regression/residual.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/tests/test_all_regressors.py` & `skpro-2.2.2/skpro/regression/tests/test_all_regressors.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/tests/test_cyclic_boosting.py` & `skpro-2.2.2/skpro/regression/tests/test_cyclic_boosting.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/regression/vendors/pymc.py` & `skpro-2.2.2/skpro/regression/vendors/pymc.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/survival/base.py` & `skpro-2.2.2/skpro/survival/base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/survival/compose/_reduce_cond_unc.py` & `skpro-2.2.2/skpro/survival/compose/_reduce_cond_unc.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class ConditionUncensored(BaseProbaRegressor):
     """Reduction to tabular probabilistic regression - conditioning on uncensored.
 
     Simple baseline reduction strategy for predictive survival analysis.
 
     Fits a probabilistic regressor on X padded with censoring information C,
-    in predict applies the fitted regressor to X padded with 0 (non-censord).
+    in predict applies the fitted regressor to X padded with 0 (non-censored).
 
     In ``fit``, passes column concat of ``X`` and ``C`` to ``regressor.fit``.
 
     In ``predict_[method]``, calls ``regressor.predict_[method]``
     on ``X`` with an additional ``C``-like column, padded with 0,
     and returns the result.
```

### Comparing `skpro-2.2.1/skpro/survival/compose/_reduce_uncensored.py` & `skpro-2.2.2/skpro/survival/compose/_reduce_uncensored.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/survival/coxph.py` & `skpro-2.2.2/skpro/survival/coxph/_coxph_statsmodels.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/tests/scenarios/scenarios.py` & `skpro-2.2.2/skpro/tests/scenarios/scenarios.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/tests/scenarios/scenarios_getter.py` & `skpro-2.2.2/skpro/tests/scenarios/scenarios_getter.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/tests/scenarios/scenarios_regressor_proba.py` & `skpro-2.2.2/skpro/tests/scenarios/scenarios_regressor_proba.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,54 +106,59 @@
 
     X, y = _load_diabetes_small()
     X_train, X_test, y_train, y_test = train_test_split(X, y)
 
     return X_train, X_test, y_train, y_test
 
 
-X_train, X_test, y_train, y_test = _get_Xy_traintest()
-C_train = pd.DataFrame(
-    np.random.choice([0, 1], size=len(y_train)),
-    index=y_train.index,
-    columns=y_train.columns,
-)
-
-
 class ProbaRegressorBasic(_ProbaRegressorTestScenario):
     """Fit/predict with multivariate pandas mtype (same dtype), and labels y."""
 
     _tags = {
         "X_univariate": False,
         "X_missing": False,
         "y_univariate": True,
         "is_enabled": True,
     }
 
-    args = {
-        "fit": {"X": X_train, "y": y_train},
-        "predict": {"X": X_test},
-    }
+    @property
+    def args(self):
+        X_train, X_test, y_train, _ = _get_Xy_traintest()
+        return {
+            "fit": {"X": X_train, "y": y_train},
+            "predict": {"X": X_test},
+        }
+
     default_method_sequence = ["fit", "predict", "predict_proba"]
     default_arg_sequence = ["fit", "predict", "predict"]
 
 
 class ProbaRegressorSurvival(_ProbaRegressorTestScenario):
     """Fit/predict with survival data, including a censoring dataset."""
 
     _tags = {
         "X_univariate": False,
         "X_missing": False,
         "y_univariate": True,
         "is_enabled": True,
     }
 
-    args = {
-        "fit": {"X": X_train, "y": y_train, "C": C_train},
-        "predict": {"X": X_test},
-    }
+    @property
+    def args(self):
+        X_train, X_test, y_train, _ = _get_Xy_traintest()
+        C_train = pd.DataFrame(
+            np.random.choice([0, 1], size=len(y_train)),
+            index=y_train.index,
+            columns=y_train.columns,
+        )
+        return {
+            "fit": {"X": X_train, "y": y_train, "C": C_train},
+            "predict": {"X": X_test},
+        }
+
     default_method_sequence = ["fit", "predict", "predict_proba"]
     default_arg_sequence = ["fit", "predict", "predict"]
 
 
 # as a function to ensure we can move to fixture-like structure later
 def _get_Xy_traintest_X_mixix_ynp():
     """Get X, y train/test data for regression tests.
@@ -178,31 +183,32 @@
     y = y.values
 
     X_train, X_test, y_train, y_test = train_test_split(X, y)
 
     return X_train, X_test, y_train, y_test
 
 
-X_train_mc, X_test_mc, y_train_mc, y_test_mc = _get_Xy_traintest_X_mixix_ynp()
-
-
 class ProbaRegressorXcolMixIxYnp(_ProbaRegressorTestScenario):
     """Fit/predict with multivariate pandas mtype, mixed col idx type."""
 
     _tags = {
         "X_univariate": False,
         "X_missing": False,
         "y_univariate": True,
         "is_enabled": True,
     }
 
-    args = {
-        "fit": {"X": X_train_mc, "y": y_train_mc},
-        "predict": {"X": X_test_mc},
-    }
+    @property
+    def args(self):
+        X_train_mc, X_test_mc, y_train_mc, _ = _get_Xy_traintest_X_mixix_ynp()
+        return {
+            "fit": {"X": X_train_mc, "y": y_train_mc},
+            "predict": {"X": X_test_mc},
+        }
+
     default_method_sequence = ["fit", "predict", "predict_proba"]
     default_arg_sequence = ["fit", "predict", "predict"]
 
 
 scenarios_regressor_proba = [
     ProbaRegressorBasic,
     ProbaRegressorXcolMixIxYnp,
```

### Comparing `skpro-2.2.1/skpro/tests/test_all_estimators.py` & `skpro-2.2.2/skpro/tests/test_all_estimators.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/tests/test_base.py` & `skpro-2.2.2/skpro/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/tests/test_baselines.py` & `skpro-2.2.2/skpro/tests/test_baselines.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/tests/test_class_register.py` & `skpro-2.2.2/skpro/tests/test_class_register.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/tests/test_density.py` & `skpro-2.2.2/skpro/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/tests/test_ensemble.py` & `skpro-2.2.2/skpro/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/tests/test_switch.py` & `skpro-2.2.2/skpro/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/tests/utils.py` & `skpro-2.2.2/skpro/tests/utils.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/_maint/_show_versions.py` & `skpro-2.2.2/skpro/utils/_maint/_show_versions.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/_maint/tests/test_show_versions.py` & `skpro-2.2.2/skpro/utils/_maint/tests/test_show_versions.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/deep_equals/_deep_equals.py` & `skpro-2.2.2/skpro/utils/deep_equals/_deep_equals.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/estimator_checks.py` & `skpro-2.2.2/skpro/utils/estimator_checks.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/git_diff.py` & `skpro-2.2.2/skpro/utils/git_diff.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/index.py` & `skpro-2.2.2/skpro/utils/index.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/numpy.py` & `skpro-2.2.2/skpro/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/pandas.py` & `skpro-2.2.2/skpro/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/parallel.py` & `skpro-2.2.2/skpro/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/plotting.py` & `skpro-2.2.2/skpro/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/random_state.py` & `skpro-2.2.2/skpro/utils/random_state.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/sklearn.py` & `skpro-2.2.2/skpro/utils/sklearn.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/tests/test_plots.py` & `skpro-2.2.2/skpro/utils/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/utils.py` & `skpro-2.2.2/skpro/utils/utils.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/utils/validation/_dependencies.py` & `skpro-2.2.2/skpro/utils/validation/_dependencies.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/workflow/base.py` & `skpro-2.2.2/skpro/workflow/base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/workflow/cross_validation.py` & `skpro-2.2.2/skpro/workflow/cross_validation.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/workflow/manager/data.py` & `skpro-2.2.2/skpro/workflow/manager/data.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/workflow/manager/models.py` & `skpro-2.2.2/skpro/workflow/manager/models.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/workflow/table/table.py` & `skpro-2.2.2/skpro/workflow/table/table.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro/workflow/utils.py` & `skpro-2.2.2/skpro/workflow/utils.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.1/skpro.egg-info/PKG-INFO` & `skpro-2.2.2/skpro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skpro
-Version: 2.2.1
+Version: 2.2.2
 Summary: A unified framework for probability distributions and probabilistic supervised regression
 Author: Franz Király, Frithjof Gressmann, Vitaly Davydov
 Author-email: skpro developers <sktime.toolbox@gmail.com>
 Maintainer: Franz Király, Frithjof Gressmann
 Maintainer-email: skpro developers <sktime.toolbox@gmail.com>
 Project-URL: Homepage, https://github.com/sktime/skpro
 Project-URL: Repository, https://github.com/sktime/skpro
@@ -37,19 +37,21 @@
 Requires-Dist: packaging
 Requires-Dist: scikit-base<0.8.0,>=0.6.1
 Requires-Dist: scikit-learn<1.5.0,>=0.24.0
 Requires-Dist: scipy<2.0.0,>=1.2.0
 Provides-Extra: all-extras
 Requires-Dist: attrs; extra == "all-extras"
 Requires-Dist: distfit; extra == "all-extras"
+Requires-Dist: lifelines<0.29.0; extra == "all-extras"
 Requires-Dist: mapie; extra == "all-extras"
 Requires-Dist: matplotlib>=3.3.2; extra == "all-extras"
 Requires-Dist: ngboost; extra == "all-extras"
 Requires-Dist: polars<0.21.0; extra == "all-extras"
 Requires-Dist: pyarrow<14.0.0; python_version < "3.12" and extra == "all-extras"
+Requires-Dist: scikit-survival<0.23.0; extra == "all-extras"
 Requires-Dist: statsmodels>=0.12.1; extra == "all-extras"
 Requires-Dist: tabulate; extra == "all-extras"
 Requires-Dist: uncertainties; extra == "all-extras"
 Requires-Dist: cyclic-boosting>=1.2.5; python_version < "3.12" and extra == "all-extras"
 Provides-Extra: dev
 Requires-Dist: backoff; extra == "dev"
 Requires-Dist: httpx; extra == "dev"
@@ -73,15 +75,15 @@
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.16.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 
 <a href="https://skpro.readthedocs.io/en/latest"><img src="https://github.com/sktime/skpro/blob/main/docs/source/images/skpro-banner.png" width="500" align="right" /></a>
 
-:rocket: **Version 2.2.1 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
+:rocket: **Version 2.2.2 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
 
 `skpro` is a library for supervised probabilistic prediction in python.
 It provides `scikit-learn`-like, `scikit-base` compatible interfaces to:
 
 * tabular **supervised regressors for probabilistic prediction** - interval, quantile and distribution predictions
 * tabular **probabilistic time-to-event and survival prediction** - instance-individual survival distributions
 * **metrics to evaluate probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS, survival losses
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skpro Version: 2.2.1 Summary: A unified framework
+Metadata-Version: 2.1 Name: skpro Version: 2.2.2 Summary: A unified framework
 for probability distributions and probabilistic supervised regression Author:
 Franz KirÃ¡ly, Frithjof Gressmann, Vitaly Davydov Author-email: skpro
 developers
 gmail.com> Maintainer: Franz KirÃ¡ly, Frithjof Gressmann Maintainer-email:
 skpro developers
 gmail.com> Project-URL: Homepage, https://github.com/sktime/skpro Project-URL:
 Repository, https://github.com/sktime/skpro Project-URL: Documentation, https:/
@@ -21,44 +21,45 @@
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Python: <3.13,>=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.txt License-File: AUTHORS.rst Requires-Dist: numpy<1.27,>=1.21.0
 Requires-Dist: pandas<2.3.0,>=1.1.0 Requires-Dist: packaging Requires-Dist:
 scikit-base<0.8.0,>=0.6.1 Requires-Dist: scikit-learn<1.5.0,>=0.24.0 Requires-
 Dist: scipy<2.0.0,>=1.2.0 Provides-Extra: all-extras Requires-Dist: attrs;
 extra == "all-extras" Requires-Dist: distfit; extra == "all-extras" Requires-
-Dist: mapie; extra == "all-extras" Requires-Dist: matplotlib>=3.3.2; extra ==
-"all-extras" Requires-Dist: ngboost; extra == "all-extras" Requires-Dist:
-polars<0.21.0; extra == "all-extras" Requires-Dist: pyarrow<14.0.0;
-python_version < "3.12" and extra == "all-extras" Requires-Dist:
-statsmodels>=0.12.1; extra == "all-extras" Requires-Dist: tabulate; extra ==
-"all-extras" Requires-Dist: uncertainties; extra == "all-extras" Requires-Dist:
-cyclic-boosting>=1.2.5; python_version < "3.12" and extra == "all-extras"
-Provides-Extra: dev Requires-Dist: backoff; extra == "dev" Requires-Dist:
-httpx; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
-pytest; extra == "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist:
-pytest-randomly; extra == "dev" Requires-Dist: pytest-timeout; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev" Requires-Dist: wheel; extra ==
-"dev" Provides-Extra: binder Requires-Dist: jupyter; extra == "binder"
-Provides-Extra: docs Requires-Dist: jupyter; extra == "docs" Requires-Dist:
-myst-parser; extra == "docs" Requires-Dist: nbsphinx>=0.8.6; extra == "docs"
-Requires-Dist: numpydoc; extra == "docs" Requires-Dist: pydata-sphinx-theme;
-extra == "docs" Requires-Dist: sphinx!=7.2.0,<8.0.0; extra == "docs" Requires-
-Dist: sphinx-design<0.6.0; extra == "docs" Requires-Dist: sphinx-issues<5.0.0;
-extra == "docs" Requires-Dist: sphinx-gallery<0.16.0; extra == "docs" Requires-
-Dist: sphinx-panels; extra == "docs" Requires-Dist: tabulate; extra == "docs"
-_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-
-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.2.1 out now!** [Read the release notes here.]
-(https://skpro.readthedocs.io/en/latest/changelog.html). `skpro` is a library
-for supervised probabilistic prediction in python. It provides `scikit-learn`-
-like, `scikit-base` compatible interfaces to: * tabular **supervised regressors
-for probabilistic prediction** - interval, quantile and distribution
-predictions * tabular **probabilistic time-to-event and survival prediction** -
-instance-individual survival distributions * **metrics to evaluate
-probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS,
-survival losses * **reductions** to turn `scikit-learn` regressors into
+Dist: lifelines<0.29.0; extra == "all-extras" Requires-Dist: mapie; extra ==
+"all-extras" Requires-Dist: matplotlib>=3.3.2; extra == "all-extras" Requires-
+Dist: ngboost; extra == "all-extras" Requires-Dist: polars<0.21.0; extra ==
+"all-extras" Requires-Dist: pyarrow<14.0.0; python_version < "3.12" and extra
+== "all-extras" Requires-Dist: scikit-survival<0.23.0; extra == "all-extras"
+Requires-Dist: statsmodels>=0.12.1; extra == "all-extras" Requires-Dist:
+tabulate; extra == "all-extras" Requires-Dist: uncertainties; extra == "all-
+extras" Requires-Dist: cyclic-boosting>=1.2.5; python_version < "3.12" and
+extra == "all-extras" Provides-Extra: dev Requires-Dist: backoff; extra ==
+"dev" Requires-Dist: httpx; extra == "dev" Requires-Dist: pre-commit; extra ==
+"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra ==
+"dev" Requires-Dist: pytest-randomly; extra == "dev" Requires-Dist: pytest-
+timeout; extra == "dev" Requires-Dist: pytest-xdist; extra == "dev" Requires-
+Dist: wheel; extra == "dev" Provides-Extra: binder Requires-Dist: jupyter;
+extra == "binder" Provides-Extra: docs Requires-Dist: jupyter; extra == "docs"
+Requires-Dist: myst-parser; extra == "docs" Requires-Dist: nbsphinx>=0.8.6;
+extra == "docs" Requires-Dist: numpydoc; extra == "docs" Requires-Dist: pydata-
+sphinx-theme; extra == "docs" Requires-Dist: sphinx!=7.2.0,<8.0.0; extra ==
+"docs" Requires-Dist: sphinx-design<0.6.0; extra == "docs" Requires-Dist:
+sphinx-issues<5.0.0; extra == "docs" Requires-Dist: sphinx-gallery<0.16.0;
+extra == "docs" Requires-Dist: sphinx-panels; extra == "docs" Requires-Dist:
+tabulate; extra == "docs" _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/
+_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.2.2 out now!** [Read the
+release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
+`skpro` is a library for supervised probabilistic prediction in python. It
+provides `scikit-learn`-like, `scikit-base` compatible interfaces to: * tabular
+**supervised regressors for probabilistic prediction** - interval, quantile and
+distribution predictions * tabular **probabilistic time-to-event and survival
+prediction** - instance-individual survival distributions * **metrics to
+evaluate probabilistic predictions**, e.g., pinball loss, empirical coverage,
+CRPS, survival losses * **reductions** to turn `scikit-learn` regressors into
 probabilistic `skpro` regressors, such as bootstrap or conformal * building
 **pipelines and composite models**, including tuning via probabilistic
 performance metrics * symbolic **probability distributions** with value domain
 of `pandas.DataFrame`-s and `pandas`-like interface | Overview | | |---|---| |
 **Open Source** | [![BSD 3-clause](https://img.shields.io/badge/License-
 BSD%203--Clause-blue.svg)](https://github.com/sktime/sktime/blob/main/LICENSE)
 | | **Tutorials** | [![Binder](https://mybinder.org/badge_logo.svg)](https://
```

### Comparing `skpro-2.2.1/skpro.egg-info/SOURCES.txt` & `skpro-2.2.2/skpro.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -52,28 +52,36 @@
 skpro/datatypes/_table/_registry.py
 skpro/datatypes/tests/__init__.py
 skpro/datatypes/tests/test_check.py
 skpro/datatypes/tests/test_convert.py
 skpro/datatypes/tests/test_convert_to.py
 skpro/datatypes/tests/test_lookup.py
 skpro/distributions/__init__.py
-skpro/distributions/base.py
 skpro/distributions/empirical.py
+skpro/distributions/fisk.py
 skpro/distributions/laplace.py
+skpro/distributions/logistic.py
+skpro/distributions/lognormal.py
 skpro/distributions/mixture.py
 skpro/distributions/normal.py
+skpro/distributions/poisson.py
 skpro/distributions/qpd.py
+skpro/distributions/qpd_empirical.py
 skpro/distributions/t.py
+skpro/distributions/weibull.py
 skpro/distributions/adapters/__init__.py
 skpro/distributions/adapters/scipy/__init__.py
 skpro/distributions/adapters/scipy/_empirical.py
 skpro/distributions/adapters/scipy/tests/__init__.py
 skpro/distributions/adapters/scipy/tests/test_scipy_adapters.py
 skpro/distributions/adapters/statsmodels/__init__.py
 skpro/distributions/adapters/statsmodels/_empirical.py
+skpro/distributions/base/__init__.py
+skpro/distributions/base/_base.py
+skpro/distributions/base/_delegate.py
 skpro/distributions/tests/__init__.py
 skpro/distributions/tests/test_all_distrs.py
 skpro/distributions/tests/test_base_default_methods.py
 skpro/distributions/tests/test_proba_basic.py
 skpro/distributions/tests/test_qpd.py
 skpro/metrics/__init__.py
 skpro/metrics/_classes.py
@@ -115,29 +123,49 @@
 skpro/regression/baselines/__init__.py
 skpro/regression/baselines/density.py
 skpro/regression/compose/__init__.py
 skpro/regression/compose/_pipeline.py
 skpro/regression/gp/__init__.py
 skpro/regression/gp/_sklearn.py
 skpro/regression/linear/__init__.py
+skpro/regression/linear/_glm.py
 skpro/regression/linear/_sklearn.py
 skpro/regression/parametric/__init__.py
 skpro/regression/parametric/estimators.py
 skpro/regression/parametric/parametric.py
 skpro/regression/tests/__init__.py
 skpro/regression/tests/test_all_regressors.py
 skpro/regression/tests/test_cyclic_boosting.py
 skpro/regression/vendors/__init__.py
 skpro/regression/vendors/pymc.py
 skpro/survival/__init__.py
 skpro/survival/base.py
-skpro/survival/coxph.py
+skpro/survival/adapters/__init__.py
+skpro/survival/adapters/_common.py
+skpro/survival/adapters/lifelines.py
+skpro/survival/adapters/sksurv.py
+skpro/survival/additive/__init__.py
+skpro/survival/additive/_aalen_lifelines.py
+skpro/survival/aft/__init__.py
+skpro/survival/aft/_aft_lifelines_fisk.py
+skpro/survival/aft/_aft_lifelines_lognormal.py
+skpro/survival/aft/_aft_lifelines_weibull.py
 skpro/survival/compose/__init__.py
 skpro/survival/compose/_reduce_cond_unc.py
 skpro/survival/compose/_reduce_uncensored.py
+skpro/survival/coxph/__init__.py
+skpro/survival/coxph/_coxnet_sksurv.py
+skpro/survival/coxph/_coxph_lifelines.py
+skpro/survival/coxph/_coxph_sksurv.py
+skpro/survival/coxph/_coxph_statsmodels.py
+skpro/survival/ensemble/__init__.py
+skpro/survival/ensemble/_grad_boost_sksurv.py
+skpro/survival/ensemble/_survforest_sksurv.py
+skpro/survival/tree/__init__.py
+skpro/survival/tree/_tree_sksurv.py
 skpro/tests/__init__.py
 skpro/tests/test_all_estimators.py
 skpro/tests/test_base.py
 skpro/tests/test_baselines.py
 skpro/tests/test_class_register.py
 skpro/tests/test_density.py
 skpro/tests/test_ensemble.py
```

### Comparing `skpro-2.2.1/skpro.egg-info/requires.txt` & `skpro-2.2.2/skpro.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 scikit-base<0.8.0,>=0.6.1
 scikit-learn<1.5.0,>=0.24.0
 scipy<2.0.0,>=1.2.0
 
 [all_extras]
 attrs
 distfit
+lifelines<0.29.0
 mapie
 matplotlib>=3.3.2
 ngboost
 polars<0.21.0
+scikit-survival<0.23.0
 statsmodels>=0.12.1
 tabulate
 uncertainties
 
 [all_extras:python_version < "3.12"]
 pyarrow<14.0.0
 cyclic-boosting>=1.2.5
```

