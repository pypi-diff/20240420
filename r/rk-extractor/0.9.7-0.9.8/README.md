# Comparing `tmp/rk_extractor-0.9.7.tar.gz` & `tmp/rk_extractor-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rk_extractor-0.9.7.tar", last modified: Fri Apr 19 15:40:21 2024, max compression
+gzip compressed data, was "rk_extractor-0.9.8.tar", last modified: Fri Apr 19 16:02:53 2024, max compression
```

## Comparing `rk_extractor-0.9.7.tar` & `rk_extractor-0.9.8.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:21.000000 rk_extractor-0.9.7/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      567 2024-04-19 15:40:21.000000 rk_extractor-0.9.7/PKG-INFO
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     9021 2024-04-18 16:29:41.000000 rk_extractor-0.9.7/README.md
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:18.000000 rk_extractor-0.9.7/scripts/
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:18.000000 rk_extractor-0.9.7/scripts/jobs/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)       35 2024-02-07 17:05:40.000000 rk_extractor-0.9.7/scripts/jobs/README.txt
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        2 2024-04-18 09:46:23.000000 rk_extractor-0.9.7/scripts/jobs/fake.sd
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     5260 2024-04-19 15:16:00.000000 rk_extractor-0.9.7/scripts/jobs/fit_toys
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     4646 2024-01-08 14:38:59.000000 rk_extractor-0.9.7/scripts/jobs/rxe_check
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)      153 2023-11-09 15:10:51.000000 rk_extractor-0.9.7/scripts/jobs/rxe_clean
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     4573 2023-12-22 15:49:05.000000 rk_extractor-0.9.7/scripts/jobs/rxe_download
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     3584 2024-02-07 14:56:43.000000 rk_extractor-0.9.7/scripts/jobs/rxe_grid_jobs
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     1791 2024-01-08 12:36:12.000000 rk_extractor-0.9.7/scripts/jobs/rxe_ihep_check
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     1894 2024-04-19 08:38:56.000000 rk_extractor-0.9.7/scripts/jobs/rxe_ihep_jobs
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     3331 2024-04-18 08:24:23.000000 rk_extractor-0.9.7/scripts/jobs/rxe_local
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)    17088 2024-02-13 18:52:18.000000 rk_extractor-0.9.7/scripts/jobs/rxe_plot_pull
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)    11926 2024-02-08 18:55:36.000000 rk_extractor-0.9.7/scripts/jobs/rxe_plot_syst
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     1353 2024-01-02 11:14:36.000000 rk_extractor-0.9.7/scripts/jobs/rxe_run_check
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     2687 2024-04-18 15:21:05.000000 rk_extractor-0.9.7/scripts/jobs/rxe_run_toys
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     7350 2024-04-19 15:40:03.000000 rk_extractor-0.9.7/scripts/jobs/rxe_toys
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:18.000000 rk_extractor-0.9.7/scripts/offline/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     5402 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/scripts/offline/analyze_result
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1647 2024-03-11 16:13:59.000000 rk_extractor-0.9.7/scripts/offline/brf_tables
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1297 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/scripts/offline/calculate_sigeff
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8172 2024-04-15 13:59:38.000000 rk_extractor-0.9.7/scripts/offline/check_dist
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     4570 2024-03-11 16:13:59.000000 rk_extractor-0.9.7/scripts/offline/check_jpsi_misid
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     4119 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/scripts/offline/cmb_prec_norm
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     3690 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/scripts/offline/make_signal_table
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     4102 2024-03-11 16:13:59.000000 rk_extractor-0.9.7/scripts/offline/make_yields_table
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     5080 2024-01-15 21:50:12.000000 rk_extractor-0.9.7/scripts/offline/plot_check
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     3020 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/scripts/offline/rare_bkg_eff
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     4836 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/scripts/offline/sbfit_analyze
--rw-r--r--   0 campoverde (12477) lhcb      (1026)       38 2024-04-19 15:40:21.000000 rk_extractor-0.9.7/setup.cfg
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1539 2024-04-19 15:40:11.000000 rk_extractor-0.9.7/setup.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:18.000000 rk_extractor-0.9.7/src/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-16 17:02:20.000000 rk_extractor-0.9.7/src/__init__.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     7529 2024-02-07 14:42:07.000000 rk_extractor-0.9.7/src/bdt_scale.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     3662 2023-12-31 20:05:12.000000 rk_extractor-0.9.7/src/cmb_ck.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     9085 2023-11-26 15:18:19.000000 rk_extractor-0.9.7/src/cs_reader.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    22377 2024-04-18 15:50:35.000000 rk_extractor-0.9.7/src/extractor.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:18.000000 rk_extractor-0.9.7/src/extractor_data/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-16 17:02:20.000000 rk_extractor-0.9.7/src/extractor_data/__init__.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:18.000000 rk_extractor-0.9.7/src/extractor_data/bdt_eff/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/bdt_eff/__init__.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:18.000000 rk_extractor-0.9.7/src/extractor_data/config/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/config/__init__.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      122 2024-04-15 14:03:50.000000 rk_extractor-0.9.7/src/extractor_data/config/v1.toml
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      156 2024-02-07 17:03:26.000000 rk_extractor-0.9.7/src/extractor_data/config/v2.toml
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      768 2024-04-18 15:09:39.000000 rk_extractor-0.9.7/src/extractor_data/config/v3.toml
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:18.000000 rk_extractor-0.9.7/src/extractor_data/npr_data/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/npr_data/__init__.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      750 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1486 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     2142 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     2142 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     2137 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     2137 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      564 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1126 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2024-01-15 21:50:12.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/__init__.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v1/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8708 2024-01-15 21:50:12.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v1/eff_real.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      299 2024-01-15 21:50:12.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v1/fr_bf.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v2/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8708 2024-01-15 21:50:12.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v2/eff_real.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-15 21:50:12.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v2/fr_bf.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v3/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8685 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v3/eff_real.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v3/fr_bf.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v4/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8656 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v4/eff_real.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v4/fr_bf.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v5/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8656 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v5/eff_real.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/src/extractor_data/rare_sf/v5/fr_bf.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/__init__.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/2017_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/2017_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      263 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/2017_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      349 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/2018_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/2018_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      267 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/2018_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      349 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/all_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      265 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/all_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      342 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/r1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      346 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/r1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      261 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/r1_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/r2p1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/r2p1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      264 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v1/r2p1_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v10/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      377 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v10/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v10/all_GTIS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v11/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      381 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v11/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v12/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      378 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v12/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v13/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v13/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v14/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      374 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v14/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v15/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      377 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v15/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v16/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      379 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v16/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v17/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v17/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v18/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      721 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v18/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v19/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1585 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v19/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v2/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      174 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v2/2017_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      176 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v2/2018_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      172 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v2/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      170 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v2/r1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      175 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v2/r2p1_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v20/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      436 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v20/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v21/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v21/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v22/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      431 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v22/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v23/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      436 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v23/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v24/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v24/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v25/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1013 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v25/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v26/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      799 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v26/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v27/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1009 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v27/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v28/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1008 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v28/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v29/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v29/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v3/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v3/2017_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      354 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v3/2018_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v3/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      344 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v3/r1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v3/r2p1_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v30/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v30/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:19.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v31/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      433 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v31/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v32/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v32/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v33/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      384 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v33/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v34/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1011 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v34/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v35/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1021 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v35/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v36/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      807 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v36/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v37/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1190 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v37/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v38/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1187 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v38/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v39/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1494 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v39/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/2017_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/2017_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      263 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/2017_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/2018_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      354 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/2018_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      267 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/2018_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/all_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      265 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/all_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      342 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/r1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      343 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/r1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      261 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/r1_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/r2p1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/r2p1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      264 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v4/r2p1_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v40/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1494 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v40/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v41/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1499 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v41/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v42/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1596 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v42/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v43/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1595 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v43/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v44/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1921 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v44/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      283 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v44/all_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v45/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      384 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v45/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v46/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      433 2024-03-11 16:13:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v46/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      292 2024-03-11 16:13:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v46/all_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/2017_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/2017_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      266 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/2017_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      355 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/2018_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/2018_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      267 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/2018_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      349 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/all_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      261 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/all_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      344 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/r1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      343 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/r1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      260 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/r1_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/r2p1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/r2p1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      266 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v5/r2p1_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v6/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      264 2023-12-28 12:06:32.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v6/all_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v7/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      374 2023-12-31 20:05:12.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v7/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      380 2023-12-31 20:05:12.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v7/all_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      281 2023-12-31 20:05:12.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v7/all_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v8/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-01-15 21:50:12.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v8/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      378 2024-01-15 21:50:12.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v8/all_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      283 2024-01-15 21:50:12.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v8/all_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:20.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v9/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-01-16 12:05:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v9/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      378 2024-01-16 12:05:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v9/all_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      283 2024-01-16 12:05:27.000000 rk_extractor-0.9.7/src/extractor_data/sb_fits/v9/all_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:18.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:21.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      530 2024-02-07 14:42:09.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      529 2024-02-07 14:42:09.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      700 2024-02-07 14:42:09.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      530 2024-02-07 14:42:09.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      182 2024-03-11 16:13:59.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_GTIS_2017.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      181 2024-03-11 16:13:59.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_GTIS_2018.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      184 2024-03-11 16:13:59.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_GTIS_r1.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      182 2024-03-11 16:13:59.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_GTIS_r2p1.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      528 2024-02-07 14:42:09.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      528 2024-02-07 14:42:09.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1441 2024-02-07 14:42:09.000000 rk_extractor-0.9.7/src/extset.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     7485 2023-11-27 10:58:34.000000 rk_extractor-0.9.7/src/mc_reader.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     6270 2024-03-11 16:13:59.000000 rk_extractor-0.9.7/src/model_manager.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    12164 2024-03-11 16:13:59.000000 rk_extractor-0.9.7/src/normalizer.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8193 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/np_reader.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:21.000000 rk_extractor-0.9.7/src/rk_extractor.egg-info/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      567 2024-04-19 15:40:16.000000 rk_extractor-0.9.7/src/rk_extractor.egg-info/PKG-INFO
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8004 2024-04-19 15:40:17.000000 rk_extractor-0.9.7/src/rk_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        1 2024-04-19 15:40:16.000000 rk_extractor-0.9.7/src/rk_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      205 2024-04-19 15:40:16.000000 rk_extractor-0.9.7/src/rk_extractor.egg-info/requires.txt
--rw-r--r--   0 campoverde (12477) lhcb      (1026)       16 2024-04-19 15:40:16.000000 rk_extractor-0.9.7/src/rk_extractor.egg-info/top_level.txt
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    18432 2024-04-19 13:19:57.000000 rk_extractor-0.9.7/src/rk_model.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    18032 2024-04-18 15:19:15.000000 rk_extractor-0.9.7/src/rkex_model.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    13795 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/src/scales.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 15:40:21.000000 rk_extractor-0.9.7/tests/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      774 2023-12-31 20:05:12.000000 rk_extractor-0.9.7/tests/test_cmb_eff.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      627 2023-11-30 15:15:15.000000 rk_extractor-0.9.7/tests/test_cs_reader.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      675 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/tests/test_effcalc.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    18502 2024-03-11 16:13:59.000000 rk_extractor-0.9.7/tests/test_extractor.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1167 2023-11-27 10:46:34.000000 rk_extractor-0.9.7/tests/test_mc_reader.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     4786 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/tests/test_model_analyzer.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     4615 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/tests/test_model_manager.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     5005 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/tests/test_normalizer.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      611 2024-02-06 13:59:27.000000 rk_extractor-0.9.7/tests/test_np_reader.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    10316 2024-04-16 12:43:12.000000 rk_extractor-0.9.7/tests/test_rkmodel.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     6686 2024-04-15 13:59:38.000000 rk_extractor-0.9.7/tests/test_rkrx_model.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1992 2024-01-30 14:14:06.000000 rk_extractor-0.9.7/tests/test_scales.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2023-12-25 18:44:59.000000 rk_extractor-0.9.7/tests/test_scl_mkr.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1652 2024-02-07 14:42:09.000000 rk_extractor-0.9.7/tests/test_scl_rdr.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:53.000000 rk_extractor-0.9.8/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      567 2024-04-19 16:02:53.000000 rk_extractor-0.9.8/PKG-INFO
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     9021 2024-04-18 16:29:41.000000 rk_extractor-0.9.8/README.md
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:50.000000 rk_extractor-0.9.8/scripts/
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:50.000000 rk_extractor-0.9.8/scripts/jobs/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)       35 2024-02-07 17:05:40.000000 rk_extractor-0.9.8/scripts/jobs/README.txt
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        2 2024-04-18 09:46:23.000000 rk_extractor-0.9.8/scripts/jobs/fake.sd
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     5261 2024-04-19 15:59:41.000000 rk_extractor-0.9.8/scripts/jobs/fit_toys
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     4646 2024-01-08 14:38:59.000000 rk_extractor-0.9.8/scripts/jobs/rxe_check
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)      153 2023-11-09 15:10:51.000000 rk_extractor-0.9.8/scripts/jobs/rxe_clean
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     4573 2023-12-22 15:49:05.000000 rk_extractor-0.9.8/scripts/jobs/rxe_download
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     3584 2024-02-07 14:56:43.000000 rk_extractor-0.9.8/scripts/jobs/rxe_grid_jobs
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     1791 2024-01-08 12:36:12.000000 rk_extractor-0.9.8/scripts/jobs/rxe_ihep_check
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     1894 2024-04-19 08:38:56.000000 rk_extractor-0.9.8/scripts/jobs/rxe_ihep_jobs
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     3331 2024-04-18 08:24:23.000000 rk_extractor-0.9.8/scripts/jobs/rxe_local
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)    17088 2024-02-13 18:52:18.000000 rk_extractor-0.9.8/scripts/jobs/rxe_plot_pull
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)    11926 2024-02-08 18:55:36.000000 rk_extractor-0.9.8/scripts/jobs/rxe_plot_syst
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     1353 2024-01-02 11:14:36.000000 rk_extractor-0.9.8/scripts/jobs/rxe_run_check
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     2687 2024-04-18 15:21:05.000000 rk_extractor-0.9.8/scripts/jobs/rxe_run_toys
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     7350 2024-04-19 15:40:03.000000 rk_extractor-0.9.8/scripts/jobs/rxe_toys
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/scripts/offline/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     5402 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/scripts/offline/analyze_result
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1647 2024-03-11 16:13:59.000000 rk_extractor-0.9.8/scripts/offline/brf_tables
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1297 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/scripts/offline/calculate_sigeff
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8172 2024-04-15 13:59:38.000000 rk_extractor-0.9.8/scripts/offline/check_dist
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     4570 2024-03-11 16:13:59.000000 rk_extractor-0.9.8/scripts/offline/check_jpsi_misid
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     4119 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/scripts/offline/cmb_prec_norm
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     3690 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/scripts/offline/make_signal_table
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     4102 2024-03-11 16:13:59.000000 rk_extractor-0.9.8/scripts/offline/make_yields_table
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     5080 2024-01-15 21:50:12.000000 rk_extractor-0.9.8/scripts/offline/plot_check
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     3020 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/scripts/offline/rare_bkg_eff
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     4836 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/scripts/offline/sbfit_analyze
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)       38 2024-04-19 16:02:53.000000 rk_extractor-0.9.8/setup.cfg
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1539 2024-04-19 15:59:55.000000 rk_extractor-0.9.8/setup.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-16 17:02:20.000000 rk_extractor-0.9.8/src/__init__.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     7529 2024-02-07 14:42:07.000000 rk_extractor-0.9.8/src/bdt_scale.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     3662 2023-12-31 20:05:12.000000 rk_extractor-0.9.8/src/cmb_ck.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     9085 2023-11-26 15:18:19.000000 rk_extractor-0.9.8/src/cs_reader.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    22377 2024-04-18 15:50:35.000000 rk_extractor-0.9.8/src/extractor.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-16 17:02:20.000000 rk_extractor-0.9.8/src/extractor_data/__init__.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/bdt_eff/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/bdt_eff/__init__.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/config/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/config/__init__.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      122 2024-04-15 14:03:50.000000 rk_extractor-0.9.8/src/extractor_data/config/v1.toml
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      156 2024-02-07 17:03:26.000000 rk_extractor-0.9.8/src/extractor_data/config/v2.toml
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      768 2024-04-18 15:09:39.000000 rk_extractor-0.9.8/src/extractor_data/config/v3.toml
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/npr_data/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/npr_data/__init__.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      750 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1486 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     2142 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     2142 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     2137 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     2137 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      564 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1126 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2024-01-15 21:50:12.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/__init__.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v1/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8708 2024-01-15 21:50:12.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v1/eff_real.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      299 2024-01-15 21:50:12.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v1/fr_bf.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v2/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8708 2024-01-15 21:50:12.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v2/eff_real.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-15 21:50:12.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v2/fr_bf.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v3/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8685 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v3/eff_real.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v3/fr_bf.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v4/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8656 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v4/eff_real.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v4/fr_bf.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v5/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8656 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v5/eff_real.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/src/extractor_data/rare_sf/v5/fr_bf.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/__init__.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/2017_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/2017_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      263 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/2017_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      349 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/2018_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/2018_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      267 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/2018_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      349 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/all_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      265 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/all_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      342 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/r1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      346 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/r1_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      261 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/r1_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/r2p1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/r2p1_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      264 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v1/r2p1_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v10/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      377 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v10/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v10/all_GTIS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v11/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      381 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v11/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v12/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      378 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v12/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v13/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v13/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v14/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      374 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v14/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v15/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      377 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v15/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v16/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      379 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v16/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v17/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v17/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:51.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v18/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      721 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v18/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v19/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1585 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v19/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v2/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      174 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v2/2017_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      176 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v2/2018_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      172 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v2/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      170 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v2/r1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      175 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v2/r2p1_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v20/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      436 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v20/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v21/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v21/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v22/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      431 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v22/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v23/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      436 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v23/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v24/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v24/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v25/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1013 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v25/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v26/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      799 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v26/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v27/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1009 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v27/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v28/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1008 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v28/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v29/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v29/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v3/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v3/2017_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      354 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v3/2018_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v3/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      344 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v3/r1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v3/r2p1_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v30/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v30/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v31/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      433 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v31/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v32/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v32/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v33/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      384 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v33/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v34/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1011 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v34/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v35/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1021 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v35/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v36/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      807 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v36/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v37/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1190 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v37/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v38/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1187 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v38/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v39/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1494 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v39/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/2017_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/2017_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      263 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/2017_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/2018_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      354 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/2018_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      267 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/2018_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/all_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      265 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/all_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      342 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/r1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      343 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/r1_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      261 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/r1_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/r2p1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/r2p1_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      264 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v4/r2p1_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v40/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1494 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v40/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v41/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1499 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v41/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v42/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1596 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v42/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v43/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1595 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v43/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v44/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1921 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v44/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      283 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v44/all_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v45/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      384 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v45/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:52.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v46/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      433 2024-03-11 16:13:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v46/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      292 2024-03-11 16:13:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v46/all_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:53.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/2017_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/2017_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      266 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/2017_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      355 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/2018_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/2018_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      267 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/2018_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      349 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/all_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      261 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/all_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      344 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/r1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      343 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/r1_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      260 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/r1_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/r2p1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/r2p1_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      266 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v5/r2p1_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:53.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v6/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      264 2023-12-28 12:06:32.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v6/all_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:53.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v7/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      374 2023-12-31 20:05:12.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v7/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      380 2023-12-31 20:05:12.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v7/all_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      281 2023-12-31 20:05:12.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v7/all_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:53.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v8/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-01-15 21:50:12.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v8/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      378 2024-01-15 21:50:12.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v8/all_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      283 2024-01-15 21:50:12.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v8/all_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:53.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v9/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-01-16 12:05:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v9/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      378 2024-01-16 12:05:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v9/all_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      283 2024-01-16 12:05:27.000000 rk_extractor-0.9.8/src/extractor_data/sb_fits/v9/all_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:50.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:53.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      530 2024-02-07 14:42:09.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      529 2024-02-07 14:42:09.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      700 2024-02-07 14:42:09.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      530 2024-02-07 14:42:09.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      182 2024-03-11 16:13:59.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_GTIS_2017.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      181 2024-03-11 16:13:59.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_GTIS_2018.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      184 2024-03-11 16:13:59.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_GTIS_r1.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      182 2024-03-11 16:13:59.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_GTIS_r2p1.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      528 2024-02-07 14:42:09.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      528 2024-02-07 14:42:09.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1441 2024-02-07 14:42:09.000000 rk_extractor-0.9.8/src/extset.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     7485 2023-11-27 10:58:34.000000 rk_extractor-0.9.8/src/mc_reader.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     6270 2024-03-11 16:13:59.000000 rk_extractor-0.9.8/src/model_manager.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    12164 2024-03-11 16:13:59.000000 rk_extractor-0.9.8/src/normalizer.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8193 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/np_reader.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:53.000000 rk_extractor-0.9.8/src/rk_extractor.egg-info/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      567 2024-04-19 16:02:49.000000 rk_extractor-0.9.8/src/rk_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8004 2024-04-19 16:02:50.000000 rk_extractor-0.9.8/src/rk_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        1 2024-04-19 16:02:49.000000 rk_extractor-0.9.8/src/rk_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      205 2024-04-19 16:02:49.000000 rk_extractor-0.9.8/src/rk_extractor.egg-info/requires.txt
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)       16 2024-04-19 16:02:49.000000 rk_extractor-0.9.8/src/rk_extractor.egg-info/top_level.txt
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    18432 2024-04-19 13:19:57.000000 rk_extractor-0.9.8/src/rk_model.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    18032 2024-04-18 15:19:15.000000 rk_extractor-0.9.8/src/rkex_model.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    13795 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/src/scales.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 16:02:53.000000 rk_extractor-0.9.8/tests/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      774 2023-12-31 20:05:12.000000 rk_extractor-0.9.8/tests/test_cmb_eff.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      627 2023-11-30 15:15:15.000000 rk_extractor-0.9.8/tests/test_cs_reader.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      675 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/tests/test_effcalc.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    18502 2024-03-11 16:13:59.000000 rk_extractor-0.9.8/tests/test_extractor.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1167 2023-11-27 10:46:34.000000 rk_extractor-0.9.8/tests/test_mc_reader.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     4786 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/tests/test_model_analyzer.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     4615 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/tests/test_model_manager.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     5005 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/tests/test_normalizer.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      611 2024-02-06 13:59:27.000000 rk_extractor-0.9.8/tests/test_np_reader.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    10316 2024-04-16 12:43:12.000000 rk_extractor-0.9.8/tests/test_rkmodel.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     6686 2024-04-15 13:59:38.000000 rk_extractor-0.9.8/tests/test_rkrx_model.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1992 2024-01-30 14:14:06.000000 rk_extractor-0.9.8/tests/test_scales.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2023-12-25 18:44:59.000000 rk_extractor-0.9.8/tests/test_scl_mkr.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1652 2024-02-07 14:42:09.000000 rk_extractor-0.9.8/tests/test_scl_rdr.py
```

### Comparing `rk_extractor-0.9.7/PKG-INFO` & `rk_extractor-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rk_extractor
-Version: 0.9.7
+Version: 0.9.8
 Summary: Used to extract RK from simultaneous fits
 Requires-Dist: numpy
 Requires-Dist: toml
 Requires-Dist: matplotlib
 Requires-Dist: logzero
 Requires-Dist: attrs
 Requires-Dist: jacobi
