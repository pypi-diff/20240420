# Comparing `tmp/srai-0.7.1.tar.gz` & `tmp/srai-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srai-0.7.1.tar", last modified: Wed Apr 17 19:17:29 2024, max compression
+gzip compressed data, was "srai-0.7.2.tar", last modified: Sat Apr 20 14:01:27 2024, max compression
```

## Comparing `srai-0.7.1.tar` & `srai-0.7.2.tar`

### file list

```diff
@@ -1,167 +1,168 @@
--rw-r--r--   0        0        0    10760 2024-04-17 19:17:06.876747 srai-0.7.1/LICENSE.md
--rw-r--r--   0        0        0    18089 2024-04-17 19:17:06.876747 srai-0.7.1/README.md
--rw-r--r--   0        0        0     5213 2024-04-17 19:17:29.209238 srai-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      428 2024-04-17 19:17:06.888747 srai-0.7.1/srai/__init__.py
--rw-r--r--   0        0        0     2904 2024-04-17 19:17:06.888747 srai-0.7.1/srai/_optional.py
--rw-r--r--   0        0        0      717 2024-04-17 19:17:06.888747 srai-0.7.1/srai/_typing.py
--rw-r--r--   0        0        0      155 2024-04-17 19:17:06.888747 srai-0.7.1/srai/constants.py
--rw-r--r--   0        0        0      854 2024-04-17 19:17:06.888747 srai-0.7.1/srai/embedders/__init__.py
--rw-r--r--   0        0        0     4846 2024-04-17 19:17:06.888747 srai-0.7.1/srai/embedders/_base.py
--rw-r--r--   0        0        0      531 2024-04-17 19:17:06.888747 srai-0.7.1/srai/embedders/_pytorch_stubs.py
--rw-r--r--   0        0        0     9181 2024-04-17 19:17:06.888747 srai-0.7.1/srai/embedders/contextual_count_embedder.py
--rw-r--r--   0        0        0     8180 2024-04-17 19:17:06.888747 srai-0.7.1/srai/embedders/count_embedder.py
--rw-r--r--   0        0        0      186 2024-04-17 19:17:06.888747 srai-0.7.1/srai/embedders/geovex/__init__.py
--rw-r--r--   0        0        0     6774 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/geovex/dataset.py
--rw-r--r--   0        0        0     9806 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/geovex/embedder.py
--rw-r--r--   0        0        0    18081 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/geovex/model.py
--rw-r--r--   0        0        0      136 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/gtfs2vec/__init__.py
--rw-r--r--   0        0        0    11335 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/gtfs2vec/embedder.py
--rw-r--r--   0        0        0     2278 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/gtfs2vec/model.py
--rw-r--r--   0        0        0      247 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/hex2vec/__init__.py
--rw-r--r--   0        0        0    10940 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/hex2vec/embedder.py
--rw-r--r--   0        0        0     6804 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/hex2vec/model.py
--rw-r--r--   0        0        0     6301 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/hex2vec/neighbour_dataset.py
--rw-r--r--   0        0        0      153 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/highway2vec/__init__.py
--rw-r--r--   0        0        0     7918 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/highway2vec/embedder.py
--rw-r--r--   0        0        0     2855 2024-04-17 19:17:06.892747 srai-0.7.1/srai/embedders/highway2vec/model.py
--rw-r--r--   0        0        0      580 2024-04-17 19:17:06.892747 srai-0.7.1/srai/exceptions.py
--rw-r--r--   0        0        0     4247 2024-04-17 19:17:06.892747 srai-0.7.1/srai/geometry.py
--rw-r--r--   0        0        0     9059 2024-04-17 19:17:06.892747 srai-0.7.1/srai/h3.py
--rw-r--r--   0        0        0      531 2024-04-17 19:17:06.892747 srai-0.7.1/srai/joiners/__init__.py
--rw-r--r--   0        0        0      731 2024-04-17 19:17:06.892747 srai-0.7.1/srai/joiners/_base.py
--rw-r--r--   0        0        0     3836 2024-04-17 19:17:06.892747 srai-0.7.1/srai/joiners/intersection_joiner.py
--rw-r--r--   0        0        0      820 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/__init__.py
--rw-r--r--   0        0        0      591 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/_base.py
--rw-r--r--   0        0        0     1343 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/download.py
--rw-r--r--   0        0        0     2189 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/geoparquet_loader.py
--rw-r--r--   0        0        0     5391 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/gtfs_loader.py
--rw-r--r--   0        0        0      257 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/__init__.py
--rw-r--r--   0        0        0     7764 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/_base.py
--rw-r--r--   0        0        0      472 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/filters/__init__.py
--rw-r--r--   0        0        0     4359 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/filters/_typing.py
--rw-r--r--   0        0        0     5315 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/filters/base_osm_groups.py
--rw-r--r--   0        0        0    10696 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/filters/geofabrik.py
--rw-r--r--   0        0        0    15751 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/filters/hex2vec.py
--rw-r--r--   0        0        0     2420 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/filters/popular.py
--rw-r--r--   0        0        0     5996 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/osm_online_loader.py
--rw-r--r--   0        0        0     9280 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/osm_pbf_loader.py
--rw-r--r--   0        0        0     2778 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/osm_tile_data_collector.py
--rw-r--r--   0        0        0     5033 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_loaders/osm_tile_loader.py
--rw-r--r--   0        0        0      124 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_way_loader/__init__.py
--rw-r--r--   0        0        0     7556 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_way_loader/constants.py
--rw-r--r--   0        0        0    14142 2024-04-17 19:17:06.892747 srai-0.7.1/srai/loaders/osm_way_loader/osm_way_loader.py
--rw-r--r--   0        0        0      468 2024-04-17 19:17:06.892747 srai-0.7.1/srai/neighbourhoods/__init__.py
--rw-r--r--   0        0        0     6071 2024-04-17 19:17:06.892747 srai-0.7.1/srai/neighbourhoods/_base.py
--rw-r--r--   0        0        0     3609 2024-04-17 19:17:06.892747 srai-0.7.1/srai/neighbourhoods/adjacency_neighbourhood.py
--rw-r--r--   0        0        0     4632 2024-04-17 19:17:06.892747 srai-0.7.1/srai/neighbourhoods/h3_neighbourhood.py
--rw-r--r--   0        0        0      497 2024-04-17 19:17:06.892747 srai-0.7.1/srai/plotting/__init__.py
--rw-r--r--   0        0        0    11418 2024-04-17 19:17:06.892747 srai-0.7.1/srai/plotting/folium_wrapper.py
--rw-r--r--   0        0        0    14129 2024-04-17 19:17:06.892747 srai-0.7.1/srai/plotting/plotly_wrapper.py
--rw-r--r--   0        0        0     1006 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/__init__.py
--rw-r--r--   0        0        0      957 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/_base.py
--rw-r--r--   0        0        0    27497 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/_spherical_voronoi.py
--rw-r--r--   0        0        0    15629 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/administrative_boundary_regionalizer.py
--rw-r--r--   0        0        0     2477 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/geocode.py
--rw-r--r--   0        0        0     2610 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/h3_regionalizer.py
--rw-r--r--   0        0        0     3136 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/s2_regionalizer.py
--rw-r--r--   0        0        0     4184 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/slippy_map_regionalizer.py
--rw-r--r--   0        0        0     6001 2024-04-17 19:17:06.892747 srai-0.7.1/srai/regionalizers/voronoi_regionalizer.py
--rw-r--r--   0        0        0       29 2024-04-17 19:17:06.892747 srai-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0     7806 2024-04-17 19:17:06.892747 srai-0.7.1/tests/embedders/conftest.py
--rw-r--r--   0        0        0     1015 2024-04-17 19:17:06.892747 srai-0.7.1/tests/embedders/geovex/constants.py
--rw-r--r--   0        0        0     6245 2024-04-17 19:17:06.892747 srai-0.7.1/tests/embedders/geovex/generation.py
--rw-r--r--   0        0        0     4197 2024-04-17 19:17:06.892747 srai-0.7.1/tests/embedders/geovex/test_dataset.py
--rw-r--r--   0        0        0     4009 2024-04-17 19:17:06.892747 srai-0.7.1/tests/embedders/geovex/test_embedder.py
--rw-r--r--   0        0        0   484605 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_0.pt
--rw-r--r--   0        0        0   484605 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_1.pt
--rw-r--r--   0        0        0   484605 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_2.pt
--rw-r--r--   0        0        0   339453 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_3.pt
--rw-r--r--   0        0        0     2139 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt
--rw-r--r--   0        0        0     2139 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt
--rw-r--r--   0        0        0     2139 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt
--rw-r--r--   0        0        0     1755 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt
--rw-r--r--   0        0        0    75958 2024-04-17 19:17:06.896747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_features.parquet
--rw-r--r--   0        0        0   968711 2024-04-17 19:17:06.900747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_0.pt
--rw-r--r--   0        0        0   968711 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_1.pt
--rw-r--r--   0        0        0   968711 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_2.pt
--rw-r--r--   0        0        0   678407 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_3.pt
--rw-r--r--   0        0        0     7011 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_joint.parquet
--rw-r--r--   0        0        0      762 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_0.pt
--rw-r--r--   0        0        0      762 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_1.pt
--rw-r--r--   0        0        0      762 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_2.pt
--rw-r--r--   0        0        0      762 2024-04-17 19:17:06.904747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_3.pt
--rw-r--r--   0        0        0    13915 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_regions.parquet
--rw-r--r--   0        0        0    24970 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/AL_10_result.parquet
--rw-r--r--   0        0        0   272893 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_batch_0.pt
--rw-r--r--   0        0        0   245693 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_batch_1.pt
--rw-r--r--   0        0        0     2139 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt
--rw-r--r--   0        0        0     2011 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt
--rw-r--r--   0        0        0   803774 2024-04-17 19:17:06.908747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_features.parquet
--rw-r--r--   0        0        0   545287 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_forward_0.pt
--rw-r--r--   0        0        0   490887 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_forward_1.pt
--rw-r--r--   0        0        0    76452 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_joint.parquet
--rw-r--r--   0        0        0      762 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_loss_0.pt
--rw-r--r--   0        0        0      762 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_loss_1.pt
--rw-r--r--   0        0        0    10162 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_regions.parquet
--rw-r--r--   0        0        0    21999 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_files/wro_9_result.parquet
--rw-r--r--   0        0        0     4560 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/geovex/test_model.py
--rw-r--r--   0        0        0      579 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/hex2vec/constants.py
--rw-r--r--   0        0        0     2782 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/hex2vec/generation.py
--rw-r--r--   0        0        0     2711 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/hex2vec/test_embedder.py
--rw-r--r--   0        0        0    97383 2024-04-17 19:17:06.912747 srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_features.parquet
--rw-r--r--   0        0        0   111218 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
--rw-r--r--   0        0        0    14226 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
--rw-r--r--   0        0        0    14498 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_result.parquet
--rw-r--r--   0        0        0    89227 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_features.parquet
--rw-r--r--   0        0        0    86944 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
--rw-r--r--   0        0        0    16794 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
--rw-r--r--   0        0        0    15781 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_result.parquet
--rw-r--r--   0        0        0     1056 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_model.py
--rw-r--r--   0        0        0     3058 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/hex2vec/test_neighbour_dataset.py
--rw-r--r--   0        0        0    26806 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/test_contextual_count_embedder.py
--rw-r--r--   0        0        0    12298 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/test_count_embedder.py
--rw-r--r--   0        0        0     7091 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/test_gtfs2vec_embedder.py
--rw-r--r--   0        0        0     3631 2024-04-17 19:17:06.916747 srai-0.7.1/tests/embedders/test_highway2vec_embedder.py
--rw-r--r--   0        0        0     2514 2024-04-17 19:17:06.916747 srai-0.7.1/tests/h3/conftest.py
--rw-r--r--   0        0        0     3035 2024-04-17 19:17:06.916747 srai-0.7.1/tests/h3/test_ij_coordinates.py
--rw-r--r--   0        0        0     3066 2024-04-17 19:17:06.916747 srai-0.7.1/tests/h3/test_shapely_conversion.py
--rw-r--r--   0        0        0     1765 2024-04-17 19:17:06.916747 srai-0.7.1/tests/joiners/conftest.py
--rw-r--r--   0        0        0     2530 2024-04-17 19:17:06.916747 srai-0.7.1/tests/joiners/test_intersection_joiner.py
--rw-r--r--   0        0        0     2745 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/conftest.py
--rw-r--r--   0        0        0     4285 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/conftest.py
--rw-r--r--   0        0        0     4824 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/filters/popular_filter_example.json
--rw-r--r--   0        0        0     4094 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
--rw-r--r--   0        0        0     3283 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
--rw-r--r--   0        0        0      342 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2024-04-17 19:17:06.916747 srai-0.7.1/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   537903 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_files/monaco.osm.pbf
--rw-r--r--   0        0        0   111539 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_files/poland.geojson
--rw-r--r--   0        0        0   252620 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
--rw-r--r--   0        0        0     3026 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_osm_online_loader.py
--rw-r--r--   0        0        0     4763 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_osm_pbf_loader.py
--rw-r--r--   0        0        0     3157 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
--rw-r--r--   0        0        0     3104 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_loaders/test_osm_tile_loader.py
--rw-r--r--   0        0        0     3803 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_1.pkl
--rw-r--r--   0        0        0     3334 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_2.pkl
--rw-r--r--   0        0        0     5099 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_3.pkl
--rw-r--r--   0        0        0     3803 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_4.pkl
--rw-r--r--   0        0        0    11090 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/osm_way_loader/test_osm_way_loader.py
--rw-r--r--   0        0        0    27801 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/test_files/example.parquet
--rw-r--r--   0        0        0     2182 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/test_geoparquet_loader.py
--rw-r--r--   0        0        0     3177 2024-04-17 19:17:06.920747 srai-0.7.1/tests/loaders/test_gtfs_loader.py
--rw-r--r--   0        0        0     4878 2024-04-17 19:17:06.920747 srai-0.7.1/tests/miscellaneous/test_optional_dependencies.py
--rw-r--r--   0        0        0     8340 2024-04-17 19:17:06.920747 srai-0.7.1/tests/neighbourhoods/h3/test_no_regions.py
--rw-r--r--   0        0        0     9166 2024-04-17 19:17:06.920747 srai-0.7.1/tests/neighbourhoods/h3/test_with_regions.py
--rw-r--r--   0        0        0    11409 2024-04-17 19:17:06.920747 srai-0.7.1/tests/neighbourhoods/test_adjacency_neighbourhood.py
--rw-r--r--   0        0        0    11019 2024-04-17 19:17:06.920747 srai-0.7.1/tests/neighbourhoods/test_neighbourhood.py
--rw-r--r--   0        0        0      765 2024-04-17 19:17:06.920747 srai-0.7.1/tests/plotting/test_folium_wrapper.py
--rw-r--r--   0        0        0     3405 2024-04-17 19:17:06.920747 srai-0.7.1/tests/regionalizers/conftest.py
--rw-r--r--   0        0        0     6509 2024-04-17 19:17:06.920747 srai-0.7.1/tests/regionalizers/test_administrative_boundary_regionalizer.py
--rw-r--r--   0        0        0     2616 2024-04-17 19:17:06.920747 srai-0.7.1/tests/regionalizers/test_h3_regionalizer.py
--rw-r--r--   0        0        0     1856 2024-04-17 19:17:06.920747 srai-0.7.1/tests/regionalizers/test_s2_regionalizer.py
--rw-r--r--   0        0        0     2690 2024-04-17 19:17:06.920747 srai-0.7.1/tests/regionalizers/test_slippy_map_regionalizer.py
--rw-r--r--   0        0        0     9215 2024-04-17 19:17:06.920747 srai-0.7.1/tests/regionalizers/test_voronoi_regionalizer.py
--rw-r--r--   0        0        0    20378 1970-01-01 00:00:00.000000 srai-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    10760 2024-04-20 14:01:08.055309 srai-0.7.2/LICENSE.md
+-rw-r--r--   0        0        0    18089 2024-04-20 14:01:08.055309 srai-0.7.2/README.md
+-rw-r--r--   0        0        0     5261 2024-04-20 14:01:27.459538 srai-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      428 2024-04-20 14:01:08.067309 srai-0.7.2/srai/__init__.py
+-rw-r--r--   0        0        0     2904 2024-04-20 14:01:08.067309 srai-0.7.2/srai/_optional.py
+-rw-r--r--   0        0        0      717 2024-04-20 14:01:08.067309 srai-0.7.2/srai/_typing.py
+-rw-r--r--   0        0        0      155 2024-04-20 14:01:08.067309 srai-0.7.2/srai/constants.py
+-rw-r--r--   0        0        0      854 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/__init__.py
+-rw-r--r--   0        0        0     4846 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/_base.py
+-rw-r--r--   0        0        0      482 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/_pytorch_stubs.py
+-rw-r--r--   0        0        0     9181 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/contextual_count_embedder.py
+-rw-r--r--   0        0        0     8180 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/count_embedder.py
+-rw-r--r--   0        0        0      186 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/geovex/__init__.py
+-rw-r--r--   0        0        0     6882 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/geovex/dataset.py
+-rw-r--r--   0        0        0     9809 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/geovex/embedder.py
+-rw-r--r--   0        0        0    18081 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/geovex/model.py
+-rw-r--r--   0        0        0      136 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/gtfs2vec/__init__.py
+-rw-r--r--   0        0        0    11336 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/gtfs2vec/embedder.py
+-rw-r--r--   0        0        0     2278 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/gtfs2vec/model.py
+-rw-r--r--   0        0        0      247 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/hex2vec/__init__.py
+-rw-r--r--   0        0        0    10941 2024-04-20 14:01:08.071309 srai-0.7.2/srai/embedders/hex2vec/embedder.py
+-rw-r--r--   0        0        0     6804 2024-04-20 14:01:08.071309 srai-0.7.2/srai/embedders/hex2vec/model.py
+-rw-r--r--   0        0        0     6301 2024-04-20 14:01:08.071309 srai-0.7.2/srai/embedders/hex2vec/neighbour_dataset.py
+-rw-r--r--   0        0        0      153 2024-04-20 14:01:08.071309 srai-0.7.2/srai/embedders/highway2vec/__init__.py
+-rw-r--r--   0        0        0     7919 2024-04-20 14:01:08.071309 srai-0.7.2/srai/embedders/highway2vec/embedder.py
+-rw-r--r--   0        0        0     2855 2024-04-20 14:01:08.071309 srai-0.7.2/srai/embedders/highway2vec/model.py
+-rw-r--r--   0        0        0      580 2024-04-20 14:01:08.071309 srai-0.7.2/srai/exceptions.py
+-rw-r--r--   0        0        0     4247 2024-04-20 14:01:08.071309 srai-0.7.2/srai/geometry.py
+-rw-r--r--   0        0        0     9060 2024-04-20 14:01:08.071309 srai-0.7.2/srai/h3.py
+-rw-r--r--   0        0        0      531 2024-04-20 14:01:08.071309 srai-0.7.2/srai/joiners/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-20 14:01:08.071309 srai-0.7.2/srai/joiners/_base.py
+-rw-r--r--   0        0        0     3836 2024-04-20 14:01:08.071309 srai-0.7.2/srai/joiners/intersection_joiner.py
+-rw-r--r--   0        0        0      820 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/__init__.py
+-rw-r--r--   0        0        0      591 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/_base.py
+-rw-r--r--   0        0        0     1343 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/download.py
+-rw-r--r--   0        0        0     2189 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/geoparquet_loader.py
+-rw-r--r--   0        0        0     5391 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/gtfs_loader.py
+-rw-r--r--   0        0        0      257 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/__init__.py
+-rw-r--r--   0        0        0     7765 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/_base.py
+-rw-r--r--   0        0        0      472 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/filters/__init__.py
+-rw-r--r--   0        0        0     4402 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/filters/_typing.py
+-rw-r--r--   0        0        0     5315 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/filters/base_osm_groups.py
+-rw-r--r--   0        0        0    10696 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/filters/geofabrik.py
+-rw-r--r--   0        0        0    15751 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/filters/hex2vec.py
+-rw-r--r--   0        0        0     2447 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/filters/popular.py
+-rw-r--r--   0        0        0     5996 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/osm_online_loader.py
+-rw-r--r--   0        0        0     9280 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/osm_pbf_loader.py
+-rw-r--r--   0        0        0     2778 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/osm_tile_data_collector.py
+-rw-r--r--   0        0        0     5033 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/osm_tile_loader.py
+-rw-r--r--   0        0        0      124 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_way_loader/__init__.py
+-rw-r--r--   0        0        0     7556 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_way_loader/constants.py
+-rw-r--r--   0        0        0    14142 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_way_loader/osm_way_loader.py
+-rw-r--r--   0        0        0      468 2024-04-20 14:01:08.071309 srai-0.7.2/srai/neighbourhoods/__init__.py
+-rw-r--r--   0        0        0     6176 2024-04-20 14:01:08.071309 srai-0.7.2/srai/neighbourhoods/_base.py
+-rw-r--r--   0        0        0     3609 2024-04-20 14:01:08.071309 srai-0.7.2/srai/neighbourhoods/adjacency_neighbourhood.py
+-rw-r--r--   0        0        0     4632 2024-04-20 14:01:08.071309 srai-0.7.2/srai/neighbourhoods/h3_neighbourhood.py
+-rw-r--r--   0        0        0      497 2024-04-20 14:01:08.071309 srai-0.7.2/srai/plotting/__init__.py
+-rw-r--r--   0        0        0    11418 2024-04-20 14:01:08.071309 srai-0.7.2/srai/plotting/folium_wrapper.py
+-rw-r--r--   0        0        0    14129 2024-04-20 14:01:08.071309 srai-0.7.2/srai/plotting/plotly_wrapper.py
+-rw-r--r--   0        0        0       55 2024-04-20 14:01:08.071309 srai-0.7.2/srai/py.typed
+-rw-r--r--   0        0        0     1006 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/__init__.py
+-rw-r--r--   0        0        0      957 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/_base.py
+-rw-r--r--   0        0        0    27555 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/_spherical_voronoi.py
+-rw-r--r--   0        0        0    15629 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0     2477 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/geocode.py
+-rw-r--r--   0        0        0     2610 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/h3_regionalizer.py
+-rw-r--r--   0        0        0     3136 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/s2_regionalizer.py
+-rw-r--r--   0        0        0     4184 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     6001 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/voronoi_regionalizer.py
+-rw-r--r--   0        0        0       29 2024-04-20 14:01:08.071309 srai-0.7.2/tests/__init__.py
+-rw-r--r--   0        0        0     7806 2024-04-20 14:01:08.071309 srai-0.7.2/tests/embedders/conftest.py
+-rw-r--r--   0        0        0     1015 2024-04-20 14:01:08.071309 srai-0.7.2/tests/embedders/geovex/constants.py
+-rw-r--r--   0        0        0     6245 2024-04-20 14:01:08.071309 srai-0.7.2/tests/embedders/geovex/generation.py
+-rw-r--r--   0        0        0     4211 2024-04-20 14:01:08.071309 srai-0.7.2/tests/embedders/geovex/test_dataset.py
+-rw-r--r--   0        0        0     4049 2024-04-20 14:01:08.071309 srai-0.7.2/tests/embedders/geovex/test_embedder.py
+-rw-r--r--   0        0        0   484605 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_0.pt
+-rw-r--r--   0        0        0   484605 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_1.pt
+-rw-r--r--   0        0        0   484605 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_2.pt
+-rw-r--r--   0        0        0   339453 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_3.pt
+-rw-r--r--   0        0        0     2139 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt
+-rw-r--r--   0        0        0     2139 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt
+-rw-r--r--   0        0        0     2139 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt
+-rw-r--r--   0        0        0     1755 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt
+-rw-r--r--   0        0        0    75958 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_features.parquet
+-rw-r--r--   0        0        0   968711 2024-04-20 14:01:08.079309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_0.pt
+-rw-r--r--   0        0        0   968711 2024-04-20 14:01:08.079309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_1.pt
+-rw-r--r--   0        0        0   968711 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_2.pt
+-rw-r--r--   0        0        0   678407 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_3.pt
+-rw-r--r--   0        0        0     7011 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_joint.parquet
+-rw-r--r--   0        0        0      762 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_0.pt
+-rw-r--r--   0        0        0      762 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_1.pt
+-rw-r--r--   0        0        0      762 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_2.pt
+-rw-r--r--   0        0        0      762 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_3.pt
+-rw-r--r--   0        0        0    13915 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_regions.parquet
+-rw-r--r--   0        0        0    24970 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_result.parquet
+-rw-r--r--   0        0        0   272893 2024-04-20 14:01:08.087309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_batch_0.pt
+-rw-r--r--   0        0        0   245693 2024-04-20 14:01:08.087309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_batch_1.pt
+-rw-r--r--   0        0        0     2139 2024-04-20 14:01:08.087309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt
+-rw-r--r--   0        0        0     2011 2024-04-20 14:01:08.087309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt
+-rw-r--r--   0        0        0   803774 2024-04-20 14:01:08.087309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_features.parquet
+-rw-r--r--   0        0        0   545287 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_forward_0.pt
+-rw-r--r--   0        0        0   490887 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_forward_1.pt
+-rw-r--r--   0        0        0    76452 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_joint.parquet
+-rw-r--r--   0        0        0      762 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_loss_0.pt
+-rw-r--r--   0        0        0      762 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_loss_1.pt
+-rw-r--r--   0        0        0    10162 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_regions.parquet
+-rw-r--r--   0        0        0    21999 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_result.parquet
+-rw-r--r--   0        0        0     4538 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_model.py
+-rw-r--r--   0        0        0      579 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/hex2vec/constants.py
+-rw-r--r--   0        0        0     2782 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/hex2vec/generation.py
+-rw-r--r--   0        0        0     3013 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/hex2vec/test_embedder.py
+-rw-r--r--   0        0        0    97383 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_features.parquet
+-rw-r--r--   0        0        0   111218 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
+-rw-r--r--   0        0        0    14226 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
+-rw-r--r--   0        0        0    14498 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_result.parquet
+-rw-r--r--   0        0        0    89227 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_features.parquet
+-rw-r--r--   0        0        0    86944 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
+-rw-r--r--   0        0        0    16794 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
+-rw-r--r--   0        0        0    15781 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_result.parquet
+-rw-r--r--   0        0        0     1056 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_model.py
+-rw-r--r--   0        0        0     3058 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_neighbour_dataset.py
+-rw-r--r--   0        0        0    27244 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/test_contextual_count_embedder.py
+-rw-r--r--   0        0        0    12298 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/test_count_embedder.py
+-rw-r--r--   0        0        0     7091 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/test_gtfs2vec_embedder.py
+-rw-r--r--   0        0        0     3631 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/test_highway2vec_embedder.py
+-rw-r--r--   0        0        0     2838 2024-04-20 14:01:08.095309 srai-0.7.2/tests/h3/conftest.py
+-rw-r--r--   0        0        0     3035 2024-04-20 14:01:08.095309 srai-0.7.2/tests/h3/test_ij_coordinates.py
+-rw-r--r--   0        0        0     3083 2024-04-20 14:01:08.095309 srai-0.7.2/tests/h3/test_shapely_conversion.py
+-rw-r--r--   0        0        0     1765 2024-04-20 14:01:08.095309 srai-0.7.2/tests/joiners/conftest.py
+-rw-r--r--   0        0        0     2530 2024-04-20 14:01:08.095309 srai-0.7.2/tests/joiners/test_intersection_joiner.py
+-rw-r--r--   0        0        0     3001 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/conftest.py
+-rw-r--r--   0        0        0     4285 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/conftest.py
+-rw-r--r--   0        0        0     4824 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/filters/popular_filter_example.json
+-rw-r--r--   0        0        0     4094 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
+-rw-r--r--   0        0        0     3283 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
+-rw-r--r--   0        0        0      342 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   537903 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/test_files/monaco.osm.pbf
+-rw-r--r--   0        0        0   111539 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_loaders/test_files/poland.geojson
+-rw-r--r--   0        0        0   252620 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
+-rw-r--r--   0        0        0     3026 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_loaders/test_osm_online_loader.py
+-rw-r--r--   0        0        0     4921 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_loaders/test_osm_pbf_loader.py
+-rw-r--r--   0        0        0     3159 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
+-rw-r--r--   0        0        0     3142 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_loaders/test_osm_tile_loader.py
+-rw-r--r--   0        0        0     3803 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_1.pkl
+-rw-r--r--   0        0        0     3334 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_2.pkl
+-rw-r--r--   0        0        0     5099 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_3.pkl
+-rw-r--r--   0        0        0     3803 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_4.pkl
+-rw-r--r--   0        0        0    11234 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_way_loader/test_osm_way_loader.py
+-rw-r--r--   0        0        0    27801 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/test_files/example.parquet
+-rw-r--r--   0        0        0     2182 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/test_geoparquet_loader.py
+-rw-r--r--   0        0        0     3177 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/test_gtfs_loader.py
+-rw-r--r--   0        0        0     4878 2024-04-20 14:01:08.099310 srai-0.7.2/tests/miscellaneous/test_optional_dependencies.py
+-rw-r--r--   0        0        0     8340 2024-04-20 14:01:08.099310 srai-0.7.2/tests/neighbourhoods/h3/test_no_regions.py
+-rw-r--r--   0        0        0     9166 2024-04-20 14:01:08.099310 srai-0.7.2/tests/neighbourhoods/h3/test_with_regions.py
+-rw-r--r--   0        0        0    11395 2024-04-20 14:01:08.099310 srai-0.7.2/tests/neighbourhoods/test_adjacency_neighbourhood.py
+-rw-r--r--   0        0        0    11019 2024-04-20 14:01:08.099310 srai-0.7.2/tests/neighbourhoods/test_neighbourhood.py
+-rw-r--r--   0        0        0      765 2024-04-20 14:01:08.099310 srai-0.7.2/tests/plotting/test_folium_wrapper.py
+-rw-r--r--   0        0        0     3729 2024-04-20 14:01:08.099310 srai-0.7.2/tests/regionalizers/conftest.py
+-rw-r--r--   0        0        0     6509 2024-04-20 14:01:08.099310 srai-0.7.2/tests/regionalizers/test_administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0     2616 2024-04-20 14:01:08.099310 srai-0.7.2/tests/regionalizers/test_h3_regionalizer.py
+-rw-r--r--   0        0        0     1856 2024-04-20 14:01:08.099310 srai-0.7.2/tests/regionalizers/test_s2_regionalizer.py
+-rw-r--r--   0        0        0     2690 2024-04-20 14:01:08.099310 srai-0.7.2/tests/regionalizers/test_slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     9215 2024-04-20 14:01:08.099310 srai-0.7.2/tests/regionalizers/test_voronoi_regionalizer.py
+-rw-r--r--   0        0        0    20378 1970-01-01 00:00:00.000000 srai-0.7.2/PKG-INFO
```

### Comparing `srai-0.7.1/LICENSE.md` & `srai-0.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/README.md` & `srai-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/pyproject.toml` & `srai-0.7.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "srai"
-version = "0.7.1"
+version = "0.7.2"
 description = "A set of python modules for geospatial machine learning and data mining"
 authors = [
     { name = "Piotr Gramacki", email = "pgramacki@kraina.ai" },
     { name = "Kacper Leśniara", email = "klesniara@kraina.ai" },
     { name = "Kamil Raczycki", email = "kraczycki@kraina.ai" },
     { name = "Szymon Woźniak", email = "swozniak@kraina.ai" },
 ]
