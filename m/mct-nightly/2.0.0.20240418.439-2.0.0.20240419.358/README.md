# Comparing `tmp/mct-nightly-2.0.0.20240418.439.tar.gz` & `tmp/mct-nightly-2.0.0.20240419.358.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-nightly-2.0.0.20240418.439.tar", last modified: Thu Apr 18 00:04:39 2024, max compression
+gzip compressed data, was "mct-nightly-2.0.0.20240419.358.tar", last modified: Fri Apr 19 00:04:00 2024, max compression
```

## Comparing `mct-nightly-2.0.0.20240418.439.tar` & `mct-nightly-2.0.0.20240419.358.tar`

### file list

```diff
@@ -1,607 +1,607 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.888596 mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    37478 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.888596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.888596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.888596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.892596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.892596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.892596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.892596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38259 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    28499 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.892596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.896596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/hessian_info_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.896596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.896596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.900596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.900596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.900596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.900596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/channels_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.900596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.904596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/memory_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/prune_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.904596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)    27014 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.908596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.908596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.908596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.908596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/remove_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.912596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21951 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/graph_prep_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.912596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.912596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15567 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/custom_layer_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.912596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.916597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.916597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    29457 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/keras_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.916597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.916597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.920596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.920596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.920596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.920596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.920596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.920596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.924596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.924596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.924596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pytorch_device_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27267 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/quantization_prep_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.932597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/data_generation_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/model_info_exctractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.932597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/keras_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.932597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.932597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20937 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/defaultdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    17705 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/keras/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/pytorch/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.952597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.952597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.952597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.952597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.952597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/immutable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.952597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10947 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-18 00:04:39.964597 mct-nightly-2.0.0.20240418.439/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.069877 mct-nightly-2.0.0.20240419.358/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-04-19 00:04:00.069877 mct-nightly-2.0.0.20240419.358/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:03:59.993877 mct-nightly-2.0.0.20240419.358/mct_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-04-19 00:03:59.000000 mct-nightly-2.0.0.20240419.358/mct_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    37478 2024-04-19 00:03:59.000000 mct-nightly-2.0.0.20240419.358/mct_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:03:59.000000 mct-nightly-2.0.0.20240419.358/mct_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-19 00:03:59.000000 mct-nightly-2.0.0.20240419.358/mct_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 00:03:59.000000 mct-nightly-2.0.0.20240419.358/mct_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:03:59.993877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-19 00:03:58.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:03:59.993877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:03:59.997877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:03:59.997877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:03:59.997877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:03:59.997877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:03:59.997877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38265 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29079 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.001877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.001877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/hessian/hessian_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.001877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.005877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.005877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.005877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.005877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.009877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/channels_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.009877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/importance_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.009877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/memory_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/prune_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/pruner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/pruning_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/pruning_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/pruning_section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.009877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26723 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.013877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.013877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.013877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.017877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.017877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21951 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/graph_prep_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.017877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.021877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16227 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15567 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/custom_layer_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.021877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.021877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8157 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.025877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29673 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/keras_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.025877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.025877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.025877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.025877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.025877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.025877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.025877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.029878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.029878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.029878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.029878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.033877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.033877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.033877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.033877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/pytorch_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27351 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.033877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.037877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.037877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/quantization_prep_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.037877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.037877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/data_generation_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/model_info_exctractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.037877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/keras_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.037877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.041877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.041877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20937 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/defaultdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.041877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.041877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.041877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.041877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.045878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.045878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.045878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.045878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.045878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.045878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.045878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.045878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.045878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17705 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.049878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.049878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.049878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.049878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.049878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.053877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.053877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.053877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.053877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/pruning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.053877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/pruning/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/pruning/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/pruning/keras/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.053877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/pruning/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/pruning/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/pruning/pytorch/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.053877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.053877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.053877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.053877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.053877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.053877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.057878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.057878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.057878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.057878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.057878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.057878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.057878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.057878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/immutable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.061878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.061878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.061878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.061878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.061878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.061878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.065878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.065878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.065878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.065878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.065878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.065878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.065878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.065878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.065878 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.069877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.069877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.069877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.069877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:04:00.069877 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-19 00:03:27.000000 mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-19 00:04:00.069877 mct-nightly-2.0.0.20240419.358/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-19 00:03:58.000000 mct-nightly-2.0.0.20240419.358/setup.py
```

### Comparing `mct-nightly-2.0.0.20240418.439/LICENSE.md` & `mct-nightly-2.0.0.20240419.358/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/PKG-INFO` & `mct-nightly-2.0.0.20240419.358/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 2.0.0.20240418.439
+Version: 2.0.0.20240419.358
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-2.0.0.20240418.439/README.md` & `mct-nightly-2.0.0.20240419.358/README.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/PKG-INFO` & `mct-nightly-2.0.0.20240419.358/mct_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 2.0.0.20240418.439
+Version: 2.0.0.20240419.358
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/SOURCES.txt` & `mct-nightly-2.0.0.20240419.358/mct_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 from model_compression_toolkit import qat
 from model_compression_toolkit import exporter
 from model_compression_toolkit import gptq
 from model_compression_toolkit import data_generation
 from model_compression_toolkit import pruning
 from model_compression_toolkit.trainable_infrastructure.keras.load_model import keras_load_quantized_model
 
-__version__ = "2.0.0.20240418.000439"
+__version__ = "2.0.0.20240419.000358"
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/constants.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/analyzer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/back2framework/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/base_substitutions.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/base_collector.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/mean_collector.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/framework_implementation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/framework_info.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/fusion/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/base_graph.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,16 @@
             tpc: TargetPlatformCapabilities object.
         """
         # validate graph nodes are either from the framework or a custom layer defined in the TPC
         # Validate graph nodes are either built-in layers from the framework or custom layers defined in the TPC
         tpc_layers = tpc.op_sets_to_layers.get_layers()
         tpc_filtered_layers = [layer for layer in tpc_layers if isinstance(layer, LayerFilterParams)]
         for n in self.nodes:
-            is_node_in_tpc = n.type in tpc_layers or any([n.is_match_filter_params(filtered_layer)
-                                                          for filtered_layer in tpc_filtered_layers])
+            is_node_in_tpc = any([n.is_match_type(_type) for _type in tpc_layers]) or \
+                             any([n.is_match_filter_params(filtered_layer) for filtered_layer in tpc_filtered_layers])
             if n.is_custom:
                 if not is_node_in_tpc:
                     Logger.critical(f'MCT does not support optimizing Keras custom layers. Found a layer of type {n.type}. '
                                     ' Please add the custom layer to Target Platform Capabilities (TPC), or file a feature '
                                     'request or an issue if you believe this should be supported.')  # pragma: no cover
                 if any([qc.default_weight_attr_config.enable_weights_quantization for qc in n.get_qco(tpc).quantization_config_list]):
                     Logger.critical(f'Layer identified: {n.type}. MCT does not support weight quantization for Keras custom layers.')  # pragma: no cover
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/base_node.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,27 +147,41 @@
         """
         Check whether the node is reused or not
         Returns:
             True if node is reused, else False
         """
         return self.reuse or self.reuse_group is not None
 
-    def get_weights_by_keys(self, name: str) -> np.ndarray:
+    def _get_weight_name(self, name: Union[str, int]) -> List[Union[str, int]]:
+        """
+        Get weight names that match argument name (either string weights or integer for
+        positional weights).
+        Args:
+            name: weight name
+
+        Returns:
+            A list of weight names that match input "name"
+
+        """
+        return [k for k in self.weights.keys()
+                if (isinstance(k, int) and name == k) or (isinstance(k, str) and name in k)]
+
+    def get_weights_by_keys(self, name: Union[str, int]) -> np.ndarray:
         """
         Get a node's weight by its name.
         Args:
             name: Name of the variable for a node's weight.
 
         Returns:
             A node's weight (by its name).
         """
         if name is None:
             return None
 
-        res = [k for k in self.weights.keys() if name in k]
+        res = self._get_weight_name(name)
         if len(res) == 1:  # Make sure there are no duplicates
             return self.weights[res[0]]
         else:
             return None
 
     def set_weights_by_keys(self, name: str, tensor: np.ndarray):
         """
@@ -175,15 +189,15 @@
 
         Args:
             name: Name of the weight the node holds.
             tensor: Numpy array to set as the weight.
 
         """
 
-        res = [k for k in self.weights.keys() if name in k]
+        res = self._get_weight_name(name)
         if len(res) == 1:
             self.weights[res[0]] = tensor
         else:  # Add if not exist
             self.weights[name] = tensor
             self.weights_keys = list(self.weights.keys())  # update keys
 
     def get_weights_list(self):
@@ -548,30 +562,33 @@
 
         if tpc is None:
             Logger.critical(f'Can not retrieve QC options for None TPC')  # pragma: no cover
 
         for fl, qco in tpc.filterlayer2qco.items():
             if self.is_match_filter_params(fl):
                 return qco
-        if self.type in tpc.layer2qco:
-            return tpc.layer2qco.get(self.type)
+        # Extract qco with is_match_type to overcome mismatch of function types in TF 2.15
+        matching_qcos = [_qco for _type, _qco in tpc.layer2qco.items() if self.is_match_type(_type)]
+        if matching_qcos:
+            if len(matching_qcos) > 1:
+                Logger.error('Found duplicate qco types!')
+            return matching_qcos[0]
         return tpc.tp_model.default_qco
 
     def is_match_type(self, _type: Type) -> bool:
         """
-        Check if input type matches the node type, either in instance type or in type name. Checking the
-        name string is required because of function types changes that occurred in TF 2.15.
+        Check if input type matches the node type, either in instance type or in type name.
 
         Args:
             _type: other node type
         Returns:
             Whether _type matches the self node type
 
         """
-        return _type == self.type or _type.__name__ == self.type.__name__
+        return _type == self.type
 
     def is_match_filter_params(self, layer_filter_params: LayerFilterParams) -> bool:
         """
         Check if the node matches a LayerFilterParams according to its
         layer, conditions and keyword-arguments.
 
         Args:
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/edge.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/functional_node.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Dict, Any, Tuple, List
+from typing import Dict, Any, Tuple, Type
 