```

### Comparing `rk_extractor-0.9.7/README.md` & `rk_extractor-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/jobs/fit_toys` & `rk_extractor-0.9.8/scripts/jobs/fit_toys`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     p_seed = f'{rseed:04}'
     
     if l_fix_var is None:
         nfixvar = 0
     else:
         nfixvar= len(l_fix_var)
 
-    p_fvar = '{nfixvar:04}' 
+    p_fvar = f'{nfixvar:04}' 
 
     if mod_var is None:
         p_mvar = 'nominal'
     else:
         p_mvar = mod_var
 
     return f'{p_seed}_{p_fvar}_{p_mvar}'
```

### Comparing `rk_extractor-0.9.7/scripts/jobs/rxe_check` & `rk_extractor-0.9.8/scripts/jobs/rxe_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/jobs/rxe_download` & `rk_extractor-0.9.8/scripts/jobs/rxe_download`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/jobs/rxe_grid_jobs` & `rk_extractor-0.9.8/scripts/jobs/rxe_grid_jobs`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/jobs/rxe_ihep_check` & `rk_extractor-0.9.8/scripts/jobs/rxe_ihep_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/jobs/rxe_ihep_jobs` & `rk_extractor-0.9.8/scripts/jobs/rxe_ihep_jobs`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/jobs/rxe_local` & `rk_extractor-0.9.8/scripts/jobs/rxe_local`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/jobs/rxe_plot_pull` & `rk_extractor-0.9.8/scripts/jobs/rxe_plot_pull`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/jobs/rxe_plot_syst` & `rk_extractor-0.9.8/scripts/jobs/rxe_plot_syst`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/jobs/rxe_run_check` & `rk_extractor-0.9.8/scripts/jobs/rxe_run_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/jobs/rxe_run_toys` & `rk_extractor-0.9.8/scripts/jobs/rxe_run_toys`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/jobs/rxe_toys` & `rk_extractor-0.9.8/scripts/jobs/rxe_toys`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/offline/analyze_result` & `rk_extractor-0.9.8/scripts/offline/analyze_result`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/offline/brf_tables` & `rk_extractor-0.9.8/scripts/offline/brf_tables`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/offline/calculate_sigeff` & `rk_extractor-0.9.8/scripts/offline/calculate_sigeff`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/offline/check_dist` & `rk_extractor-0.9.8/scripts/offline/check_dist`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/offline/check_jpsi_misid` & `rk_extractor-0.9.8/scripts/offline/check_jpsi_misid`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/offline/cmb_prec_norm` & `rk_extractor-0.9.8/scripts/offline/cmb_prec_norm`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/offline/make_signal_table` & `rk_extractor-0.9.8/scripts/offline/make_signal_table`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/offline/make_yields_table` & `rk_extractor-0.9.8/scripts/offline/make_yields_table`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/offline/plot_check` & `rk_extractor-0.9.8/scripts/offline/plot_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/offline/rare_bkg_eff` & `rk_extractor-0.9.8/scripts/offline/rare_bkg_eff`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/scripts/offline/sbfit_analyze` & `rk_extractor-0.9.8/scripts/offline/sbfit_analyze`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/setup.py` & `rk_extractor-0.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     else:
         raise
 
     return l_pkg
 #----------------------------------------------
 setup(
         name              = 'rk_extractor',
-        version           = '0.9.7',
+        version           = '0.9.8',
         description       = 'Used to extract RK from simultaneous fits',
         scripts           = get_scripts('scripts/jobs') + get_scripts('scripts/offline'),
         long_description  = '',
         packages          = get_packages(),
         package_dir       = {'' : 'src'},
         package_data      = {'extractor_data' : get_data_packages('extractor_data')}, 
         install_requires  = open('requirements.txt').read().splitlines()
```

### Comparing `rk_extractor-0.9.7/src/bdt_scale.py` & `rk_extractor-0.9.8/src/bdt_scale.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/cmb_ck.py` & `rk_extractor-0.9.8/src/cmb_ck.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/cs_reader.py` & `rk_extractor-0.9.8/src/cs_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor.py` & `rk_extractor-0.9.8/src/extractor.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/config/v3.toml` & `rk_extractor-0.9.8/src/extractor_data/config/v3.toml`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json` & `rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json` & `rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json` & `rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json` & `rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json` & `rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json` & `rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json` & `rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json` & `rk_extractor-0.9.8/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/rare_sf/v1/eff_real.json` & `rk_extractor-0.9.8/src/extractor_data/rare_sf/v1/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/rare_sf/v2/eff_real.json` & `rk_extractor-0.9.8/src/extractor_data/rare_sf/v2/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/rare_sf/v3/eff_real.json` & `rk_extractor-0.9.8/src/extractor_data/rare_sf/v3/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/rare_sf/v4/eff_real.json` & `rk_extractor-0.9.8/src/extractor_data/rare_sf/v4/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/rare_sf/v5/eff_real.json` & `rk_extractor-0.9.8/src/extractor_data/rare_sf/v5/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v18/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v18/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v19/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v19/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v25/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v25/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v26/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v26/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v27/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v27/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v28/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v28/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v34/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v34/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v35/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v35/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v36/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v36/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v37/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v37/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v38/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v38/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v39/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v39/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v40/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v40/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v41/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v41/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v42/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v42/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v43/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v43/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sb_fits/v44/all_ETOS.json` & `rk_extractor-0.9.8/src/extractor_data/sb_fits/v44/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json` & `rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json` & `rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json` & `rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json` & `rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json` & `rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json` & `rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json` & `rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json` & `rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json` & `rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json` & `rk_extractor-0.9.8/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/extset.py` & `rk_extractor-0.9.8/src/extset.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/mc_reader.py` & `rk_extractor-0.9.8/src/mc_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/model_manager.py` & `rk_extractor-0.9.8/src/model_manager.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/normalizer.py` & `rk_extractor-0.9.8/src/normalizer.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/np_reader.py` & `rk_extractor-0.9.8/src/np_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/rk_extractor.egg-info/PKG-INFO` & `rk_extractor-0.9.8/src/rk_extractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rk_extractor
-Version: 0.9.7
+Version: 0.9.8
 Summary: Used to extract RK from simultaneous fits
 Requires-Dist: numpy
 Requires-Dist: toml
 Requires-Dist: matplotlib
 Requires-Dist: logzero
 Requires-Dist: attrs
 Requires-Dist: jacobi
```

### Comparing `rk_extractor-0.9.7/src/rk_extractor.egg-info/SOURCES.txt` & `rk_extractor-0.9.8/src/rk_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/rk_model.py` & `rk_extractor-0.9.8/src/rk_model.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/rkex_model.py` & `rk_extractor-0.9.8/src/rkex_model.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/src/scales.py` & `rk_extractor-0.9.8/src/scales.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_cmb_eff.py` & `rk_extractor-0.9.8/tests/test_cmb_eff.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_cs_reader.py` & `rk_extractor-0.9.8/tests/test_cs_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_effcalc.py` & `rk_extractor-0.9.8/tests/test_effcalc.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_extractor.py` & `rk_extractor-0.9.8/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_mc_reader.py` & `rk_extractor-0.9.8/tests/test_mc_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_model_analyzer.py` & `rk_extractor-0.9.8/tests/test_model_analyzer.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_model_manager.py` & `rk_extractor-0.9.8/tests/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_normalizer.py` & `rk_extractor-0.9.8/tests/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_np_reader.py` & `rk_extractor-0.9.8/tests/test_np_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_rkmodel.py` & `rk_extractor-0.9.8/tests/test_rkmodel.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_rkrx_model.py` & `rk_extractor-0.9.8/tests/test_rkrx_model.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_scales.py` & `rk_extractor-0.9.8/tests/test_scales.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_scl_mkr.py` & `rk_extractor-0.9.8/tests/test_scl_mkr.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.7/tests/test_scl_rdr.py` & `rk_extractor-0.9.8/tests/test_scl_rdr.py`

 * *Files identical despite different names*