@@ -93,29 +93,29 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "bumpver",
     "types-requests",
 ]
 lint = [
     "pre-commit",
-    "black[jupyter]",
     "mypy",
     "docformatter[tomli]",
     "ruff",
 ]
 test = [
     "pytest",
     "tox-pdm",
     "pytest-mock",
     "requests-mock",
     "pytest-check",
     "pytest-parametrization",
     "pytest-xdist",
     "pyogrio",
     "six",
+    "pytest-snapshot",
 ]
 visualization = [
     "keplergl",
     "matplotlib",
 ]
 docs = [
     "mkdocs",
@@ -126,36 +126,32 @@
     "ipykernel",
     "mkdocs-gen-files",
     "mkdocs-awesome-pages-plugin",
     "mike<2",
     "scikit-learn",
     "umap-learn",
 ]
-performance = [
-    "scalene",
-]
 license = [
     "licensecheck",
 ]
 
 [tool.pdm.scripts]
 post_install = "pre-commit install"
 
-[tool.black]
-line-length = 100
-target-version = [
-    "py39",
-    "py310",
-    "py311",
-]
-preview = true
-
 [tool.ruff]
 line-length = 100
 target-version = "py39"
+extend-exclude = [
+    "old",
+]
+extend-include = [
+    "*.ipynb",
+]
+
+[tool.ruff.lint]
 select = [
     "E",
     "W",
     "F",
     "UP",
     "D",
     "I",
@@ -168,47 +164,49 @@
     "PIE",
     "TID",
     "ISC",
     "TCH",
 ]
 ignore = [
     "D212",
-]
-extend-exclude = [
-    "old",
+    "ISC001",
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.pycodestyle]
+[tool.ruff.lint.pycodestyle]
 max-doc-length = 100
 