+from model_compression_toolkit.constants import FOUND_TF
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 import numpy as np
 
 
 class FunctionalNode(BaseNode):
     """
     Node that represents function ops with arguments to pass when building back the model.
@@ -67,7 +68,23 @@
     @property
     def type(self):
         """
         A function to get the node's function op for convenient comparison (instead of the layer_class)
         :return: the node's functional_op
         """
         return self.functional_op
+
+    def is_match_type(self, _type: Type) -> bool:
+        """
+        Check if input type matches the node type, either in instance type or in type name. Checking the
+        name string is required because of function types changes that occurred in TF 2.15, because it
+        changes the "function" attribute object (e.g. a different tf.add function that will fail the
+        equal operation).
+
+        Args:
+            _type: other node type
+        Returns:
+            Whether _type matches the self node type
+
+        """
+        names_match = _type.__name__ == self.type.__name__ if FOUND_TF else False
+        return super().is_match_type(_type) or names_match
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/graph_matchers.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/graph_searches.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/hessian_info_service.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/hessian/hessian_info_service.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/hessian_info_utils.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/hessian/hessian_info_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/trace_hessian_request.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/hessian/trace_hessian_request.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/base_matcher.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/function.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/node_matcher.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/memory_computation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/memory_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/model_builder_mode.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/model_collector.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/model_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/model_validation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/actions.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/edit_network.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/node_filters.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import Any
 from model_compression_toolkit.core.common.matchers.node_matcher import BaseNodeMatcher
+from model_compression_toolkit.core.common.graph.base_node import BaseNode
 
 
 class NodeTypeFilter(BaseNodeMatcher):
     """
     Class NodeNameFilter to check if a node is of a specific type.
     """
     def __init__(self, node_type):
@@ -26,25 +27,25 @@
         Init a NodeTypeFilter object.
 
         Args:
             node_type: Node type to check.
         """
         self.node_type = node_type
 
-    def apply(self, input_object: Any) -> bool:
+    def apply(self, input_object: BaseNode) -> bool:
         """
         Check if input_object is of the type that NodeTypeFilter contains.
 
         Args:
             input_object: Node object to check for its type.
 
         Returns:
-            True if the node if of the type that was passed during the initialization of NodeTypeFilter.
+            True if the node is of the type that was passed during the initialization of NodeTypeFilter.
         """
-        if input_object.type == self.node_type:
+        if input_object.is_match_type(self.node_type):
             return True
 
 
 class NodeNameFilter(BaseNodeMatcher):
     """
     Class NodeNameFilter to check if a node's name has a specific value.
     """
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/node_prior_info.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/channels_grouping.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/channels_grouping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/memory_calculator.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/memory_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/prune_graph.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/prune_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruner.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/pruner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/pruning_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_info.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/pruning_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_section.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/pruning/pruning_section.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/core_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/debug_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,16 +261,14 @@
         self.weights_quantization_method = weights_attr_cfg.weights_quantization_method
         self.weights_error_method = qc.weights_error_method
         self.weights_n_bits = weights_attr_cfg.weights_n_bits
         self.weights_per_channel_threshold = weights_attr_cfg.weights_per_channel_threshold
         self.enable_weights_quantization = weights_attr_cfg.enable_weights_quantization
         self.l_p_value = qc.l_p_value
 
-
-
     @property
     def weights_error_method(self) -> QuantizationErrorMethod:
         """
         weights_error_method getter.
         """
         return self._weights_error_method
 
@@ -408,17 +406,14 @@
 
         # Initialize a quantization configuration for each of the node's attributes
         self.attributes_config_mapping = {}
         self.pos_attributes_config_mapping = {}
         for attr in node_attrs_list:
             if isinstance(attr, int):
                 # this is a positional attribute, so it needs to be handled separately.
-                # we assume that a positional attribute is quantized with the default configuration provided in the TPC.
-                if op_cfg.default_weight_attr_config.enable_weights_quantization:
-                    Logger.critical(f"Quantizing constant weights is not supported.")
                 self.pos_attributes_config_mapping[attr] = WeightsAttrQuantizationConfig(qc=qc,
                                                                                          weights_attr_cfg=op_cfg.default_weight_attr_config,
                                                                                          weights_channels_axis=weights_channels_axis)
             else:
                 # In Tensorflow, the attribute name is composed of the framework attribute name and the layer name,
                 # therefore, we need to look for the attribute in the op_cfg that is contained in the node attribute's name.
                 attrs_included_in_name = {k: v for k, v in op_cfg.attr_weights_configs_mapping.items() if k in attr}
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
+from typing import Dict
 import numpy as np
 from sklearn.cluster import KMeans
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
 from model_compression_toolkit.constants import LUT_VALUES, MIN_THRESHOLD, SCALE_PER_CHANNEL, \
     LUT_VALUES_BITWIDTH, THRESHOLD, NUM_QPARAM_HESSIAN_SAMPLES
 from model_compression_toolkit.core.common.hessian import HessianInfoService
@@ -34,18 +35,18 @@
                       p: int,
                       n_bits: int,
                       per_channel: bool = False,
                       channel_axis: int = 1,
                       n_iter: int = 10,
                       min_threshold: float = MIN_THRESHOLD,
                       quant_error_method: qc.QuantizationErrorMethod = None,
-                      is_symmetric=False,
+                      is_symmetric: bool = False,
                       node=None,
                       hessian_info_service: HessianInfoService = None,
-                      num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> dict:
+                      num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> Dict:
     """
     The quantizer first finds the closest max value per channel of tensor_data.
     Now, we divide tensor_data with the threshold vector per channel. In addition, we scale the result to the range
     [-2^(LUT_VALUES_BITWIDTH-1), 2^(LUT_VALUES_BITWIDTH-1)-1].
     Next, we take the scaled tensor_data and perform k-means clustering with 2^nbit clusters.
     We return the rounded cluster centers, and threshold per channel. We use these to quantize the data.
     Args:
@@ -97,15 +98,15 @@
                          p: int,
                          n_bits: int,
                          min_value: float,
                          max_value: float,
                          constrained: bool = True,
                          n_iter: int = 20,
                          min_threshold: float = MIN_THRESHOLD,
-                         quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE) -> dict:
+                         quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE) -> Dict:
     """
     Finds quantization cluster points for non-uniform activation quantization.
     The quantizer first finds the closest power-of-two number to the max value of the given histogram,
     and scales the bins within 8-bit quantization range.
     Next, it performs a weighted k-means clustering with 2^nbit clusters (using the histogram counts as weights).
     Returns the rounded cluster centers, and 8-bit quantization threshold.
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantize_node.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/similarity_analyzer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
     return error
 
 
 def compute_kl_divergence(float_tensor: np.ndarray, fxp_tensor: np.ndarray, batch: bool = False,
                           axis: int = None) -> float:
     """
     Compute the similarity between two tensor using KL-divergence.
-    The returned values is between 0 to 1: the smaller returned value,
+    The returned values is between 0 and 1: the smaller returned value,
     the greater similarity there is between the two tensors.
 
     Args:
         float_tensor: First tensor to compare.
         fxp_tensor: Second tensor to compare.
         batch: Whether to run batch similarity analysis or not.
         axis: Axis along which the operator has been computed.
@@ -253,10 +253,10 @@
     float_flat = flatten_tensor(float_tensor, batch, axis)
     fxp_flat = flatten_tensor(fxp_tensor, batch, axis)
 
     non_zero_fxp_tensor = fxp_flat.copy()
     non_zero_fxp_tensor[non_zero_fxp_tensor == 0] = EPS
 
     prob_distance = np.where(float_flat != 0, float_flat * np.log(float_flat / non_zero_fxp_tensor), 0)
-    # The sum is part of the KL-Divergance function.
+    # The sum is part of the KL-Divergence function.
     # The mean is to aggregate the distance between each output probability vectors.
     return np.mean(np.sum(prob_distance, axis=-1), axis=-1)
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/remove_identity.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/remove_identity.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/user_info.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/graph_prep_runner.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/graph_prep_runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.graph.edge import EDGE_SINK_INDEX
 from model_compression_toolkit.core.keras.back2framework.instance_builder import OperationHandler
 from model_compression_toolkit.core.keras.reader.connectivity_handler import OutTensor
+from mct_quantizers import KerasQuantizationWrapper
 
 # In tf2.3 fake quant node is implemented as TensorFlowOpLayer, while in tf2.4 as TFOpLambda.
 FQ_NODE_OP_V2_3 = 'FakeQuantWithMinMaxVars'
 FQ_NODE_OP_V2_4 = 'quantization.fake_quant_with_min_max_vars'
 BATCH_INPUT_SHAPE = 'batch_input_shape'
 
 
@@ -266,15 +267,17 @@
         """
         if len(input_tensors) == 0:  # Placeholder handling
             out_tensors_of_n_float = input_nodes_to_input_tensors[n]
             out_tensors_of_n = self._run_operation_activation_quantization(n,
                                                                            out_tensors_of_n_float)
         else:
             input_tensors = [tensor for tensor_list in input_tensors for tensor in tensor_list]  # flat list of lists
