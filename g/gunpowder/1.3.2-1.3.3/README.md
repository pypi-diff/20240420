# Comparing `tmp/gunpowder-1.3.2.tar.gz` & `tmp/gunpowder-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gunpowder-1.3.2.tar", last modified: Wed Jan  3 05:32:39 2024, max compression
+gzip compressed data, was "gunpowder-1.3.3.tar", last modified: Sat Apr 20 01:12:08 2024, max compression
```

## Comparing `gunpowder-1.3.2.tar` & `gunpowder-1.3.3.tar`

### file list

```diff
@@ -1,124 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.193826 gunpowder-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-03 05:32:31.000000 gunpowder-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-01-03 05:32:39.193826 gunpowder-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-01-03 05:32:31.000000 gunpowder-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.177826 gunpowder-1.3.2/gunpowder/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/array_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/batch_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.177826 gunpowder-1.3.2/gunpowder/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.181825 gunpowder-1.3.2/gunpowder/contrib/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/contrib/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/contrib/nodes/add_blobs_from_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/contrib/nodes/add_boundary_distance_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/contrib/nodes/add_gt_mask_exclusive_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/contrib/nodes/add_nonsymmetric_affinities.py
--rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/contrib/nodes/add_vector_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/contrib/nodes/dvid_partner_annotation_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/contrib/nodes/hdf5_points_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/contrib/nodes/prepare_malis.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/contrib/nodes/zero_out_const_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/coordinate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.181825 gunpowder-1.3.2/gunpowder/ext/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/ext/zarr_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/freezable.py
--rw-r--r--   0 runner    (1001) docker     (127)    20675 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/graph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.181825 gunpowder-1.3.2/gunpowder/jax/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/jax/generic_jax_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.181825 gunpowder-1.3.2/gunpowder/jax/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/jax/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/jax/nodes/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/jax/nodes/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.189826 gunpowder-1.3.2/gunpowder/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/add_affinities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/astype.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/balance_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/batch_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14045 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/batch_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/csv_points_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/daisy_request_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12989 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/defect_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    24904 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/deform_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/downsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/dvid_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    23829 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/elastic_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/exclude_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/generic_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/generic_train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/graph_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/grow_boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/hdf5_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/hdf5_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/hdf5like_source_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/hdf5like_write_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/intensity_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/intensity_scale_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/iterate_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/klb_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/merge_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/noise_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/precache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/print_profiling_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    17506 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/random_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/random_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    15392 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/rasterize_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/reject.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/renumber_connected_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/resample.py
--rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/shift_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/simple_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/specified_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/squeeze.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/unsqueeze.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/upsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/zarr_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/nodes/zarr_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/producer_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/provider_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/roi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.189826 gunpowder-1.3.2/gunpowder/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/tensorflow/local_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.189826 gunpowder-1.3.2/gunpowder/tensorflow/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/tensorflow/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/tensorflow/nodes/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/tensorflow/nodes/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.189826 gunpowder-1.3.2/gunpowder/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.193826 gunpowder-1.3.2/gunpowder/torch/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/torch/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/torch/nodes/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/torch/nodes/train.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/version_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.193826 gunpowder-1.3.2/gunpowder/zoo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.193826 gunpowder-1.3.2/gunpowder/zoo/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/zoo/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-01-03 05:32:31.000000 gunpowder-1.3.2/gunpowder/zoo/tensorflow/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:32:39.193826 gunpowder-1.3.2/gunpowder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-01-03 05:32:39.000000 gunpowder-1.3.2/gunpowder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-01-03 05:32:39.000000 gunpowder-1.3.2/gunpowder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 05:32:39.000000 gunpowder-1.3.2/gunpowder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-03 05:32:39.000000 gunpowder-1.3.2/gunpowder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-03 05:32:39.000000 gunpowder-1.3.2/gunpowder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-01-03 05:32:31.000000 gunpowder-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-03 05:32:39.193826 gunpowder-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.257500 gunpowder-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-20 01:12:04.000000 gunpowder-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-20 01:12:08.257500 gunpowder-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-20 01:12:04.000000 gunpowder-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.237501 gunpowder-1.3.3/gunpowder/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/array_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.241500 gunpowder-1.3.3/gunpowder/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.241500 gunpowder-1.3.3/gunpowder/contrib/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/contrib/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/contrib/nodes/add_blobs_from_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/contrib/nodes/add_boundary_distance_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/contrib/nodes/add_gt_mask_exclusive_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/contrib/nodes/add_nonsymmetric_affinities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/contrib/nodes/add_vector_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/contrib/nodes/dvid_partner_annotation_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/contrib/nodes/hdf5_points_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/contrib/nodes/prepare_malis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/contrib/nodes/zero_out_const_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.241500 gunpowder-1.3.3/gunpowder/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/ext/zarr_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/freezable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21058 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.241500 gunpowder-1.3.3/gunpowder/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/jax/generic_jax_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.241500 gunpowder-1.3.3/gunpowder/jax/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/jax/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/jax/nodes/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/jax/nodes/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.253500 gunpowder-1.3.3/gunpowder/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/add_affinities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/astype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/balance_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/batch_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14045 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/batch_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/csv_points_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/daisy_request_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/defect_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24904 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/deform_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/dvid_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23829 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/elastic_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/exclude_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/generic_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/generic_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/graph_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/grow_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/hdf5_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/hdf5_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/hdf5like_source_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/hdf5like_write_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/intensity_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/intensity_scale_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/iterate_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/klb_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/merge_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/noise_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/precache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/print_profiling_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17506 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/random_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/random_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/rasterize_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/reject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/renumber_connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/shift_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/simple_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/specified_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/unsqueeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/zarr_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/nodes/zarr_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/producer_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/provider_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/roi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.253500 gunpowder-1.3.3/gunpowder/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/tensorflow/local_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.253500 gunpowder-1.3.3/gunpowder/tensorflow/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/tensorflow/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/tensorflow/nodes/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/tensorflow/nodes/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.253500 gunpowder-1.3.3/gunpowder/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.253500 gunpowder-1.3.3/gunpowder/torch/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/torch/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/torch/nodes/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/torch/nodes/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/version_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.253500 gunpowder-1.3.3/gunpowder/zoo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.253500 gunpowder-1.3.3/gunpowder/zoo/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/zoo/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-20 01:12:04.000000 gunpowder-1.3.3/gunpowder/zoo/tensorflow/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:12:08.253500 gunpowder-1.3.3/gunpowder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-20 01:12:08.000000 gunpowder-1.3.3/gunpowder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-20 01:12:08.000000 gunpowder-1.3.3/gunpowder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:12:08.000000 gunpowder-1.3.3/gunpowder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-20 01:12:08.000000 gunpowder-1.3.3/gunpowder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 01:12:08.000000 gunpowder-1.3.3/gunpowder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-20 01:12:04.000000 gunpowder-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:12:08.257500 gunpowder-1.3.3/setup.cfg
```

### Comparing `gunpowder-1.3.2/LICENSE` & `gunpowder-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/PKG-INFO` & `gunpowder-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunpowder
-Version: 1.3.2
+Version: 1.3.3
 Summary: A library to facilitate machine learning on large, multi-dimensional images.
 Author: Renate Krause, Julia Buhmann, Rodrigo Ceballos Lentini, William Grisaitis, Chris Barnes, Caroline Malin-Mayor, Larissa Heinrich, Philipp Hanslovsky, Sherry Ding, Andrew Champion, Arlo Sheridan, Constantin Pape
 Author-email: Jan Funke <funkej@hhmi.org>, William Patton <pattonw@hhmi.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gunpowder-1.3.2/README.md` & `gunpowder-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/__init__.py` & `gunpowder-1.3.3/gunpowder/__init__.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/array.py` & `gunpowder-1.3.3/gunpowder/array.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/array_spec.py` & `gunpowder-1.3.3/gunpowder/array_spec.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/batch.py` & `gunpowder-1.3.3/gunpowder/batch.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/batch_request.py` & `gunpowder-1.3.3/gunpowder/batch_request.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/build.py` & `gunpowder-1.3.3/gunpowder/build.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/contrib/nodes/__init__.py` & `gunpowder-1.3.3/gunpowder/contrib/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/contrib/nodes/add_blobs_from_points.py` & `gunpowder-1.3.3/gunpowder/contrib/nodes/add_blobs_from_points.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/contrib/nodes/add_boundary_distance_gradients.py` & `gunpowder-1.3.3/gunpowder/contrib/nodes/add_boundary_distance_gradients.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/contrib/nodes/add_gt_mask_exclusive_zone.py` & `gunpowder-1.3.3/gunpowder/contrib/nodes/add_gt_mask_exclusive_zone.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/contrib/nodes/add_nonsymmetric_affinities.py` & `gunpowder-1.3.3/gunpowder/contrib/nodes/add_nonsymmetric_affinities.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/contrib/nodes/add_vector_map.py` & `gunpowder-1.3.3/gunpowder/contrib/nodes/add_vector_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,17 +211,17 @@
                     # check for target node with largest distance first and add vector pointing to it to vector_map_total
                     num_src_vectors_per_trg_loc = len(
                         locations_to_fill_abs_phys
                     ) // len(relevant_partner_loc)
                     if num_src_vectors_per_trg_loc > 0:
                         dist_to_locs = {}
                         for phys_loc in relevant_partner_loc:
-                            dist_to_locs[
-                                np.linalg.norm(node.location - phys_loc)
-                            ] = phys_loc
+                            dist_to_locs[np.linalg.norm(node.location - phys_loc)] = (
+                                phys_loc
+                            )
                         for nr, dist in enumerate(
                             reversed(np.sort(list(dist_to_locs.keys())))
                         ):
                             trg_loc_abs_phys = dist_to_locs[dist]
                             kdtree_locs_vector_map = KDTree(locations_to_fill_abs_phys)
                             if nr == len(relevant_partner_loc) - 1:
                                 num_src_vectors_per_trg_loc = len(
```

### Comparing `gunpowder-1.3.2/gunpowder/contrib/nodes/dvid_partner_annotation_source.py` & `gunpowder-1.3.3/gunpowder/contrib/nodes/dvid_partner_annotation_source.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/contrib/nodes/hdf5_points_source.py` & `gunpowder-1.3.3/gunpowder/contrib/nodes/hdf5_points_source.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/contrib/nodes/prepare_malis.py` & `gunpowder-1.3.3/gunpowder/contrib/nodes/prepare_malis.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/contrib/nodes/zero_out_const_sections.py` & `gunpowder-1.3.3/gunpowder/contrib/nodes/zero_out_const_sections.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/ext/__init__.py` & `gunpowder-1.3.3/gunpowder/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/graph.py` & `gunpowder-1.3.3/gunpowder/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,17 +147,27 @@
         return self.__u
 
     @property
     def v(self):
         return self.__v
 
     @property
+    def attrs(self):
+        return self.__attrs
+
+    @property
     def all(self):
         return self.__attrs
 
+    @classmethod
+    def from_attrs(cls, attrs: Dict[str, Any]):
+        u = attrs["u"]
+        v = attrs["v"]
+        return cls(u, v, attrs=attrs)
+
     def __iter__(self):
         return iter([self.u, self.v])
 
     def __str__(self):
         return f"({self.u}, {self.v})"
 
     def __repr__(self):
@@ -283,14 +293,21 @@
     def node(self, id: int):
         """
         Get node with a specific id
         """
         attrs = self.__graph.nodes[id]
         return Node.from_attrs(attrs)
 
+    def edge(self, id: tuple[int, int]):
+        """
+        Get specific edge
+        """
+        attrs = self.__graph.edges[id]
+        return Edge.from_attrs(attrs)
+
     def contains(self, node_id: int):
         return node_id in self.__graph.nodes
 
     def remove_node(self, node: Node, retain_connectivity=False):
         """
         Remove a node.
```

### Comparing `gunpowder-1.3.2/gunpowder/graph_spec.py` & `gunpowder-1.3.3/gunpowder/graph_spec.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/jax/generic_jax_model.py` & `gunpowder-1.3.3/gunpowder/jax/generic_jax_model.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/jax/nodes/predict.py` & `gunpowder-1.3.3/gunpowder/jax/nodes/predict.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/jax/nodes/train.py` & `gunpowder-1.3.3/gunpowder/jax/nodes/train.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/morphology.py` & `gunpowder-1.3.3/gunpowder/morphology.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/__init__.py` & `gunpowder-1.3.3/gunpowder/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/add_affinities.py` & `gunpowder-1.3.3/gunpowder/nodes/add_affinities.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/astype.py` & `gunpowder-1.3.3/gunpowder/nodes/astype.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/balance_labels.py` & `gunpowder-1.3.3/gunpowder/nodes/balance_labels.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/batch_filter.py` & `gunpowder-1.3.3/gunpowder/nodes/batch_filter.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/batch_provider.py` & `gunpowder-1.3.3/gunpowder/nodes/batch_provider.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/crop.py` & `gunpowder-1.3.3/gunpowder/nodes/crop.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/csv_points_source.py` & `gunpowder-1.3.3/gunpowder/nodes/csv_points_source.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/daisy_request_blocks.py` & `gunpowder-1.3.3/gunpowder/nodes/daisy_request_blocks.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/defect_augment.py` & `gunpowder-1.3.3/gunpowder/nodes/defect_augment.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,17 +155,19 @@
         # prepare transformation and
         # request bigger upstream roi for deformed slice
         if "deformed_slice" in self.slice_to_augmentation.values():
             # create roi sufficiently large to feed deformation
             logger.debug("before growth: %s" % spec.roi)
             growth = Coordinate(
                 tuple(
-                    0
-                    if d == self.axis
-                    else raw_voxel_size[d] * self.deformation_strength
+                    (
+                        0
+                        if d == self.axis
+                        else raw_voxel_size[d] * self.deformation_strength
+                    )
                     for d in range(spec.roi.dims)
                 )
             )
             logger.debug("growing request by %s" % str(growth))
             source_roi = roi.grow(growth, growth)
 
             # update request ROI to get all voxels necessary to perfrom
@@ -186,15 +188,15 @@
                 slice(None if d != self.axis else c, None if d != self.axis else c + 1)
                 for d in range(raw.spec.roi.dims)
             )
 
             if augmentation_type == "zero_out":
                 raw.data[section_selector] = 0
 
-            elif augmentation_type == "low_contrast":
+            elif augmentation_type == "lower_contrast":
                 section = raw.data[section_selector]
 
                 mean = section.mean()
                 section -= mean
                 section *= self.contrast_scale
                 section += mean
 
@@ -263,17 +265,19 @@
 
         # in case we needed to change the ROI due to a deformation augment,
         # restore original ROI and crop the array data
         if "deformed_slice" in self.slice_to_augmentation.values():
             old_roi = request[self.intensities].roi
             logger.debug("resetting roi to %s" % old_roi)
             crop = tuple(
-                slice(None)
-                if d == self.axis
-                else slice(self.deformation_strength, -self.deformation_strength)
+                (
+                    slice(None)
+                    if d == self.axis
+                    else slice(self.deformation_strength, -self.deformation_strength)
+                )
                 for d in range(raw.spec.roi.dims)
             )
             raw.data = raw.data[crop]
             raw.spec.roi = old_roi
 
     def __prepare_deform_slice(self, slice_shape):
         # grow slice shape by 2 x deformation strength
```

### Comparing `gunpowder-1.3.2/gunpowder/nodes/deform_augment.py` & `gunpowder-1.3.3/gunpowder/nodes/deform_augment.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/downsample.py` & `gunpowder-1.3.3/gunpowder/nodes/downsample.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/dvid_source.py` & `gunpowder-1.3.3/gunpowder/nodes/dvid_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,20 +178,20 @@
                     data_dtype,
                 )
             )
         else:
             spec.dtype = data_dtype
 
         if spec.interpolatable is None:
-            spec.interpolatable = spec.dtype in [
-                np.float32,
-                np.float64,
-                np.float128,
-                np.uint8,  # assuming this is not used for labels
-            ]
+            spec.interpolatable = spec.dtype in (
+                np.sctypes["float"]
+                + [
+                    np.uint8,  # assuming this is not used for labels
+                ]
+            )
             logger.warning(
                 "WARNING: You didn't set 'interpolatable' for %s. "
                 "Based on the dtype %s, it has been set to %s. "
                 "This might not be what you want.",
                 array_key,
                 spec.dtype,
                 spec.interpolatable,
```

### Comparing `gunpowder-1.3.2/gunpowder/nodes/elastic_augment.py` & `gunpowder-1.3.3/gunpowder/nodes/elastic_augment.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/exclude_labels.py` & `gunpowder-1.3.3/gunpowder/nodes/exclude_labels.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/generic_predict.py` & `gunpowder-1.3.3/gunpowder/nodes/generic_predict.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/generic_train.py` & `gunpowder-1.3.3/gunpowder/nodes/generic_train.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/graph_source.py` & `gunpowder-1.3.3/gunpowder/nodes/graph_source.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/grow_boundary.py` & `gunpowder-1.3.3/gunpowder/nodes/grow_boundary.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/hdf5_source.py` & `gunpowder-1.3.3/gunpowder/nodes/hdf5_source.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/hdf5_write.py` & `gunpowder-1.3.3/gunpowder/nodes/hdf5_write.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/hdf5like_source_base.py` & `gunpowder-1.3.3/gunpowder/nodes/hdf5like_source_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,20 +170,20 @@
                 "but differs from dataset %s dtype %s"
                 % (self.array_specs[array_key].dtype, array_key, ds_name, dataset.dtype)
             )
         else:
             spec.dtype = dataset.dtype
 
         if spec.interpolatable is None:
-            spec.interpolatable = spec.dtype in [
-                np.float32,
-                np.float64,
-                np.float128,
-                np.uint8,  # assuming this is not used for labels
-            ]
+            spec.interpolatable = spec.dtype in (
+                np.sctypes["float"]
+                + [
+                    np.uint8,  # assuming this is not used for labels
+                ]
+            )
             logger.warning(
                 "WARNING: You didn't set 'interpolatable' for %s "
                 "(dataset %s). Based on the dtype %s, it has been "
                 "set to %s. This might not be what you want.",
                 array_key,
                 ds_name,
                 spec.dtype,
```

### Comparing `gunpowder-1.3.2/gunpowder/nodes/hdf5like_write_base.py` & `gunpowder-1.3.3/gunpowder/nodes/hdf5like_write_base.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/intensity_augment.py` & `gunpowder-1.3.3/gunpowder/nodes/intensity_augment.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/intensity_scale_shift.py` & `gunpowder-1.3.3/gunpowder/nodes/intensity_scale_shift.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/iterate_locations.py` & `gunpowder-1.3.3/gunpowder/nodes/iterate_locations.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/klb_source.py` & `gunpowder-1.3.3/gunpowder/nodes/klb_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,20 +151,20 @@
                 "dataset dtype %s"
                 % (self.array_specs[self.array].dtype, self.array, dataset.dtype)
             )
         else:
             spec.dtype = dtype
 
         if spec.interpolatable is None:
-            spec.interpolatable = spec.dtype in [
-                np.float32,
-                np.float64,
-                np.float128,
-                np.uint8,  # assuming this is not used for labels
-            ]
+            spec.interpolatable = spec.dtype in (
+                np.sctypes["float"]
+                + [
+                    np.uint8,  # assuming this is not used for labels
+                ]
+            )
             logger.warning(
                 "WARNING: You didn't set 'interpolatable' for %s. "
                 "Based on the dtype %s, it has been set to %s. "
                 "This might not be what you want.",
                 self.array,
                 spec.dtype,
                 spec.interpolatable,
```

### Comparing `gunpowder-1.3.2/gunpowder/nodes/merge_provider.py` & `gunpowder-1.3.3/gunpowder/nodes/merge_provider.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/noise_augment.py` & `gunpowder-1.3.3/gunpowder/nodes/noise_augment.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/normalize.py` & `gunpowder-1.3.3/gunpowder/nodes/normalize.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/pad.py` & `gunpowder-1.3.3/gunpowder/nodes/pad.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,19 @@
             Only used for :class:`Array<Arrays>`.
     """
 
     def __init__(self, key, size, mode="constant", value=None):
         self.key = key
         self.size = size
         self.mode = mode
+        if self.mode not in ["constant", "reflect"]:
+            raise ValueError(
+                "Invalid padding mode %s provided. Must be 'constant' or 'reflect'."
+                % self.mode
+            )
         self.value = value
 
     def setup(self):
         self.enable_autoskip()
 
         assert self.key in self.spec, (
             "Asked to pad %s, but is not provided upstream." % self.key
@@ -125,12 +130,17 @@
             "expanding array of shape %s from %s to %s", str(a.shape), from_roi, to_roi
         )
 
         num_channels = len(a.shape) - from_roi.dims
         lower_pad = from_roi.begin - to_roi.begin
         upper_pad = to_roi.end - from_roi.end
         pad_width = [(0, 0)] * num_channels + list(zip(lower_pad, upper_pad))
-        if self.mode == "constant":
-            padded = np.pad(a, pad_width, "constant", constant_values=value)
-        elif self.mode == "reflect":
+        if self.mode == "reflect":
             padded = np.pad(a, pad_width, "reflect")
+        elif self.mode == "constant":
+            padded = np.pad(a, pad_width, "constant", constant_values=value)
+        else:
+            raise ValueError(
+                "Invalid padding mode %s provided. Must be 'constant' or 'reflect'."
+                % self.mode
+            )
         return padded
```

### Comparing `gunpowder-1.3.2/gunpowder/nodes/precache.py` & `gunpowder-1.3.3/gunpowder/nodes/precache.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/print_profiling_stats.py` & `gunpowder-1.3.3/gunpowder/nodes/print_profiling_stats.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/random_location.py` & `gunpowder-1.3.3/gunpowder/nodes/random_location.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/random_provider.py` & `gunpowder-1.3.3/gunpowder/nodes/random_provider.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/rasterize_graph.py` & `gunpowder-1.3.3/gunpowder/nodes/rasterize_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -295,14 +295,15 @@
 
         # Fast rasterization currently only implemented for mode ball without
         # inner radius set
         use_fast_rasterization = (
             settings.mode == "ball"
             and settings.inner_radius_fraction is None
             and len(list(graph.edges)) == 0
+            and settings.color_attr is None
         )
 
         if use_fast_rasterization:
             dims = len(rasterized_graph.shape)
 
             # get structuring element for mode ball
             ball_kernel = create_ball_kernel(settings.radius, voxel_size)
@@ -343,15 +344,15 @@
 
                 rasterized_graph[arr_crop_ind] = np.logical_or(
                     ball_kernel[kernel_crop_ind], rasterized_graph[arr_crop_ind]
                 )
 
             else:
                 if settings.color_attr is not None:
-                    c = graph.nodes[node].get(settings.color_attr)
+                    c = node.attrs.get(settings.color_attr)
                     if c is None:
                         logger.debug(f"Skipping node: {node}")
                         continue
                     elif np.isclose(c, 1) and not np.isclose(settings.fg_value, 1):
                         logger.warning(
                             f"Node {node} is being colored with color {c} according to "
                             f"attribute {settings.color_attr} "
@@ -359,43 +360,60 @@
                         )
                 else:
                     c = 1
                 rasterized_graph[v] = c
         if settings.edges:
             for e in graph.edges:
                 if settings.color_attr is not None:
-                    c = graph.edges[e].get(settings.color_attr)
+                    c = e.attrs.get(settings.color_attr)
                     if c is None:
                         continue
                     elif np.isclose(c, 1) and not np.isclose(settings.fg_value, 1):
                         logger.warning(
                             f"Edge {e} is being colored with color {c} according to "
                             f"attribute {settings.color_attr} "
                             f"but color 1 will be replaced with fg_value: {settings.fg_value}"
                         )
+                else:
+                    c = 1
 
                 u = graph.node(e.u)
                 v = graph.node(e.v)
                 u_coord = Coordinate(u.location / voxel_size)
                 v_coord = Coordinate(v.location / voxel_size)
                 line = draw.line_nd(u_coord, v_coord, endpoint=True)
-                rasterized_graph[line] = 1
+                rasterized_graph[line] = c
 
         # grow graph
         if not use_fast_rasterization:
             if settings.mode == "ball":
-                enlarge_binary_map(
-                    rasterized_graph,
-                    settings.radius,
-                    voxel_size,
-                    settings.inner_radius_fraction,
-                    in_place=True,
-                )
+                if settings.color_attr is not None:
+                    for color in np.unique(rasterized_graph):
+                        if color == 0:
+                            continue
+                        mask = rasterized_graph == color
+                        enlarge_binary_map(
+                            mask,
+                            settings.radius,
+                            voxel_size,
+                            settings.inner_radius_fraction,
+                            in_place=True,
+                        )
+                        rasterized_graph[mask] = color
+                else:
+                    enlarge_binary_map(
+                        rasterized_graph,
+                        settings.radius,
+                        voxel_size,
+                        settings.inner_radius_fraction,
+                        in_place=True,
+                    )
 
             else:
+
                 sigmas = settings.radius / voxel_size
 
                 gaussian_filter(
                     rasterized_graph, sigmas, output=rasterized_graph, mode="constant"
                 )
 
                 # renormalize to have 1 be the highest value
```

### Comparing `gunpowder-1.3.2/gunpowder/nodes/reject.py` & `gunpowder-1.3.3/gunpowder/nodes/reject.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/renumber_connected_components.py` & `gunpowder-1.3.3/gunpowder/nodes/renumber_connected_components.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/resample.py` & `gunpowder-1.3.3/gunpowder/nodes/resample.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,14 @@
         source_voxel_size = self.spec[self.source].voxel_size
         spec.voxel_size = self.target_voxel_size
         self.pad = Coordinate(
             (0,) * (len(source_voxel_size) - self.ndim)
             + source_voxel_size[-self.ndim :]
         )
 
-        spec.roi = spec.roi.grow(
-            -self.pad, -self.pad
-        )  # Pad w/ 1 voxel per side for interpolation to avoid edge effects
         spec.roi = spec.roi.snap_to_grid(
             np.lcm(source_voxel_size, self.target_voxel_size), mode="shrink"
         )
 
         self.provides(self.target, spec)
         self.enable_autoskip()
```

### Comparing `gunpowder-1.3.2/gunpowder/nodes/scan.py` & `gunpowder-1.3.3/gunpowder/nodes/scan.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/shift_augment.py` & `gunpowder-1.3.3/gunpowder/nodes/shift_augment.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/simple_augment.py` & `gunpowder-1.3.3/gunpowder/nodes/simple_augment.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,17 +172,15 @@
 
             num_channels = len(array.data.shape) - self.dims
             channel_slices = (slice(None, None),) * num_channels
 
             array.data = array.data[channel_slices + mirror]
 
             transpose = [t + num_channels for t in self.transpose]
-            array.data = array.data = array.data.transpose(
-                list(range(num_channels)) + transpose
-            )
+            array.data = array.data.transpose(list(range(num_channels)) + transpose)
 
         # graphs
         total_roi_offset = total_roi.offset
         total_roi_center = total_roi.center
         if lcm_voxel_size is not None:
             nearest_voxel_shift = Coordinate(
                 (d % v) for d, v in zip(total_roi_center, lcm_voxel_size)
@@ -199,17 +197,19 @@
             for node in list(graph.nodes):
                 logger.debug("old location: %s, %s", node.id, node.location)
 
                 # mirror
                 location_in_total_offset = np.asarray(node.location) - total_roi_offset
                 node.location = np.asarray(
                     [
-                        total_roi_end[dim] - location_in_total_offset[dim]
-                        if m
-                        else node.location[dim]
+                        (
+                            total_roi_end[dim] - location_in_total_offset[dim]
+                            if m
+                            else node.location[dim]
+                        )
                         for dim, m in enumerate(self.mirror)
                     ],
                     dtype=graph.spec.dtype,
                 )
 
                 logger.debug("after mirror: %s, %s", node.id, node.location)
 
@@ -251,17 +251,19 @@
         roi_offset = roi.offset
         roi_shape = roi.shape
 
         roi_in_total_offset = roi_offset - total_roi_offset
         end_of_roi_in_total = roi_in_total_offset + roi_shape
         roi_in_total_offset_mirrored = total_roi_shape - end_of_roi_in_total
         roi_offset = Coordinate(
-            total_roi_offset[d] + roi_in_total_offset_mirrored[d]
-            if mirror[d]
-            else roi_offset[d]
+            (
+                total_roi_offset[d] + roi_in_total_offset_mirrored[d]
+                if mirror[d]
+                else roi_offset[d]
+            )
             for d in range(self.dims)
         )
 
         roi.offset = roi_offset
 
     def __transpose_roi(self, roi, total_roi, transpose, lcm_voxel_size):
         logger.debug("original roi = %s", roi)
```

### Comparing `gunpowder-1.3.2/gunpowder/nodes/snapshot.py` & `gunpowder-1.3.3/gunpowder/nodes/snapshot.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/specified_location.py` & `gunpowder-1.3.3/gunpowder/nodes/specified_location.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,23 +40,37 @@
 
         jitter (``tuple`` of int):
 
             How far to allow the point to shift in each direction.
             Default is None, which places the point in the center.
             Chooses uniformly from [loc - jitter, loc + jitter] in each
             direction.
+
+        attempt_factor (``int``):
+
+            If choosing randomly then given `n` points, sample
+            `attempt_factor * n` points at most before giving up and
+            throwing an error.
     """
 
-    def __init__(self, locations, choose_randomly=False, extra_data=None, jitter=None):
+    def __init__(
+        self,
+        locations,
+        choose_randomly=False,
+        extra_data=None,
+        jitter=None,
+        attempt_factor: int = 5,
+    ):
         self.coordinates = locations
         self.choose_randomly = choose_randomly
         self.jitter = jitter
         self.loc_i = -1
         self.upstream_spec = None
         self.specified_shift = None
+        self.attempt_factor = attempt_factor
 
         if extra_data is not None:
             assert len(extra_data) == len(locations), (
                 "extra_data (%d) should match the length of specified locations (%d)"
                 % (len(extra_data), len(locations))
             )
 
@@ -75,21 +89,36 @@
         lcm_voxel_size = self.spec.get_lcm_voxel_size(request.array_specs.keys())
 
         # shift to center
         total_roi = request.get_total_roi()
         request_center = total_roi.shape / 2 + total_roi.offset
 
         self.specified_shift = self._get_next_shift(request_center, lcm_voxel_size)
+        loop_counter = 0
         while not self.__check_shift(request):
             logger.warning(
                 "Location %s (shift %s) skipped"
                 % (self.coordinates[self.loc_i], self.specified_shift)
             )
             self.specified_shift = self._get_next_shift(request_center, lcm_voxel_size)
 
+            loop_counter += 1
+            if loop_counter >= len(self.coordinates) * (
+                1 + (self.attempt_factor - 1) * int(self.choose_randomly)
+            ):
+                if self.choose_randomly:
+                    raise Exception(
+                        f"Took {5*len(self.coordinates)} samples of {len(self.coordinates)} points "
+                        "and did not find a suitible location"
+                    )
+                else:
+                    raise Exception(
+                        "Looped through every possible location and None are valid"
+                    )
+
         # Set shift for all requests
         for specs_type in [request.array_specs, request.graph_specs]:
             for key, spec in specs_type.items():
                 roi = spec.roi.shift(self.specified_shift)
                 specs_type[key].roi = roi
 
         logger.debug(
@@ -102,17 +131,17 @@
         return deps
 
     def process(self, batch, request):
         # reset ROIs to request
         for array_key, spec in request.array_specs.items():
             batch.arrays[array_key].spec.roi = spec.roi
             if self.extra_data is not None:
-                batch.arrays[array_key].attrs[
-                    "specified_location_extra_data"
-                ] = self.extra_data[self.loc_i]
+                batch.arrays[array_key].attrs["specified_location_extra_data"] = (
+                    self.extra_data[self.loc_i]
+                )
 
         for graph_key, spec in request.graph_specs.items():
             batch.points[graph_key].spec.roi = spec.roi
 
         # change shift point locations to lie within roi
         for graph_key in request.graph_specs.keys():
             batch.points[graph_key].shift(-self.specified_shift)
```

### Comparing `gunpowder-1.3.2/gunpowder/nodes/squeeze.py` & `gunpowder-1.3.3/gunpowder/nodes/squeeze.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/stack.py` & `gunpowder-1.3.3/gunpowder/nodes/stack.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/unsqueeze.py` & `gunpowder-1.3.3/gunpowder/nodes/unsqueeze.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/upsample.py` & `gunpowder-1.3.3/gunpowder/nodes/upsample.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/nodes/zarr_source.py` & `gunpowder-1.3.3/gunpowder/nodes/zarr_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,20 +202,20 @@
                 "but differs from dataset %s dtype %s"
                 % (self.array_specs[array_key].dtype, array_key, ds_name, dataset.dtype)
             )
         else:
             spec.dtype = dataset.dtype
 
         if spec.interpolatable is None:
-            spec.interpolatable = spec.dtype in [
-                np.float32,
-                np.float64,
-                np.float128,
-                np.uint8,  # assuming this is not used for labels
-            ]
+            spec.interpolatable = spec.dtype in (
+                np.sctypes["float"]
+                + [
+                    np.uint8,  # assuming this is not used for labels
+                ]
+            )
             logger.warning(
                 "WARNING: You didn't set 'interpolatable' for %s "
                 "(dataset %s). Based on the dtype %s, it has been "
                 "set to %s. This might not be what you want.",
                 array_key,
                 ds_name,
                 spec.dtype,
```

### Comparing `gunpowder-1.3.2/gunpowder/nodes/zarr_write.py` & `gunpowder-1.3.3/gunpowder/nodes/zarr_write.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/pipeline.py` & `gunpowder-1.3.3/gunpowder/pipeline.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/producer_pool.py` & `gunpowder-1.3.3/gunpowder/producer_pool.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/profiling.py` & `gunpowder-1.3.3/gunpowder/profiling.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/provider_spec.py` & `gunpowder-1.3.3/gunpowder/provider_spec.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/tensorflow/local_server.py` & `gunpowder-1.3.3/gunpowder/tensorflow/local_server.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/tensorflow/nodes/predict.py` & `gunpowder-1.3.3/gunpowder/tensorflow/nodes/predict.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/tensorflow/nodes/train.py` & `gunpowder-1.3.3/gunpowder/tensorflow/nodes/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,16 +136,15 @@
         self.full_saver = None
         self.save_every = save_every
         self.iteration = None
         self.iteration_increment = None
         self.summary_saver = None
         self.log_dir = log_dir
         self.log_every = log_every
-        # Check if optimizer is a str in python 2/3 compatible way.
-        if isinstance(optimizer, ("".__class__, "".__class__)):
+        if isinstance(optimizer, str):
             self.optimizer_loss_names = (optimizer, loss)
         else:
             self.optimizer_func = optimizer
 
         # at least for some versions of tensorflow, the checkpoint name has to
         # start with a . if it is a relative path
         if not os.path.isabs(self.meta_graph_filename):
```

### Comparing `gunpowder-1.3.2/gunpowder/torch/nodes/predict.py` & `gunpowder-1.3.3/gunpowder/torch/nodes/predict.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/torch/nodes/train.py` & `gunpowder-1.3.3/gunpowder/torch/nodes/train.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder/version_info.py` & `gunpowder-1.3.3/gunpowder/version_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __major__ = 1
 __minor__ = 3
-__patch__ = 2
+__patch__ = 3
 __tag__ = ""
 __version__ = "{}.{}.{}{}".format(__major__, __minor__, __patch__, __tag__).strip(".")
 
 
 class _Version(object):
     def major(self):
         return __major__
```

### Comparing `gunpowder-1.3.2/gunpowder/zoo/tensorflow/unet.py` & `gunpowder-1.3.3/gunpowder/zoo/tensorflow/unet.py`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/gunpowder.egg-info/PKG-INFO` & `gunpowder-1.3.3/gunpowder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunpowder
-Version: 1.3.2
+Version: 1.3.3
 Summary: A library to facilitate machine learning on large, multi-dimensional images.
 Author: Renate Krause, Julia Buhmann, Rodrigo Ceballos Lentini, William Grisaitis, Chris Barnes, Caroline Malin-Mayor, Larissa Heinrich, Philipp Hanslovsky, Sherry Ding, Andrew Champion, Arlo Sheridan, Constantin Pape
 Author-email: Jan Funke <funkej@hhmi.org>, William Patton <pattonw@hhmi.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gunpowder-1.3.2/gunpowder.egg-info/SOURCES.txt` & `gunpowder-1.3.3/gunpowder.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pyproject.toml
 gunpowder/__init__.py
 gunpowder/array.py
 gunpowder/array_spec.py
 gunpowder/batch.py
 gunpowder/batch_request.py
 gunpowder/build.py
-gunpowder/compat.py
 gunpowder/coordinate.py
 gunpowder/freezable.py
 gunpowder/graph.py
 gunpowder/graph_spec.py
 gunpowder/morphology.py
 gunpowder/ndarray.py
 gunpowder/pipeline.py
```

### Comparing `gunpowder-1.3.2/gunpowder.egg-info/requires.txt` & `gunpowder-1.3.3/gunpowder.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gunpowder-1.3.2/pyproject.toml` & `gunpowder-1.3.3/pyproject.toml`

 * *Files identical despite different names*