+[tool.ruff.format]
+docstring-code-format = true
+
 [tool.mypy]
 strict = true
 show_column_numbers = true
 disallow_untyped_defs = true
 no_implicit_optional = true
 check_untyped_defs = true
 warn_return_any = true
+ignore_missing_imports = true
 
 [tool.docformatter]
 syntax = "google"
 black = true
 recursive = true
 wrap-summaries = 100
 wrap-descriptions = 100
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.7.1"
+current_version = "0.7.2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore(CI/CD): bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
@@ -264,8 +262,9 @@
     "nvidia-cudnn-cu12",
     "nvidia-cufft-cu12",
     "nvidia-curand-cu12",
     "nvidia-cusolver-cu12",
     "nvidia-cusparse-cu12",
     "nvidia-nccl-cu12",
     "nvidia-nvtx-cu12",
+    "nvidia-nvjitlink-cu12",
 ]
```

### Comparing `srai-0.7.1/srai/_optional.py` & `srai-0.7.2/srai/_optional.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/_typing.py` & `srai-0.7.2/srai/_typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/embedders/__init__.py` & `srai-0.7.2/srai/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/embedders/_base.py` & `srai-0.7.2/srai/embedders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/embedders/contextual_count_embedder.py` & `srai-0.7.2/srai/embedders/contextual_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/embedders/count_embedder.py` & `srai-0.7.2/srai/embedders/count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/embedders/geovex/dataset.py` & `srai-0.7.2/srai/embedders/geovex/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,23 +91,25 @@
         for h3_index in tqdm(data.index, total=len(data)):
             neighbors = neighbourhood.get_neighbours_up_to_distance(
                 h3_index, neighbor_k_ring, include_center=False, unchecked=True
             )
             # check if all the neighbors are in the dataset
             if len(neighbors.intersection(all_indices)) == len(neighbors):
                 # add the h3_index to the valid h3 indices, with the ring of neighbors