-            input_tensors = n.insert_positional_weights_to_input_list(input_tensors)
+            if not isinstance(op_func, KerasQuantizationWrapper):
+                # The KerasQuantizationWrapper will insert the quantized positional weights internally.
+                input_tensors = n.insert_positional_weights_to_input_list(input_tensors)
             # Build a functional node using its args
             if isinstance(n, FunctionalNode):
                 if n.inputs_as_list:  # If the first argument should be a list of tensors:
                     out_tensors_of_n_float = op_func(input_tensors, *n.op_call_args, **n.op_call_kwargs)
                 else:  # If the input tensors should not be a list but iterated:
                     out_tensors_of_n_float = op_func(*input_tensors, *n.op_call_args, **n.op_call_kwargs)
             else:
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/constants.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/custom_layer_validation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/custom_layer_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/default_framework_info.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,17 +66,17 @@
         conv_node: Convolution node to update the weight/kernel.
         kernel: The Convolution node's weight
         weights_scale: Weight scale factor in which to multiply the conv node's weight.
 
     Returns:
         The modified convolution node's weight/kernel/
     """
-    if conv_node.type == DepthwiseConv2D:
+    if conv_node.is_match_type(DepthwiseConv2D):
         kernel = kernel * weights_scale.reshape((1, 1, kernel.shape[-2], kernel.shape[-1]))
-    elif conv_node.type == Conv2DTranspose:
+    elif conv_node.is_match_type(Conv2DTranspose):
         kernel = kernel * weights_scale.reshape((1, 1, -1, 1))
     else:
         kernel = kernel * weights_scale.reshape((1, 1, 1, -1))
 
     kernel_name = DEFAULT_KERAS_INFO.get_kernel_op_attributes(conv_node.type)[0]
 
     return kernel, kernel_name
@@ -94,18 +94,18 @@
         bias: The Convolution node's bias
         weights_scale: Weight scale factor in which to multiply the conv node's weight.
         bias_factor: factor for kernel to update the bias with: (beta - moving_mean * weights_scale)
 
     Returns:
         The modified convolution node's weight/kernel/
     """
-    if conv_node.type == DepthwiseConv2D:
+    if conv_node.is_match_type(DepthwiseConv2D):
         bias_update = kernel * bias_factor.reshape((1, 1, -1, 1))
         kernel = kernel * weights_scale.reshape((1, 1, -1, 1))
-    elif conv_node.type == Conv2DTranspose:
+    elif conv_node.is_match_type(Conv2DTranspose):
         bias_update = (kernel * bias_factor.reshape((1, 1, 1, -1))).sum(3)
         kernel = kernel * weights_scale.reshape((1, 1, 1, -1))
     else:
         bias_update = (kernel * bias_factor.reshape((1, 1, -1, 1))).sum(2)
         kernel = kernel * weights_scale.reshape((1, 1, -1, 1))
 
     kernel_name = DEFAULT_KERAS_INFO.get_kernel_op_attributes(conv_node.type)[0]
@@ -129,30 +129,30 @@
     Check whether the node is a group-convolution
     Args:
         node: The Convolution node
 
     Returns:
         True if the node is a group convolution, else False
     """
-    return (node.type == Conv2D) and node.framework_attr[GROUPS] > 1
+    return (node.is_match_type(Conv2D)) and node.framework_attr[GROUPS] > 1
 
 
 def get_foldable_node_type_and_validity_fn(node: BaseNode) -> [bool, bool]:
     """
     Check whether the node to forward fold is a valid dw-convolution node or a
     batch-normalization node
     Args:
         node: The node to fold
 
     Returns:
         is_bn: True if the node is a batch norm, else False
         is_dw_valid: True if the node is a dw-convolution valid for folding or a batch-norm node, else False
     """
-    is_bn = node.type is BatchNormalization
-    is_dw = node.type is DepthwiseConv2D
+    is_bn = node.is_match_type(BatchNormalization)
+    is_dw = node.is_match_type(DepthwiseConv2D)
     is_dw_valid = is_dw and np.all(np.array(node.get_weights_by_keys(DEPTHWISE_KERNEL).shape[:2]) == 1)
     return is_bn, is_dw_valid
 
 
 def keras_batchnorm_folding() -> BatchNormalizationFolding:
     """
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         first_node: First layer node to collapse to second layer node
         second_node: Second layer node
         kernel_str: The framework specific attribute name of the convolution layer's weight/kernel.
         bias_str: The framework specific attribute name of the convolution layer's bias.
     Returns:
         The modified layer node's weights: kernel, bias
     """
-    if first_node.type == Conv2D and second_node.type == Conv2D:
+    if first_node.is_match_type(Conv2D) and second_node.is_match_type(Conv2D):
         # Get nodes attributes
         kernel1 = first_node.get_weights_by_keys(kernel_str)
         kernel2 = second_node.get_weights_by_keys(kernel_str)
         bias1 = first_node.get_weights_by_keys(bias_str)
         bias2 = second_node.get_weights_by_keys(bias_str)
         strides1 = first_node.framework_attr[STRIDES]
         strides2 = second_node.framework_attr[STRIDES]
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     Inspired by https://arxiv.org/pdf/2103.09404.pdf - Algorithm2
     Args:
         first_node: First layer node to collapse into.
         kernel_str: The framework specific attribute name of the convolution layer's weight/kernel.
     Returns:
         The modified layer node's weights: kernel
     """
-    if first_node.type == Conv2D:
+    if first_node.is_match_type(Conv2D):
         # Get nodes attributes
         kernel = first_node.get_weights_by_keys(kernel_str)
         (kH, kW, Cin, Cout) = kernel.shape
 
         # Collapsing residual by adding "1" to kernel diagonal
         idxH = (kH - 1) // 2
         idxW = (kW - 1) // 2
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/keras_implementation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from functools import partial
-from typing import List, Any, Tuple, Callable, Dict
+from typing import List, Any, Tuple, Callable, Dict, Union
 
 import numpy as np
 import tensorflow as tf
 from mct_quantizers import KerasQuantizationWrapper, KerasActivationQuantizationHolder
 from tensorflow.keras.models import Model
 
 from model_compression_toolkit.constants import HESSIAN_NUM_ITERATIONS
@@ -408,20 +408,21 @@
         """
         Returns whether a given node in considered as a potential interest point for mp metric computation purposes.
         Args:
             node: Node to indicate whether it needs to be part of the interest points set.
         Returns: True if the node should be considered an interest point, False otherwise.
         """
 
-        if node.type == Activation:
+        if node.is_match_type(Activation):
             node_type_name = node.framework_attr[keras_constants.ACTIVATION]
             if node_type_name in [keras_constants.SOFTMAX, keras_constants.SIGMOID]:
                 return True
