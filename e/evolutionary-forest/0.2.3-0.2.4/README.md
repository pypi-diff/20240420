# Comparing `tmp/evolutionary_forest-0.2.3.tar.gz` & `tmp/evolutionary_forest-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evolutionary_forest-0.2.3.tar", last modified: Wed Dec 13 23:09:35 2023, max compression
+gzip compressed data, was "evolutionary_forest-0.2.4.tar", last modified: Sat Apr 20 10:05:16 2024, max compression
```

## Comparing `evolutionary_forest-0.2.3.tar` & `evolutionary_forest-0.2.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-12-13 23:09:35.084510 evolutionary_forest-0.2.3/
--rw-rw-rw-   0        0        0      174 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/AUTHORS.rst
--rw-rw-rw-   0        0        0     3786 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/HISTORY.rst
--rw-rw-rw-   0        0        0     7817 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      273 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6126 2023-12-13 23:09:35.084510 evolutionary_forest-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     5215 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-12-13 23:09:35.014856 evolutionary_forest-0.2.3/docs/
--rw-rw-rw-   0        0        0      640 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/docs/authors.rst
--rw-rw-rw-   0        0        0     5107 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/docs/conf.py
--rw-rw-rw-   0        0        0    35548 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/docs/constructed_features.png
--rw-rw-rw-   0        0        0       34 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/docs/history.rst
--rw-rw-rw-   0        0        0      336 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/docs/index.rst
--rw-rw-rw-   0        0        0     1269 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/docs/installation.rst
--rwxrwxrwx   0        0        0      817 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/docs/readme.rst
--rw-rw-rw-   0        0        0      100 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-12-13 23:09:35.026191 evolutionary_forest-0.2.3/evolutionary_forest/
--rw-rw-rw-   0        0        0      147 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-13 23:09:35.039567 evolutionary_forest-0.2.3/evolutionary_forest/application/
--rw-rw-rw-   0        0        0        0 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/application/__init__.py
--rw-rw-rw-   0        0        0     2201 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/application/baes_class.py
--rw-rw-rw-   0        0        0     6086 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/application/expensive_benchmark.py
--rw-rw-rw-   0        0        0      927 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/application/gp_function_test.py
-drwxrwxrwx   0        0        0        0 2023-12-13 23:09:35.064999 evolutionary_forest-0.2.3/evolutionary_forest/component/
--rw-rw-rw-   0        0        0        0 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/__init__.py
--rw-rw-rw-   0        0        0    23442 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/archive.py
--rw-rw-rw-   0        0        0     8426 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/configuration.py
--rw-rw-rw-   0        0        0    13410 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/crossover_mutation.py
--rw-rw-rw-   0        0        0    28649 2023-11-18 06:40:12.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/evaluation.py
--rw-rw-rw-   0        0        0     6840 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/generation.py
--rw-rw-rw-   0        0        0    16237 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/mutation_transformer.py
--rw-rw-rw-   0        0        0     8844 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/pac_bayesian.py
--rw-rw-rw-   0        0        0     9958 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/primitives.py
--rw-rw-rw-   0        0        0     5598 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/rademacher_complexity.py
--rw-rw-rw-   0        0        0    34616 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/selection.py
--rw-rw-rw-   0        0        0     3535 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/stateful_gp.py
--rw-rw-rw-   0        0        0     4546 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/subset_selection.py
--rw-rw-rw-   0        0        0     3645 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/syntax_tools.py
--rw-rw-rw-   0        0        0      839 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/toolbox.py
--rw-rw-rw-   0        0        0    14885 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/translation_transformer.py
--rw-rw-rw-   0        0        0     2989 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/tree_utils.py
--rw-rw-rw-   0        0        0     4614 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/component/vc_dimension.py
--rw-rw-rw-   0        0        0   262919 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/forest.py
-drwxrwxrwx   0        0        0        0 2023-12-13 23:09:35.071075 evolutionary_forest-0.2.3/evolutionary_forest/model/
--rw-rw-rw-   0        0        0    24048 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/model/PLTree.py
--rw-rw-rw-   0        0        0     2586 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/model/RBFN.py
--rw-rw-rw-   0        0        0      221 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/model/SafetyLR.py
--rw-rw-rw-   0        0        0     1414 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/model/SafetyScaler.py
--rw-rw-rw-   0        0        0     2847 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/model/VAE.py
--rw-rw-rw-   0        0        0        0 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/model/__init__.py
--rw-rw-rw-   0        0        0    54133 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/multigene_gp.py
--rw-rw-rw-   0        0        0     3864 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/preprocess_utils.py
--rw-rw-rw-   0        0        0     5494 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/probability_gp.py
--rw-rw-rw-   0        0        0     2162 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/pruning.py
--rw-rw-rw-   0        0        0    10933 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/sklearn_utils.py
-drwxrwxrwx   0        0        0        0 2023-12-13 23:09:35.081513 evolutionary_forest-0.2.3/evolutionary_forest/strategies/
--rw-rw-rw-   0        0        0        0 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/strategies/__init__.py
--rw-rw-rw-   0        0        0     1121 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/strategies/adaptive_rate.py
--rw-rw-rw-   0        0        0    22230 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/strategies/estimation_of_distribution.py
--rw-rw-rw-   0        0        0     2072 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/strategies/multiarm_bandit.py
--rw-rw-rw-   0        0        0      274 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/strategies/prune_strategy.py
--rw-rw-rw-   0        0        0     5037 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/strategies/space_partition.py
--rw-rw-rw-   0        0        0    10393 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/strategies/surrogate_model.py
--rw-rw-rw-   0        0        0    14125 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/evolutionary_forest/utils.py
-drwxrwxrwx   0        0        0        0 2023-12-13 23:09:35.033261 evolutionary_forest-0.2.3/evolutionary_forest.egg-info/
--rw-rw-rw-   0        0        0     6126 2023-12-13 23:09:34.000000 evolutionary_forest-0.2.3/evolutionary_forest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2476 2023-12-13 23:09:34.000000 evolutionary_forest-0.2.3/evolutionary_forest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-13 23:09:34.000000 evolutionary_forest-0.2.3/evolutionary_forest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-12-13 23:09:34.000000 evolutionary_forest-0.2.3/evolutionary_forest.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      181 2023-12-13 23:09:34.000000 evolutionary_forest-0.2.3/evolutionary_forest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-12-13 23:09:34.000000 evolutionary_forest-0.2.3/evolutionary_forest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      490 2023-12-13 23:09:35.086033 evolutionary_forest-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1897 2023-12-13 23:09:32.000000 evolutionary_forest-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-13 23:09:35.084510 evolutionary_forest-0.2.3/tests/
--rw-rw-rw-   0        0        0       50 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/tests/__init__.py
--rw-rw-rw-   0        0        0      736 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.3/tests/test_evolutionary_forest.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:05:16.430129 evolutionary_forest-0.2.4/
+-rw-rw-rw-   0        0        0      174 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3786 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/HISTORY.rst
+-rw-rw-rw-   0        0        0     7817 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6126 2024-04-20 10:05:16.431132 evolutionary_forest-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5215 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-20 10:05:16.312640 evolutionary_forest-0.2.4/docs/
+-rw-rw-rw-   0        0        0      640 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/docs/authors.rst
+-rw-rw-rw-   0        0        0     5107 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/docs/conf.py
+-rw-rw-rw-   0        0        0    35548 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/docs/constructed_features.png
+-rw-rw-rw-   0        0        0       34 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/docs/history.rst
+-rw-rw-rw-   0        0        0      336 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/docs/index.rst
+-rw-rw-rw-   0        0        0     1269 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/docs/installation.rst
+-rwxrwxrwx   0        0        0      817 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/docs/readme.rst
+-rw-rw-rw-   0        0        0      100 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2024-04-20 10:05:16.333681 evolutionary_forest-0.2.4/evolutionary_forest/
+-rw-rw-rw-   0        0        0      152 2024-03-06 02:18:19.000000 evolutionary_forest-0.2.4/evolutionary_forest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:05:16.354674 evolutionary_forest-0.2.4/evolutionary_forest/application/
+-rw-rw-rw-   0        0        0        0 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/application/__init__.py
+-rw-rw-rw-   0        0        0     2201 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/application/baes_class.py
+-rw-rw-rw-   0        0        0     6086 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/application/expensive_benchmark.py
+-rw-rw-rw-   0        0        0      927 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/application/gp_function_test.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:05:16.393040 evolutionary_forest-0.2.4/evolutionary_forest/component/
+-rw-rw-rw-   0        0        0        0 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/__init__.py
+-rw-rw-rw-   0        0        0    23442 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/archive.py
+-rw-rw-rw-   0        0        0     8426 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/configuration.py
+-rw-rw-rw-   0        0        0    13410 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/crossover_mutation.py
+-rw-rw-rw-   0        0        0    28649 2023-11-18 06:40:12.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/evaluation.py
+-rw-rw-rw-   0        0        0     6840 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/generation.py
+-rw-rw-rw-   0        0        0    16237 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/mutation_transformer.py
+-rw-rw-rw-   0        0        0     8844 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/pac_bayesian.py
+-rw-rw-rw-   0        0        0     9958 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/primitives.py
+-rw-rw-rw-   0        0        0     5598 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/rademacher_complexity.py
+-rw-rw-rw-   0        0        0    34616 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/selection.py
+-rw-rw-rw-   0        0        0     3535 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/stateful_gp.py
+-rw-rw-rw-   0        0        0     4546 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/subset_selection.py
+-rw-rw-rw-   0        0        0     3645 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/syntax_tools.py
+-rw-rw-rw-   0        0        0      839 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/toolbox.py
+-rw-rw-rw-   0        0        0    14885 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/translation_transformer.py
+-rw-rw-rw-   0        0        0     2989 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/tree_utils.py
+-rw-rw-rw-   0        0        0     4614 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/component/vc_dimension.py
+-rw-rw-rw-   0        0        0   262919 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/forest.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:05:16.406561 evolutionary_forest-0.2.4/evolutionary_forest/model/
+-rw-rw-rw-   0        0        0    24048 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/model/PLTree.py
+-rw-rw-rw-   0        0        0     2586 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/model/RBFN.py
+-rw-rw-rw-   0        0        0      221 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/model/SafetyLR.py
+-rw-rw-rw-   0        0        0     1414 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/model/SafetyScaler.py
+-rw-rw-rw-   0        0        0     2847 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/model/VAE.py
+-rw-rw-rw-   0        0        0        0 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/model/__init__.py
+-rw-rw-rw-   0        0        0    54133 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/multigene_gp.py
+-rw-rw-rw-   0        0        0     3864 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/preprocess_utils.py
+-rw-rw-rw-   0        0        0     5494 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/probability_gp.py
+-rw-rw-rw-   0        0        0     2162 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/pruning.py
+-rw-rw-rw-   0        0        0    10819 2024-03-06 02:17:40.000000 evolutionary_forest-0.2.4/evolutionary_forest/sklearn_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:05:16.421116 evolutionary_forest-0.2.4/evolutionary_forest/strategies/
+-rw-rw-rw-   0        0        0        0 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/strategies/__init__.py
+-rw-rw-rw-   0        0        0     1121 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/strategies/adaptive_rate.py
+-rw-rw-rw-   0        0        0    22230 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/strategies/estimation_of_distribution.py
+-rw-rw-rw-   0        0        0     2072 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/strategies/multiarm_bandit.py
+-rw-rw-rw-   0        0        0      274 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/strategies/prune_strategy.py
+-rw-rw-rw-   0        0        0     5037 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/strategies/space_partition.py
+-rw-rw-rw-   0        0        0    10393 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/strategies/surrogate_model.py
+-rw-rw-rw-   0        0        0    14125 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/evolutionary_forest/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:05:16.346947 evolutionary_forest-0.2.4/evolutionary_forest.egg-info/
+-rw-rw-rw-   0        0        0     6126 2024-04-20 10:05:15.000000 evolutionary_forest-0.2.4/evolutionary_forest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2476 2024-04-20 10:05:16.000000 evolutionary_forest-0.2.4/evolutionary_forest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 10:05:15.000000 evolutionary_forest-0.2.4/evolutionary_forest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-12-13 23:09:34.000000 evolutionary_forest-0.2.4/evolutionary_forest.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      181 2024-04-20 10:05:15.000000 evolutionary_forest-0.2.4/evolutionary_forest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-20 10:05:15.000000 evolutionary_forest-0.2.4/evolutionary_forest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      490 2024-04-20 10:05:16.435660 evolutionary_forest-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1899 2024-03-06 02:18:40.000000 evolutionary_forest-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:05:16.426131 evolutionary_forest-0.2.4/tests/
+-rw-rw-rw-   0        0        0       50 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      736 2023-11-18 06:39:15.000000 evolutionary_forest-0.2.4/tests/test_evolutionary_forest.py
```

### Comparing `evolutionary_forest-0.2.3/CONTRIBUTING.rst` & `evolutionary_forest-0.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/LICENSE` & `evolutionary_forest-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/PKG-INFO` & `evolutionary_forest-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evolutionary_forest
-Version: 0.2.3
+Version: 0.2.4
 Summary: An open source python library for automated feature engineering based on Genetic Programming
 Home-page: https://github.com/zhenlingcn/evolutionary_forest
 Author: Hengzhe Zhang
 Author-email: zhenlingcn@foxmail.com
 License: BSD license
 Keywords: evolutionary_forest
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `evolutionary_forest-0.2.3/README.rst` & `evolutionary_forest-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/docs/Makefile` & `evolutionary_forest-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/docs/conf.py` & `evolutionary_forest-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/docs/constructed_features.png` & `evolutionary_forest-0.2.4/docs/constructed_features.png`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/docs/installation.rst` & `evolutionary_forest-0.2.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/docs/make.bat` & `evolutionary_forest-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/application/baes_class.py` & `evolutionary_forest-0.2.4/evolutionary_forest/application/baes_class.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/application/expensive_benchmark.py` & `evolutionary_forest-0.2.4/evolutionary_forest/application/expensive_benchmark.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/application/gp_function_test.py` & `evolutionary_forest-0.2.4/evolutionary_forest/application/gp_function_test.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/archive.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/archive.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/configuration.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/configuration.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/crossover_mutation.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/crossover_mutation.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/evaluation.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/evaluation.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/generation.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/generation.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/mutation_transformer.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/mutation_transformer.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/pac_bayesian.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/pac_bayesian.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/primitives.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/primitives.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/rademacher_complexity.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/rademacher_complexity.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/selection.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/selection.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/stateful_gp.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/stateful_gp.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/subset_selection.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/subset_selection.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/syntax_tools.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/syntax_tools.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/toolbox.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/toolbox.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/translation_transformer.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/translation_transformer.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/tree_utils.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/tree_utils.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/component/vc_dimension.py` & `evolutionary_forest-0.2.4/evolutionary_forest/component/vc_dimension.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/forest.py` & `evolutionary_forest-0.2.4/evolutionary_forest/forest.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/model/PLTree.py` & `evolutionary_forest-0.2.4/evolutionary_forest/model/PLTree.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/model/RBFN.py` & `evolutionary_forest-0.2.4/evolutionary_forest/model/RBFN.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/model/SafetyScaler.py` & `evolutionary_forest-0.2.4/evolutionary_forest/model/SafetyScaler.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/model/VAE.py` & `evolutionary_forest-0.2.4/evolutionary_forest/model/VAE.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/multigene_gp.py` & `evolutionary_forest-0.2.4/evolutionary_forest/multigene_gp.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/preprocess_utils.py` & `evolutionary_forest-0.2.4/evolutionary_forest/preprocess_utils.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/probability_gp.py` & `evolutionary_forest-0.2.4/evolutionary_forest/probability_gp.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/pruning.py` & `evolutionary_forest-0.2.4/evolutionary_forest/pruning.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/sklearn_utils.py` & `evolutionary_forest-0.2.4/evolutionary_forest/sklearn_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from joblib import Parallel, delayed
 from sklearn.base import is_classifier, clone
 from sklearn.model_selection import check_cv
 from sklearn.model_selection._validation import _check_is_permutation, _enforce_prediction_order
 from sklearn.preprocessing import LabelEncoder
 from sklearn.utils import (indexable)
 from sklearn.utils.metaestimators import _safe_split