-                valid_h3s.append((
-                    h3_index,
-                    data.index.get_loc(h3_index),
-                    [
-                        # get the index of the h3 in the dataset
-                        (data.index.get_loc(_h), get_local_ij_index(h3_index, _h))
-                        for _h in neighbors
-                    ],
-                ))
+                valid_h3s.append(
+                    (
+                        h3_index,
+                        data.index.get_loc(h3_index),
+                        [
+                            # get the index of the h3 in the dataset
+                            (data.index.get_loc(_h), get_local_ij_index(h3_index, _h))
+                            for _h in neighbors
+                        ],
+                    )
+                )
             else:
                 # some of the neighbors are not in the dataset, add the h3_index to the invalid h3s
                 invalid_h3s.add(h3_index)
         return invalid_h3s, valid_h3s
 
     def __len__(self) -> int:
         """
@@ -136,19 +138,21 @@
 
         # build the 3d tensor
         # it is a tensor with diagonals of length neighbor_k_ring
         # the diagonals are the neighbors of the target h3
         # the target h3 is in the center of the tensor
         # the tensor is 2*neighbor_k_ring + 1 x 2*neighbor_k_ring + 1 x 2*neighbor_k_ring + 1
         # make a tensor of zeros, padded by 1 zero all around to make it even for the convolutions
-        tensor: torch.Tensor = torch.zeros((
-            self._N,
-            2 * self._k + 2,
-            2 * self._k + 2,
-        ))
+        tensor: torch.Tensor = torch.zeros(
+            (
+                self._N,
+                2 * self._k + 2,
+                2 * self._k + 2,
+            )
+        )
 
         # set the target h3 to the center of the tensor
         tensor[
             :,
             self._k,
             self._k,
         ] = self._data_torch[target_idx]
```

### Comparing `srai-0.7.1/srai/embedders/geovex/embedder.py` & `srai-0.7.2/srai/embedders/geovex/embedder.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,17 +123,18 @@
         dataset: HexagonalDataset[T],
         dataloader: Optional[DataLoader] = None,
     ) -> pd.DataFrame:
         if dataloader is None:
             dataloader = DataLoader(dataset, batch_size=self._batch_size, shuffle=False)
 
         embeddings = [
-            self._model.encoder(batch).detach().numpy() for batch in dataloader  # type: ignore
+            self._model.encoder(batch).detach().numpy()  # type: ignore
+            for batch in dataloader
         ]
-        if len(dataset.get_invalid_cells()) > 0:
+        if dataset.get_invalid_cells():
             print(
                 "Warning: Some regions were not able to be encoded, as they don't have"
                 f" r={self._r} neighbors."
             )
         df = pd.DataFrame(np.concatenate(embeddings), index=dataset.get_valid_cells())
         df.index.name = REGIONS_INDEX
         return df
```

### Comparing `srai-0.7.1/srai/embedders/geovex/model.py` & `srai-0.7.2/srai/embedders/geovex/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/embedders/gtfs2vec/embedder.py` & `srai-0.7.2/srai/embedders/gtfs2vec/embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,15 +286,15 @@
 
         model.save(path / "model.pt")
 
         config = {
             "model_config": model.get_config(),
             "embedder_config": embedder_config,
         }
-        with open(path / "config.json", "w") as f:
+        with (path / "config.json").open("w") as f:
             json.dump(config, f, ensure_ascii=False, indent=4)
 
     def save(self, path: Union[Path, str]) -> None:
         """
         Save the model to a directory.
 
         Args:
```

### Comparing `srai-0.7.1/srai/embedders/gtfs2vec/model.py` & `srai-0.7.2/srai/embedders/gtfs2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/embedders/hex2vec/embedder.py` & `srai-0.7.2/srai/embedders/hex2vec/embedder.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
 
         self._model.save(path / "model.pt")  # type: ignore
 
         config = {
             "model_config": self._model.get_config(),  # type: ignore
             "embedder_config": embedder_config,
         }
-        with open(path / "config.json", "w") as f:
+        with (path / "config.json").open("w") as f:
             json.dump(config, f, ensure_ascii=False, indent=4)
 
     def save(self, path: Union[Path, str]) -> None:
         """
         Save the model to a directory.
 
         Args:
```

### Comparing `srai-0.7.1/srai/embedders/hex2vec/model.py` & `srai-0.7.2/srai/embedders/hex2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/embedders/hex2vec/neighbour_dataset.py` & `srai-0.7.2/srai/embedders/hex2vec/neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/embedders/highway2vec/embedder.py` & `srai-0.7.2/srai/embedders/highway2vec/embedder.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
         self._model.save(path / "model.pt")  # type: ignore
 
         config = {
             "model_config": self._model.get_config(),  # type: ignore
             "embedder_config": embedder_config,
         }
-        with open(path / "config.json", "w") as f:
+        with (path / "config.json").open("w") as f:
             json.dump(config, f, ensure_ascii=False, indent=4)
 
     def save(self, path: Union[Path, str]) -> None:
         """
         Save the model to a directory.
 
         Args:
```

### Comparing `srai-0.7.1/srai/embedders/highway2vec/model.py` & `srai-0.7.2/srai/embedders/highway2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/exceptions.py` & `srai-0.7.2/srai/exceptions.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/geometry.py` & `srai-0.7.2/srai/geometry.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/h3.py` & `srai-0.7.2/srai/h3.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 @overload
 def h3_to_shapely_geometry(h3_index: Iterable[Union[int, str]]) -> list[Polygon]: ...
 
 
 # TODO: write tests (#322)
 def h3_to_shapely_geometry(
-    h3_index: Union[int, str, Iterable[Union[int, str]]]
+    h3_index: Union[int, str, Iterable[Union[int, str]]],
 ) -> Union[Polygon, list[Polygon]]:
     """
     Convert H3 index to Shapely polygon.
 
     Args:
         h3_index (Union[int, str, Iterable[Union[int, str]]]): H3 index (or list of indexes)
             to be converted.
```

### Comparing `srai-0.7.1/srai/joiners/__init__.py` & `srai-0.7.2/srai/joiners/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/joiners/_base.py` & `srai-0.7.2/srai/joiners/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/joiners/intersection_joiner.py` & `srai-0.7.2/srai/joiners/intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/__init__.py` & `srai-0.7.2/srai/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/_base.py` & `srai-0.7.2/srai/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/download.py` & `srai-0.7.2/srai/loaders/download.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/geoparquet_loader.py` & `srai-0.7.2/srai/loaders/geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/gtfs_loader.py` & `srai-0.7.2/srai/loaders/gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/osm_loaders/_base.py` & `srai-0.7.2/srai/loaders/osm_loaders/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from srai._typing import is_expected_type
 from srai.constants import WGS84_CRS
 from srai.loaders import Loader
 from srai.loaders.osm_loaders.filters import GroupedOsmTagsFilter, OsmTagsFilter
 
 
 def prepare_area_gdf_for_loader(
-    area: Union[BaseGeometry, Iterable[BaseGeometry], gpd.GeoSeries, gpd.GeoDataFrame]
+    area: Union[BaseGeometry, Iterable[BaseGeometry], gpd.GeoSeries, gpd.GeoDataFrame],
 ) -> gpd.GeoDataFrame:
     """
     Prepare an area for the loader.
 
     Loader expects a GeoDataFrame input, but users shouldn't be limited by this requirement.
     All Shapely geometries will by transformed into GeoDataFrame with proper CRS.
```

### Comparing `srai-0.7.1/srai/loaders/osm_loaders/filters/_typing.py` & `srai-0.7.2/srai/loaders/osm_loaders/filters/_typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 @overload
 def merge_osm_tags_filter(osm_tags_filter: Iterable[GroupedOsmTagsFilter]) -> OsmTagsFilter: ...
 
 
 def merge_osm_tags_filter(
     osm_tags_filter: Union[
         OsmTagsFilter, GroupedOsmTagsFilter, Iterable[OsmTagsFilter], Iterable[GroupedOsmTagsFilter]
-    ]
+    ],
 ) -> OsmTagsFilter:
     """
     Merge OSM tags filter into `OsmTagsFilter` type.
 
     Optionally merges `GroupedOsmTagsFilter` into `OsmTagsFilter` to allow loaders to load all
     defined groups during single operation.
 
@@ -48,20 +48,22 @@
         OsmTagsFilter: Merged filters.
     """
     if is_expected_type(osm_tags_filter, OsmTagsFilter):
         return cast(OsmTagsFilter, osm_tags_filter)
     elif is_expected_type(osm_tags_filter, GroupedOsmTagsFilter):
         return _merge_grouped_osm_tags_filter(cast(GroupedOsmTagsFilter, osm_tags_filter))
     elif is_expected_type(osm_tags_filter, Iterable):
-        return _merge_multiple_osm_tags_filters([
-            merge_osm_tags_filter(
-                cast(Union[OsmTagsFilter, GroupedOsmTagsFilter], sub_osm_tags_filter)
-            )
-            for sub_osm_tags_filter in osm_tags_filter
-        ])
+        return _merge_multiple_osm_tags_filters(
+            [
+                merge_osm_tags_filter(
+                    cast(Union[OsmTagsFilter, GroupedOsmTagsFilter], sub_osm_tags_filter)
+                )
+                for sub_osm_tags_filter in osm_tags_filter
+            ]
+        )
 
     raise AttributeError(
         "Provided tags don't match required type definitions"
         " (OsmTagsFilter or GroupedOsmTagsFilter)."
     )
```

### Comparing `srai-0.7.1/srai/loaders/osm_loaders/filters/base_osm_groups.py` & `srai-0.7.2/srai/loaders/osm_loaders/filters/base_osm_groups.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/osm_loaders/filters/geofabrik.py` & `srai-0.7.2/srai/loaders/osm_loaders/filters/geofabrik.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/osm_loaders/filters/hex2vec.py` & `srai-0.7.2/srai/loaders/osm_loaders/filters/hex2vec.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/osm_loaders/filters/popular.py` & `srai-0.7.2/srai/loaders/osm_loaders/filters/popular.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 This module exposes a function `get_popular_tags` that uses taginfo[1] API
 to download the most popular tags from OSM
 
 References:
     1. https://taginfo.openstreetmap.org/
 """
 
+import operator
 from typing import Any
 
 import requests
 from functional import seq
 
 from srai.loaders.osm_loaders.filters import OsmTagsFilter
 
@@ -57,12 +58,12 @@
 ) -> OsmTagsFilter:
     result_tags = (
         seq(taginfo_data)
         .filter(lambda t: t["count_all"] >= min_count)
         .filter(lambda t: t["count_all_fraction"] >= min_fraction)
     )
     if in_wiki_only:
-        result_tags = result_tags.filter(lambda t: t["in_wiki"])
+        result_tags = result_tags.filter(operator.itemgetter("in_wiki"))
     taginfo_grouped: OsmTagsFilter = (
-        result_tags.map(lambda t: (t["key"], t["value"])).group_by_key().to_dict()
+        result_tags.map(operator.itemgetter("key", "value")).group_by_key().to_dict()
     )
     return taginfo_grouped
```

### Comparing `srai-0.7.1/srai/loaders/osm_loaders/osm_online_loader.py` & `srai-0.7.2/srai/loaders/osm_loaders/osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/osm_loaders/osm_pbf_loader.py` & `srai-0.7.2/srai/loaders/osm_loaders/osm_pbf_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/osm_loaders/osm_tile_data_collector.py` & `srai-0.7.2/srai/loaders/osm_loaders/osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/osm_loaders/osm_tile_loader.py` & `srai-0.7.2/srai/loaders/osm_loaders/osm_tile_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/osm_way_loader/constants.py` & `srai-0.7.2/srai/loaders/osm_way_loader/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/loaders/osm_way_loader/osm_way_loader.py` & `srai-0.7.2/srai/loaders/osm_way_loader/osm_way_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/neighbourhoods/_base.py` & `srai-0.7.2/srai/neighbourhoods/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Neighbourhood interface."""
 
+import operator
 from abc import ABC, abstractmethod
 from queue import Queue
 from typing import Generic, Optional, TypeVar
 
 from functional import seq
 
 IndexType = TypeVar("IndexType")
@@ -66,17 +67,23 @@
             include_center (Optional[bool]): Whether to include the region itself in the neighbours.
             If None, the value set in __init__ is used. Defaults to None.
 
         Returns:
             Set[IndexType]: Indexes of the neighbours.
         """
         neighbours_with_distances = self._get_neighbours_with_distances(index, distance)
-        neighbours: set[IndexType] = seq(neighbours_with_distances).map(lambda x: x[0]).to_set()
+        neighbours: set[IndexType] = (
+            seq(neighbours_with_distances).map(operator.itemgetter(0)).to_set()
+        )
         neighbours = self._handle_center(
-            index, distance, neighbours, at_distance=False, include_center_override=include_center
+            index,
+            distance,
+            neighbours,
+            at_distance=False,
+            include_center_override=include_center,
         )
         return neighbours
 
     def get_neighbours_at_distance(
         self, index: IndexType, distance: int, include_center: Optional[bool] = None
     ) -> set[IndexType]:
         """