-        elif node.type in [tf.nn.softmax, tf.keras.layers.Softmax, tf.nn.sigmoid, Conv2D, DepthwiseConv2D, Conv2DTranspose, Dense, Concatenate,
-                           tf.concat, Add, tf.add]:
+        elif any([node.is_match_type(_type) for _type in [tf.nn.softmax, tf.keras.layers.Softmax, tf.nn.sigmoid, Conv2D,
+                                                          DepthwiseConv2D, Conv2DTranspose, Dense, Concatenate, tf.concat,
+                                                          Add, tf.add]]):
             return True
 
         return False
 
     def get_node_distance_fn(self, layer_class: type,
                              framework_attrs: Dict[str, Any],
                              compute_distance_fn: Callable = None,
@@ -525,26 +526,26 @@
         Returns: The MAC count og the operation
         """
 
         output_shape = node.output_shape
         kernel_shape = node.get_weights_by_keys(fw_info.get_kernel_op_attributes(node.type)[0]).shape
         output_channel_axis, input_channel_axis = fw_info.kernel_channels_mapping.get(node.type)
 
-        if node.type is Conv2D or node.type is Conv2DTranspose:
+        if node.is_match_type(Conv2D) or node.is_match_type(Conv2DTranspose):
             # (C_out * W_out * H_out) * C_in * (W_kernel * H_kernel)
             return np.prod([x for x in output_shape if x is not None]) * \
                    kernel_shape[input_channel_axis] * \
                    (kernel_shape[0] * kernel_shape[1])
-        elif node.type is DepthwiseConv2D:
+        elif node.is_match_type(DepthwiseConv2D):
             # Depth * (W_out * H_out) * C_in * (W_kernel * H_kernel)
             return node.framework_attr.get(DEPTH_MULTIPLIER) * \
                    np.prod([x for x in output_shape if x is not None]) / output_shape[output_channel_axis] * \
                    kernel_shape[input_channel_axis] * \
                    (kernel_shape[0] * kernel_shape[1])
-        elif node.type is Dense:
+        elif node.is_match_type(Dense):
             # IN * OUT
             return kernel_shape[0] * kernel_shape[1]
         else:
             return 0
 
     def apply_second_moment_correction(self,
                                        quantized_model: Any,
@@ -589,31 +590,30 @@
 
         Args:
            node: Node to get quantizers for.
 
         Returns:
             weight_quantizers: A dictionary between a weight's name to its quantizer.
             activation_quantizers: A list of activations quantization, one for each layer output.
-
         """
 
-        def _weight_name(w: str) -> str:
+        def _weight_name(w: Union[str, int]) -> Union[str, int]:
             """
             Extracts the weight name from the full TensorFlow variable name.
 
             For example, returns 'kernel' for 'dense_2/kernel:0'.
 
             Args:
               w: TensorFlow variable name.
 
             Returns:
               Extracted weight name.
             """
 
-            return w.split(':')[0].split('/')[-1]
+            return w.split(':')[0].split('/')[-1] if isinstance(w, str) else w
 
         attribute_names = [_weight_name(wn) for wn in node.get_node_weights_attributes()
                            if node.is_weights_quantization_enabled(wn)]
 
         return get_inferable_quantizers(node,
                                         get_weights_quantizer_for_node,
                                         get_activations_quantizer_for_node,
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/keras_model_validation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,21 +52,21 @@
         fw_info: Information about a specific framework the node was generated from.
 
     Returns:
         Min/max output values if known.
     """
     min_output, max_output = None, None
 
-    if node.type == ReLU:
+    if node.is_match_type(ReLU):
         min_output = node.framework_attr[THRESHOLD] if node.framework_attr[NEGATIVE_SLOPE] == 0 else None
 
     elif fw_info.layers_has_min_max(node.type):
         min_output, max_output = fw_info.layer_min_max_mapping[node.type]
 
-    elif node.type == Activation and fw_info.activation_has_min_max(node.framework_attr[ACTIVATION]):
+    elif node.is_match_type(Activation) and fw_info.activation_has_min_max(node.framework_attr[ACTIVATION]):
         min_output, max_output = fw_info.activation_min_max_mapping[node.framework_attr[ACTIVATION]]
 
     return min_output, max_output
 
 
 def _get_mean_std_outputs(node: BaseNode,
                           graph: Graph) -> Tuple[Any, Any]:
@@ -78,24 +78,24 @@
         graph: Graph to check the next node type.
 
     Returns:
         Mean/Std output values if known.
     """
     mean_output, std_output = None, None
 
-    if node.type == BatchNormalization:
+    if node.is_match_type(BatchNormalization):
         mean_output = node.get_weights_by_keys(BETA)
         if node.get_weights_by_keys(GAMMA) is None:
             std_output = 1.0
         else:
             std_output = np.abs(node.get_weights_by_keys(GAMMA))
         if mean_output is None:
             mean_output = 0.0
     else:
         next_node_list = graph.get_next_nodes(node)
-        bn_nodes = [bn_node for bn_node in next_node_list if bn_node.type == BatchNormalization]
+        bn_nodes = [bn_node for bn_node in next_node_list if bn_node.is_match_type(BatchNormalization)]
         if len(bn_nodes) != 0:
             bn_node = bn_nodes[0]
             moving_variance = bn_node.get_weights_by_keys(MOVING_VARIANCE)
             std_output = np.sqrt(moving_variance)
             mean_output = bn_node.get_weights_by_keys(MOVING_MEAN)
     return mean_output, std_output
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/pruning/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,18 +205,17 @@
         node (BaseNode): The node to be evaluated.
 
     Returns:
         bool: True if the node is an edge of a pruning section, False otherwise.
     """
 
     # Check if the node is a Conv2D or Conv2DTranspose layer with groups set to 1.
-    if node.type in [keras.layers.Conv2D, keras.layers.Conv2DTranspose]:
+    if node.is_match_type(keras.layers.Conv2D) or node.is_match_type(keras.layers.Conv2DTranspose):
         return node.framework_attr[GROUPS] == 1
-    return node.type == keras.layers.Dense
-
+    return node.is_match_type(keras.layers.Dense)
 
 
 def _prune_keras_edge_node(node: BaseNode,
                            mask: np.ndarray,
                            fw_info: FrameworkInfo,
                            is_exit_node: bool):
     """
@@ -246,17 +245,17 @@
         # Prune the bias if applicable and it's an entry node.
         bias = node.get_weights_by_keys(BIAS)
         pruned_bias = bias.compress(mask_bool)
         node.set_weights_by_keys(name=BIAS, tensor=pruned_bias)
 
     if not is_exit_node:
         # Update 'filters' or 'units' attributes for entry node Conv2D/Conv2DTranspose layers.
-        if node.type in [keras.layers.Conv2D, keras.layers.Conv2DTranspose]:
+        if node.is_match_type(keras.layers.Conv2D) or node.is_match_type(keras.layers.Conv2DTranspose):
             node.framework_attr[FILTERS] = int(np.sum(mask))
-        elif node.type == keras.layers.Dense:
+        elif node.is_match_type(keras.layers.Dense):
             node.framework_attr[UNITS] = int(np.sum(mask))
 
     if is_exit_node:
         # Adjust the input shape for the last node in the section.
         _edit_node_input_shape(mask_bool, node)
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/common.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     Args:
         node: Node to check if its an input layer.
 
     Returns:
         Whether the node represents an input layer or not.
     """
     if isinstance(node, BaseNode):
-        return node.type == InputLayer
+        return node.is_match_type(InputLayer)
     elif isinstance(node, KerasNode):
         return isinstance(node.layer, InputLayer)
     else:
         Logger.critical('Node must be a graph node or a Keras node for input layer check.')  # pragma: no cover
 
 
 def is_node_a_model(node: BaseNode) -> bool:
@@ -56,13 +56,13 @@
     Args:
         node: Node to check if its a Keras model by itself.
 
     Returns:
         Whether the node represents a Keras model or not.
     """
     if isinstance(node, BaseNode):
-        return node.type in [Functional, Sequential]
+        return node.is_match_type(Functional) or node.is_match_type(Sequential)
     elif isinstance(node, KerasNode):
         return isinstance(node.layer, Functional) or isinstance(node.layer, Sequential)
     else:
         Logger.critical('Node must be a graph node or a Keras node.')  # pragma: no cover
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/node_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 
 keras = tf.keras
 layers = keras.layers
 
 REUSED_IDENTIFIER = '_reused_'
 
-is_const = lambda x: isinstance(x, (tf.Variable, tf.Tensor, np.ndarray))
+is_const = lambda x: isinstance(x, (tf.Variable, tf.Tensor, np.ndarray, float))
 is_tensor = lambda x: isinstance(x, KerasTensor)
 
 
 def get_tf_function_symbols() -> List[str]:
     """
     Create a list of tf function symbols, as they are created in the TFOpLambda layer. The
     symbols are serializations of the function names.
@@ -57,26 +57,44 @@
                                            tf.truediv, tf.pow, tf.matmul]]
 
 
 def get_kwargs2index(tfoplambda_layer: TFOpLambda) -> Dict[str, int]:
     """
     Positional weights are saved according to their index in the node's call arguments, so
     need to know the function arguments' names in case the weights are in the kwargs.
+
+    Note: the kwargs2index dictionary is initialized manually (and not with tf_inspect) so
+    it will only include the arguments that may contain constants. For example, we don't
+    want the transpose_a attribute of tf.matmul to be saved as a constant.
+
+    Every operation we add support to, needs to be added here.
+
     Args:
         tfoplambda_layer: TFOpLambda layer.
 
     Returns:
         A dictionary with argument number and index: {arg_name: arg_index}.
     """
-    if tfoplambda_layer.function in [tf.add, tf.subtract, tf.divide, tf.truediv, tf.multiply, tf.pow,
-                                     tf.matmul, tf.image.crop_and_resize, tf.image.combined_non_max_suppression] or \
-            tfoplambda_layer.symbol in ['__operators__.add', 'math.add', 'math.multiply', 'linalg.matmul', 'concat']:
-        return {arg_name: i for i, arg_name in enumerate(tf_inspect.getfullargspec(tfoplambda_layer.function).args)}
-    else:
-        return {}
+    kwargs2index = {tf.add: {'x': 0, 'y': 1},
+                    tf.subtract: {'x': 0, 'y': 1},
+                    tf.divide: {'x': 0, 'y': 1},
+                    tf.truediv: {'x': 0, 'y': 1},
+                    tf.multiply: {'x': 0, 'y': 1},
+                    tf.pow: {'x': 0, 'y': 1},
+                    tf.matmul: {'a': 0, 'b': 1}}.get(tfoplambda_layer.function)
+    if not kwargs2index:
+        # In TF 2.15 the function attribute is different and doesn't match the original
+        # operation object we use. Therefore, we extract kwargs2index with the symbol.
+        kwargs2index = {'__operators__.add': {'x': 0, 'y': 1},
+                        'math.add': {'x': 0, 'y': 1},
+                        'math.multiply': {'x': 0, 'y': 1},
+                        'linalg.matmul': {'a': 0, 'b': 1},
+                        'concat': {'values': 0}}.get(tfoplambda_layer.symbol, {})
+
+    return kwargs2index
 
 
 def build_node(node: KerasNode,
                node_name_to_node: dict) -> BaseNode:
     """
     Build a node from a Keras node. A node contains all information to reconstruct the layer it's representing
     in a model:
@@ -150,16 +168,17 @@
 
         # read weights from call kwargs
         weight_keys = []
         for k, v in op_call_kwargs.items():
             if is_const(v) or (keras_layer.function in [tf.add, tf.multiply, tf.subtract, tf.divide, tf.truediv, tf.pow,
                                                         tf.matmul] and
                                isinstance(v, (tuple, list))):
-                weights.update({kwarg2index[k]: to_numpy(v, is_single_tensor=True)})
-                weight_keys.append(k)
+                if k in kwarg2index:
+                    weights.update({kwarg2index[k]: to_numpy(v, is_single_tensor=True)})
+                    weight_keys.append(k)
         # remove weights and KerasTensors and weights from op_call_kwargs
         op_call_kwargs = {k: v for k, v in op_call_kwargs.items()
                           if not (kwarg2index.get(k) in weights or is_tensor(v))}
 
         node = FunctionalNode(node_name,
                               layer_config,
                               input_shape,
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/reader.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/resource_utilization_data_facade.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         return (to_tf_tensor(t) for t in tensor)
     elif isinstance(tensor, np.ndarray):
         return tf.convert_to_tensor(tensor.astype(np.float32))
     else:
         Logger.critical(f'Unsupported type for conversion to TF tensor: {type(tensor)}.')
 
 
-def tf_tensor_to_numpy(tensor: Union[List, Tuple, np.ndarray, tf.Tensor],
+def tf_tensor_to_numpy(tensor: Union[List, Tuple, np.ndarray, tf.Tensor, float],
                        is_single_tensor=False) -> np.ndarray:
     """
     Convert a TF tensor to a Numpy array.
     Args:
         tensor: TF tensor.
         is_single_tensor: whether input is a value to be converted to a single tensor.
                           if False, recurse the lists and tuples
@@ -61,10 +61,13 @@
             return [tf_tensor_to_numpy(t) for t in tensor]
     elif isinstance(tensor, tuple):
         if is_single_tensor:
             return np.array(tensor)
         else:
             return (tf_tensor_to_numpy(t) for t in tensor)
     elif isinstance(tensor, tf.Tensor):
-        return tensor.numpy()
+        np_tensor = tensor.numpy()
+        return np.array([np_tensor]) if np.isscalar(np_tensor) else np_tensor
+    elif isinstance(tensor, float):
+        return np.array([tensor])
     else:
         Logger.critical(f'Unsupported type for conversion to Numpy array: {type(tensor)}.')
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/visualization/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,67 +29,78 @@
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.core.pytorch.back2framework.instance_builder import node_builder, identity_wrapper
 from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
 from model_compression_toolkit.core.pytorch.pytorch_device_config import get_working_device
 from model_compression_toolkit.core.pytorch.reader.node_holders import DummyPlaceHolder
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from mct_quantizers.common.constants import ACTIVATION_HOLDER_QUANTIZER
+from mct_quantizers import PytorchQuantizationWrapper
 
 
 def _build_input_tensors_list(node: BaseNode,
                               graph: Graph,
                               inputs: Tuple[Any],
-                              node_to_output_tensors_dict: Dict[BaseNode, List]) -> List[List]:
+                              node_to_output_tensors_dict: Dict[BaseNode, List],
+                              is_op_quantize_wrapper: bool) -> List[List]:
     """
-    Given a node, build a list of input tensors the node gets. The list is built
-    based on the node's incoming edges and previous nodes' output tensors.
+    Given a node, build a list of input tensors the node gets. The list is built based on the
+    node's incoming edges, previous nodes' output tensors and the node's positional weights.
+    Positional weights aren't used if the node's op is PytorchQuantizationWrapper, since it's
+    positional weights are already in the wrapper.
 
     Args:
         node: Node to build its input tensors list.
         graph: Graph the node is in.
-        inputs: list of input tensors to model
+        inputs: list of input tensors to model.
         node_to_output_tensors_dict: A dictionary from a node to its output tensors.
+        is_op_quantize_wrapper: Whether the func_op is a PytorchQuantizationWrapper or not.
 
     Returns:
         A list of the node's input tensors.
     """
-    if node.type == DummyPlaceHolder:
+    if node.is_match_type(DummyPlaceHolder):
         input_tensors = [inputs[graph.get_inputs().index(node)]]
     else:
         input_tensors = []
         # Go over a sorted list of the node's incoming edges, and for each source node get its output tensors.
         # Append them in a result list.
         for ie in graph.incoming_edges(node, sort_by_attr=EDGE_SINK_INDEX):
             _input_tensors = node_to_output_tensors_dict[ie.source_node]
             input_tensors.append(_input_tensors)
         input_tensors = [tensor for tensor_list in input_tensors for tensor in tensor_list]  # flat list of lists
-        input_tensors = node.insert_positional_weights_to_input_list(input_tensors)
+        if not is_op_quantize_wrapper:
+            input_tensors = node.insert_positional_weights_to_input_list(input_tensors)
         # convert inputs from positional weights (numpy arrays) to tensors. Must handle each element in the
         # list separately, because in FX the tensors are FX objects and fail to_torch_tensor
         input_tensors = [to_torch_tensor(t) if isinstance(t, np.ndarray) else t
                          for t in input_tensors]
     return input_tensors
 
 
-def _merge_inputs(_node, input_tensors: List, op_call_args: List) -> List:
+def _merge_inputs(_node: BaseNode, input_tensors: List, op_call_args: List,
+                  is_op_quantize_wrapper: bool) -> List:
     """
-    Merge input tensors list with op_call_args, according to correct order
+    Merge input tensors list with op_call_args, according to correct order.
 
     Args:
-        _node: The node the inputs are for
+        _node: The node the inputs are for.
         input_tensors: activation input tensors to node.
-        op_call_args: framework node call args
+        op_call_args: framework node call args.
+        is_op_quantize_wrapper: Whether the func_op is a PytorchQuantizationWrapper or not.
     Returns:
-        Combined list of input_tensors and op_call_args
+        Combined list of input_tensors and op_call_args.
     """
     if isinstance(_node, FunctionalNode) and _node.tensor_input_indices:
-        assert len(_node.tensor_input_indices) == len(input_tensors), 'Mismatch between input tensors and indices'
         _input_list = op_call_args.copy()
-        for i, t in zip(_node.tensor_input_indices, input_tensors):
-            _input_list.insert(i, t)
+        if is_op_quantize_wrapper:
+            _input_list = input_tensors + _input_list
+        else:
+            assert len(_node.tensor_input_indices) == len(input_tensors), 'Mismatch between input tensors and indices'
+            for i, t in zip(_node.tensor_input_indices, input_tensors):
+                _input_list.insert(i, t)
     else:
         _input_list = input_tensors + op_call_args
 
     return _input_list
 
 
 def _run_operation(n: BaseNode,
@@ -114,15 +125,16 @@
     """
 
     op_call_args = n.op_call_args if isinstance(n, FunctionalNode) else []
     functional_kwargs = n.op_call_kwargs if isinstance(n, FunctionalNode) else {}
     if isinstance(n, FunctionalNode) and n.inputs_as_list:
         out_tensors_of_n_float = op_func(input_tensors, *op_call_args, **functional_kwargs)
     else:
-        out_tensors_of_n_float = op_func(*_merge_inputs(n, input_tensors, op_call_args), **functional_kwargs)
+        merged_inputs = _merge_inputs(n, input_tensors, op_call_args, isinstance(op_func, PytorchQuantizationWrapper))
+        out_tensors_of_n_float = op_func(*merged_inputs, **functional_kwargs)
 
     # Add a fake quant node if the node has an activation threshold.
     out_tensors_of_n = out_tensors_of_n_float
     if use_activation_quantization:
         if isinstance(out_tensors_of_n_float, list):
             out_tensors_of_n_float = torch.cat(out_tensors_of_n_float, dim=0)
         out_tensors_of_n = quantize_node_activation_fn(out_tensors_of_n_float)
@@ -275,20 +287,20 @@
         Returns:
             torch Tensor/s which is/are the output of the model logic.
         """
         node_to_output_tensors_dict = dict()
         node_to_output_tensors_dict_float = dict()
         configurable_nodes = self.graph.get_configurable_sorted_nodes_names(DEFAULT_PYTORCH_INFO)
         for node in self.node_sort:
+            op_func = self._get_op_func(node, configurable_nodes)
             input_tensors = _build_input_tensors_list(node,
                                                       self.graph,
                                                       args,
-                                                      node_to_output_tensors_dict)
-
-            op_func = self._get_op_func(node, configurable_nodes)
+                                                      node_to_output_tensors_dict,
+                                                      isinstance(op_func, PytorchQuantizationWrapper))
             use_activation_quantization, activation_quantization_fn = self._get_activation_quantization_fn(node)
 
             # Run node operation and fetch outputs
             out_tensors_of_n, out_tensors_of_n_float = _run_operation(node,
                                                                       input_tensors,
                                                                       op_func=op_func,
                                                                       quantize_node_activation_fn=activation_quantization_fn,
@@ -322,23 +334,24 @@
             configurable_nodes_names: A list of names of configurable nodes in the quantized model.
 
         Returns: Module/functional to apply to the input tensors.
 
         """
         return getattr(self, node.name)
 
-    def _get_activation_quantization_fn(self, node) -> Tuple[bool, bool, Callable]:
+    def _get_activation_quantization_fn(self, node) -> Tuple[bool, Callable]:
         """
         Get activation quantization parameters for this node.
 
         Args:
             node: Node from which to extract the activation quantization parameters.
 
-        Returns: Flag to indicate if we quantize activations, flag to indicate if we quantize activations
-        using a quantization holder and a quantization function to use for the node's activations.
+        Returns:
+            Flag to indicate if we quantize activations using a quantization holder and a quantization
+            function to use for the node's activations.
         """
         activation_quantization_holder = self.node_to_activation_quantization_holder.get(node.name)
         use_activation_quantization = node.is_activation_quantization_enabled()
         if use_activation_quantization:
             if activation_quantization_holder is None:
                 activation_quantization_fn = partial(self._quantize_node_activations, node)
                 use_activation_quantization = self.wrapper is None
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/constants.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/default_framework_info.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,19 +58,19 @@
         conv_node: Convolution node to update the weight/kernel.
         kernel: The Convolution node's weight
         weights_scale: Weight scale factor in which to multiply the conv node's weight.
 
     Returns:
         The modified convolution node's weight/kernel/
     """
-    if conv_node.type == ConvTranspose2d:
+    if conv_node.is_match_type(ConvTranspose2d):
         _scale = weights_scale[None, :, None, None]
     else:
         _scale = weights_scale[:, None, None, None]
-    if conv_node.type == ConvTranspose2d and conv_node.framework_attr[GROUPS] > 1:
+    if conv_node.is_match_type(ConvTranspose2d) and conv_node.framework_attr[GROUPS] > 1:
         # PyTorch ConvTranspose2d kernel with groups stacks groups on in_channels axis, so need to reshape the kernel
         # so the groups are stacked on the out_channels axis to match the scale vector (then reshape back to original
         # shape)
         _in_channels = int(conv_node.framework_attr[IN_CHANNELS]/conv_node.framework_attr[GROUPS])
         _out_channels = conv_node.framework_attr[OUT_CHANNELS]
         return (kernel.reshape((_in_channels, _out_channels, -1, 1)) * _scale).reshape(kernel.shape), KERNEL
     else:
@@ -89,18 +89,18 @@
         bias: The Convolution node's bias
         weights_scale: Weight scale factor in which to multiply the conv node's weight.
         bias_factor: factor for kernel to update the bias with: (beta - moving_mean * weights_scale)
 
     Returns:
         The modified convolution node's weight/kernel/
     """
-    if conv_node.type == Conv2d and conv_node.framework_attr[GROUPS] > 1:
+    if conv_node.is_match_type(Conv2d) and conv_node.framework_attr[GROUPS] > 1:
         bias_update = (kernel * bias_factor[:, None, None, None]).flatten()
         _scale = weights_scale[:, None, None, None]
-    elif conv_node.type == ConvTranspose2d:
+    elif conv_node.is_match_type(ConvTranspose2d):
         bias_update = (kernel * bias_factor[:, None, None, None]).sum(axis=0).flatten()
         _scale = weights_scale[:, None, None, None]
     else:
         bias_update = (kernel * bias_factor[None, :, None, None]).sum(axis=1).flatten()
         _scale = weights_scale[None, :, None, None]
     return kernel * _scale, bias + bias_update, KERNEL
 
@@ -121,31 +121,31 @@
     Check whether the node is a group-convolution
     Args:
         node: The Convolution node
 
     Returns:
         True if the node is a group convolution, else False
     """
-    return node.type in [Conv2d, ConvTranspose2d] and \
-           node.framework_attr[GROUPS] not in [node.framework_attr[IN_CHANNELS], 1]
+    return (node.is_match_type(Conv2d) or node.is_match_type(ConvTranspose2d)) and \
+        node.framework_attr[GROUPS] not in [node.framework_attr[IN_CHANNELS], 1]
 
 
 def get_foldable_node_type_and_validity_fn(node: BaseNode) -> [bool, bool]:
     """
     Check whether the node to forward fold is a valid dw-convolution node or a
     batch-normalization node
     Args:
         node: The node to fold
 
     Returns:
         is_bn: True if the node is a batch norm, else False
         is_dw_valid: True if the node is a dw-convolution valid for folding or a batch-norm node, else False
     """
-    is_bn = node.type is BatchNorm2d
-    is_dw = node.type is Conv2d and node.framework_attr[GROUPS] == node.framework_attr[IN_CHANNELS]
+    is_bn = node.is_match_type(BatchNorm2d)
+    is_dw = node.is_match_type(Conv2d) and node.framework_attr[GROUPS] == node.framework_attr[IN_CHANNELS]
     is_dw_valid = is_dw and np.all(np.array(node.get_weights_by_keys(KERNEL).shape[2:]) == 1)
     return is_bn, is_dw_valid
 
 
 def pytorch_batchnorm_folding() -> BatchNormalizationFolding:
     """
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
             graph: Graph we apply the substitution on.
             func_node: node that match the pattern in the substitution init.
 
         Returns:
             Graph after applying the substitution.
         """
         # Set new layer
-        if func_node.type == conv2d:
+        if func_node.is_match_type(conv2d):
             new_layer = Conv2d
-        elif func_node.type == conv_transpose2d:
+        elif func_node.is_match_type(conv_transpose2d):
             new_layer = ConvTranspose2d
         else:
             Logger.critical(f'Substitution filter mismatch. Layer {func_node.type}. Must be {type(Conv2d)} or {type(ConvTranspose2d)}.')  # pragma: no cover
 
         out_channel_index, in_channel_index = self.fw_info.kernel_channels_mapping.get(new_layer)
 
         # Create new node of layer convolution
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         first_node: First layer node to collapse to second layer node
         second_node: Second layer node
         kernel_str: The framework specific attribute name of the convolution layer's weight/kernel.
         bias_str: The framework specific attribute name of the convolution layer's bias.
     Returns:
         The modified layer node's weights: kernel, bias
     """
-    if first_node.type == Conv2d and second_node.type == Conv2d:
+    if first_node.is_match_type(Conv2d) and second_node.is_match_type(Conv2d):
         # Get nodes attributes
         kernel1 = first_node.get_weights_by_keys(kernel_str)
         kernel2 = second_node.get_weights_by_keys(kernel_str)
         bias1 = first_node.get_weights_by_keys(bias_str)
         bias2 = second_node.get_weights_by_keys(bias_str)
         strides1 = first_node.framework_attr[STRIDES]
         strides2 = second_node.framework_attr[STRIDES]
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,33 +72,33 @@
         """
 
         first_op2d_node = nodes_list[0]
         non_linear_node = nodes_list[1]
         second_op2d_node = nodes_list[2]
 
         # only act on bound relu with not POT max value and 0 min value
-        if non_linear_node.type == ReLU6:
+        if non_linear_node.is_match_type(ReLU6):
             scale_factor = 6.0 / self.threshold
             non_linear_node.layer_class = Hardtanh
             non_linear_node.framework_attr[INPLACE] = False
             non_linear_node.framework_attr[HARDTANH_MIN_VAL] = 0.0
             non_linear_node.framework_attr[HARDTANH_MAX_VAL] = self.threshold
-        elif non_linear_node.type == relu6:
+        elif non_linear_node.is_match_type(relu6):
             scale_factor = 6.0 / self.threshold
             non_linear_node.functional_op = hardtanh
             non_linear_node.functional_op.__defaults__ = (0.0, self.threshold, False)
-        elif non_linear_node.type == Hardtanh:
+        elif non_linear_node.is_match_type(Hardtanh):
             if (non_linear_node.framework_attr[HARDTANH_MIN_VAL] == 0.0) and not \
                     (np.log2(non_linear_node.framework_attr[HARDTANH_MAX_VAL]).astype(int) -
                      np.log2(non_linear_node.framework_attr[HARDTANH_MAX_VAL]) == 0):
                 scale_factor = non_linear_node.framework_attr[HARDTANH_MAX_VAL] / self.threshold
                 non_linear_node.framework_attr[HARDTANH_MAX_VAL] = self.threshold
             else:
                 return graph
-        elif non_linear_node.type == hardtanh:
+        elif non_linear_node.is_match_type(hardtanh):
             if (non_linear_node.framework_attr[HARDTANH_MIN_VAL] == 0.0) and not \
                     (np.log2(non_linear_node.framework_attr[HARDTANH_MAX_VAL]).astype(int) -
                      np.log2(non_linear_node.framework_attr[HARDTANH_MAX_VAL]) == 0):
                 scale_factor = non_linear_node.framework_attr[HARDTANH_MAX_VAL] / self.threshold
                 non_linear_node.functional_op.__defaults__ = (0.0, self.threshold, non_linear_node.framework_attr[INPLACE])
             else:
                 return graph
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     Inspired by https://arxiv.org/pdf/2103.09404.pdf - Algorithm2
     Args:
         first_node: First layer node to collapse into.
         kernel_str: The framework specific attribute name of the convolution layer's weight/kernel.
     Returns:
         The modified layer node's weights: kernel
     """
-    if first_node.type == Conv2d:
+    if first_node.is_match_type(Conv2d):
         # Get nodes attributes
         kernel = first_node.get_weights_by_keys(kernel_str)
         (Cout, Cin, kH, kW) = kernel.shape
 
         # Collapsing residual by adding "1" to kernel diagonal
         idxH = (kH - 1) // 2
         idxW = (kW - 1) // 2
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pruning/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,17 +72,17 @@
         """
         # TODO (reuvenp/liord): Address handling of node parameters that can be either a single value across all channels or distinct per channel, e.g., PReLU. Consider developing a structured approach.
         pruning_en = True
         _edit_node_input_shape(node, input_mask, fw_info)
         pruned_parameters = {}
         mask_bool = output_mask.astype(bool)
         node.weights = pruned_parameters
-        if node.type == torch.nn.BatchNorm2d:
+        if node.is_match_type(torch.nn.BatchNorm2d):
             node.framework_attr[NUM_FEATURES] = int(np.sum(input_mask))
-        elif node.type == torch.nn.PReLU:
+        elif node.is_match_type(torch.nn.PReLU):
             if node.framework_attr[NUM_PARAMETERS] > 1:
                 node.framework_attr[NUM_PARAMETERS] = int(np.sum(input_mask))
             else:
                 pruning_en = False
 
         if pruning_en:
             for k, v in node.weights.items():
@@ -223,17 +223,17 @@
         node (BaseNode): The node to be evaluated.
 
     Returns:
         bool: True if the node is an edge of a pruning section, False otherwise.
     """
 
     # Check if the node is a Conv2D or Conv2DTranspose layer with groups set to 1.
-    if node.type in [torch.nn.Conv2d, torch.nn.ConvTranspose2d]:
+    if node.is_match_type(torch.nn.Conv2d) or node.is_match_type(torch.nn.ConvTranspose2d):
         return node.framework_attr[GROUPS] == 1
-    return node.type == torch.nn.Linear
+    return node.is_match_type(torch.nn.Linear)
 
 
 def _prune_pytorch_edge_node(node: BaseNode,
                              mask: np.ndarray,
                              fw_info: FrameworkInfo,
                              is_exit_node: bool):
     """
@@ -264,26 +264,26 @@
         bias = node.get_weights_by_keys(BIAS)
         pruned_bias = bias.compress(mask_bool)
         node.set_weights_by_keys(name=BIAS, tensor=pruned_bias)
 
     if not is_exit_node:
         # Update 'out_channels' or 'out_features' attributes for entry nodes
         # Conv2d,ConvTranspose2d / Linear layers.
-        if node.type in [torch.nn.Conv2d, torch.nn.ConvTranspose2d]:
+        if node.is_match_type(torch.nn.Conv2d) or node.is_match_type(torch.nn.ConvTranspose2d):
             node.framework_attr[OUT_CHANNELS] = int(np.sum(mask))
-        elif node.type == torch.nn.Linear:
+        elif node.is_match_type(torch.nn.Linear):
             node.framework_attr[OUT_FEATURES] = int(np.sum(mask))
         else:
             Logger.critical(f"{node.type} is currently not supported"
                              f"as an edge node in a pruning section")
 
     if is_exit_node:
-        if node.type in [torch.nn.Conv2d, torch.nn.ConvTranspose2d]:
+        if node.is_match_type(torch.nn.Conv2d) or node.is_match_type(torch.nn.ConvTranspose2d):
             node.framework_attr[IN_CHANNELS] = int(np.sum(mask))
-        elif node.type == torch.nn.Linear:
+        elif node.is_match_type(torch.nn.Linear):
             node.framework_attr[IN_FEATURES] = int(np.sum(mask))
         else:
             Logger.critical(f"{node.type} is currently not supported"
                              f"as an edge node in a pruning section")
         # Adjust the input shape for the last node in the section.
         _edit_node_input_shape(node, mask_bool, fw_info)
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pytorch_device_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/pytorch_device_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files 4% similar despite different names*

```diff
@@ -394,16 +394,16 @@
         """
         Returns whether a given node in considered as a potential interest point for mp metric computation purposes.
         Args:
             node: Node to indicate whether it needs to be part of the interest points set.
         Returns: True if the node should be considered an interest point, False otherwise.
         """
 
-        if node.type in [Conv2d, Linear, ConvTranspose2d, Sigmoid, sigmoid, Softmax, softmax, operator.add, add, cat,
-                         operator.concat]:
+        if any([node.is_match_type(_type) for _type in [Conv2d, Linear, ConvTranspose2d, Sigmoid, sigmoid, Softmax,
+                                                        softmax, operator.add, add, cat, operator.concat]]):
             return True
         return False
 
     def get_node_distance_fn(self, layer_class: type,
                              framework_attrs: Dict[str, Any],
                              compute_distance_fn: Callable = None,
                              axis: int = None) -> Callable:
@@ -460,20 +460,20 @@
         Returns: The MAC count of the operation
         """
 
         output_shape = node.output_shape[0]
         kernel_shape = node.get_weights_by_keys(fw_info.get_kernel_op_attributes(node.type)[0]).shape
         output_channel_axis, input_channel_axis = fw_info.kernel_channels_mapping.get(node.type)
 
-        if node.type is Conv2d or node.type is ConvTranspose2d:
+        if node.is_match_type(Conv2d) or node.is_match_type(ConvTranspose2d):
             # (C_out * W_out * H_out) * C_in * (W_kernel * H_kernel)
             return np.prod([x for x in output_shape if x is not None]) * \
                    kernel_shape[input_channel_axis] * \
                    (kernel_shape[0] * kernel_shape[1])
-        elif node.type is Linear:
+        elif node.is_match_type(Linear):
             # IN * OUT
             return kernel_shape[0] * kernel_shape[1]
         else:
             return 0
 
     def apply_second_moment_correction(self,
                                        quantized_model: Any,
@@ -548,14 +548,13 @@
 
         Args:
            node: Node to get quantizers for.
 
         Returns:
             weight_quantizers: A dictionary between a weight's name to its quantizer.
             activation_quantizers: A list of activations quantization, one for each layer output.
-
         """
 
         return get_inferable_quantizers(node,
                                         get_weights_quantizer_for_node,
                                         get_activations_quantizer_for_node,
                                         node.get_node_weights_attributes())
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,25 +58,25 @@
         graph: Graph to check the next node type.
 
     Returns:
         Mean/Std output values if known.
     """
     mean_output, std_output = None, None
 
-    if node.type == BatchNorm2d:
+    if node.is_match_type(BatchNorm2d):
         mean_output = node.get_weights_by_keys(BETA)
         if node.get_weights_by_keys(GAMMA) is None:
             std_output = 1.0
         else:
             std_output = np.abs(node.get_weights_by_keys(GAMMA))
         if mean_output is None:
             mean_output = 0.0
     else:
         next_node_list = graph.get_next_nodes(node)
-        bn_nodes = [bn_node for bn_node in next_node_list if bn_node.type == BatchNorm2d]
+        bn_nodes = [bn_node for bn_node in next_node_list if bn_node.is_match_type(BatchNorm2d)]
         if len(bn_nodes) != 0:
             bn_node = bn_nodes[0]
             moving_variance = bn_node.get_weights_by_keys(MOVING_VARIANCE)
             std_output = np.sqrt(moving_variance)
             mean_output = bn_node.get_weights_by_keys(MOVING_MEAN)
 
     return mean_output, std_output
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/reader.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/utils.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/quantization_prep_runner.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/quantization_prep_runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/runner.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/core/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/constants.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/data_generation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/data_generation_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/data_generation_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/enums.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/enums.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/image_pipeline.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/model_info_exctractors.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/optimization_utils.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/common/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/constants.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/image_pipeline.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/keras_data_generation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/keras_data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/model_info_exctractors.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_utils.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/keras/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/constants.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/image_pipeline.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_utils.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/defaultdict.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/defaultdict.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,20 @@
             layer: A keras layer
 
         Returns: Wrapped layer with weights quantizers and activation quantizers
 
         """
         weights_quantizers, _ = fw_impl.get_inferable_quantizers(node)
         if len(weights_quantizers) > 0:
+            # for positional weights we need to extract the weight's value.
+            weights_values = {attr: node.get_weights_by_keys(attr)
+                              for attr in weights_quantizers if isinstance(attr, int)}
             return KerasQuantizationWrapper(layer,
-                                            weights_quantizers)
+                                            weights_quantizers,
+                                            weights_values)
         return layer
 
 
     def get_activation_quantizer_holder(node: common.BaseNode, fw_impl) -> Callable:
         """
         Retrieve a ActivationQuantizationHolder layer to use for activation quantization for a node.
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,49 +25,56 @@
     import torch
     from mct_quantizers import PytorchQuantizationWrapper, PytorchActivationQuantizationHolder
     from model_compression_toolkit.core.pytorch.back2framework.pytorch_model_builder import PyTorchModelBuilder
 
 
     def fully_quantized_wrapper(node: common.BaseNode,
                                 module: torch.nn.Module,
-                                fw_impl) -> Union[torch.nn.Module,PytorchQuantizationWrapper]:
+                                fw_impl) -> Union[torch.nn.Module, PytorchQuantizationWrapper]:
         """
         A function which takes a computational graph node and a pytorch module and
         perform the quantization wrapping
 
         Args:
             node: A node of mct graph.
             module: A Pytorch module
+            fw_impl: FrameworkImplementation object with a specific framework methods implementation.
         Returns: Wrapped layer
 
         """
         weight_quantizers, _ = fw_impl.get_inferable_quantizers(node)
         if len(weight_quantizers) > 0:
-            return PytorchQuantizationWrapper(module, weight_quantizers)
+            # for positional weights we need to extract the weight's value.
+            weights_values = {attr: fw_impl.to_tensor(node.get_weights_by_keys(attr))
+                              for attr in weight_quantizers if isinstance(attr, int)}
+            return PytorchQuantizationWrapper(module, weight_quantizers, weights_values)
         return module
 
+
     def get_activation_quantizer_holder(node: BaseNode, fw_impl) -> Callable:
         """
         Retrieve a PytorchActivationQuantizationHolder layer to use for activation quantization of a node.
         If the layer is not supposed to be wrapped with an activation quantizer - return None.
         Args:
             node: Node to attach a PytorchActivationQuantizationHolder to its output.
+            fw_impl: FrameworkImplementation object with a specific framework methods implementation.
         Returns:
             A PytorchActivationQuantizationHolder module for the node's activation quantization.
         """
         _, activation_quantizers = fw_impl.get_inferable_quantizers(node)
         # Holder by definition uses a single quantizer for the activation quantization
         # thus we make sure this is the only possible case (unless it's a node we no activation
         # quantization, which in this case has an empty list).
         if len(activation_quantizers) == 1:
             return PytorchActivationQuantizationHolder(activation_quantizers[0])
         Logger.critical(
             f'PytorchActivationQuantizationHolder supports a single quantizer but {len(activation_quantizers)} quantizers '
             f'were found for node {node}')
 
+
     def get_exportable_pytorch_model(graph: Graph):
         """
         Convert graph to fully quantized PyTorch model.
 
         Args:
             graph: Graph to convert to a PyTorch model.
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_constants.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_framework_implementation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/common/gptq_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_graph.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_training.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/gptq_loss.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/gptq_training.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/graph_info.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/graph_info.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/runner.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/gptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/logger.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/metadata.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/metadata.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/keras/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/pruning/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/keras/pruning_facade.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/pruning/keras/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/pytorch/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/pruning/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/pytorch/pruning_facade.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/pruning/pytorch/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/keras/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/pytorch/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/runner.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/common/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/common/qat_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/common/qat_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/constants.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/immutable.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/immutable.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     Returns: An OpQuantizationConfig config object and a list of OpQuantizationConfig objects.
 
     """
 
     # We define a default quantization config for all non-specified weights attributes.
     default_weight_attr_config = AttributeQuantizationConfig(
-        weights_quantization_method=tp.QuantizationMethod.SYMMETRIC,
+        weights_quantization_method=tp.QuantizationMethod.POWER_OF_TWO,
         weights_n_bits=8,
         weights_per_channel_threshold=False,
         enable_weights_quantization=False,
         lut_values_bitwidth=None)
 
     # We define a quantization config to quantize the kernel (for layers where there is a kernel attribute).
     kernel_base_config = AttributeQuantizationConfig(
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,27 +28,28 @@
 def get_tp_model() -> TargetPlatformModel:
     """
     A method that generates a default target platform model, with base 8-bit quantization configuration and 8, 4, 2
     bits configuration list for mixed-precision quantization.
     NOTE: in order to generate a target platform model with different configurations but with the same Operators Sets
     (for tests, experiments, etc.), use this method implementation as a test-case, i.e., override the
     'get_op_quantization_configs' method and use its output to call 'generate_tp_model' with your configurations.
-    This version enables metadata by default
+    This version enables metadata by default.
 
     Returns: A TargetPlatformModel object.
 
     """
     base_config, mixed_precision_cfg_list, default_config = get_op_quantization_configs()
     return generate_tp_model(default_config=default_config,
                              base_config=base_config,
                              mixed_precision_cfg_list=mixed_precision_cfg_list,
                              name='imx500_tp_model')
 
 
-def get_op_quantization_configs() -> Tuple[OpQuantizationConfig, List[OpQuantizationConfig], OpQuantizationConfig]:
+def get_op_quantization_configs() -> \
+        Tuple[OpQuantizationConfig, List[OpQuantizationConfig], OpQuantizationConfig]:
     """
     Creates a default configuration object for 8-bit quantization, to be used to set a default TargetPlatformModel.
     In addition, creates a default configuration objects list (with 8, 4 and 2 bit quantization) to be used as
     default configuration for mixed-precision quantization.
 
     Returns: An OpQuantizationConfig config object and a list of OpQuantizationConfig objects.
 
@@ -147,14 +148,27 @@
     """
     # Create a QuantizationConfigOptions, which defines a set
     # of possible configurations to consider when quantizing a set of operations (in mixed-precision, for example).
     # If the QuantizationConfigOptions contains only one configuration,
     # this configuration will be used for the operation quantization:
     default_configuration_options = tp.QuantizationConfigOptions([default_config])
 
+    # Create a QuantizationConfigOptions for quantizing constants in functional ops.
+    # Constant configuration is similar to the default eight bit configuration except for PoT
+    # quantization method for the constant.
+    # Since the constants are not named attributes of the layer, we use the default_weight_attr_config to
+    # define the desired quantization properties for them.
+    const_config = default_config.clone_and_edit(
+        default_weight_attr_config=default_config.default_weight_attr_config.clone_and_edit(
+            enable_weights_quantization=True))
+    if not (const_config.default_weight_attr_config.weights_quantization_method == tp.QuantizationMethod.POWER_OF_TWO and
+            const_config.default_weight_attr_config.weights_per_channel_threshold is False):
+        mct.logger.Logger.error('Constant quantization config should be per-tensor PoT.')
+    const_configuration_options = tp.QuantizationConfigOptions([const_config])
+
     # Create a TargetPlatformModel and set its default quantization config.
     # This default configuration will be used for all operations
     # unless specified otherwise (see OperatorsSet, for example):
     generated_tpm = tp.TargetPlatformModel(default_configuration_options, add_metadata=True, name=name)
 
     # To start defining the model's components (such as operator sets, and fusing patterns),
     # use 'with' the TargetPlatformModel instance, and create them as below:
@@ -180,18 +194,18 @@
         # Define operator sets that use mixed_precision_configuration_options:
         conv = tp.OperatorsSet("Conv", mixed_precision_configuration_options)
         fc = tp.OperatorsSet("FullyConnected", mixed_precision_configuration_options)
 
         # Define operations sets without quantization configuration
         # options (useful for creating fusing patterns, for example):
         any_relu = tp.OperatorsSet("AnyReLU")
-        add = tp.OperatorsSet("Add")
-        sub = tp.OperatorsSet("Sub")
-        mul = tp.OperatorsSet("Mul")
-        div = tp.OperatorsSet("Div")
+        add = tp.OperatorsSet("Add", const_configuration_options)
+        sub = tp.OperatorsSet("Sub", const_configuration_options)
+        mul = tp.OperatorsSet("Mul", const_configuration_options)
+        div = tp.OperatorsSet("Div", const_configuration_options)
         prelu = tp.OperatorsSet("PReLU")
         swish = tp.OperatorsSet("Swish")
         sigmoid = tp.OperatorsSet("Sigmoid")
         tanh = tp.OperatorsSet("Tanh")
 
         # Combine multiple operators into a single operator to avoid quantization between
         # them. To do this we define fusing patterns using the OperatorsSets that were created.
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,14 @@
                                              ReLU,
                                              LeakyReLU,
                                              tp.LayerFilterParams(Activation, activation="relu"),
                                              tp.LayerFilterParams(Activation, activation="leaky_relu")])
         tp.OperationsSetToLayers("Add", [tf.add, Add])
         tp.OperationsSetToLayers("Sub", [tf.subtract, Subtract])
         tp.OperationsSetToLayers("Mul", [tf.math.multiply, Multiply])
-        tp.OperationsSetToLayers("Div", [tf.math.divide])
+        tp.OperationsSetToLayers("Div", [tf.math.divide, tf.math.truediv])
         tp.OperationsSetToLayers("PReLU", [PReLU])
         tp.OperationsSetToLayers("Swish", [tf.nn.swish, tp.LayerFilterParams(Activation, activation="swish")])
         tp.OperationsSetToLayers("Sigmoid", [tf.nn.sigmoid, tp.LayerFilterParams(Activation, activation="sigmoid")])
         tp.OperationsSetToLayers("Tanh", [tf.nn.tanh, tp.LayerFilterParams(Activation, activation="tanh")])
 
     return keras_tpc
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,45 +29,46 @@
 def get_tp_model() -> TargetPlatformModel:
     """
     A method that generates a default target platform model, with base 8-bit quantization configuration and 8, 4, 2
     bits configuration list for mixed-precision quantization.
     NOTE: in order to generate a target platform model with different configurations but with the same Operators Sets
     (for tests, experiments, etc.), use this method implementation as a test-case, i.e., override the
     'get_op_quantization_configs' method and use its output to call 'generate_tp_model' with your configurations.
-    This version enables metadata by default
+    This version enables metadata by default.
 
     Returns: A TargetPlatformModel object.
 
     """
     base_config, mixed_precision_cfg_list, default_config = get_op_quantization_configs()
     return generate_tp_model(default_config=default_config,
                              base_config=base_config,
                              mixed_precision_cfg_list=mixed_precision_cfg_list,
                              name='imx500_lut_tp_model')
 
 
-def get_op_quantization_configs() -> Tuple[OpQuantizationConfig, List[OpQuantizationConfig], OpQuantizationConfig]:
+def get_op_quantization_configs() -> \
+        Tuple[OpQuantizationConfig, List[OpQuantizationConfig], OpQuantizationConfig]:
     """
     Creates a default configuration object for 8-bit quantization, to be used to set a default TargetPlatformModel.
     In addition, creates a default configuration objects list (with 8, 4 and 2 bit quantization) to be used as
     default configuration for mixed-precision quantization with non-uniform quantizer for 2 and 4 bit candidates.
 
     Returns: An OpQuantizationConfig config object and a list of OpQuantizationConfig objects.
 
     """
 
     # We define a default quantization config for all non-specified weights attributes.
     default_weight_attr_config = AttributeQuantizationConfig(
-        weights_quantization_method=tp.QuantizationMethod.SYMMETRIC,
+        weights_quantization_method=tp.QuantizationMethod.POWER_OF_TWO,
         weights_n_bits=8,
         weights_per_channel_threshold=False,
         enable_weights_quantization=False,
         lut_values_bitwidth=None)
 
-    # We define a quantization config to quantize the kernel (for layers where there is a kernel attribute).
+    # define a quantization config to quantize the kernel (for layers where there is a kernel attribute).
     kernel_base_config = AttributeQuantizationConfig(
         weights_quantization_method=tp.QuantizationMethod.SYMMETRIC,
         weights_n_bits=8,
         weights_per_channel_threshold=True,
         enable_weights_quantization=True,
         lut_values_bitwidth=None)
 
@@ -146,14 +147,27 @@
     """
     # Create a QuantizationConfigOptions, which defines a set
     # of possible configurations to consider when quantizing a set of operations (in mixed-precision, for example).
     # If the QuantizationConfigOptions contains only one configuration,
     # this configuration will be used for the operation quantization:
     default_configuration_options = tp.QuantizationConfigOptions([default_config])
 
+    # Create a QuantizationConfigOptions for quantizing constants in functional ops.
+    # Constant configuration is similar to the default eight bit configuration except for PoT
+    # quantization method for the constant.
+    # Since the constants are not named attributes of the layer, we use the default_weight_attr_config to
+    # define the desired quantization properties for them.
+    const_config = default_config.clone_and_edit(
+        default_weight_attr_config=default_config.default_weight_attr_config.clone_and_edit(
+            enable_weights_quantization=True))
+    if not (const_config.default_weight_attr_config.weights_quantization_method == tp.QuantizationMethod.POWER_OF_TWO and
+            const_config.default_weight_attr_config.weights_per_channel_threshold is False):
+        mct.logger.Logger.error('Constant quantization config should be per-tensor PoT.')
+    const_configuration_options = tp.QuantizationConfigOptions([const_config])
+
     # Create a TargetPlatformModel and set its default quantization config.
     # This default configuration will be used for all operations
     # unless specified otherwise (see OperatorsSet, for example):
     generated_tpm = tp.TargetPlatformModel(default_configuration_options, add_metadata=True, name=name)
 
     # To start defining the model's components (such as operator sets, and fusing patterns),
     # use 'with' the TargetPlatformModel instance, and create them as below:
@@ -177,18 +191,18 @@
         # Define operator sets that use mixed_precision_configuration_options:
         conv = tp.OperatorsSet("Conv", mixed_precision_configuration_options)
         fc = tp.OperatorsSet("FullyConnected", mixed_precision_configuration_options)
 
         # Define operations sets without quantization configuration
         # options (useful for creating fusing patterns, for example):
         any_relu = tp.OperatorsSet("AnyReLU")
-        add = tp.OperatorsSet("Add")
-        sub = tp.OperatorsSet("Sub")
-        mul = tp.OperatorsSet("Mul")
-        div = tp.OperatorsSet("Div")
+        add = tp.OperatorsSet("Add", const_configuration_options)
+        sub = tp.OperatorsSet("Sub", const_configuration_options)
+        mul = tp.OperatorsSet("Mul", const_configuration_options)
+        div = tp.OperatorsSet("Div", const_configuration_options)
         prelu = tp.OperatorsSet("PReLU")
         swish = tp.OperatorsSet("Swish")
         sigmoid = tp.OperatorsSet("Sigmoid")
         tanh = tp.OperatorsSet("Tanh")
 
         # Combine multiple operators into a single operator to avoid quantization between
         # them. To do this we define fusing patterns using the OperatorsSets that were created.
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,14 +118,14 @@
                                              ReLU,
                                              LeakyReLU,
                                              tp.LayerFilterParams(Activation, activation="relu"),
                                              tp.LayerFilterParams(Activation, activation="leaky_relu")])
         tp.OperationsSetToLayers("Add", [tf.add, Add])
         tp.OperationsSetToLayers("Sub", [tf.subtract, Subtract])
         tp.OperationsSetToLayers("Mul", [tf.math.multiply, Multiply])
-        tp.OperationsSetToLayers("Div", [tf.math.divide])
+        tp.OperationsSetToLayers("Div", [tf.math.divide, tf.math.truediv])
         tp.OperationsSetToLayers("PReLU", [PReLU])
         tp.OperationsSetToLayers("Swish", [tf.nn.swish, tp.LayerFilterParams(Activation, activation="swish")])
         tp.OperationsSetToLayers("Sigmoid", [tf.nn.sigmoid, tp.LayerFilterParams(Activation, activation="sigmoid")])
         tp.OperationsSetToLayers("Tanh", [tf.nn.tanh, tp.LayerFilterParams(Activation, activation="tanh")])
 
     return keras_tpc
```

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/constants.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/load_model.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py` & `mct-nightly-2.0.0.20240419.358/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240418.439/setup.py` & `mct-nightly-2.0.0.20240419.358/setup.py`

 * *Files identical despite different names*