-from sklearn.utils.validation import _check_fit_params
 from sklearn.utils.validation import _deprecate_positional_args
 from sklearn.utils.validation import _num_samples
 
 
 @_deprecate_positional_args
 def cross_val_predict(estimator, X, y=None, *, groups=None, cv=None,
                       n_jobs=None, verbose=0, fit_params=None,
@@ -233,15 +232,14 @@
         Result of calling 'estimator.method'
 
     test : array-like
         This is the value of the test parameter
     """
     # Adjust length of sample weights
     fit_params = fit_params if fit_params is not None else {}
-    fit_params = _check_fit_params(X, fit_params, train)
 
     X_train, y_train = _safe_split(estimator, X, y, train)
     X_test, _ = _safe_split(estimator, X, y, test, train)
 
     if y_train is None:
         estimator.fit(X_train, **fit_params)
     else:
```

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/strategies/adaptive_rate.py` & `evolutionary_forest-0.2.4/evolutionary_forest/strategies/adaptive_rate.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/strategies/estimation_of_distribution.py` & `evolutionary_forest-0.2.4/evolutionary_forest/strategies/estimation_of_distribution.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/strategies/multiarm_bandit.py` & `evolutionary_forest-0.2.4/evolutionary_forest/strategies/multiarm_bandit.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/strategies/space_partition.py` & `evolutionary_forest-0.2.4/evolutionary_forest/strategies/space_partition.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/strategies/surrogate_model.py` & `evolutionary_forest-0.2.4/evolutionary_forest/strategies/surrogate_model.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest/utils.py` & `evolutionary_forest-0.2.4/evolutionary_forest/utils.py`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest.egg-info/PKG-INFO` & `evolutionary_forest-0.2.4/evolutionary_forest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evolutionary-forest
-Version: 0.2.3
+Version: 0.2.4
 Summary: An open source python library for automated feature engineering based on Genetic Programming
 Home-page: https://github.com/zhenlingcn/evolutionary_forest
 Author: Hengzhe Zhang
 Author-email: zhenlingcn@foxmail.com
 License: BSD license
 Keywords: evolutionary_forest
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `evolutionary_forest-0.2.3/evolutionary_forest.egg-info/SOURCES.txt` & `evolutionary_forest-0.2.4/evolutionary_forest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evolutionary_forest-0.2.3/setup.py` & `evolutionary_forest-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-with open('README.rst',encoding='utf-8') as readme_file:
+with open('README.rst', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
-with open('HISTORY.rst',encoding='utf-8') as history_file:
+with open('HISTORY.rst', encoding='utf-8') as history_file:
     history = history_file.read()
 
 requirements = [
     'scipy',
     'hdfe',
     'numpy',
     'seaborn',
@@ -61,10 +61,10 @@
     keywords='evolutionary_forest',
     name='evolutionary_forest',
     packages=find_packages(include=['evolutionary_forest', 'evolutionary_forest.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zhenlingcn/evolutionary_forest',
-    version='0.2.3',
+    version='0.2.4',
     zip_safe=False,
 )
```

### Comparing `evolutionary_forest-0.2.3/tests/test_evolutionary_forest.py` & `evolutionary_forest-0.2.4/tests/test_evolutionary_forest.py`

 * *Files identical despite different names*