@@ -92,15 +99,15 @@
         Returns:
             Set[IndexType]: Indexes of the neighbours.
         """
         neighbours_up_to_distance = self._get_neighbours_with_distances(index, distance)
         neighbours_at_distance: set[IndexType] = (
             seq(neighbours_up_to_distance)
             .filter(lambda x: x[1] == distance)
-            .map(lambda x: x[0])
+            .map(operator.itemgetter(0))
             .to_set()
         )
         neighbours_at_distance = self._handle_center(
             index,
             distance,
             neighbours_at_distance,
             at_distance=True,
```

### Comparing `srai-0.7.1/srai/neighbourhoods/adjacency_neighbourhood.py` & `srai-0.7.2/srai/neighbourhoods/adjacency_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/neighbourhoods/h3_neighbourhood.py` & `srai-0.7.2/srai/neighbourhoods/h3_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/plotting/folium_wrapper.py` & `srai-0.7.2/srai/plotting/folium_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/plotting/plotly_wrapper.py` & `srai-0.7.2/srai/plotting/plotly_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/regionalizers/__init__.py` & `srai-0.7.2/srai/regionalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/regionalizers/_base.py` & `srai-0.7.2/srai/regionalizers/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/regionalizers/_spherical_voronoi.py` & `srai-0.7.2/srai/regionalizers/_spherical_voronoi.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,18 +210,20 @@
 
                 polygon_edges.append((start_hash, end_hash))
 
                 if (start_hash, end_hash) not in hashed_edges and (
                     end_hash,
                     start_hash,
                 ) not in hashed_edges:
-                    hashed_edges.add((
-                        start_hash,
-                        end_hash,
-                    ))
+                    hashed_edges.add(
+                        (
+                            start_hash,
+                            end_hash,
+                        )
+                    )
 
             regions_parts[region_id].append((sphere_part_id, polygon_edges))
 
         # interpolate unique ones
 
         interpolated_edges: dict[EdgeHash, list[tuple[float, float]]]
```

### Comparing `srai-0.7.1/srai/regionalizers/administrative_boundary_regionalizer.py` & `srai-0.7.2/srai/regionalizers/administrative_boundary_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/regionalizers/geocode.py` & `srai-0.7.2/srai/regionalizers/geocode.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/regionalizers/h3_regionalizer.py` & `srai-0.7.2/srai/regionalizers/h3_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/regionalizers/s2_regionalizer.py` & `srai-0.7.2/srai/regionalizers/s2_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/regionalizers/slippy_map_regionalizer.py` & `srai-0.7.2/srai/regionalizers/slippy_map_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/srai/regionalizers/voronoi_regionalizer.py` & `srai-0.7.2/srai/regionalizers/voronoi_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/conftest.py` & `srai-0.7.2/tests/embedders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/constants.py` & `srai-0.7.2/tests/embedders/geovex/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/generation.py` & `srai-0.7.2/tests/embedders/geovex/generation.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_dataset.py` & `srai-0.7.2/tests/embedders/geovex/test_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,15 @@
 @pytest.mark.parametrize(
     "ring_distance",
     [2, 3, 4],
 )  # type: ignore
 def test_dataset_length(ring_distance: int, regions_data_df: pd.DataFrame):
     """Test if HexagonalDataset constructs lookup tables correctly."""
     neighbourhood: H3Neighbourhood = H3Neighbourhood(regions_data_df)
-    dataset = HexagonalDataset(
-        regions_data_df, neighbourhood, neighbor_k_ring=ring_distance
-    )  # type: ignore
+    dataset = HexagonalDataset(regions_data_df, neighbourhood, neighbor_k_ring=ring_distance)  # type: ignore
     assert len(dataset) == len(
         neighbourhood.get_neighbours_up_to_distance(
             ROOT_REGION, distance=RING_DISTANCE - ring_distance, include_center=True, unchecked=True
         )
     )
 
 
@@ -96,32 +94,32 @@
 def test_dataset_item(regions_data_df: pd.DataFrame) -> None:
     """Test if HexagonalDataset constructs lookup tables correctly."""
     import numpy as np
 
     ring_distance = 2
 
     neighbourhood = H3Neighbourhood(regions_data_df)
-    dataset = HexagonalDataset(
-        regions_data_df, neighbourhood, neighbor_k_ring=ring_distance
-    )  # type: ignore
+    dataset = HexagonalDataset(regions_data_df, neighbourhood, neighbor_k_ring=ring_distance)  # type: ignore
     item = next(iter(dataset)).detach().numpy()
     # flatten it out and get the corresponding hexagons
     cells = regions_data_df.reset_index().set_index("data").loc[item.reshape(-1).tolist()].values
 
     # it starts with the root region
     # for each of the h3s, calculate the ij index
     ijs = np.array([get_local_ij_index(ROOT_REGION, _cell) for _cell in cells])
 
     ijs = ijs.reshape(ring_distance * 2 + 2, ring_distance * 2 + 2, 2)
 
     # commpare to the transposed image in the paper
     # specifically fig. 3
     # the bottom and right are padded by 0s for even #
-    desired = np.array([
-        [(0, 0), (0, 0), (0, 2), (1, 2), (2, 2), (0, 0)],
-        [(0, 0), (-1, 1), (0, 1), (1, 1), (2, 1), (0, 0)],
-        [(-2, 0), (-1, 0), (0, 0), (1, 0), (2, 0), (0, 0)],
-        [(-2, -1), (-1, -1), (0, -1), (1, -1), (0, 0), (0, 0)],
-        [(-2, -2), (-1, -2), (0, -2), (0, 0), (0, 0), (0, 0)],
-        [(0, 0), (0, 0), (0, 0), (0, 0), (0, 0), (0, 0)],
-    ])
+    desired = np.array(
+        [
+            [(0, 0), (0, 0), (0, 2), (1, 2), (2, 2), (0, 0)],
+            [(0, 0), (-1, 1), (0, 1), (1, 1), (2, 1), (0, 0)],
+            [(-2, 0), (-1, 0), (0, 0), (1, 0), (2, 0), (0, 0)],
+            [(-2, -1), (-1, -1), (0, -1), (1, -1), (0, 0), (0, 0)],
+            [(-2, -2), (-1, -2), (0, -2), (0, 0), (0, 0), (0, 0)],
+            [(0, 0), (0, 0), (0, 0), (0, 0), (0, 0), (0, 0)],
+        ]
+    )
     assert np.all(ijs.transpose(1, 0, -1) == desired)
```

### Comparing `srai-0.7.1/tests/embedders/geovex/test_embedder.py` & `srai-0.7.2/tests/embedders/geovex/test_embedder.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,17 @@
         joint_gdf = pd.read_parquet(test_files_path / f"{name}_joint.parquet")
         seed_everything(seed, workers=True)
         os.environ["PYTHONHASHSEED"] = str(seed)
         torch.use_deterministic_algorithms(True)
 
         neighbourhood = H3Neighbourhood(regions_gdf)
         target_features = [
-            f"{st}_{t}" for st in test_case["tags"] for t in test_case["tags"][st]  # type: ignore
+            f"{st}_{t}"
+            for st in test_case["tags"]  # type: ignore
+            for t in test_case["tags"][st]  # type: ignore
         ]
         embedder = GeoVexEmbedder(
             target_features=target_features,
             batch_size=10,
             neighbourhood_radius=radius,
             embedding_size=EMBEDDING_SIZE,
             convolutional_layers=test_case["num_layers"],  # type: ignore
```

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_0.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_1.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_2.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_batch_3.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_features.parquet` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_0.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_1.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_2.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_forward_3.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_joint.parquet` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_0.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_1.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_2.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_loss_3.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_regions.parquet` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/AL_10_result.parquet` & `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_batch_0.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_batch_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_batch_1.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_batch_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_features.parquet` & `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_forward_0.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_forward_1.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_joint.parquet` & `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_loss_0.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_loss_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_loss_1.pt` & `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_loss_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_regions.parquet` & `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_files/wro_9_result.parquet` & `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/geovex/test_model.py` & `srai-0.7.2/tests/embedders/geovex/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,17 +78,15 @@
         joint_gdf = pd.read_parquet(test_files_path / f"{name}_joint.parquet")
 
         seed_everything(seed, workers=True)
         os.environ["PYTHONHASHSEED"] = str(seed)
         torch.use_deterministic_algorithms(True)
 
         neighbourhood = H3Neighbourhood(regions_gdf)
-        target_features = [
-            f"{st}_{t}" for st in test_case["tags"] for t in test_case["tags"][st]  # type: ignore
-        ]
+        target_features = [f"{st}_{t}" for st in test_case["tags"] for t in test_case["tags"][st]]  # type: ignore
         embedder = GeoVexEmbedder(
             target_features=target_features,
             batch_size=10,
             neighbourhood_radius=radius,
             embedding_size=EMBEDDING_SIZE,
             convolutional_layers=test_case["num_layers"],  # type: ignore
             convolutional_layer_size=test_case["convolutional_layer_size"],  # type: ignore
```

### Comparing `srai-0.7.1/tests/embedders/hex2vec/constants.py` & `srai-0.7.2/tests/embedders/hex2vec/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/hex2vec/generation.py` & `srai-0.7.2/tests/embedders/hex2vec/generation.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/hex2vec/test_embedder.py` & `srai-0.7.2/tests/embedders/hex2vec/test_embedder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Hex2VecEmbedder tests."""
 
 from contextlib import nullcontext as does_not_raise
 from pathlib import Path
 from typing import Any
 
 import geopandas as gpd
-import pandas as pd
 import pytest
-from pandas.testing import assert_frame_equal
+from pytest_snapshot.plugin import Snapshot
 from pytorch_lightning import seed_everything
 
 from srai.embedders.hex2vec.embedder import Hex2VecEmbedder
 from srai.exceptions import ModelNotFitException
 from srai.neighbourhoods import H3Neighbourhood
 from tests.embedders.hex2vec.constants import ENCODER_SIZES, PREDEFINED_TEST_CASES, TRAINER_KWARGS
 
@@ -42,30 +41,38 @@
 
 def test_embedder_default_encoder_sizes() -> None:
     """Test that Hex2VecEmbedder uses default encoder sizes if not specified."""
     embedder = Hex2VecEmbedder()
     assert embedder._encoder_sizes == Hex2VecEmbedder.DEFAULT_ENCODER_SIZES
 
 
-def test_embedder() -> None:
+def test_embedder(snapshot: Snapshot) -> None:
     """Test Hex2VecEmbedder on predefined test cases."""
     test_files_path = Path(__file__).parent / "test_files"
+    snapshot.snapshot_dir = test_files_path.as_posix()
+
     for test_case in PREDEFINED_TEST_CASES:
         name = test_case["test_case_name"]
         seed = test_case["seed"]
         print(name, seed)
 
-        expected = pd.read_parquet(test_files_path / f"{name}_result.parquet")
         regions_gdf = gpd.read_parquet(test_files_path / f"{name}_regions.parquet")
         features_gdf = gpd.read_parquet(test_files_path / f"{name}_features.parquet")
         joint_gdf = gpd.read_parquet(test_files_path / f"{name}_joint.parquet")
         seed_everything(seed)
 
         neighbourhood = H3Neighbourhood(regions_gdf)
         embedder = Hex2VecEmbedder(encoder_sizes=ENCODER_SIZES)
         result_df = embedder.fit_transform(
             regions_gdf, features_gdf, joint_gdf, neighbourhood, trainer_kwargs=TRAINER_KWARGS
         )
         result_df.columns = result_df.columns.astype(str)
         print(result_df.head())
-        print(expected.head())
-        assert_frame_equal(result_df, expected, atol=1e-1)
+
+        # FIXME(Calychas): readd after making neighbourhoods deterministic.
+        # See [#441](https://github.com/kraina-ai/srai/pull/441)
+        # snapshot.assert_match(result_df.to_json(
+        #     orient="index", indent=True), f"{name}_result.json"
+        # )
+        assert not result_df.empty
+        assert result_df.shape[0] == regions_gdf.shape[0]
+        assert result_df.shape[1] == ENCODER_SIZES[-1]
```

### Comparing `srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_features.parquet` & `srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_joint.parquet` & `srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_regions.parquet` & `srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/hex2vec/test_files/poz_8_result.parquet` & `srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_features.parquet` & `srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_joint.parquet` & `srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_regions.parquet` & `srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/hex2vec/test_files/wro_9_result.parquet` & `srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/hex2vec/test_model.py` & `srai-0.7.2/tests/embedders/hex2vec/test_model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/hex2vec/test_neighbour_dataset.py` & `srai-0.7.2/tests/embedders/hex2vec/test_neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/test_contextual_count_embedder.py` & `srai-0.7.2/tests/embedders/test_contextual_count_embedder.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,21 @@
 @pytest.fixture  # type: ignore
 def expected_embedding_df_squashed_distance_0() -> pd.DataFrame:
     """
     Get expected ContextualCountEmbedder output.
 
     Count without subcategories. Squashed features, distance 0.
     """
-    return _create_features_dataframe({
-        REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
-        "leisure": [0, 1, 1],
-        "amenity": [1, 0, 1],
-    })
+    return _create_features_dataframe(
+        {
+            REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
+            "leisure": [0, 1, 1],
+            "amenity": [1, 0, 1],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def expected_embedding_df_squashed_distance_1() -> pd.DataFrame:
     """
     Get expected ContextualCountEmbedder output.
 
@@ -54,19 +56,21 @@
 @pytest.fixture  # type: ignore
 def expected_embedding_df_concatenated_distance_0() -> pd.DataFrame:
     """
     Get expected ContextualCountEmbedder output.
 
     Count without subcategories. Concatenated features, distance 0.
     """
-    return _create_features_dataframe({
-        REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
-        "leisure_0": [0, 1, 1],
-        "amenity_0": [1, 0, 1],
-    })
+    return _create_features_dataframe(
+        {
+            REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
+            "leisure_0": [0, 1, 1],
+            "amenity_0": [1, 0, 1],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def expected_embedding_df_concatenated_distance_1() -> pd.DataFrame:
     """
     Get expected ContextualCountEmbedder output.
 
@@ -217,164 +221,182 @@
 @pytest.fixture  # type: ignore
 def specified_features_expected_embedding_df_squashed_empty() -> pd.DataFrame:
     """
     Get expected ContextualCountEmbedder output for the case with specified features.
 
     Count without subcategories. Squashed features, distance 0+.
     """
-    return _create_features_dataframe({
-        REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
-        "amenity_parking": [0, 0, 0],
-        "leisure_park": [0, 0, 0],
-        "amenity_pub": [0, 0, 0],
-    })
+    return _create_features_dataframe(
+        {
+            REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
+            "amenity_parking": [0, 0, 0],
+            "leisure_park": [0, 0, 0],
+            "amenity_pub": [0, 0, 0],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def specified_features_expected_subcategories_embedding_df_squashed_distance_0() -> pd.DataFrame:
     """
     Get expected ContextualCountEmbedder output for the case with specified features.
 
     Count with subcategories. Squashed features, distance 0.
     """
-    return _create_features_dataframe({
-        REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
-        "amenity_parking": [0, 0, 0],
-        "leisure_park": [0, 0, 0],
-        "amenity_pub": [1, 0, 1],
-    })
+    return _create_features_dataframe(
+        {
+            REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
+            "amenity_parking": [0, 0, 0],
+            "leisure_park": [0, 0, 0],
+            "amenity_pub": [1, 0, 1],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def specified_features_expected_subcategories_embedding_df_squashed_distance_1() -> pd.DataFrame:
     """
     Get expected ContextualCountEmbedder output for the case with specified features.
 
     Count with subcategories. Squashed features, distance 1+.
     """
-    return _create_features_dataframe({
-        REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
-        "amenity_parking": [0, 0, 0],
-        "leisure_park": [0, 0, 0],
-        "amenity_pub": [1.125, 0.25, 1.125],
-    })
+    return _create_features_dataframe(
+        {
+            REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
+            "amenity_parking": [0, 0, 0],
+            "leisure_park": [0, 0, 0],
+            "amenity_pub": [1.125, 0.25, 1.125],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def specified_features_expected_embedding_df_concatenated_distance_0() -> pd.DataFrame:
     """
     Get expected ContextualCountEmbedder output for the case with specified features.
 
     Count without subcategories. Concatenated features, distance 0.
     """
-    return _create_features_dataframe({
-        REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
-        "amenity_parking_0": [0, 0, 0],
-        "leisure_park_0": [0, 0, 0],
-        "amenity_pub_0": [0, 0, 0],
-    })
+    return _create_features_dataframe(
+        {
+            REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
+            "amenity_parking_0": [0, 0, 0],
+            "leisure_park_0": [0, 0, 0],
+            "amenity_pub_0": [0, 0, 0],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def specified_features_expected_embedding_df_concatenated_distance_1() -> pd.DataFrame:
     """
     Get expected ContextualCountEmbedder output for the case with specified features.
 
     Count without subcategories. Concatenated features, distance 1.
     """
-    return _create_features_dataframe({
-        REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
-        "amenity_parking_0": [0, 0, 0],
-        "leisure_park_0": [0, 0, 0],
-        "amenity_pub_0": [0, 0, 0],
-        "amenity_parking_1": [0, 0, 0],
-        "leisure_park_1": [0, 0, 0],
-        "amenity_pub_1": [0, 0, 0],
-    })
+    return _create_features_dataframe(
+        {
+            REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
+            "amenity_parking_0": [0, 0, 0],
+            "leisure_park_0": [0, 0, 0],
+            "amenity_pub_0": [0, 0, 0],
+            "amenity_parking_1": [0, 0, 0],
+            "leisure_park_1": [0, 0, 0],
+            "amenity_pub_1": [0, 0, 0],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def specified_features_expected_embedding_df_concatenated_distance_2() -> pd.DataFrame:
     """
     Get expected ContextualCountEmbedder output for the case with specified features.
 
     Count without subcategories. Concatenated features, distance 2.
     """
-    return _create_features_dataframe({
-        REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
-        "amenity_parking_0": [0, 0, 0],
-        "leisure_park_0": [0, 0, 0],
-        "amenity_pub_0": [0, 0, 0],
-        "amenity_parking_1": [0, 0, 0],
-        "leisure_park_1": [0, 0, 0],
-        "amenity_pub_1": [0, 0, 0],
-        "amenity_parking_2": [0, 0, 0],
-        "leisure_park_2": [0, 0, 0],
-        "amenity_pub_2": [0, 0, 0],
-    })
+    return _create_features_dataframe(
+        {
+            REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
+            "amenity_parking_0": [0, 0, 0],
+            "leisure_park_0": [0, 0, 0],
+            "amenity_pub_0": [0, 0, 0],
+            "amenity_parking_1": [0, 0, 0],
+            "leisure_park_1": [0, 0, 0],
+            "amenity_pub_1": [0, 0, 0],
+            "amenity_parking_2": [0, 0, 0],
+            "leisure_park_2": [0, 0, 0],
+            "amenity_pub_2": [0, 0, 0],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def specified_features_expected_subcategories_embedding_df_concatenated_distance_0() -> (
     pd.DataFrame
 ):
     """
     Get expected ContextualCountEmbedder output for the case with specified features.
 
     Count with subcategories. Concatenated features, distance 0.
     """
-    return _create_features_dataframe({
-        REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
-        "amenity_parking_0": [0, 0, 0],
-        "leisure_park_0": [0, 0, 0],
-        "amenity_pub_0": [1, 0, 1],
-    })
+    return _create_features_dataframe(
+        {
+            REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
+            "amenity_parking_0": [0, 0, 0],
+            "leisure_park_0": [0, 0, 0],
+            "amenity_pub_0": [1, 0, 1],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def specified_features_expected_subcategories_embedding_df_concatenated_distance_1() -> (
     pd.DataFrame
 ):
     """
     Get expected ContextualCountEmbedder output for the case with specified features.
 
     Count with subcategories. Concatenated features, distance 1.
     """
-    return _create_features_dataframe({
-        REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
-        "amenity_parking_0": [0, 0, 0],
-        "leisure_park_0": [0, 0, 0],
-        "amenity_pub_0": [1, 0, 1],
-        "amenity_parking_1": [0, 0, 0],
-        "leisure_park_1": [0, 0, 0],
-        "amenity_pub_1": [0.5, 1, 0.5],
-    })
+    return _create_features_dataframe(
+        {
+            REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
+            "amenity_parking_0": [0, 0, 0],
+            "leisure_park_0": [0, 0, 0],
+            "amenity_pub_0": [1, 0, 1],
+            "amenity_parking_1": [0, 0, 0],
+            "leisure_park_1": [0, 0, 0],
+            "amenity_pub_1": [0.5, 1, 0.5],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def specified_features_expected_subcategories_embedding_df_concatenated_distance_2() -> (
     pd.DataFrame
 ):
     """
     Get expected ContextualCountEmbedder output for the case with specified features.
 
     Count with subcategories. Concatenated features, distance 2.
     """
-    return _create_features_dataframe({
-        REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
-        "amenity_parking_0": [0, 0, 0],
-        "leisure_park_0": [0, 0, 0],
-        "amenity_pub_0": [1, 0, 1],
-        "amenity_parking_1": [0, 0, 0],
-        "leisure_park_1": [0, 0, 0],
-        "amenity_pub_1": [0.5, 1, 0.5],
-        "amenity_parking_2": [0, 0, 0],
-        "leisure_park_2": [0, 0, 0],
-        "amenity_pub_2": [0, 0, 0],
-    })
+    return _create_features_dataframe(
+        {
+            REGIONS_INDEX: ["891e2040897ffff", "891e2040d4bffff", "891e2040d5bffff"],
+            "amenity_parking_0": [0, 0, 0],
+            "leisure_park_0": [0, 0, 0],
+            "amenity_pub_0": [1, 0, 1],
+            "amenity_parking_1": [0, 0, 0],
+            "leisure_park_1": [0, 0, 0],
+            "amenity_pub_1": [0.5, 1, 0.5],
+            "amenity_parking_2": [0, 0, 0],
+            "leisure_park_2": [0, 0, 0],
+            "amenity_pub_2": [0, 0, 0],
+        }
+    )
 
 
 @P.parameters(
     "expected_embedding_fixture",
     "neighbourhood_distance",
     "concatenate_features",
     "count_subcategories",
```

### Comparing `srai-0.7.1/tests/embedders/test_count_embedder.py` & `srai-0.7.2/tests/embedders/test_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/test_gtfs2vec_embedder.py` & `srai-0.7.2/tests/embedders/test_gtfs2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/embedders/test_highway2vec_embedder.py` & `srai-0.7.2/tests/embedders/test_highway2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/h3/conftest.py` & `srai-0.7.2/tests/h3/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,53 +30,61 @@
                 shell=[
                     (-1, 0),
                     (0, 0.5),
                     (1, 0),
                     (1, 1),
                     (0, 1),
                 ],
-                holes=[[
-                    (0.8, 0.9),
-                    (0.9, 0.55),
-                    (0.8, 0.3),
-                    (0.5, 0.4),
-                ]],
+                holes=[
+                    [
+                        (0.8, 0.9),
+                        (0.9, 0.55),
+                        (0.8, 0.3),
+                        (0.5, 0.4),
+                    ]
+                ],
             ),
             geometry.Polygon(shell=[(-0.25, 0), (0.25, 0), (0, 0.2)]),
         ],
         crs=WGS84_CRS,
     )
 
 
 @pytest.fixture  # type: ignore
 def gdf_multipolygon() -> gpd.GeoDataFrame:
     """Get GeoDataFrame with multipolygon."""
     return gpd.GeoDataFrame(
         geometry=[
-            geometry.MultiPolygon([
-                (
-                    [
-                        (-1, 0),
-                        (0, 0.5),
-                        (1, 0),
-                        (1, 1),
-                        (0, 1),
-                    ],
-                    ([[
-                        (0.8, 0.9),
-                        (0.9, 0.55),
-                        (0.8, 0.3),
-                        (0.5, 0.4),
-                    ]]),
-                ),
-                (
-                    [(-0.25, 0), (0.25, 0), (0, 0.2)],
-                    (),
-                ),
-            ])
+            geometry.MultiPolygon(
+                [
+                    (
+                        [
+                            (-1, 0),
+                            (0, 0.5),
+                            (1, 0),
+                            (1, 1),
+                            (0, 1),
+                        ],
+                        (
+                            [
+                                [
+                                    (0.8, 0.9),
+                                    (0.9, 0.55),
+                                    (0.8, 0.3),
+                                    (0.5, 0.4),
+                                ]
+                            ]
+                        ),
+                    ),
+                    (
+                        [(-0.25, 0), (0.25, 0), (0, 0.2)],
+                        (),
+                    ),
+                ]
+            )
         ],
         crs=WGS84_CRS,
     )
 
 
 @pytest.fixture  # type: ignore
 def expected_h3_indexes() -> list[str]:
```

### Comparing `srai-0.7.1/tests/h3/test_ij_coordinates.py` & `srai-0.7.2/tests/h3/test_ij_coordinates.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/h3/test_shapely_conversion.py` & `srai-0.7.2/tests/h3/test_shapely_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ut = TestCase()
 
 
 def _gdf_noop(gdf_fixture: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
     return gdf_fixture
 
 
-def _gdf_to_geoseries(gdf_fixture: gpd.GeoDataFrame) -> gpd.GeoSeries:
+def _gdf_to_geoseries(gdf_fixture: gpd.GeoDataFrame) -> gpd.GeoSeries:  # noqa: FURB118
     return gdf_fixture[GEOMETRY_COLUMN]
 
 
 def _gdf_to_geometry_list(gdf_fixture: gpd.GeoDataFrame) -> list[BaseGeometry]:
     return list(gdf_fixture[GEOMETRY_COLUMN])
```

### Comparing `srai-0.7.1/tests/joiners/conftest.py` & `srai-0.7.2/tests/joiners/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/joiners/test_intersection_joiner.py` & `srai-0.7.2/tests/joiners/test_intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/conftest.py` & `srai-0.7.2/tests/loaders/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,90 +7,106 @@
 import pytest
 from pytest_mock import MockerFixture
 
 
 @pytest.fixture  # type: ignore
 def gtfs_validation_ok() -> pd.DataFrame:
     """Get GTFS validation result with no errors."""
-    return pd.DataFrame({
-        "type": ["warning", "warning"],
-        "message": ["test warning", "test warning"],
-        "table": ["test_table", "test_table"],
-        "rows": [[1, 2], [3, 4]],
-    })
+    return pd.DataFrame(
+        {
+            "type": ["warning", "warning"],
+            "message": ["test warning", "test warning"],
+            "table": ["test_table", "test_table"],
+            "rows": [[1, 2], [3, 4]],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def gtfs_validation_error() -> pd.DataFrame:
     """Get GTFS validation result with errors."""
-    return pd.DataFrame({
-        "type": ["error", "error", "warning", "warning"],
-        "message": ["test error", "test error", "test warning", "test warning"],
-        "table": ["test_table", "test_table", "test_table", "test_table"],
-        "rows": [[1, 2], [3, 4], [5, 6], [7, 8]],
-    })
+    return pd.DataFrame(
+        {
+            "type": ["error", "error", "warning", "warning"],
+            "message": ["test error", "test error", "test warning", "test warning"],
+            "table": ["test_table", "test_table", "test_table", "test_table"],
+            "rows": [[1, 2], [3, 4], [5, 6], [7, 8]],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def stop_time_series() -> pd.DataFrame:
     """Get mocked stop time series."""
-    ts = pd.DataFrame.from_dict({
-        "datetime": pd.DatetimeIndex([datetime(2022, 1, 2, 12, 0), datetime(2022, 1, 2, 13, 0)]),
-        "42": pd.Series([0, 2]),
-        "76": pd.Series([12, 12]),
-    }).set_index("datetime")
+    ts = pd.DataFrame.from_dict(
+        {
+            "datetime": pd.DatetimeIndex(
+                [datetime(2022, 1, 2, 12, 0), datetime(2022, 1, 2, 13, 0)]
+            ),
+            "42": pd.Series([0, 2]),
+            "76": pd.Series([12, 12]),
+        }
+    ).set_index("datetime")
 
     ts.columns = pd.MultiIndex.from_tuples(
         [("num_trips", "42"), ("num_trips", "76")], names=["indicator", "stop_id"]
     )
 
     return ts
 
 
 @pytest.fixture  # type: ignore
 def stop_times() -> pd.DataFrame:
     """Get mocked stop times."""
-    return pd.DataFrame({
-        "trip_id": ["1", "1", "2", "2"],
-        "arrival_time": ["12:00:00", "13:00:00", "12:00:00", "13:00:00"],
-        "departure_time": ["12:00:00", "12:00:00", "13:00:00", "13:00:00"],
-        "stop_id": ["42", "76", "42", "76"],
-    })
+    return pd.DataFrame(
+        {
+            "trip_id": ["1", "1", "2", "2"],
+            "arrival_time": ["12:00:00", "13:00:00", "12:00:00", "13:00:00"],
+            "departure_time": ["12:00:00", "12:00:00", "13:00:00", "13:00:00"],
+            "stop_id": ["42", "76", "42", "76"],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def trips() -> pd.DataFrame:
     """Get mocked trips."""
-    return pd.DataFrame({
-        "trip_id": ["1", "2"],
-        "trip_headsign": ["A", "B"],
-    })
+    return pd.DataFrame(
+        {
+            "trip_id": ["1", "2"],
+            "trip_headsign": ["A", "B"],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def stops() -> pd.DataFrame:
     """Get mocked stops."""
-    return pd.DataFrame({
-        "stop_id": ["42", "76"],
-        "stop_lat": [51.198083, 51.107133],
-        "stop_lon": [16.905892, 17.019394],
-    })
+    return pd.DataFrame(
+        {
+            "stop_id": ["42", "76"],
+            "stop_lat": [51.198083, 51.107133],
+            "stop_lon": [16.905892, 17.019394],
+        }
+    )
 
 
 @pytest.fixture  # type: ignore
 def feed(
     mocker: MockerFixture,
     stop_time_series: pd.DataFrame,
     stop_times: pd.DataFrame,
     trips: pd.DataFrame,
     stops: pd.DataFrame,
 ) -> Any:
     """Get mocked feed."""
     feed_mock = mocker.MagicMock()
-    feed_mock.configure_mock(**{
-        "get_first_week.return_value": ["", "", "20220102"],
-        "compute_stop_time_series.return_value": stop_time_series,
-        "stop_times": stop_times,
-        "trips": trips,
-        "stops": stops,
-    })
+    feed_mock.configure_mock(
+        **{
+            "get_first_week.return_value": ["", "", "20220102"],
+            "compute_stop_time_series.return_value": stop_time_series,
+            "stop_times": stop_times,
+            "trips": trips,
+            "stops": stops,
+        }
+    )
     return feed_mock
```

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/conftest.py` & `srai-0.7.2/tests/loaders/osm_loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/filters/popular_filter_example.json` & `srai-0.7.2/tests/loaders/osm_loaders/filters/popular_filter_example.json`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/filters/test_merge_filter_types.py` & `srai-0.7.2/tests/loaders/osm_loaders/filters/test_merge_filter_types.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py` & `srai-0.7.2/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `srai-0.7.2/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `srai-0.7.2/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `srai-0.7.2/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/test_files/monaco.osm.pbf` & `srai-0.7.2/tests/loaders/osm_loaders/test_files/monaco.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/test_files/poland.geojson` & `srai-0.7.2/tests/loaders/osm_loaders/test_files/poland.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson` & `srai-0.7.2/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/test_osm_online_loader.py` & `srai-0.7.2/tests/loaders/osm_loaders/test_osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/test_osm_pbf_loader.py` & `srai-0.7.2/tests/loaders/osm_loaders/test_osm_pbf_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,38 +23,42 @@
 
 @pytest.mark.parametrize("explode_tags", [True, False])  # type: ignore
 @pytest.mark.parametrize("keep_all_tags", [True, False])  # type: ignore
 def test_pbf_to_geoparquet_parsing(explode_tags: bool, keep_all_tags: bool):
     """Test if pbf to geoparquet conversion works."""
     pbf_file = Path(__file__).parent / "test_files" / "monaco.osm.pbf"
     OSMPbfLoader(pbf_file=pbf_file).load_to_geoparquet(
-        area=Polygon([
-            (7.416769421059001, 43.7346112362936),
-            (7.416769421059001, 43.730681304758946),
-            (7.4218262821731, 43.730681304758946),
-            (7.4218262821731, 43.7346112362936),
-        ]),
+        area=Polygon(
+            [
+                (7.416769421059001, 43.7346112362936),
+                (7.416769421059001, 43.730681304758946),
+                (7.4218262821731, 43.730681304758946),
+                (7.4218262821731, 43.7346112362936),
+            ]
+        ),
         tags=GEOFABRIK_LAYERS,
         ignore_cache=True,
         explode_tags=explode_tags,
         keep_all_tags=keep_all_tags,
     )
 
 
 @pytest.mark.parametrize(  # type: ignore
     "test_geometries,pbf_file,query,pbf_source,expected_result_length,expected_features_columns_length,expected_features_columns_names",
     [
         (
             [
-                Polygon([
-                    (7.416769421059001, 43.7346112362936),
-                    (7.416769421059001, 43.730681304758946),
-                    (7.4218262821731, 43.730681304758946),
-                    (7.4218262821731, 43.7346112362936),
-                ])
+                Polygon(
+                    [
+                        (7.416769421059001, 43.7346112362936),
+                        (7.416769421059001, 43.730681304758946),
+                        (7.4218262821731, 43.730681304758946),
+                        (7.4218262821731, 43.7346112362936),
+                    ]
+                )
             ],
             Path(__file__).parent / "test_files" / "monaco.osm.pbf",
             HEX2VEC_FILTER,
             "geofabrik",
             403,
             12,
             [
@@ -70,20 +74,22 @@
                 "sport",
                 "tourism",
                 "water",
             ],
         ),
         (
             [
-                Polygon([
-                    (7.416769421059001, 43.7346112362936),
-                    (7.416769421059001, 43.730681304758946),
-                    (7.4218262821731, 43.730681304758946),
-                    (7.4218262821731, 43.7346112362936),
-                ])
+                Polygon(
+                    [
+                        (7.416769421059001, 43.7346112362936),
+                        (7.416769421059001, 43.730681304758946),
+                        (7.4218262821731, 43.730681304758946),
+                        (7.4218262821731, 43.7346112362936),
+                    ]
+                )
             ],
             Path(__file__).parent / "test_files" / "monaco.osm.pbf",
             GEOFABRIK_LAYERS,
             "geofabrik",
             958,
             23,
             [
```

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/test_osm_tile_data_collector.py` & `srai-0.7.2/tests/loaders/osm_loaders/test_osm_tile_data_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,27 +69,27 @@
         assert stored == img
 
 
 @pytest.mark.parametrize(  # type: ignore
     "collector_type", [(collectors.DataCollectorType.RETURN), "return"]
 )
 def test_in_memory_collector_creation(
-    collector_type: Union[str, collectors.DataCollectorType]
+    collector_type: Union[str, collectors.DataCollectorType],
 ) -> None:
     """Test if factory creates properly InMemoryDataCollector."""
     created = collectors.get_collector(collector_type)
 
     assert isinstance(created, collectors.InMemoryDataCollector)
 
 
 @pytest.mark.parametrize(  # type: ignore
     "collector_type", [(collectors.DataCollectorType.SAVE), "save"]
 )
 def test_saving_collector_creation(
-    collector_type: Union[str, collectors.DataCollectorType]
+    collector_type: Union[str, collectors.DataCollectorType],
 ) -> None:
     """Test if factory creates properly SavingDataCollector."""
     created = collectors.get_collector(collector_type, save_path=PATH, file_extension=FILE_TYPE)
 
     assert isinstance(created, collectors.SavingDataCollector), f"Invalid type {type(created)}"
     assert created.format == FILE_TYPE
     assert str(created.save_path) == PATH
```

### Comparing `srai-0.7.1/tests/loaders/osm_loaders/test_osm_tile_loader.py` & `srai-0.7.2/tests/loaders/osm_loaders/test_osm_tile_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,21 +44,23 @@
         for _ in range(3)
     ]
 
 
 @pytest.fixture  # type: ignore
 def gdf() -> gpd.GeoDataFrame:
     """GeoDataFrame approximating Wroclaw bounds."""
-    polygon = Polygon([
-        (16.8073393, 51.1389477),
-        (17.0278673, 51.0426754),
-        (17.1762192, 51.1063195),
-        (16.9580276, 51.2093551),
-        (16.8073393, 51.1389477),
-    ])
+    polygon = Polygon(
+        [
+            (16.8073393, 51.1389477),
+            (17.0278673, 51.0426754),
+            (17.1762192, 51.1063195),
+            (16.9580276, 51.2093551),
+            (16.8073393, 51.1389477),
+        ]
+    )
     gdf = gpd.GeoDataFrame({"geometry": [polygon]}, crs=WGS84_CRS)
     return gdf
 
 
 def mock_requests(images: list[bytes], m: requests_mock.Mocker) -> None:
     """Make mocks for requests."""
     m.get(urljoin(TEST_DOMAIN, f"10/560/341.{RESOURCE_TYPE}"), content=images[0])
```

### Comparing `srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_1.pkl` & `srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_1.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_2.pkl` & `srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_2.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_3.pkl` & `srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_3.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_way_loader/test_files/graph_4.pkl` & `srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_4.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/osm_way_loader/test_osm_way_loader.py` & `srai-0.7.2/tests/loaders/osm_way_loader/test_osm_way_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,35 +54,39 @@
     gdf = gpd.GeoDataFrame({GEOMETRY_COLUMN: [polygon]}, crs=WGS84_CRS)
     return gdf
 
 
 @pytest.fixture  # type: ignore
 def first_polygon_area_gdf() -> gpd.GeoDataFrame:
     """Get an example area gdf with one polygon."""
-    polygon = shpg.Polygon([
-        (17.1005309, 51.1100158),
-        (17.1020436, 51.1100427),
-        (17.1021938, 51.1082509),
-        (17.1006274, 51.1081027),
-        (17.1005201, 51.1099956),
-    ])
+    polygon = shpg.Polygon(
+        [
+            (17.1005309, 51.1100158),
+            (17.1020436, 51.1100427),
+            (17.1021938, 51.1082509),
+            (17.1006274, 51.1081027),
+            (17.1005201, 51.1099956),
+        ]
+    )
 
     gdf = gpd.GeoDataFrame({GEOMETRY_COLUMN: [polygon]}, crs=WGS84_CRS)
     return gdf
 
 
 @pytest.fixture  # type: ignore
 def second_polygon_area_gdf() -> gpd.GeoDataFrame:
     """Get an example area gdf with one polygon."""
-    polygon = shpg.Polygon([
-        (17.0994473, 51.1084126),
-        (17.1023226, 51.1086551),
-        (17.1023333, 51.1076312),
-        (17.0994473, 51.1083722),
-    ])
+    polygon = shpg.Polygon(
+        [
+            (17.0994473, 51.1084126),
+            (17.1023226, 51.1086551),
+            (17.1023333, 51.1076312),
+            (17.0994473, 51.1083722),
+        ]
+    )
 
     gdf = gpd.GeoDataFrame({GEOMETRY_COLUMN: [polygon]}, crs=WGS84_CRS)
     return gdf
 
 
 @pytest.fixture  # type: ignore
 def multiple_polygons_overlapping_area_gdf(
@@ -91,27 +95,31 @@
     """Get an example area gdf with two polygons."""
     return pd.concat([first_polygon_area_gdf, second_polygon_area_gdf], axis=0)
 
 
 @pytest.fixture  # type: ignore
 def multipolygons_area_gdf() -> gpd.GeoDataFrame:
     """Get an example area gdf with a multipolygon."""
-    polygon1 = shpg.Polygon([
-        (17.1005309, 51.1100158),
-        (17.1020436, 51.1100427),
-        (17.1021938, 51.1082509),
-        (17.1006274, 51.1081027),
-        (17.1005201, 51.1099956),
-    ])
-    polygon2 = shpg.Polygon([
-        (17.0997584, 51.1049434),
-        (17.0995009, 51.1044112),
-        (17.1003485, 51.1043910),
-        (17.0997584, 51.1049434),
-    ])
+    polygon1 = shpg.Polygon(
+        [
+            (17.1005309, 51.1100158),
+            (17.1020436, 51.1100427),
+            (17.1021938, 51.1082509),
+            (17.1006274, 51.1081027),
+            (17.1005201, 51.1099956),
+        ]
+    )
+    polygon2 = shpg.Polygon(
+        [
+            (17.0997584, 51.1049434),
+            (17.0995009, 51.1044112),
+            (17.1003485, 51.1043910),
+            (17.0997584, 51.1049434),
+        ]
+    )
     multipolygon = shpg.MultiPolygon([polygon1, polygon2])
     return gpd.GeoDataFrame(geometry=[multipolygon], crs=WGS84_CRS)
 
 
 @pytest.fixture  # type: ignore
 def valid_and_empty_polygons_area_gdf(
     first_polygon_area_gdf: gpd.GeoDataFrame, empty_polygon_area_gdf: gpd.GeoDataFrame
```

### Comparing `srai-0.7.1/tests/loaders/test_files/example.parquet` & `srai-0.7.2/tests/loaders/test_files/example.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/test_geoparquet_loader.py` & `srai-0.7.2/tests/loaders/test_geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/loaders/test_gtfs_loader.py` & `srai-0.7.2/tests/loaders/test_gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/miscellaneous/test_optional_dependencies.py` & `srai-0.7.2/tests/miscellaneous/test_optional_dependencies.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/neighbourhoods/h3/test_no_regions.py` & `srai-0.7.2/tests/neighbourhoods/h3/test_no_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/neighbourhoods/h3/test_with_regions.py` & `srai-0.7.2/tests/neighbourhoods/h3/test_with_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/neighbourhoods/test_adjacency_neighbourhood.py` & `srai-0.7.2/tests/neighbourhoods/test_adjacency_neighbourhood.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,33 +93,33 @@
     with pytest.raises(ValueError):
         AdjacencyNeighbourhood(no_geometry_gdf)
 
 
 def test_empty_gdf_empty_set(empty_gdf: gpd.GeoDataFrame) -> None:
     """Test checks if empty GeoDataFrames return empty neighbourhoods."""
     neighbourhood = AdjacencyNeighbourhood(empty_gdf)
-    assert neighbourhood.get_neighbours(1) == set()
+    assert not neighbourhood.get_neighbours(1)
 
 
 def test_empty_gdf_empty_set_include_center(empty_gdf: gpd.GeoDataFrame) -> None:
     """Test checks if empty GeoDataFrames return empty neighbourhoods."""
     neighbourhood = AdjacencyNeighbourhood(empty_gdf, include_center=True)
-    assert neighbourhood.get_neighbours(1) == set()
+    assert not neighbourhood.get_neighbours(1)
 
 
 def test_lazy_loading_empty_set(squares_regions_fixture: gpd.GeoDataFrame) -> None:
     """Test checks if lookup table is empty after init."""
     neighbourhood = AdjacencyNeighbourhood(squares_regions_fixture)
-    assert neighbourhood.lookup == {}
+    assert not neighbourhood.lookup
 
 
 def test_lazy_loading_empty_set_include_center(squares_regions_fixture: gpd.GeoDataFrame) -> None:
     """Test checks if lookup table is empty after init."""
     neighbourhood = AdjacencyNeighbourhood(squares_regions_fixture, include_center=True)
-    assert neighbourhood.lookup == {}
+    assert not neighbourhood.lookup
 
 
 def test_adjacency_lazy_loading(rounded_regions_fixture: gpd.GeoDataFrame) -> None:
     """Test checks if lookup table is lazily populated."""
     neighbourhood = AdjacencyNeighbourhood(rounded_regions_fixture)
     neighbours = neighbourhood.get_neighbours("SW")
     assert neighbours == {"W", "S"}
```

### Comparing `srai-0.7.1/tests/neighbourhoods/test_neighbourhood.py` & `srai-0.7.2/tests/neighbourhoods/test_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/plotting/test_folium_wrapper.py` & `srai-0.7.2/tests/plotting/test_folium_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/regionalizers/conftest.py` & `srai-0.7.2/tests/regionalizers/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,53 +40,61 @@
                 shell=[
                     (-1, 0),
                     (0, 0.5),
                     (1, 0),
                     (1, 1),
                     (0, 1),
                 ],
-                holes=[[
-                    (0.8, 0.9),
-                    (0.9, 0.55),
-                    (0.8, 0.3),
-                    (0.5, 0.4),
-                ]],
+                holes=[
+                    [
+                        (0.8, 0.9),
+                        (0.9, 0.55),
+                        (0.8, 0.3),
+                        (0.5, 0.4),
+                    ]
+                ],
             ),
             geometry.Polygon(shell=[(-0.25, 0), (0.25, 0), (0, 0.2)]),
         ],
         crs=WGS84_CRS,
     )
 
 
 @pytest.fixture  # type: ignore
 def gdf_multipolygon() -> gpd.GeoDataFrame:
     """Get GeoDataFrame with multipolygon."""
     return gpd.GeoDataFrame(
         geometry=[
-            geometry.MultiPolygon([
-                (
-                    [
-                        (-1, 0),
-                        (0, 0.5),
-                        (1, 0),
-                        (1, 1),
-                        (0, 1),
-                    ],
-                    ([[
-                        (0.8, 0.9),
-                        (0.9, 0.55),
-                        (0.8, 0.3),
-                        (0.5, 0.4),
-                    ]]),
-                ),
-                (
-                    [(-0.25, 0), (0.25, 0), (0, 0.2)],
-                    (),
-                ),
-            ])
+            geometry.MultiPolygon(
+                [
+                    (
+                        [
+                            (-1, 0),
+                            (0, 0.5),
+                            (1, 0),
+                            (1, 1),
+                            (0, 1),
+                        ],
+                        (
+                            [
+                                [
+                                    (0.8, 0.9),
+                                    (0.9, 0.55),
+                                    (0.8, 0.3),
+                                    (0.5, 0.4),
+                                ]
+                            ]
+                        ),
+                    ),
+                    (
+                        [(-0.25, 0), (0.25, 0), (0, 0.2)],
+                        (),
+                    ),
+                ]
+            )
         ],
         crs=WGS84_CRS,
     )
 
 
 @pytest.fixture  # type: ignore
 def earth_poles() -> list[geometry.Point]:
```

### Comparing `srai-0.7.1/tests/regionalizers/test_administrative_boundary_regionalizer.py` & `srai-0.7.2/tests/regionalizers/test_administrative_boundary_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/regionalizers/test_h3_regionalizer.py` & `srai-0.7.2/tests/regionalizers/test_h3_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/regionalizers/test_s2_regionalizer.py` & `srai-0.7.2/tests/regionalizers/test_s2_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/regionalizers/test_slippy_map_regionalizer.py` & `srai-0.7.2/tests/regionalizers/test_slippy_map_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/tests/regionalizers/test_voronoi_regionalizer.py` & `srai-0.7.2/tests/regionalizers/test_voronoi_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.1/PKG-INFO` & `srai-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srai
-Version: 0.7.1
+Version: 0.7.2
 Summary: A set of python modules for geospatial machine learning and data mining
 Author-Email: Piotr Gramacki <pgramacki@kraina.ai>, =?utf-8?q?Kacper_Le=C5=9Bniara?= <klesniara@kraina.ai>, Kamil Raczycki <kraczycki@kraina.ai>, =?utf-8?q?Szymon_Wo=C5=BAniak?= <swozniak@kraina.ai>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: GIS
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: srai Version: 0.7.1 Summary: A set of python
+Metadata-Version: 2.1 Name: srai Version: 0.7.2 Summary: A set of python
 modules for geospatial machine learning and data mining Author-Email: Piotr
 Gramacki
 kraina.ai>, =?utf-8?q?Kacper_Le=C5=9Bniara?=
 kraina.ai>, Kamil Raczycki
 kraina.ai>, =?utf-8?q?Szymon_Wo=C5=BAniak?=
 kraina.ai> License: Apache-2.0 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
```

