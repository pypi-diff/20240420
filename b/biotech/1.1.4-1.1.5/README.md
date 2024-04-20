# Comparing `tmp/biotech-1.1.4.tar.gz` & `tmp/biotech-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotech-1.1.4.tar", max compression
+gzip compressed data, was "biotech-1.1.5.tar", max compression
```

## Comparing `biotech-1.1.4.tar` & `biotech-1.1.5.tar`

### file list

```diff
@@ -1,761 +1,739 @@
--rwxr-xr-x   0        0        0      211 2024-04-16 02:07:59.993436 biotech-1.1.4/license.S.HTML
--rwxr-xr-x   0        0        0     1145 2024-04-19 23:43:10.476201 biotech-1.1.4/pyproject.toml
--rwxr-xr-x   0        0        0     3866 2024-04-16 20:53:30.034757 biotech-1.1.4/readme.md
--rwxr-xr-x   0        0        0     2331 2024-04-19 15:34:34.407444 biotech-1.1.4/venue.S.HTML
--rwxr-xr-x   0        0        0   838272 2024-04-16 02:03:26.700967 biotech-1.1.4/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
--rwxr-xr-x   0        0        0     1270 2024-04-17 22:22:59.944800 biotech-1.1.4/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
--rwxr-xr-x   0        0        0     4079 2024-04-16 20:48:34.871383 biotech-1.1.4/venues/stages/biotech/___itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0      645 2024-04-16 20:48:34.875383 biotech-1.1.4/venues/stages/biotech/___itinerary/maybes.s.HTML
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout/script.py
--rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout/start.py
--rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
--rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
--rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
--rwxr-xr-x   0        0        0      385 2024-04-17 18:49:44.656786 biotech-1.1.4/venues/stages/biotech/__glossary/biotech_1
--rwxr-xr-x   0        0        0      114 2024-04-17 18:45:06.744254 biotech-1.1.4/venues/stages/biotech/__glossary/glossary.S.HTML
--rwxr-xr-x   0        0        0      130 2024-04-19 16:49:02.311131 biotech-1.1.4/venues/stages/biotech/__init__.py
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 biotech-1.1.4/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0     1252 2024-04-16 20:48:34.867383 biotech-1.1.4/venues/stages/biotech/_book/advanced tutorial.s.HTML
--rwxr-xr-x   0        0        0     1786 2024-04-16 20:48:34.867383 biotech-1.1.4/venues/stages/biotech/_book/book.s.HTML
--rwxr-xr-x   0        0        0      542 2024-04-16 20:48:34.867383 biotech-1.1.4/venues/stages/biotech/_book/relevant.s.HTML
--rwxr-xr-x   0        0        0     2129 2024-04-17 19:24:51.191926 biotech-1.1.4/venues/stages/biotech/_clique/__init__.py
--rwxr-xr-x   0        0        0     2493 2024-04-17 19:24:52.839918 biotech-1.1.4/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 biotech-1.1.4/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 biotech-1.1.4/venues/stages/biotech/_clique/group/__init__.py
--rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 biotech-1.1.4/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 biotech-1.1.4/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0  1411387 2024-04-19 23:40:10.090237 biotech-1.1.4/venues/stages/biotech/_status/DB/records.json
--rw-r--r--   0        0        0     1172 2024-04-19 22:15:38.920875 biotech-1.1.4/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
--rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 biotech-1.1.4/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
--rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 biotech-1.1.4/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
--rwxr-xr-x   0        0        0     1487 2024-04-19 22:15:36.412903 biotech-1.1.4/venues/stages/biotech/_status/establish.py
--rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416142 biotech-1.1.4/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 biotech-1.1.4/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      720 2024-04-16 20:48:34.887383 biotech-1.1.4/venues/stages/biotech/_status/monitors/-01_start/status_1.py
--rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 biotech-1.1.4/venues/stages/biotech/_status/monitors/00_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 biotech-1.1.4/venues/stages/biotech/_status/monitors/00_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      793 2024-04-16 20:48:34.883383 biotech-1.1.4/venues/stages/biotech/_status/monitors/00_start/status_1.py
--rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708148 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/path_1_health.py
--rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/path_2_health.py
--rwxr-xr-x   0        0        0     1161 2024-04-16 20:48:34.903383 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/status_1.py
--rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/1_health.py
--rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/2_health.py
--rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/modules/MODULE_1.py
--rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1214 2024-04-16 20:48:34.899383 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/status_1.py
--rwxr-xr-x   0        0        0      794 2024-04-16 20:48:34.891383 biotech-1.1.4/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py
--rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 biotech-1.1.4/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 biotech-1.1.4/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      939 2024-04-16 20:48:34.887383 biotech-1.1.4/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py
--rwxr-xr-x   0        0        0      289 2024-04-16 00:28:17.871373 biotech-1.1.4/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      517 2024-04-16 00:32:46.948536 biotech-1.1.4/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      942 2024-04-16 20:48:34.883383 biotech-1.1.4/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py
--rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py
--rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      867 2024-04-16 20:48:34.891383 biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/status_1.py
--rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/stasis/1_health.py
--rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/stasis/2_health.py
--rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/stasis/3_health.py
--rw-r--r--   0        0        0     1036 2024-04-19 19:54:47.501752 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/1_health.cpython-310.pyc
--rw-r--r--   0        0        0      183 2024-04-19 19:54:47.501752 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/2_health.cpython-310.pyc
--rw-r--r--   0        0        0      169 2024-04-19 19:54:47.505751 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/3_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      955 2024-04-19 22:40:42.880411 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/status_1.py
--rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 biotech-1.1.4/venues/stages/biotech/_status/monitors/07/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 biotech-1.1.4/venues/stages/biotech/_status/monitors/07/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0      809 2024-04-16 20:48:34.907383 biotech-1.1.4/venues/stages/biotech/_status/monitors/07/status_1.py
--rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 biotech-1.1.4/venues/stages/biotech/_status/monitors/08_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 biotech-1.1.4/venues/stages/biotech/_status/monitors/08_DB/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0     1561 2024-04-19 19:13:07.956368 biotech-1.1.4/venues/stages/biotech/_status/monitors/08_DB/status_1.py
--rwxr-xr-x   0        0        0    98385 2024-04-19 23:39:44.894524 biotech-1.1.4/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_2.py
--rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_3.py
--rwxr-xr-x   0        0        0     1442 2024-04-19 22:43:25.306602 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py
--rwxr-xr-x   0        0        0      367 2024-04-16 03:23:58.043895 biotech-1.1.4/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 biotech-1.1.4/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1189 2024-04-19 21:55:08.998787 biotech-1.1.4/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
--rw-r--r--   0        0        0      316 2024-04-19 18:57:32.516036 biotech-1.1.4/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       77 2024-04-19 18:57:24.196146 biotech-1.1.4/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1250 2024-04-19 21:55:16.358703 biotech-1.1.4/venues/stages/biotech/_status/monitors/11/status_1.py
--rwxr-xr-x   0        0        0      984 2024-04-18 03:32:30.971629 biotech-1.1.4/venues/stages/biotech/_status/status.proc.py
--rwxr-xr-x   0        0        0      256 2024-04-16 20:48:34.875383 biotech-1.1.4/venues/stages/biotech/_status/status.s.HTML
--rwxr-xr-x   0        0        0     1483 2024-04-16 20:48:34.851384 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
--rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
--rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
--rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 biotech-1.1.4/venues/stages/biotech/_status_advanced/status.proc.py
--rwxr-xr-x   0        0        0     1779 2024-04-16 20:48:34.575388 biotech-1.1.4/venues/stages/biotech/architecture.s.HTML
--rwxr-xr-x   0        0        0      241 2024-04-16 20:53:18.546926 biotech-1.1.4/venues/stages/biotech/emojis.S.HTML
--rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 biotech-1.1.4/venues/stages/biotech/license.S.HTML
--rwxr-xr-x   0        0        0     3068 2024-04-16 20:48:34.543389 biotech-1.1.4/venues/stages/biotech/module.s.HTML
--rw-r--r--   0        0        0     1596 2024-04-19 21:12:05.931720 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      640 2024-04-19 16:26:52.595637 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      259 2024-04-19 16:20:24.028904 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
--rwxr-xr-x   0        0        0     1478 2024-04-19 21:11:18.368263 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.648116 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/paths.py
--rwxr-xr-x   0        0        0      666 2024-04-19 21:46:15.516790 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
--rwxr-xr-x   0        0        0      562 2024-04-17 21:48:05.111704 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
--rwxr-xr-x   0        0        0     1163 2024-04-17 21:49:49.362841 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3193 2024-04-19 23:42:26.432696 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
--rw-r--r--   0        0        0     3137 2024-04-19 23:42:29.804658 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      999 2024-04-19 20:57:55.937395 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0     2881 2024-04-19 21:20:39.102102 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
--rw-r--r--   0        0        0     1152 2024-04-19 21:06:40.923425 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      653 2024-04-19 20:56:23.606442 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
--rwxr-xr-x   0        0        0     3572 2024-04-19 21:20:33.674162 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
--rwxr-xr-x   0        0        0      769 2024-04-19 21:06:33.619508 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
--rw-r--r--   0        0        0     2031 2024-04-19 23:33:27.678892 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
--rw-r--r--   0        0        0     2159 2024-04-19 23:33:27.678892 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      420 2024-04-19 23:33:27.678892 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
--rw-r--r--   0        0        0      728 2024-04-19 23:33:27.682892 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
--rwxr-xr-x   0        0        0     3451 2024-04-19 16:26:14.724115 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
--rwxr-xr-x   0        0        0     3235 2024-04-19 23:04:19.789690 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
--rwxr-xr-x   0        0        0      193 2024-04-17 20:02:37.661229 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
--rwxr-xr-x   0        0        0      514 2024-04-19 20:59:00.568662 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
--rwxr-xr-x   0        0        0     1830 2024-04-19 23:29:07.554044 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
--rw-r--r--   0        0        0     1851 2024-04-19 23:33:27.678892 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      799 2024-04-19 16:27:13.563375 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
--rw-r--r--   0        0        0     4346 2024-04-19 23:33:27.682892 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
--rw-r--r--   0        0        0     1268 2024-04-19 23:09:27.226569 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc
--rw-r--r--   0        0        0     1489 2024-04-19 23:09:22.198620 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py
--rwxr-xr-x   0        0        0      754 2024-04-18 00:33:41.120405 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
--rw-r--r--   0        0        0     1826 2024-04-19 18:56:22.468973 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-19 18:56:27.160910 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      996 2024-04-19 16:26:14.764114 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
--rwxr-xr-x   0        0        0     9825 2024-04-19 23:33:20.738974 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
--rwxr-xr-x   0        0        0     3303 2024-04-19 23:03:08.158399 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
--rw-r--r--   0        0        0     2018 2024-04-19 23:06:58.864088 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      834 2024-04-16 20:48:34.547389 biotech-1.1.4/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
--rwxr-xr-x   0        0        0      951 2024-04-16 20:49:56.266040 biotech-1.1.4/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      609 2024-04-19 22:29:43.435688 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
--rw-r--r--   0        0        0     1904 2024-04-19 22:33:09.357432 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      500 2024-04-19 22:29:36.979758 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/dynamic_port.py
--rwxr-xr-x   0        0        0     2161 2024-04-19 22:31:07.314772 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/on.py
--rwxr-xr-x   0        0        0     2200 2024-04-19 22:24:22.967141 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
--rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
--rwxr-xr-x   0        0        0     1441 2024-04-18 02:04:22.961501 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
--rwxr-xr-x   0        0        0      774 2024-04-16 20:48:34.555389 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
--rwxr-xr-x   0        0        0     1336 2024-04-15 21:13:32.676638 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      309 2024-04-17 23:41:26.722721 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      562 2024-04-17 23:41:26.734721 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      525 2024-04-17 23:09:55.764639 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      908 2024-04-19 20:05:11.362609 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0      636 2024-04-18 01:15:59.039315 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      289 2024-04-17 23:05:28.138584 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
--rwxr-xr-x   0        0        0      803 2024-04-19 20:05:09.858629 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
--rwxr-xr-x   0        0        0      378 2024-04-18 01:13:51.928249 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
--rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
--rwxr-xr-x   0        0        0     2182 2024-04-18 01:57:52.896535 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
--rwxr-xr-x   0        0        0     2125 2024-04-18 01:58:34.052216 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1828 2024-04-19 21:04:56.668613 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0     2295 2024-04-19 21:04:32.800884 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
--rw-r--r--   0        0        0        2 2024-04-19 22:32:11.666067 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/start.py
--rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
--rwxr-xr-x   0        0        0      152 2024-04-19 16:48:50.419277 biotech-1.1.4/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4699 2024-04-19 22:17:01.343942 biotech-1.1.4/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.4/venues/stages/biotech/procedures/intro/intro.S.HTML
--rwxr-xr-x   0        0        0     6305 2024-04-19 22:16:54.188023 biotech-1.1.4/venues/stages/biotech/procedures/intro/on.py
--rw-r--r--   0        0        0     2906 2024-04-19 21:43:07.254923 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
--rw-r--r--   0        0        0     4000 2024-04-19 21:42:57.331035 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/adventure.py
--rw-r--r--   0        0        0     1330 2024-04-19 21:12:05.939720 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      905 2024-04-19 16:56:52.013564 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      959 2024-04-19 21:11:59.243796 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      614 2024-04-19 16:56:41.273688 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
--rwxr-xr-x   0        0        0      138 2024-04-19 17:33:23.717242 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/intro.proc.py
--rwxr-xr-x   0        0        0     3084 2024-04-19 21:01:52.394709 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/keg/__init__.py
--rw-r--r--   0        0        0     3068 2024-04-19 21:01:58.358642 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/variables/__init__.py
--rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321766 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      172 2024-04-16 20:48:34.551389 biotech-1.1.4/venues/stages/biotech/procedures/procedures.S.HTML
--rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 biotech-1.1.4/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
--rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 biotech-1.1.4/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
--rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 biotech-1.1.4/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 biotech-1.1.4/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 biotech-1.1.4/venues/stages/biotech/topics/aggregate/__init__.py
--rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 biotech-1.1.4/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 biotech-1.1.4/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      708 2024-04-16 20:48:34.591388 biotech-1.1.4/venues/stages/biotech/topics/alarm_parser/__init__.py
--rwxr-xr-x   0        0        0      673 2024-04-16 20:49:28.126498 biotech-1.1.4/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 biotech-1.1.4/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      405 2024-04-16 20:48:34.579388 biotech-1.1.4/venues/stages/biotech/topics/exceptions.py
--rwxr-xr-x   0        0        0     1190 2024-01-27 05:31:08.525189 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
--rwxr-xr-x   0        0        0     2446 2024-04-17 19:24:25.140060 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__init__.py
--rwxr-xr-x   0        0        0     2491 2024-04-17 19:24:52.839918 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4471 2024-02-01 06:11:56.801715 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1050 2024-04-16 06:10:03.111579 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     1920 2024-01-31 18:50:23.812071 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
--rwxr-xr-x   0        0        0       24 2024-01-26 17:38:56.558087 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
--rwxr-xr-x   0        0        0       24 2024-01-26 17:38:52.854129 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
--rwxr-xr-x   0        0        0      751 2024-04-17 19:16:04.226583 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
--rwxr-xr-x   0        0        0     1981 2024-04-17 19:25:47.591625 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__init__.py
--rwxr-xr-x   0        0        0     2283 2024-04-17 19:25:53.011595 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4019 2024-01-31 18:51:47.652157 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     3843 2024-04-17 19:25:53.099595 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
--rwxr-xr-x   0        0        0     4426 2024-01-27 06:34:32.979965 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
--rwxr-xr-x   0        0        0     3559 2024-04-17 19:25:22.227762 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/treasury.py
--rwxr-xr-x   0        0        0     1727 2024-04-17 19:15:19.882965 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/shares.s.HTML
--rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 biotech-1.1.4/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1558 2024-04-18 05:22:02.832642 biotech-1.1.4/venues/stages/biotech/topics/implicit/proc/__init__.py
--rwxr-xr-x   0        0        0     1158 2024-04-19 21:23:01.800513 biotech-1.1.4/venues/stages/biotech/topics/implicit/thread/__init__.py
--rw-r--r--   0        0        0      855 2024-04-19 21:23:28.056219 biotech-1.1.4/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       90 2024-04-17 22:51:08.968798 biotech-1.1.4/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 22:33:48.860256 biotech-1.1.4/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
--rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 biotech-1.1.4/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
--rwxr-xr-x   0        0        0      470 2024-04-17 23:02:14.419990 biotech-1.1.4/venues/stages/biotech/topics/printout/bracket.py
--rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 biotech-1.1.4/venues/stages/biotech/topics/printout/passes.py
--rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 biotech-1.1.4/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2166 2024-04-19 22:38:28.357906 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__init__.py
--rw-r--r--   0        0        0     1997 2024-04-19 22:38:43.137742 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
--rw-r--r--   0        0        0     1818 2024-04-19 23:33:25.614916 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-18 01:45:27.254200 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1586 2024-04-19 23:27:54.158868 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-18 01:48:34.504806 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-18 01:45:24.082223 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
--rwxr-xr-x   0        0        0      195 2024-04-16 22:50:54.515336 biotech-1.1.4/venues/stages/biotech/topics/process_on/process_on.S.HTML
--rwxr-xr-x   0        0        0     1470 2024-04-18 04:12:56.845888 biotech-1.1.4/venues/stages/biotech/topics/quay/garage.py
--rwxr-xr-x   0        0        0     2546 2024-04-18 04:38:41.478278 biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_1.py
--rwxr-xr-x   0        0        0     1612 2024-04-18 04:54:58.414971 biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_2.py
--rwxr-xr-x   0        0        0      551 2024-04-18 05:20:40.701113 biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_3.py
--rwxr-xr-x   0        0        0     1083 2024-04-18 05:19:11.645613 biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_4.py
--rwxr-xr-x   0        0        0     1448 2024-04-19 22:40:22.232641 biotech-1.1.4/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
--rw-r--r--   0        0        0     1464 2024-04-19 22:41:14.292061 biotech-1.1.4/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 biotech-1.1.4/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
--rw-r--r--   0        0        0      246 2024-04-19 21:18:20.963631 biotech-1.1.4/venues/stages/biotech/topics/report_formats/report_formats.S.HTML
--rw-r--r--   0        0        0     1772 2024-04-19 20:59:56.440027 biotech-1.1.4/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0      461 2024-04-17 23:59:06.614967 biotech-1.1.4/venues/stages/biotech/topics/show/show.S.HTML
--rwxr-xr-x   0        0        0     2295 2024-04-19 20:59:53.444061 biotech-1.1.4/venues/stages/biotech/topics/show/variable.py
--rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
--rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
--rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
--rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
--rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
--rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
--rwxr-xr-x   0        0        0      273 2024-04-16 20:48:34.583388 biotech-1.1.4/venues/stages/biotech/topics/start--/one.py
--rwxr-xr-x   0        0        0      406 2024-04-16 20:48:34.587388 biotech-1.1.4/venues/stages/biotech/topics/start--/sequentially.py
--rwxr-xr-x   0        0        0      532 2024-04-16 20:48:34.587388 biotech-1.1.4/venues/stages/biotech/topics/start--/simultaneously.py
--rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 biotech-1.1.4/venues/stages/biotech/topics/topics.S.HTML
--rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 biotech-1.1.4/venues/stages/biotech/variables/__init__.py
--rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0      211 2024-04-16 02:07:59.993436 biotech-1.1.5/license.S.HTML
+-rwxr-xr-x   0        0        0     1145 2024-04-20 04:04:21.233505 biotech-1.1.5/pyproject.toml
+-rwxr-xr-x   0        0        0     3866 2024-04-16 20:53:30.034757 biotech-1.1.5/readme.md
+-rwxr-xr-x   0        0        0     2331 2024-04-19 15:34:34.407444 biotech-1.1.5/venue.S.HTML
+-rwxr-xr-x   0        0        0   838272 2024-04-16 02:03:26.700967 biotech-1.1.5/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
+-rwxr-xr-x   0        0        0     1270 2024-04-17 22:22:59.944800 biotech-1.1.5/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
+-rwxr-xr-x   0        0        0     4125 2024-04-20 02:56:26.812886 biotech-1.1.5/venues/stages/biotech/___itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      645 2024-04-16 20:48:34.875383 biotech-1.1.5/venues/stages/biotech/___itinerary/maybes.s.HTML
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.5/venues/stages/biotech/___itinerary/processes/errout/script.py
+-rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 biotech-1.1.5/venues/stages/biotech/___itinerary/processes/errout/start.py
+-rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 biotech-1.1.5/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
+-rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 biotech-1.1.5/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.5/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
+-rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 biotech-1.1.5/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
+-rwxr-xr-x   0        0        0      385 2024-04-17 18:49:44.656786 biotech-1.1.5/venues/stages/biotech/__glossary/biotech_1
+-rwxr-xr-x   0        0        0      114 2024-04-17 18:45:06.744254 biotech-1.1.5/venues/stages/biotech/__glossary/glossary.S.HTML
+-rwxr-xr-x   0        0        0      130 2024-04-19 16:49:02.311131 biotech-1.1.5/venues/stages/biotech/__init__.py
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 biotech-1.1.5/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0     1252 2024-04-16 20:48:34.867383 biotech-1.1.5/venues/stages/biotech/_book/advanced tutorial.s.HTML
+-rwxr-xr-x   0        0        0     1786 2024-04-16 20:48:34.867383 biotech-1.1.5/venues/stages/biotech/_book/book.s.HTML
+-rwxr-xr-x   0        0        0      542 2024-04-16 20:48:34.867383 biotech-1.1.5/venues/stages/biotech/_book/relevant.s.HTML
+-rwxr-xr-x   0        0        0     2129 2024-04-17 19:24:51.191926 biotech-1.1.5/venues/stages/biotech/_clique/__init__.py
+-rwxr-xr-x   0        0        0     2493 2024-04-17 19:24:52.839918 biotech-1.1.5/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 biotech-1.1.5/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 biotech-1.1.5/venues/stages/biotech/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 biotech-1.1.5/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 biotech-1.1.5/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0  1424183 2024-04-20 04:03:39.917934 biotech-1.1.5/venues/stages/biotech/_status/DB/records.json
+-rw-r--r--   0        0        0     1172 2024-04-19 22:15:38.920875 biotech-1.1.5/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 biotech-1.1.5/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 biotech-1.1.5/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1487 2024-04-19 22:15:36.412903 biotech-1.1.5/venues/stages/biotech/_status/establish.py
+-rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 biotech-1.1.5/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      720 2024-04-16 20:48:34.887383 biotech-1.1.5/venues/stages/biotech/_status/monitors/-01_start/status_1.py
+-rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 biotech-1.1.5/venues/stages/biotech/_status/monitors/00_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      793 2024-04-16 20:48:34.883383 biotech-1.1.5/venues/stages/biotech/_status/monitors/00_start/status_1.py
+-rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708148 biotech-1.1.5/venues/stages/biotech/_status/monitors/01/stasis/path_1_health.py
+-rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 biotech-1.1.5/venues/stages/biotech/_status/monitors/01/stasis/path_2_health.py
+-rwxr-xr-x   0        0        0     1161 2024-04-16 20:48:34.903383 biotech-1.1.5/venues/stages/biotech/_status/monitors/01/status_1.py
+-rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 biotech-1.1.5/venues/stages/biotech/_status/monitors/02/stasis/1_health.py
+-rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 biotech-1.1.5/venues/stages/biotech/_status/monitors/02/stasis/2_health.py
+-rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 biotech-1.1.5/venues/stages/biotech/_status/monitors/02/stasis/modules/MODULE_1.py
+-rwxr-xr-x   0        0        0     1214 2024-04-16 20:48:34.899383 biotech-1.1.5/venues/stages/biotech/_status/monitors/02/status_1.py
+-rwxr-xr-x   0        0        0      794 2024-04-16 20:48:34.891383 biotech-1.1.5/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py
+-rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 biotech-1.1.5/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      939 2024-04-16 20:48:34.887383 biotech-1.1.5/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      289 2024-04-16 00:28:17.871373 biotech-1.1.5/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      942 2024-04-16 20:48:34.883383 biotech-1.1.5/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 biotech-1.1.5/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py
+-rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 biotech-1.1.5/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      867 2024-04-16 20:48:34.891383 biotech-1.1.5/venues/stages/biotech/_status/monitors/05__file__/status_1.py
+-rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 biotech-1.1.5/venues/stages/biotech/_status/monitors/06_various/stasis/1_health.py
+-rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 biotech-1.1.5/venues/stages/biotech/_status/monitors/06_various/stasis/2_health.py
+-rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 biotech-1.1.5/venues/stages/biotech/_status/monitors/06_various/stasis/3_health.py
+-rwxr-xr-x   0        0        0      955 2024-04-19 22:40:42.880411 biotech-1.1.5/venues/stages/biotech/_status/monitors/06_various/status_1.py
+-rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 biotech-1.1.5/venues/stages/biotech/_status/monitors/07/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0      809 2024-04-16 20:48:34.907383 biotech-1.1.5/venues/stages/biotech/_status/monitors/07/status_1.py
+-rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 biotech-1.1.5/venues/stages/biotech/_status/monitors/08_DB/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0     1561 2024-04-19 19:13:07.956368 biotech-1.1.5/venues/stages/biotech/_status/monitors/08_DB/status_1.py
+-rwxr-xr-x   0        0        0   101963 2024-04-20 04:03:14.586196 biotech-1.1.5/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 biotech-1.1.5/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 biotech-1.1.5/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_2.py
+-rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 biotech-1.1.5/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_3.py
+-rwxr-xr-x   0        0        0     1442 2024-04-19 22:43:25.306602 biotech-1.1.5/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py
+-rwxr-xr-x   0        0        0      367 2024-04-16 03:23:58.043895 biotech-1.1.5/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.5/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.5/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 biotech-1.1.5/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1189 2024-04-19 21:55:08.998787 biotech-1.1.5/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
+-rw-r--r--   0        0        0      316 2024-04-19 18:57:32.516036 biotech-1.1.5/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.5/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.5/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       77 2024-04-19 18:57:24.196146 biotech-1.1.5/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1250 2024-04-19 21:55:16.358703 biotech-1.1.5/venues/stages/biotech/_status/monitors/11/status_1.py
+-rwxr-xr-x   0        0        0      984 2024-04-18 03:32:30.971629 biotech-1.1.5/venues/stages/biotech/_status/status.proc.py
+-rwxr-xr-x   0        0        0      256 2024-04-16 20:48:34.875383 biotech-1.1.5/venues/stages/biotech/_status/status.s.HTML
+-rwxr-xr-x   0        0        0     1483 2024-04-16 20:48:34.851384 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
+-rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
+-rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 biotech-1.1.5/venues/stages/biotech/_status_advanced/status.proc.py
+-rwxr-xr-x   0        0        0     1779 2024-04-16 20:48:34.575388 biotech-1.1.5/venues/stages/biotech/architecture.s.HTML
+-rwxr-xr-x   0        0        0      241 2024-04-16 20:53:18.546926 biotech-1.1.5/venues/stages/biotech/emojis.S.HTML
+-rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 biotech-1.1.5/venues/stages/biotech/license.S.HTML
+-rwxr-xr-x   0        0        0     3068 2024-04-16 20:48:34.543389 biotech-1.1.5/venues/stages/biotech/module.s.HTML
+-rw-r--r--   0        0        0     1596 2024-04-19 21:12:05.931720 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      640 2024-04-19 16:26:52.595637 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      259 2024-04-19 16:20:24.028904 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
+-rwxr-xr-x   0        0        0     1478 2024-04-19 21:11:18.368263 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.648116 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/paths.py
+-rwxr-xr-x   0        0        0      666 2024-04-19 21:46:15.516790 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
+-rwxr-xr-x   0        0        0      562 2024-04-17 21:48:05.111704 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
+-rwxr-xr-x   0        0        0     1163 2024-04-17 21:49:49.362841 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3300 2024-04-20 00:23:15.176206 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-20 00:23:22.860118 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0      999 2024-04-19 20:57:55.937395 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0     2881 2024-04-19 21:20:39.102102 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
+-rw-r--r--   0        0        0     1152 2024-04-19 21:06:40.923425 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      653 2024-04-19 20:56:23.606442 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
+-rwxr-xr-x   0        0        0     3572 2024-04-19 21:20:33.674162 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
+-rwxr-xr-x   0        0        0      769 2024-04-19 21:06:33.619508 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
+-rw-r--r--   0        0        0     2031 2024-04-19 23:33:27.678892 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
+-rw-r--r--   0        0        0     2159 2024-04-19 23:33:27.678892 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      420 2024-04-19 23:33:27.678892 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
+-rw-r--r--   0        0        0      728 2024-04-19 23:33:27.682892 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3451 2024-04-19 16:26:14.724115 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
+-rwxr-xr-x   0        0        0     3235 2024-04-19 23:04:19.789690 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
+-rwxr-xr-x   0        0        0      193 2024-04-17 20:02:37.661229 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
+-rwxr-xr-x   0        0        0      514 2024-04-19 20:59:00.568662 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
+-rwxr-xr-x   0        0        0     2440 2024-04-20 00:16:58.220578 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
+-rw-r--r--   0        0        0     2352 2024-04-20 00:17:02.472528 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      799 2024-04-19 16:27:13.563375 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
+-rw-r--r--   0        0        0     4019 2024-04-20 03:44:13.494628 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
+-rw-r--r--   0        0        0     1634 2024-04-20 00:31:08.822804 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py
+-rw-r--r--   0        0        0     2916 2024-04-20 00:25:32.746630 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/no_records.py
+-rwxr-xr-x   0        0        0      754 2024-04-18 00:33:41.120405 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
+-rw-r--r--   0        0        0     1826 2024-04-19 18:56:22.468973 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-19 18:56:27.160910 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      996 2024-04-19 16:26:14.764114 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
+-rwxr-xr-x   0        0        0     8732 2024-04-20 03:44:09.758669 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
+-rwxr-xr-x   0        0        0     3561 2024-04-20 00:22:42.788579 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
+-rw-r--r--   0        0        0     2178 2024-04-20 00:22:47.936519 biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      834 2024-04-16 20:48:34.547389 biotech-1.1.5/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
+-rwxr-xr-x   0        0        0      951 2024-04-16 20:49:56.266040 biotech-1.1.5/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      690 2024-04-20 03:54:03.628185 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
+-rw-r--r--   0        0        0     1904 2024-04-19 22:33:09.357432 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      706 2024-04-20 04:03:48.877841 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/dynamic_port.py
+-rwxr-xr-x   0        0        0     2161 2024-04-19 22:31:07.314772 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/on.py
+-rwxr-xr-x   0        0        0     2200 2024-04-19 22:24:22.967141 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
+-rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
+-rwxr-xr-x   0        0        0     1441 2024-04-18 02:04:22.961501 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
+-rwxr-xr-x   0        0        0      774 2024-04-16 20:48:34.555389 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
+-rwxr-xr-x   0        0        0     1336 2024-04-15 21:13:32.676638 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      309 2024-04-17 23:41:26.722721 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      562 2024-04-17 23:41:26.734721 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      525 2024-04-17 23:09:55.764639 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      908 2024-04-19 20:05:11.362609 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      636 2024-04-18 01:15:59.039315 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      289 2024-04-17 23:05:28.138584 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
+-rwxr-xr-x   0        0        0      803 2024-04-19 20:05:09.858629 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
+-rwxr-xr-x   0        0        0      378 2024-04-18 01:13:51.928249 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
+-rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
+-rwxr-xr-x   0        0        0     2182 2024-04-18 01:57:52.896535 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
+-rwxr-xr-x   0        0        0     2125 2024-04-18 01:58:34.052216 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1828 2024-04-19 21:04:56.668613 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2295 2024-04-19 21:04:32.800884 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
+-rw-r--r--   0        0        0        2 2024-04-19 22:32:11.666067 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/start.py
+-rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
+-rwxr-xr-x   0        0        0      152 2024-04-19 16:48:50.419277 biotech-1.1.5/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4699 2024-04-19 22:17:01.343942 biotech-1.1.5/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.5/venues/stages/biotech/procedures/intro/intro.S.HTML
+-rwxr-xr-x   0        0        0     6305 2024-04-19 22:16:54.188023 biotech-1.1.5/venues/stages/biotech/procedures/intro/on.py
+-rw-r--r--   0        0        0     2906 2024-04-19 21:43:07.254923 biotech-1.1.5/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
+-rw-r--r--   0        0        0     4000 2024-04-19 21:42:57.331035 biotech-1.1.5/venues/stages/biotech/procedures/intro/process/adventure.py
+-rw-r--r--   0        0        0     1330 2024-04-19 21:12:05.939720 biotech-1.1.5/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      905 2024-04-19 16:56:52.013564 biotech-1.1.5/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      959 2024-04-19 21:11:59.243796 biotech-1.1.5/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      614 2024-04-19 16:56:41.273688 biotech-1.1.5/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
+-rwxr-xr-x   0        0        0      138 2024-04-19 17:33:23.717242 biotech-1.1.5/venues/stages/biotech/procedures/intro/process/intro.proc.py
+-rwxr-xr-x   0        0        0     3084 2024-04-19 21:01:52.394709 biotech-1.1.5/venues/stages/biotech/procedures/intro/process/keg/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-19 21:01:58.358642 biotech-1.1.5/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.5/venues/stages/biotech/procedures/intro/process/variables/__init__.py
+-rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321766 biotech-1.1.5/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      172 2024-04-16 20:48:34.551389 biotech-1.1.5/venues/stages/biotech/procedures/procedures.S.HTML
+-rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 biotech-1.1.5/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 biotech-1.1.5/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
+-rw-r--r--   0        0        0      933 2024-04-20 00:12:18.383907 biotech-1.1.5/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 biotech-1.1.5/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 biotech-1.1.5/venues/stages/biotech/topics/aggregate/__init__.py
+-rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 biotech-1.1.5/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 biotech-1.1.5/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      708 2024-04-16 20:48:34.591388 biotech-1.1.5/venues/stages/biotech/topics/alarm_parser/__init__.py
+-rwxr-xr-x   0        0        0      673 2024-04-16 20:49:28.126498 biotech-1.1.5/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 biotech-1.1.5/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      764 2024-04-20 00:12:12.679976 biotech-1.1.5/venues/stages/biotech/topics/exceptions.py
+-rwxr-xr-x   0        0        0     1190 2024-01-27 05:31:08.525189 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
+-rwxr-xr-x   0        0        0     2446 2024-04-17 19:24:25.140060 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/__init__.py
+-rwxr-xr-x   0        0        0     2491 2024-04-17 19:24:52.839918 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4471 2024-02-01 06:11:56.801715 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1050 2024-04-16 06:10:03.111579 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1920 2024-01-31 18:50:23.812071 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
+-rwxr-xr-x   0        0        0       24 2024-01-26 17:38:56.558087 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
+-rwxr-xr-x   0        0        0       24 2024-01-26 17:38:52.854129 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
+-rwxr-xr-x   0        0        0      751 2024-04-17 19:16:04.226583 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
+-rwxr-xr-x   0        0        0     1981 2024-04-17 19:25:47.591625 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/basin/__init__.py
+-rwxr-xr-x   0        0        0     2283 2024-04-17 19:25:53.011595 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4019 2024-01-31 18:51:47.652157 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3843 2024-04-17 19:25:53.099595 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4426 2024-01-27 06:34:32.979965 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3559 2024-04-17 19:25:22.227762 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/basin/treasury.py
+-rwxr-xr-x   0        0        0     1727 2024-04-17 19:15:19.882965 biotech-1.1.5/venues/stages/biotech/topics/help_documentation/shares.s.HTML
+-rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 biotech-1.1.5/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1558 2024-04-18 05:22:02.832642 biotech-1.1.5/venues/stages/biotech/topics/implicit/proc/__init__.py
+-rwxr-xr-x   0        0        0     1158 2024-04-19 21:23:01.800513 biotech-1.1.5/venues/stages/biotech/topics/implicit/thread/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-19 21:23:28.056219 biotech-1.1.5/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       90 2024-04-17 22:51:08.968798 biotech-1.1.5/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 22:33:48.860256 biotech-1.1.5/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
+-rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 biotech-1.1.5/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
+-rwxr-xr-x   0        0        0      470 2024-04-17 23:02:14.419990 biotech-1.1.5/venues/stages/biotech/topics/printout/bracket.py
+-rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 biotech-1.1.5/venues/stages/biotech/topics/printout/passes.py
+-rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 biotech-1.1.5/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2166 2024-04-19 22:38:28.357906 biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/__init__.py
+-rw-r--r--   0        0        0     1997 2024-04-19 22:38:43.137742 biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
+-rw-r--r--   0        0        0     2184 2024-04-20 03:38:57.814039 biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-18 01:45:27.254200 biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1956 2024-04-20 03:38:53.142089 biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-18 01:48:34.504806 biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-18 01:45:24.082223 biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
+-rwxr-xr-x   0        0        0      195 2024-04-16 22:50:54.515336 biotech-1.1.5/venues/stages/biotech/topics/process_on/process_on.S.HTML
+-rw-r--r--   0        0        0      832 2024-04-20 01:28:37.993409 biotech-1.1.5/venues/stages/biotech/topics/process_on/sub/explicit.py
+-rw-r--r--   0        0        0     1015 2024-04-20 03:49:41.395055 biotech-1.1.5/venues/stages/biotech/topics/process_on/sub/implicit.py
+-rwxr-xr-x   0        0        0     1470 2024-04-18 04:12:56.845888 biotech-1.1.5/venues/stages/biotech/topics/quay/garage.py
+-rwxr-xr-x   0        0        0     2546 2024-04-18 04:38:41.478278 biotech-1.1.5/venues/stages/biotech/topics/quay/implicit_process_test_1.py
+-rwxr-xr-x   0        0        0     1612 2024-04-18 04:54:58.414971 biotech-1.1.5/venues/stages/biotech/topics/quay/implicit_process_test_2.py
+-rwxr-xr-x   0        0        0      551 2024-04-18 05:20:40.701113 biotech-1.1.5/venues/stages/biotech/topics/quay/implicit_process_test_3.py
+-rwxr-xr-x   0        0        0     1083 2024-04-18 05:19:11.645613 biotech-1.1.5/venues/stages/biotech/topics/quay/implicit_process_test_4.py
+-rwxr-xr-x   0        0        0     1448 2024-04-19 22:40:22.232641 biotech-1.1.5/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
+-rw-r--r--   0        0        0     1464 2024-04-19 22:41:14.292061 biotech-1.1.5/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 biotech-1.1.5/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-19 21:18:20.963631 biotech-1.1.5/venues/stages/biotech/topics/report_formats/report_formats.S.HTML
+-rw-r--r--   0        0        0     1772 2024-04-19 20:59:56.440027 biotech-1.1.5/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0      461 2024-04-17 23:59:06.614967 biotech-1.1.5/venues/stages/biotech/topics/show/show.S.HTML
+-rwxr-xr-x   0        0        0     2295 2024-04-19 20:59:53.444061 biotech-1.1.5/venues/stages/biotech/topics/show/variable.py
+-rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 biotech-1.1.5/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
+-rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 biotech-1.1.5/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
+-rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 biotech-1.1.5/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
+-rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 biotech-1.1.5/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
+-rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 biotech-1.1.5/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 biotech-1.1.5/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 biotech-1.1.5/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
+-rwxr-xr-x   0        0        0      273 2024-04-16 20:48:34.583388 biotech-1.1.5/venues/stages/biotech/topics/start--/one.py
+-rwxr-xr-x   0        0        0      406 2024-04-16 20:48:34.587388 biotech-1.1.5/venues/stages/biotech/topics/start--/sequentially.py
+-rwxr-xr-x   0        0        0      532 2024-04-16 20:48:34.587388 biotech-1.1.5/venues/stages/biotech/topics/start--/simultaneously.py
+-rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 biotech-1.1.5/venues/stages/biotech/topics/topics.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 biotech-1.1.5/venues/stages/biotech/variables/__init__.py
+-rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.5/PKG-INFO
```

### Comparing `biotech-1.1.4/pyproject.toml` & `biotech-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 [tool.poetry]
 name = "biotech"
-version = "1.1.4"
+version = "1.1.5"
 description = "A health monitoring stack"
 authors = []
 readme = "readme.md"
 
 packages = [
     { include = "biotech", from = "venues/stages" }
 ]
```

### Comparing `biotech-1.1.4/readme.md` & `biotech-1.1.5/readme.md`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venue.S.HTML` & `biotech-1.1.5/venue.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg` & `biotech-1.1.5/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML` & `biotech-1.1.5/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/___itinerary/itinerary.S.HTML` & `biotech-1.1.5/venues/stages/biotech/___itinerary/itinerary.S.HTML`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 					
 					
 				[ ] there could have been an error
 					sending /done_with_scan
 					to the aggregator
 
 
+			[ ] scribbles
+			
+					scribble ()
+			
+			
 
 		<h2>ranked</h2>
 			
 	
 			
 			
 			[ ] before and after were lost
```

### Comparing `biotech-1.1.4/venues/stages/biotech/___itinerary/maybes.s.HTML` & `biotech-1.1.5/venues/stages/biotech/___itinerary/maybes.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout/start.py` & `biotech-1.1.5/venues/stages/biotech/___itinerary/processes/errout/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout_v2/start.py` & `biotech-1.1.5/venues/stages/biotech/___itinerary/processes/errout_v2/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/__license/options/gpl-3.0-standalone.html` & `biotech-1.1.5/venues/stages/biotech/__license/options/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_book/advanced tutorial.s.HTML` & `biotech-1.1.5/venues/stages/biotech/_book/advanced tutorial.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_book/book.s.HTML` & `biotech-1.1.5/venues/stages/biotech/_book/book.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_book/relevant.s.HTML` & `biotech-1.1.5/venues/stages/biotech/_book/relevant.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_clique/__init__.py` & `biotech-1.1.5/venues/stages/biotech/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/DB/records.json` & `biotech-1.1.5/venues/stages/biotech/_status/DB/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949748743718593%*

 * *Differences: {"'_default'": "{'395': OrderedDict([('paths', [OrderedDict([('path', "*

 * *               "'_status/monitors/-01_start/status_1.py'), ('empty', False), ('parsed', True), "*

 * *               "('stats', OrderedDict([('passes', 1), ('alarms', 0)])), ('checks', "*

 * *               "[OrderedDict([('check', 'check 1'), ('passed', True), ('elapsed', "*

 * *               "[6.0801009420029, 'seconds'])])])]), OrderedDict([('path', "*

 * *               "'_status/monitors/00_start/status_1.py'), ('empty', False), ('parsed', True), "*

 * *  […]*

```diff
@@ -53097,14 +53097,1130 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 14
                 },
                 "empty": 0
             }
         },
+        "395": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.0801009420029,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/-01_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.046785377002379,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/00_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.199513528001262,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/01/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.080170635999821,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/02/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.162111441997695,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/03_empty_glob/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.048570229999314,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/04.0_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.099145612999564,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/04.1_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.184785694000311,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/05__file__/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.097288977005519,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/06_various/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.1577708369950415,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/07/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "tinyDB database can be utilized",
+                            "elapsed": [
+                                6.171911722005461,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/08_DB/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                6.058288223001,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/09_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                10.082430556998588,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/10_time_limits/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                6.082896704996529,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/11/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 14
+                },
+                "empty": 0
+            }
+        },
+        "396": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.0809428349966765,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/-01_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.091619138001988,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/00_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.204494247998809,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/01/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.10166757999832,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/02/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.147007315004885,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/03_empty_glob/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.063444291998167,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/04.0_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.098316358002194,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/04.1_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.173119044004125,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/05__file__/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.111150221004209,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/06_various/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.159311062998313,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/07/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "tinyDB database can be utilized",
+                            "elapsed": [
+                                6.207606190997467,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/08_DB/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                6.143101157002093,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/09_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                10.08862113399664,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/10_time_limits/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                6.093511977000162,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/11/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 14
+                },
+                "empty": 0
+            }
+        },
+        "397": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.101720537000801,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/-01_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.072959956996783,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/00_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.186398932004522,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/01/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.097455152004841,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/02/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.163751473002776,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/03_empty_glob/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.07257694999862,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/04.0_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.107195391996356,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/04.1_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.194276248999813,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/05__file__/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.121067924003,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/06_various/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.131049930998415,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/07/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "tinyDB database can be utilized",
+                            "elapsed": [
+                                6.251327249003225,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/08_DB/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                6.093128403001174,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/09_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                10.108095773997775,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/10_time_limits/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                6.053487810997467,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/11/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 14
+                },
+                "empty": 0
+            }
+        },
+        "398": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.073719908999919,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/-01_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.088487248001911,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/00_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.183202519001497,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/01/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.083420858994941,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/02/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.1576204860029975,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/03_empty_glob/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.072253856000316,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/04.0_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.093301105000137,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/04.1_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.186563698996906,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/05__file__/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.101107882001088,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/06_various/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.148870719000115,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/07/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "tinyDB database can be utilized",
+                            "elapsed": [
+                                6.228749085996242,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/08_DB/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                6.138250427000457,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/09_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                10.128856211995299,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/10_time_limits/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                6.069548381994537,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/11/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 14
+                },
+                "empty": 0
+            }
+        },
         "4": {
             "alarms": [],
             "paths": [
                 {
                     "empty": true,
                     "parsed": true,
                     "path": "_status/status_py.py"
```

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/establish.py` & `biotech-1.1.5/venues/stages/biotech/_status/establish.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/-01_start/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/-01_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/00_start/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/00_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/01/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/01/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/02/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/02/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/05__file__/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/06_various/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/07/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/07/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/08_DB/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/08_DB/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666667%*

 * *Differences: {"'_default'": "{'237': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [1.2835000234190375e-05, 'seconds']), ('passed', "*

 * *               "True)])]), ('empty', False), ('parsed', True), ('path', 'guarantee_1.py'), "*

 * *               "('records', ['proceeds None\\r\\n', 'checks in module True\\r\\n', 'check "*

 * *               '1\\r\\n\', \'{\\r\\n\', \'  "variable": {\\r\\n\', \'    "pid": 16146,\\r\\n\', '*

 * *               '\'    "proceeds": {\\r\\ […]*

```diff
@@ -5733,14 +5733,203 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 1
                 },
                 "empty": 0
             }
         },
+        "237": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.2835000234190375e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "guarantee_1.py",
+                    "records": [
+                        "proceeds None\r\n",
+                        "checks in module True\r\n",
+                        "check 1\r\n",
+                        "{\r\n",
+                        "  \"variable\": {\r\n",
+                        "    \"pid\": 16146,\r\n",
+                        "    \"proceeds\": {\r\n",
+                        "      \"empty\": false,\r\n",
+                        "      \"parsed\": true,\r\n",
+                        "      \"stats\": {\r\n",
+                        "        \"passes\": 1,\r\n",
+                        "        \"alarms\": 0\r\n",
+                        "      },\r\n",
+                        "      \"checks\": [\r\n",
+                        "        {\r\n",
+                        "          \"check\": \"check 1\",\r\n",
+                        "          \"passed\": true,\r\n",
+                        "          \"elapsed\": [\r\n",
+                        "            1.2835000234190375e-05,\r\n",
+                        "            \"seconds\"\r\n",
+                        "          ]\r\n",
+                        "        }\r\n",
+                        "      ]\r\n",
+                        "    },\r\n",
+                        "    \"harbor\": {\r\n",
+                        "      \"host\": \"0.0.0.0\",\r\n",
+                        "      \"port\": 52435\r\n",
+                        "    }\r\n",
+                        "  },\r\n",
+                        "  \"path\": \"/biotech/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py\",\r\n",
+                        "  \"line\": 77\r\n"
+                    ],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "238": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.269100175704807e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "guarantee_1.py",
+                    "records": [
+                        "proceeds None\r\n",
+                        "checks in module True\r\n",
+                        "check 1\r\n",
+                        "{\r\n",
+                        "  \"variable\": {\r\n",
+                        "    \"pid\": 17101,\r\n",
+                        "    \"proceeds\": {\r\n",
+                        "      \"empty\": false,\r\n",
+                        "      \"parsed\": true,\r\n",
+                        "      \"stats\": {\r\n",
+                        "        \"passes\": 1,\r\n",
+                        "        \"alarms\": 0\r\n",
+                        "      },\r\n",
+                        "      \"checks\": [\r\n",
+                        "        {\r\n",
+                        "          \"check\": \"check 1\",\r\n",
+                        "          \"passed\": true,\r\n",
+                        "          \"elapsed\": [\r\n",
+                        "            1.269100175704807e-05,\r\n",
+                        "            \"seconds\"\r\n",
+                        "          ]\r\n",
+                        "        }\r\n",
+                        "      ]\r\n",
+                        "    },\r\n",
+                        "    \"harbor\": {\r\n",
+                        "      \"host\": \"0.0.0.0\",\r\n",
+                        "      \"port\": 52435\r\n",
+                        "    }\r\n",
+                        "  },\r\n",
+                        "  \"path\": \"/biotech/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py\",\r\n",
+                        "  \"line\": 77\r\n",
+                        "}\r\n"
+                    ],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "239": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.1937001545447856e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "guarantee_1.py",
+                    "records": [
+                        "proceeds None\r\n",
+                        "checks in module True\r\n",
+                        "check 1\r\n",
+                        "{\r\n",
+                        "  \"variable\": {\r\n",
+                        "    \"pid\": 846,\r\n",
+                        "    \"proceeds\": {\r\n",
+                        "      \"empty\": false,\r\n",
+                        "      \"parsed\": true,\r\n",
+                        "      \"stats\": {\r\n",
+                        "        \"passes\": 1,\r\n",
+                        "        \"alarms\": 0\r\n",
+                        "      },\r\n",
+                        "      \"checks\": [\r\n",
+                        "        {\r\n",
+                        "          \"check\": \"check 1\",\r\n",
+                        "          \"passed\": true,\r\n",
+                        "          \"elapsed\": [\r\n",
+                        "            1.1937001545447856e-05,\r\n",
+                        "            \"seconds\"\r\n",
+                        "          ]\r\n",
+                        "        }\r\n",
+                        "      ]\r\n",
+                        "    },\r\n"
+                    ],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
         "24": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
@@ -5757,14 +5946,47 @@
                     "stats": {
                         "alarms": 0,
                         "passes": 1
                     }
                 }
             ],
             "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "240": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.4845998268574476e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "guarantee_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
                 "alarms": 0,
                 "checks": {
                     "alarms": 0,
                     "passes": 1
                 },
                 "empty": 0
             }
```

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/monitors/11/status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status/monitors/11/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status/status.proc.py` & `biotech-1.1.5/venues/stages/biotech/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py` & `biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json` & `biotech-1.1.5/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/_status_advanced/status.proc.py` & `biotech-1.1.5/venues/stages/biotech/_status_advanced/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/architecture.s.HTML` & `biotech-1.1.5/venues/stages/biotech/architecture.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/module.s.HTML` & `biotech-1.1.5/venues/stages/biotech/module.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/on.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #----
 #
 from .spaces.done_with_scan import done_with_scan
 from .spaces.paths_patch import paths_patch
 from .spaces.the_health_scan_started import the_health_scan_started
 #
 from biotech.procedures.aggregator_procedure.process.variables import retrieve_aggregator_variables
+from biotech.procedures.aggregator_procedure.process.variables import add_anomaly
 #
 #
 from flask import Flask, request, jsonify
 import rich
 #
 #
 import json
@@ -63,20 +64,22 @@
 	def on_get ():	
 		return "yes"
 		
 	@app.route ("/anomalies", methods = [ 'GET' ])
 	def on_anomalies ():	
 		try:
 			aggregator_variables = retrieve_aggregator_variables ()
+			return jsonify ({
+				"anomalies": aggregator_variables ["anomalies"]
+			})
 			
-			return {
-				"anomalies": jsonify (aggregator_variables ["anomalies"])
-			}
+		except Exception as E:
+			print (E)
 			
-		except Exception:
+		
 			pass;
 			
 		return "not parseable"
 
 
 	@app.route ("/waiting_for", methods = [ 'GET' ])
 	def on_waiting_for ():	
@@ -118,15 +121,18 @@
 			})
 			
 		except Exception as E:
 			print ("exception:", E)
 			pass;
 			
 		return "not parseable"
-		
+	
+	
+
+	
 	@app.route ('/health_scans/paths', methods = [ 'GET' ])
 	def on__get__health_scans__paths ():	
 		aggregator_variables = retrieve_aggregator_variables ()
 		
 		the_paths = {}
 		
 		for path in aggregator_variables ["internal_statuses"]:
```

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 23:42:26 2024 UTC, .py size: 3193 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,197 +1,201 @@
-00000000: 6f0d 0d0a 0000 0000 6201 2366 790c 0000  o.......b.#fy...
+00000000: 6f0d 0d0a 0000 0000 f30a 2366 e40c 0000  o.........#f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6405 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 0100 6405 6407 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
-00000070: 6d0c 5a0c 0100 6405 6408 6c0d 5a0d 6405  m.Z...d.d.l.Z.d.
-00000080: 6408 6c0e 5a0e 6405 6408 6c0f 5a0f 6405  d.l.Z.d.d.l.Z.d.
-00000090: 6408 6c10 5a10 6405 6409 6c11 6d12 5a12  d.l.Z.d.d.l.m.Z.
-000000a0: 6d13 5a13 6d14 5a14 0100 6405 6408 6c15  m.Z.m.Z...d.d.l.
-000000b0: 5a15 6405 6408 6c16 5a16 6405 6408 6c17  Z.d.d.l.Z.d.d.l.
-000000c0: 5a17 0905 0905 640c 640a 640b 8401 5a18  Z.....d.d.d...Z.
-000000d0: 6408 5300 290d 7a68 0a09 6f62 6a65 6374  d.S.).zh..object
-000000e0: 6976 6573 3a0a 090a 0909 5b20 5d20 2f61  ives:.....[ ] /a
-000000f0: 6767 7265 6761 746f 722f 7265 636f 7264  ggregator/record
-00000100: 730a 0909 0a09 095b 205d 202f 6865 616c  s......[ ] /heal
-00000110: 7468 5f73 6361 6e73 2f70 6174 6873 0a09  th_scans/paths..
-00000120: 090a 0909 5b20 5d20 2f68 6561 6c74 685f  ....[ ] /health_
-00000130: 7363 616e 2f7b 2070 6174 6820 7d09 090a  scan/{ path }...
-00000140: e901 0000 0029 01da 0e64 6f6e 655f 7769  .....)...done_wi
-00000150: 7468 5f73 6361 6e29 01da 0b70 6174 6873  th_scan)...paths
-00000160: 5f70 6174 6368 2901 da17 7468 655f 6865  _patch)...the_he
-00000170: 616c 7468 5f73 6361 6e5f 7374 6172 7465  alth_scan_starte
-00000180: 64e9 0000 0000 2901 da1d 7265 7472 6965  d.....)...retrie
-00000190: 7665 5f61 6767 7265 6761 746f 725f 7661  ve_aggregator_va
-000001a0: 7269 6162 6c65 7329 03da 0546 6c61 736b  riables)...Flask
-000001b0: da07 7265 7175 6573 74da 076a 736f 6e69  ..request..jsoni
-000001c0: 6679 4e29 03da 0764 6972 6e61 6d65 da04  fyN)...dirname..
-000001d0: 6a6f 696e da08 6e6f 726d 7061 7468 6302  join..normpathc.
-000001e0: 0000 0000 0000 0000 0000 0009 0000 0005  ................
-000001f0: 0000 0043 0000 0073 dc00 0000 7c01 6401  ...C...s....|.d.
-00000200: 6b05 7209 7400 6402 7c00 8302 0100 7401  k.r.t.d.|.....t.
-00000210: 6403 8301 7d02 0900 7402 7c02 7c00 6404  d...}...t.|.|.d.
-00000220: 8d02 0100 7c02 6a03 6405 6406 6701 6407  ....|.j.d.d.g.d.
-00000230: 8d02 6408 6409 8400 8301 7d03 7c02 6a03  ..d.d.....}.|.j.
-00000240: 640a 6406 6701 6407 8d02 640b 640c 8400  d.d.g.d...d.d...
-00000250: 8301 7d04 7c02 6a03 640d 6406 6701 6407  ..}.|.j.d.d.g.d.
-00000260: 8d02 640e 640f 8400 8301 7d05 7c02 6a03  ..d.d.....}.|.j.
-00000270: 6410 6406 6701 6407 8d02 6411 6412 8400  d.d.g.d...d.d...
-00000280: 8301 7d06 7c02 6a03 6413 6406 6701 6407  ..}.|.j.d.d.g.d.
-00000290: 8d02 6414 6415 8400 8301 7d07 7c02 6a03  ..d.d.....}.|.j.
-000002a0: 6416 6406 6701 6407 8d02 6417 6418 8400  d.d.g.d...d.d...
-000002b0: 8301 7d08 7404 7c02 8301 0100 7405 7c02  ..}.t.|.....t.|.
-000002c0: 8301 0100 7c02 6a06 6419 7c00 641a 641b  ....|.j.d.|.d.d.
-000002d0: 8d03 0100 6400 5300 291c 4e72 0100 0000  ....d.S.).Nr....
-000002e0: 7a21 6f70 656e 696e 6720 7363 616e 2070  z!opening scan p
-000002f0: 726f 6365 7373 206b 6567 206f 6e20 706f  rocess keg on po
-00000300: 7274 3a7a 1161 6767 7265 6761 746f 7220  rt:z.aggregator 
-00000310: 6861 7262 6f72 2901 da19 6167 6772 6567  harbor)...aggreg
-00000320: 6174 6f72 5f70 726f 6365 6475 7265 5f70  ator_procedure_p
-00000330: 6f72 74fa 012f da03 4745 5429 01da 076d  ort../..GET)...m
-00000340: 6574 686f 6473 6300 0000 0000 0000 0000  ethodsc.........
-00000350: 0000 0000 0000 0006 0000 0053 0000 0073  ...........S...s
-00000360: 1a00 0000 7400 6401 6701 6401 6701 6401  ....t.d.g.d.g.d.
-00000370: 6701 6401 6701 6402 9c04 8301 5300 2903  g.d.g.d.....S.).
-00000380: 4eda 0367 6574 2904 fa24 2f68 6561 6c74  N..get)..$/healt
-00000390: 685f 7363 616e 2f3c 7061 7468 3a68 6561  h_scan/<path:hea
-000003a0: 6c74 685f 7363 616e 5f70 6174 683e fa13  lth_scan_path>..
-000003b0: 2f68 6561 6c74 685f 7363 616e 732f 7061  /health_scans/pa
-000003c0: 7468 73fa 032f 6f6e fa0a 2f61 6e6f 6d61  ths../on../anoma
-000003d0: 6c69 6573 2901 7209 0000 00a9 0072 1600  lies).r......r..
-000003e0: 0000 7216 0000 00fa 562f 6269 6f74 6563  ..r.....V/biotec
-000003f0: 682f 7665 6e75 6573 2f73 7461 6765 732f  h/venues/stages/
-00000400: 6269 6f74 6563 682f 7072 6f63 6564 7572  biotech/procedur
-00000410: 6573 2f61 6767 7265 6761 746f 725f 7072  es/aggregator_pr
-00000420: 6f63 6564 7572 652f 7072 6f63 6573 732f  ocedure/process/
-00000430: 6b65 672f 5f5f 696e 6974 5f5f 2e70 79da  keg/__init__.py.
-00000440: 0868 6f6d 655f 6765 7434 0000 0073 0c00  .home_get4...s..
-00000450: 0000 0202 0401 0401 0401 0401 08fc 7a1d  ..............z.
-00000460: 6f70 656e 5f68 6172 626f 722e 3c6c 6f63  open_harbor.<loc
-00000470: 616c 733e 2e68 6f6d 655f 6765 7472 1400  als>.home_getr..
-00000480: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000490: 0000 0001 0000 0053 0000 00f3 0400 0000  .......S........
-000004a0: 6401 5300 a902 4eda 0379 6573 7216 0000  d.S...N..yesr...
-000004b0: 0072 1600 0000 7216 0000 0072 1600 0000  .r....r....r....
-000004c0: 7217 0000 00da 066f 6e5f 6765 743e 0000  r......on_get>..
-000004d0: 00f3 0200 0000 0402 7a1b 6f70 656e 5f68  ........z.open_h
-000004e0: 6172 626f 722e 3c6c 6f63 616c 733e 2e6f  arbor.<locals>.o
-000004f0: 6e5f 6765 7472 1500 0000 6300 0000 0000  n_getr....c.....
-00000500: 0000 0000 0000 0001 0000 0008 0000 0053  ...............S
-00000510: 0000 0073 2e00 0000 7a0c 7400 8300 7d00  ...s....z.t...}.
-00000520: 6401 7401 7c00 6401 1900 8301 6901 5700  d.t.|.d.....i.W.
-00000530: 5300 0400 7402 7916 0100 0100 0100 5900  S...t.y.......Y.
-00000540: 6402 5300 7700 2903 4eda 0961 6e6f 6d61  d.S.w.).N..anoma
-00000550: 6c69 6573 fa0d 6e6f 7420 7061 7273 6561  lies..not parsea
-00000560: 626c 6529 0372 0600 0000 7209 0000 00da  ble).r....r.....
-00000570: 0945 7863 6570 7469 6f6e 2901 da14 6167  .Exception)...ag
-00000580: 6772 6567 6174 6f72 5f76 6172 6961 626c  gregator_variabl
-00000590: 6573 7216 0000 0072 1600 0000 7217 0000  esr....r....r...
-000005a0: 00da 0c6f 6e5f 616e 6f6d 616c 6965 7342  ...on_anomaliesB
-000005b0: 0000 0073 1000 0000 0202 0601 0c03 06ff  ...s............
-000005c0: 0c04 0201 0402 02fd 7a21 6f70 656e 5f68  ........z!open_h
-000005d0: 6172 626f 722e 3c6c 6f63 616c 733e 2e6f  arbor.<locals>.o
-000005e0: 6e5f 616e 6f6d 616c 6965 737a 0c2f 7761  n_anomaliesz./wa
-000005f0: 6974 696e 675f 666f 7263 0000 0000 0000  iting_forc......
-00000600: 0000 0000 0000 0800 0000 0a00 0000 5300  ..............S.
-00000610: 0000 7308 0100 007a 6b74 0083 007d 007c  ..s....zkt...}.|
-00000620: 0064 0119 007d 0167 007d 027c 0144 005d  .d...}.g.}.|.D.]
-00000630: 587d 0364 027d 047a 0a7c 0064 0119 007c  X}.d.}.z.|.d...|
-00000640: 0319 0064 0319 007d 0457 006e 0904 0074  ...d...}.W.n...t
-00000650: 0179 2301 0001 0001 0059 006e 0177 0064  .y#......Y.n.w.d
-00000660: 027d 057a 0a7c 0064 0119 007c 0319 0064  .}.z.|.d...|...d
-00000670: 0419 007d 0557 006e 0904 0074 0179 3901  ...}.W.n...t.y9.
-00000680: 0001 0001 0059 006e 0177 0064 027d 067a  .....Y.n.w.d.}.z
-00000690: 0a7c 0064 0119 007c 0319 0064 0519 007d  .|.d...|...d...}
-000006a0: 0657 006e 0904 0074 0179 4f01 0001 0001  .W.n...t.yO.....
-000006b0: 0059 006e 0177 007c 017c 0319 0064 0619  .Y.n.w.|.|...d..
-000006c0: 0064 0719 0064 086b 0372 647c 02a0 027c  .d...d.k.rd|...|
-000006d0: 037c 047c 057c 0664 099c 04a1 0101 0071  .|.|.|.d.......q
-000006e0: 0c74 0364 0a7c 0269 0183 0157 0053 0004  .t.d.|.i...W.S..
-000006f0: 0074 0179 8301 007d 0701 007a 0c74 0464  .t.y...}...z.t.d
-00000700: 0b7c 0783 0201 0057 0059 0064 007d 077e  .|.....W.Y.d.}.~
-00000710: 0764 0253 0064 007d 077e 0777 0177 0029  .d.S.d.}.~.w.w.)
-00000720: 0c4e da11 696e 7465 726e 616c 5f73 7461  .N..internal_sta
-00000730: 7475 7365 7372 1f00 0000 da0b 6f63 6375  tusesr......occu
-00000740: 7272 656e 6365 73da 0772 6563 6f72 6473  rrences..records
-00000750: da05 7469 6d65 73da 0673 7461 7475 73da  ..times..status.
-00000760: 0770 726f 6365 7373 da04 646f 6e65 2904  .process..done).
-00000770: da04 7061 7468 7224 0000 0072 2500 0000  ..pathr$...r%...
-00000780: 7226 0000 00da 0b77 6169 7469 6e67 5f66  r&.....waiting_f
-00000790: 6f72 7a0a 6578 6365 7074 696f 6e3a 2905  orz.exception:).
-000007a0: 7206 0000 0072 2000 0000 da06 6170 7065  r....r .....appe
-000007b0: 6e64 7209 0000 00da 0570 7269 6e74 2908  ndr......print).
-000007c0: 7221 0000 0072 2300 0000 722b 0000 00da  r!...r#...r+....
-000007d0: 0b73 7461 7475 735f 7061 7468 7224 0000  .status_pathr$..
-000007e0: 0072 2500 0000 7226 0000 00da 0145 7216  .r%...r&.....Er.
-000007f0: 0000 0072 1600 0000 7217 0000 00da 0e6f  ...r....r......o
-00000800: 6e5f 7761 6974 696e 675f 666f 7251 0000  n_waiting_forQ..
-00000810: 0073 5000 0000 0202 0601 0801 0403 0801  .sP.............
-00000820: 0401 0201 1401 0c01 0401 02ff 0403 0201  ................
-00000830: 1401 0c01 0401 02ff 0403 0201 1401 0c01  ................
-00000840: 0401 02ff 1403 0401 0201 0201 0201 0201  ................
-00000850: 08fc 0280 0207 0401 08ff 0e04 0a01 0a01  ................
-00000860: 0402 0880 02fc 7a23 6f70 656e 5f68 6172  ......z#open_har
-00000870: 626f 722e 3c6c 6f63 616c 733e 2e6f 6e5f  bor.<locals>.on_
-00000880: 7761 6974 696e 675f 666f 7272 1300 0000  waiting_forr....
-00000890: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
-000008a0: 0004 0000 0053 0000 0073 2800 0000 7400  .....S...s(...t.
-000008b0: 8300 7d00 6900 7d01 7c00 6401 1900 4400  ..}.i.}.|.d...D.
-000008c0: 5d06 7d02 6402 7c01 7c02 3c00 7109 7401  ].}.d.|.|.<.q.t.
-000008d0: 7c01 8301 5300 2903 4e72 2300 0000 da00  |...S.).Nr#.....
-000008e0: 2902 7206 0000 0072 0900 0000 2903 7221  ).r....r....).r!
-000008f0: 0000 00da 0974 6865 5f70 6174 6873 722a  .....the_pathsr*
-00000900: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00000910: 0000 da1c 6f6e 5f5f 6765 745f 5f68 6561  ....on__get__hea
-00000920: 6c74 685f 7363 616e 735f 5f70 6174 6873  lth_scans__paths
-00000930: 7e00 0000 730a 0000 0006 0204 020c 020a  ~...s...........
-00000940: 0108 027a 316f 7065 6e5f 6861 7262 6f72  ...z1open_harbor
-00000950: 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f5f 6765  .<locals>.on__ge
-00000960: 745f 5f68 6561 6c74 685f 7363 616e 735f  t__health_scans_
-00000970: 5f70 6174 6873 7212 0000 0063 0100 0000  _pathsr....c....
-00000980: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00000990: 5300 0000 7219 0000 0072 1a00 0000 7216  S...r....r....r.
-000009a0: 0000 0029 01da 1068 6561 6c74 685f 7363  ...)...health_sc
-000009b0: 616e 5f70 6174 6872 1600 0000 7216 0000  an_pathr....r...
-000009c0: 0072 1700 0000 da1a 6f6e 5f5f 6765 745f  .r......on__get_
-000009d0: 5f68 6561 6c74 685f 7363 616e 5f5f 7061  _health_scan__pa
-000009e0: 7468 8900 0000 721d 0000 007a 2f6f 7065  th....r....z/ope
-000009f0: 6e5f 6861 7262 6f72 2e3c 6c6f 6361 6c73  n_harbor.<locals
-00000a00: 3e2e 6f6e 5f5f 6765 745f 5f68 6561 6c74  >.on__get__healt
-00000a10: 685f 7363 616e 5f5f 7061 7468 7a07 302e  h_scan__pathz.0.
-00000a20: 302e 302e 3046 2902 da04 706f 7274 da05  0.0.0F)...port..
-00000a30: 6465 6275 6729 0772 2d00 0000 7207 0000  debug).r-...r...
-00000a40: 0072 0300 0000 da05 726f 7574 6572 0400  .r......router..
-00000a50: 0000 7202 0000 00da 0372 756e 2909 7236  ..r......run).r6
-00000a60: 0000 0072 2500 0000 da03 6170 7072 1800  ...r%.....appr..
-00000a70: 0000 721c 0000 0072 2200 0000 7230 0000  ..r....r"...r0..
-00000a80: 0072 3300 0000 7235 0000 0072 1600 0000  .r3...r5...r....
-00000a90: 7216 0000 0072 1700 0000 da0b 6f70 656e  r....r......open
-00000aa0: 5f68 6172 626f 7224 0000 0073 3000 0000  _harbor$...s0...
-00000ab0: 0804 0a01 0804 0202 0c03 0e02 0a01 0e09  ................
-00000ac0: 0a01 0e03 0a01 0e0e 0a01 0e2c 0a01 0e0a  ...........,....
-00000ad0: 0a01 0804 0802 0404 0201 0201 0201 0afd  ................
-00000ae0: 723b 0000 0029 0272 0500 0000 7205 0000  r;...).r....r...
-00000af0: 0029 19da 075f 5f64 6f63 5f5f da15 7370  .)...__doc__..sp
-00000b00: 6163 6573 2e64 6f6e 655f 7769 7468 5f73  aces.done_with_s
-00000b10: 6361 6e72 0200 0000 da12 7370 6163 6573  canr......spaces
-00000b20: 2e70 6174 6873 5f70 6174 6368 7203 0000  .paths_patchr...
-00000b30: 00da 1e73 7061 6365 732e 7468 655f 6865  ...spaces.the_he
-00000b40: 616c 7468 5f73 6361 6e5f 7374 6172 7465  alth_scan_starte
-00000b50: 6472 0400 0000 da39 6269 6f74 6563 682e  dr.....9biotech.
-00000b60: 7072 6f63 6564 7572 6573 2e61 6767 7265  procedures.aggre
-00000b70: 6761 746f 725f 7072 6f63 6564 7572 652e  gator_procedure.
-00000b80: 7072 6f63 6573 732e 7661 7269 6162 6c65  process.variable
-00000b90: 7372 0600 0000 da05 666c 6173 6b72 0700  sr......flaskr..
-00000ba0: 0000 7208 0000 0072 0900 0000 da04 7269  ..r....r......ri
-00000bb0: 6368 da04 6a73 6f6e da07 7061 7468 6c69  ch..json..pathli
-00000bc0: 62da 026f 73da 076f 732e 7061 7468 720a  b..os..os.pathr.
-00000bd0: 0000 0072 0b00 0000 720c 0000 00da 0373  ...r....r......s
-00000be0: 7973 da09 7468 7265 6164 696e 67da 0474  ys..threading..t
-00000bf0: 696d 6572 3b00 0000 7216 0000 0072 1600  imer;...r....r..
-00000c00: 0000 7216 0000 0072 1700 0000 da08 3c6d  ..r....r......<m
-00000c10: 6f64 756c 653e 0100 0000 7322 0000 0004  odule>....s"....
-00000c20: 020c 0c0c 010c 010c 0214 0308 0108 0308  ................
-00000c30: 0108 0114 0108 0108 0108 0102 0502 010e  ................
-00000c40: fe                                       .
+00000060: 0100 6405 6407 6c07 6d09 5a09 0100 6405  ..d.d.l.m.Z...d.
+00000070: 6408 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  d.l.m.Z.m.Z.m.Z.
+00000080: 0100 6405 6409 6c0e 5a0e 6405 6409 6c0f  ..d.d.l.Z.d.d.l.
+00000090: 5a0f 6405 6409 6c10 5a10 6405 6409 6c11  Z.d.d.l.Z.d.d.l.
+000000a0: 5a11 6405 640a 6c12 6d13 5a13 6d14 5a14  Z.d.d.l.m.Z.m.Z.
+000000b0: 6d15 5a15 0100 6405 6409 6c16 5a16 6405  m.Z...d.d.l.Z.d.
+000000c0: 6409 6c17 5a17 6405 6409 6c18 5a18 0905  d.l.Z.d.d.l.Z...
+000000d0: 0905 640d 640b 640c 8401 5a19 6409 5300  ..d.d.d...Z.d.S.
+000000e0: 290e 7a68 0a09 6f62 6a65 6374 6976 6573  ).zh..objectives
+000000f0: 3a0a 090a 0909 5b20 5d20 2f61 6767 7265  :.....[ ] /aggre
+00000100: 6761 746f 722f 7265 636f 7264 730a 0909  gator/records...
+00000110: 0a09 095b 205d 202f 6865 616c 7468 5f73  ...[ ] /health_s
+00000120: 6361 6e73 2f70 6174 6873 0a09 090a 0909  cans/paths......
+00000130: 5b20 5d20 2f68 6561 6c74 685f 7363 616e  [ ] /health_scan
+00000140: 2f7b 2070 6174 6820 7d09 090a e901 0000  /{ path }.......
+00000150: 0029 01da 0e64 6f6e 655f 7769 7468 5f73  .)...done_with_s
+00000160: 6361 6e29 01da 0b70 6174 6873 5f70 6174  can)...paths_pat
+00000170: 6368 2901 da17 7468 655f 6865 616c 7468  ch)...the_health
+00000180: 5f73 6361 6e5f 7374 6172 7465 64e9 0000  _scan_started...
+00000190: 0000 2901 da1d 7265 7472 6965 7665 5f61  ..)...retrieve_a
+000001a0: 6767 7265 6761 746f 725f 7661 7269 6162  ggregator_variab
+000001b0: 6c65 7329 01da 0b61 6464 5f61 6e6f 6d61  les)...add_anoma
+000001c0: 6c79 2903 da05 466c 6173 6bda 0772 6571  ly)...Flask..req
+000001d0: 7565 7374 da07 6a73 6f6e 6966 794e 2903  uest..jsonifyN).
+000001e0: da07 6469 726e 616d 65da 046a 6f69 6eda  ..dirname..join.
+000001f0: 086e 6f72 6d70 6174 6863 0200 0000 0000  .normpathc......
+00000200: 0000 0000 0000 0900 0000 0500 0000 4300  ..............C.
+00000210: 0000 73dc 0000 007c 0164 016b 0572 0974  ..s....|.d.k.r.t
+00000220: 0064 027c 0083 0201 0074 0164 0383 017d  .d.|.....t.d...}
+00000230: 0209 0074 027c 027c 0064 048d 0201 007c  ...t.|.|.d.....|
+00000240: 026a 0364 0564 0667 0164 078d 0264 0864  .j.d.d.g.d...d.d
+00000250: 0984 0083 017d 037c 026a 0364 0a64 0667  .....}.|.j.d.d.g
+00000260: 0164 078d 0264 0b64 0c84 0083 017d 047c  .d...d.d.....}.|
+00000270: 026a 0364 0d64 0667 0164 078d 0264 0e64  .j.d.d.g.d...d.d
+00000280: 0f84 0083 017d 057c 026a 0364 1064 0667  .....}.|.j.d.d.g
+00000290: 0164 078d 0264 1164 1284 0083 017d 067c  .d...d.d.....}.|
+000002a0: 026a 0364 1364 0667 0164 078d 0264 1464  .j.d.d.g.d...d.d
+000002b0: 1584 0083 017d 077c 026a 0364 1664 0667  .....}.|.j.d.d.g
+000002c0: 0164 078d 0264 1764 1884 0083 017d 0874  .d...d.d.....}.t
+000002d0: 047c 0283 0101 0074 057c 0283 0101 007c  .|.....t.|.....|
+000002e0: 026a 0664 197c 0064 1a64 1b8d 0301 0064  .j.d.|.d.d.....d
+000002f0: 0053 0029 1c4e 7201 0000 007a 216f 7065  .S.).Nr....z!ope
+00000300: 6e69 6e67 2073 6361 6e20 7072 6f63 6573  ning scan proces
+00000310: 7320 6b65 6720 6f6e 2070 6f72 743a 7a11  s keg on port:z.
+00000320: 6167 6772 6567 6174 6f72 2068 6172 626f  aggregator harbo
+00000330: 7229 01da 1961 6767 7265 6761 746f 725f  r)...aggregator_
+00000340: 7072 6f63 6564 7572 655f 706f 7274 fa01  procedure_port..
+00000350: 2fda 0347 4554 2901 da07 6d65 7468 6f64  /..GET)...method
+00000360: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
+00000370: 0000 0600 0000 5300 0000 731a 0000 0074  ......S...s....t
+00000380: 0064 0167 0164 0167 0164 0167 0164 0167  .d.g.d.g.d.g.d.g
+00000390: 0164 029c 0483 0153 0029 034e da03 6765  .d.....S.).N..ge
+000003a0: 7429 04fa 242f 6865 616c 7468 5f73 6361  t)..$/health_sca
+000003b0: 6e2f 3c70 6174 683a 6865 616c 7468 5f73  n/<path:health_s
+000003c0: 6361 6e5f 7061 7468 3efa 132f 6865 616c  can_path>../heal
+000003d0: 7468 5f73 6361 6e73 2f70 6174 6873 fa03  th_scans/paths..
+000003e0: 2f6f 6efa 0a2f 616e 6f6d 616c 6965 7329  /on../anomalies)
+000003f0: 0172 0a00 0000 a900 7217 0000 0072 1700  .r......r....r..
+00000400: 0000 fa56 2f62 696f 7465 6368 2f76 656e  ...V/biotech/ven
+00000410: 7565 732f 7374 6167 6573 2f62 696f 7465  ues/stages/biote
+00000420: 6368 2f70 726f 6365 6475 7265 732f 6167  ch/procedures/ag
+00000430: 6772 6567 6174 6f72 5f70 726f 6365 6475  gregator_procedu
+00000440: 7265 2f70 726f 6365 7373 2f6b 6567 2f5f  re/process/keg/_
+00000450: 5f69 6e69 745f 5f2e 7079 da08 686f 6d65  _init__.py..home
+00000460: 5f67 6574 3500 0000 730c 0000 0002 0204  _get5...s.......
+00000470: 0104 0104 0104 0108 fc7a 1d6f 7065 6e5f  .........z.open_
+00000480: 6861 7262 6f72 2e3c 6c6f 6361 6c73 3e2e  harbor.<locals>.
+00000490: 686f 6d65 5f67 6574 7215 0000 0063 0000  home_getr....c..
+000004a0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+000004b0: 0000 5300 0000 f304 0000 0064 0153 00a9  ..S........d.S..
+000004c0: 024e da03 7965 7372 1700 0000 7217 0000  .N..yesr....r...
+000004d0: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+000004e0: da06 6f6e 5f67 6574 3f00 0000 f302 0000  ..on_get?.......
+000004f0: 0004 027a 1b6f 7065 6e5f 6861 7262 6f72  ...z.open_harbor
+00000500: 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f67 6574  .<locals>.on_get
+00000510: 7216 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000520: 0000 0200 0000 0a00 0000 5300 0000 7348  ..........S...sH
+00000530: 0000 007a 0c74 0083 007d 0074 0164 017c  ...z.t...}.t.d.|
+00000540: 0064 0119 0069 0183 0157 0053 0004 0074  .d...i...W.S...t
+00000550: 0279 2301 007d 0101 007a 0b74 037c 0183  .y#..}...z.t.|..
+00000560: 0101 0057 0059 0064 007d 017e 0164 0253  ...W.Y.d.}.~.d.S
+00000570: 0064 007d 017e 0177 0177 0029 034e da09  .d.}.~.w.w.).N..
+00000580: 616e 6f6d 616c 6965 73fa 0d6e 6f74 2070  anomalies..not p
+00000590: 6172 7365 6162 6c65 2904 7206 0000 0072  arseable).r....r
+000005a0: 0a00 0000 da09 4578 6365 7074 696f 6eda  ......Exception.
+000005b0: 0570 7269 6e74 2902 da14 6167 6772 6567  .print)...aggreg
+000005c0: 6174 6f72 5f76 6172 6961 626c 6573 da01  ator_variables..
+000005d0: 4572 1700 0000 7217 0000 0072 1800 0000  Er....r....r....
+000005e0: da0c 6f6e 5f61 6e6f 6d61 6c69 6573 4300  ..on_anomaliesC.
+000005f0: 0000 7316 0000 0002 0206 0102 0108 0108  ..s.............
+00000600: ff0e 0408 010a 0304 0208 8002 fa7a 216f  .............z!o
+00000610: 7065 6e5f 6861 7262 6f72 2e3c 6c6f 6361  pen_harbor.<loca
+00000620: 6c73 3e2e 6f6e 5f61 6e6f 6d61 6c69 6573  ls>.on_anomalies
+00000630: 7a0c 2f77 6169 7469 6e67 5f66 6f72 6300  z./waiting_forc.
+00000640: 0000 0000 0000 0000 0000 0008 0000 000a  ................
+00000650: 0000 0053 0000 0073 0801 0000 7a6b 7400  ...S...s....zkt.
+00000660: 8300 7d00 7c00 6401 1900 7d01 6700 7d02  ..}.|.d...}.g.}.
+00000670: 7c01 4400 5d58 7d03 6402 7d04 7a0a 7c00  |.D.]X}.d.}.z.|.
+00000680: 6401 1900 7c03 1900 6403 1900 7d04 5700  d...|...d...}.W.
+00000690: 6e09 0400 7401 7923 0100 0100 0100 5900  n...t.y#......Y.
+000006a0: 6e01 7700 6402 7d05 7a0a 7c00 6401 1900  n.w.d.}.z.|.d...
+000006b0: 7c03 1900 6404 1900 7d05 5700 6e09 0400  |...d...}.W.n...
+000006c0: 7401 7939 0100 0100 0100 5900 6e01 7700  t.y9......Y.n.w.
+000006d0: 6402 7d06 7a0a 7c00 6401 1900 7c03 1900  d.}.z.|.d...|...
+000006e0: 6405 1900 7d06 5700 6e09 0400 7401 794f  d...}.W.n...t.yO
+000006f0: 0100 0100 0100 5900 6e01 7700 7c01 7c03  ......Y.n.w.|.|.
+00000700: 1900 6406 1900 6407 1900 6408 6b03 7264  ..d...d...d.k.rd
+00000710: 7c02 a002 7c03 7c04 7c05 7c06 6409 9c04  |...|.|.|.|.d...
+00000720: a101 0100 710c 7403 640a 7c02 6901 8301  ....q.t.d.|.i...
+00000730: 5700 5300 0400 7401 7983 0100 7d07 0100  W.S...t.y...}...
+00000740: 7a0c 7404 640b 7c07 8302 0100 5700 5900  z.t.d.|.....W.Y.
+00000750: 6400 7d07 7e07 6402 5300 6400 7d07 7e07  d.}.~.d.S.d.}.~.
+00000760: 7701 7700 290c 4eda 1169 6e74 6572 6e61  w.w.).N..interna
+00000770: 6c5f 7374 6174 7573 6573 7220 0000 00da  l_statusesr ....
+00000780: 0b6f 6363 7572 7265 6e63 6573 da07 7265  .occurrences..re
+00000790: 636f 7264 73da 0574 696d 6573 da06 7374  cords..times..st
+000007a0: 6174 7573 da07 7072 6f63 6573 73da 0464  atus..process..d
+000007b0: 6f6e 6529 04da 0470 6174 6872 2700 0000  one)...pathr'...
+000007c0: 7228 0000 0072 2900 0000 da0b 7761 6974  r(...r).....wait
+000007d0: 696e 675f 666f 727a 0a65 7863 6570 7469  ing_forz.excepti
+000007e0: 6f6e 3a29 0572 0600 0000 7221 0000 00da  on:).r....r!....
+000007f0: 0661 7070 656e 6472 0a00 0000 7222 0000  .appendr....r"..
+00000800: 0029 0872 2300 0000 7226 0000 0072 2e00  .).r#...r&...r..
+00000810: 0000 da0b 7374 6174 7573 5f70 6174 6872  ....status_pathr
+00000820: 2700 0000 7228 0000 0072 2900 0000 7224  '...r(...r)...r$
+00000830: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00000840: 0000 da0e 6f6e 5f77 6169 7469 6e67 5f66  ....on_waiting_f
+00000850: 6f72 5400 0000 7350 0000 0002 0206 0108  orT...sP........
+00000860: 0104 0308 0104 0102 0114 010c 0104 0102  ................
+00000870: ff04 0302 0114 010c 0104 0102 ff04 0302  ................
+00000880: 0114 010c 0104 0102 ff14 0304 0102 0102  ................
+00000890: 0102 0102 0108 fc02 8002 0704 0108 ff0e  ................
+000008a0: 040a 010a 0104 0208 8002 fc7a 236f 7065  ...........z#ope
+000008b0: 6e5f 6861 7262 6f72 2e3c 6c6f 6361 6c73  n_harbor.<locals
+000008c0: 3e2e 6f6e 5f77 6169 7469 6e67 5f66 6f72  >.on_waiting_for
+000008d0: 7214 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000008e0: 0000 0300 0000 0400 0000 5300 0000 7328  ..........S...s(
+000008f0: 0000 0074 0083 007d 0069 007d 017c 0064  ...t...}.i.}.|.d
+00000900: 0119 0044 005d 067d 0264 027c 017c 023c  ...D.].}.d.|.|.<
+00000910: 0071 0974 017c 0183 0153 0029 034e 7226  .q.t.|...S.).Nr&
+00000920: 0000 00da 0029 0272 0600 0000 720a 0000  .....).r....r...
+00000930: 0029 0372 2300 0000 da09 7468 655f 7061  .).r#.....the_pa
+00000940: 7468 7372 2d00 0000 7217 0000 0072 1700  thsr-...r....r..
+00000950: 0000 7218 0000 00da 1c6f 6e5f 5f67 6574  ..r......on__get
+00000960: 5f5f 6865 616c 7468 5f73 6361 6e73 5f5f  __health_scans__
+00000970: 7061 7468 7384 0000 0073 0a00 0000 0602  paths....s......
+00000980: 0402 0c02 0a01 0802 7a31 6f70 656e 5f68  ........z1open_h
+00000990: 6172 626f 722e 3c6c 6f63 616c 733e 2e6f  arbor.<locals>.o
+000009a0: 6e5f 5f67 6574 5f5f 6865 616c 7468 5f73  n__get__health_s
+000009b0: 6361 6e73 5f5f 7061 7468 7372 1300 0000  cans__pathsr....
+000009c0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000009d0: 0001 0000 0053 0000 0072 1a00 0000 721b  .....S...r....r.
+000009e0: 0000 0072 1700 0000 2901 da10 6865 616c  ...r....)...heal
+000009f0: 7468 5f73 6361 6e5f 7061 7468 7217 0000  th_scan_pathr...
+00000a00: 0072 1700 0000 7218 0000 00da 1a6f 6e5f  .r....r......on_
+00000a10: 5f67 6574 5f5f 6865 616c 7468 5f73 6361  _get__health_sca
+00000a20: 6e5f 5f70 6174 688f 0000 0072 1e00 0000  n__path....r....
+00000a30: 7a2f 6f70 656e 5f68 6172 626f 722e 3c6c  z/open_harbor.<l
+00000a40: 6f63 616c 733e 2e6f 6e5f 5f67 6574 5f5f  ocals>.on__get__
+00000a50: 6865 616c 7468 5f73 6361 6e5f 5f70 6174  health_scan__pat
+00000a60: 687a 0730 2e30 2e30 2e30 4629 02da 0470  hz.0.0.0.0F)...p
+00000a70: 6f72 74da 0564 6562 7567 2907 7222 0000  ort..debug).r"..
+00000a80: 0072 0800 0000 7203 0000 00da 0572 6f75  .r....r......rou
+00000a90: 7465 7204 0000 0072 0200 0000 da03 7275  ter....r......ru
+00000aa0: 6e29 0972 3700 0000 7228 0000 00da 0361  n).r7...r(.....a
+00000ab0: 7070 7219 0000 0072 1d00 0000 7225 0000  ppr....r....r%..
+00000ac0: 0072 3100 0000 7234 0000 0072 3600 0000  .r1...r4...r6...
+00000ad0: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
+00000ae0: 0b6f 7065 6e5f 6861 7262 6f72 2500 0000  .open_harbor%...
+00000af0: 7330 0000 0008 040a 0108 0402 020c 030e  s0..............
+00000b00: 020a 010e 090a 010e 030a 010e 100a 010e  ................
+00000b10: 2f0a 010e 0a0a 0108 0408 0204 0402 0102  /...............
+00000b20: 0102 010a fd72 3c00 0000 2902 7205 0000  .....r<...).r...
+00000b30: 0072 0500 0000 291a da07 5f5f 646f 635f  .r....)...__doc_
+00000b40: 5fda 1573 7061 6365 732e 646f 6e65 5f77  _..spaces.done_w
+00000b50: 6974 685f 7363 616e 7202 0000 00da 1273  ith_scanr......s
+00000b60: 7061 6365 732e 7061 7468 735f 7061 7463  paces.paths_patc
+00000b70: 6872 0300 0000 da1e 7370 6163 6573 2e74  hr......spaces.t
+00000b80: 6865 5f68 6561 6c74 685f 7363 616e 5f73  he_health_scan_s
+00000b90: 7461 7274 6564 7204 0000 00da 3962 696f  tartedr.....9bio
+00000ba0: 7465 6368 2e70 726f 6365 6475 7265 732e  tech.procedures.
+00000bb0: 6167 6772 6567 6174 6f72 5f70 726f 6365  aggregator_proce
+00000bc0: 6475 7265 2e70 726f 6365 7373 2e76 6172  dure.process.var
+00000bd0: 6961 626c 6573 7206 0000 0072 0700 0000  iablesr....r....
+00000be0: da05 666c 6173 6b72 0800 0000 7209 0000  ..flaskr....r...
+00000bf0: 0072 0a00 0000 da04 7269 6368 da04 6a73  .r......rich..js
+00000c00: 6f6e da07 7061 7468 6c69 62da 026f 73da  on..pathlib..os.
+00000c10: 076f 732e 7061 7468 720b 0000 0072 0c00  .os.pathr....r..
+00000c20: 0000 720d 0000 00da 0373 7973 da09 7468  ..r......sys..th
+00000c30: 7265 6164 696e 67da 0474 696d 6572 3c00  reading..timer<.
+00000c40: 0000 7217 0000 0072 1700 0000 7217 0000  ..r....r....r...
+00000c50: 0072 1800 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000c60: 0100 0000 7324 0000 0004 020c 0c0c 010c  ....s$..........
+00000c70: 010c 020c 0114 0308 0108 0308 0108 0114  ................
+00000c80: 0108 0108 0108 0102 0502 010e fe         .............
```

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 23:33:20 2024 UTC, .py size: 9825 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,272 +1,252 @@
-00000000: 6f0d 0d0a 0000 0000 40ff 2266 6126 0000  o.......@."fa&..
+00000000: 6f0d 0d0a 0000 0000 093a 2366 1c22 0000  o........:#f."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
-00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6405 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6406 6c08 6d09 5a09 0100 6400 6407 6c0a  d.l.m.Z...d.d.l.
-00000070: 6d0a 5a0a 0100 6400 6408 6c0b 5a0b 6400  m.Z...d.d.l.Z.d.
-00000080: 6408 6c0c 5a0c 6400 6408 6c0d 5a0d 0900  d.l.Z.d.d.l.Z...
-00000090: 6409 640a 8400 5a0e 6408 5300 290b e900  d.d...Z.d.S.)...
-000000a0: 0000 0029 01da 1272 6574 7269 6576 655f  ...)...retrieve_
-000000b0: 7661 7269 6162 6c65 73e9 0100 0000 2901  variables.....).
-000000c0: da0e 6174 7461 6368 5f72 6563 6f72 6473  ..attach_records
-000000d0: 2901 da27 6c65 6172 6e5f 6966 5f67 6c6f  )..'learn_if_glo
-000000e0: 6261 6c5f 7469 6d65 5f6c 696d 6974 5f77  bal_time_limit_w
-000000f0: 6173 5f65 7863 6565 6465 6429 01da 1670  as_exceeded)...p
-00000100: 6172 7365 5f70 5f65 7870 6563 745f 7265  arse_p_expect_re
-00000110: 636f 7264 7329 01da 0d73 686f 775f 7661  cords)...show_va
-00000120: 7269 6162 6c65 2901 da06 7070 7269 6e74  riable)...pprint
-00000130: 4e63 0000 0000 0000 0000 0000 0000 0d00  Nc..............
-00000140: 0000 0b00 0000 4300 0000 73ae 0600 0074  ......C...s....t
-00000150: 0083 007d 007c 0064 0119 007d 017c 0064  ...}.|.d...}.|.d
-00000160: 0219 007d 027c 0064 0319 0064 0419 007d  ...}.|.d...d...}
-00000170: 0369 007d 0467 007d 057c 0244 0090 035d  .i.}.g.}.|.D...]
-00000180: 1f7d 067c 027c 0619 007d 077c 0764 0519  .}.|.|...}.|.d..
-00000190: 007d 0809 007a 2d64 067c 027c 0619 0064  .}...z-d.|.|...d
-000001a0: 0619 0076 0072 4f74 017c 027c 0619 0064  ...v.rOt.|.|...d
-000001b0: 0619 0064 0619 0083 0164 006b 0372 4f7c  ...d.....d.k.rO|
-000001c0: 027c 0619 0064 0619 0064 0619 00a0 02a1  .|...d...d......
-000001d0: 007d 097c 0964 076b 0272 4b64 087c 0864  .}.|.d.k.rKd.|.d
-000001e0: 093c 006e 0464 0a7c 0864 093c 0057 006e  .<.n.d.|.d.<.W.n
-000001f0: 1b04 0074 0379 6b01 007d 0a01 007a 0f74  ...t.yk..}...z.t
-00000200: 0464 0b7c 0a83 0201 0064 0c7c 0864 093c  .d.|.....d.|.d.<
-00000210: 0057 0059 0064 007d 0a7e 0a6e 0564 007d  .W.Y.d.}.~.n.d.}
-00000220: 0a7e 0a77 0177 0074 057c 0683 0101 0074  .~.w.w.t.|.....t
-00000230: 067c 0683 0101 0009 007a 687c 0864 0d19  .|.......zh|.d..
-00000240: 0064 086b 0272 dc7c 0864 0e19 0064 0a6b  .d.k.r.|.d...d.k
-00000250: 0272 dc7c 0864 0f19 0064 0a6b 0272 dc74  .r.|.d...d.k.r.t
-00000260: 07a0 07a1 0074 087c 027c 0619 0064 1019  .....t.|.|...d..
-00000270: 0064 1119 0083 0118 007d 0b7c 0b64 126b  .d.......}.|.d.k
-00000280: 0572 dc7a 087c 027c 0619 0064 1319 007d  .r.z.|.|...d...}
-00000290: 0857 006e 0b04 0074 0379 ad01 0001 0001  .W.n...t.y......
-000002a0: 0064 147d 0859 006e 0177 007c 0664 1567  .d.}.Y.n.w.|.d.g
-000002b0: 007c 0864 0764 169c 057c 0064 0219 007c  .|.d.d...|.d...|
-000002c0: 0619 0064 173c 0064 187c 0064 0219 007c  ...d.<.d.|.d...|
-000002d0: 0619 0064 1919 0064 063c 0064 1a7c 0064  ...d...d.<.d.|.d
-000002e0: 0219 007c 0619 0064 0519 0064 1b3c 007c  ...|...d...d.<.|
-000002f0: 0064 0219 007c 0619 0064 0619 0064 0619  .d...|...d...d..
-00000300: 00a0 09a1 0001 0057 006e 1904 0074 0379  .......W.n...t.y
-00000310: f601 007d 0a01 007a 0d74 0464 1c74 0aa0  ...}...z.t.d.t..
-00000320: 0ba1 0083 0201 0057 0059 0064 007d 0a7e  .......W.Y.d.}.~
-00000330: 0a6e 0564 007d 0a7e 0a77 0177 0009 007a  .n.d.}.~.w.w...z
-00000340: 3a7c 0864 1d19 0064 086b 0290 0172 317c  :|.d...d.k...r1|
-00000350: 0864 1e19 0064 0a6b 0290 0172 3174 07a0  .d...d.k...r1t..
-00000360: 07a1 0074 087c 027c 0619 0064 1019 0064  ...t.|.|...d...d
-00000370: 1119 0083 0118 007d 0b7c 0b64 1f6b 0590  .......}.|.d.k..
-00000380: 0172 317c 0664 2067 007c 0864 219c 047c  .r1|.d g.|.d!..|
-00000390: 0064 0219 007c 0619 0064 173c 0064 187c  .d...|...d.<.d.|
-000003a0: 0064 0219 007c 0619 0064 1919 0064 063c  .d...|...d...d.<
-000003b0: 0057 006e 1804 0074 0390 0179 4a01 007d  .W.n...t...yJ..}
-000003c0: 0a01 007a 0b74 0464 1c7c 0a83 0201 0057  ...z.t.d.|.....W
-000003d0: 0059 0064 007d 0a7e 0a6e 0564 007d 0a7e  .Y.d.}.~.n.d.}.~
-000003e0: 0a77 0177 0009 007a 6c7c 0864 0e19 0064  .w.w...zl|.d...d
-000003f0: 086b 0290 0172 b77c 0864 0f19 0064 0a6b  .k...r.|.d...d.k
-00000400: 0290 0172 b774 07a0 07a1 0074 087c 027c  ...r.t.....t.|.|
-00000410: 0619 0064 1019 0064 1119 0083 0118 007d  ...d...d.......}
-00000420: 0b7c 0b64 226b 0590 0172 b77a 087c 027c  .|.d"k...r.z.|.|
-00000430: 0619 0064 1319 007d 0857 006e 0c04 0074  ...d...}.W.n...t
-00000440: 0390 0179 8201 0001 0001 0064 147d 0859  ...y.......d.}.Y
-00000450: 006e 0177 007c 0664 2367 007c 0864 0764  .n.w.|.d#g.|.d.d
-00000460: 169c 057c 0064 0219 007c 0619 0064 173c  ...|.d...|...d.<
-00000470: 0064 187c 0064 0219 007c 0619 0064 1919  .d.|.d...|...d..
-00000480: 0064 063c 0064 1a7c 0064 0219 007c 0619  .d.<.d.|.d...|..
-00000490: 0064 0519 0064 1b3c 007c 0064 0219 007c  .d...d.<.|.d...|
-000004a0: 0619 0064 0619 0064 0619 00a0 09a1 0001  ...d...d........
-000004b0: 0074 0c64 247c 0669 0183 0101 0057 006e  .t.d$|.i.....W.n
-000004c0: 1a04 0074 0390 0179 d201 007d 0a01 007a  ...t...y...}...z
-000004d0: 0d74 0464 1c74 0aa0 0ba1 0083 0201 0057  .t.d.t.........W
-000004e0: 0059 0064 007d 0a7e 0a6e 0564 007d 0a7e  .Y.d.}.~.n.d.}.~
-000004f0: 0a77 0177 0009 007a b47c 0864 0e19 0064  .w.w...z.|.d...d
-00000500: 086b 027c 0864 0919 0064 086b 027c 0864  .k.|.d...d.k.|.d
-00000510: 2519 0064 0a6b 0274 0d7c 027c 0619 0064  %..d.k.t.|.|...d
-00000520: 1019 0064 1119 0083 0164 266b 0574 0d7c  ...d.....d&k.t.|
-00000530: 027c 0619 0064 2719 0083 0164 286b 0274  .|...d'....d(k.t
-00000540: 07a0 07a1 0074 087c 027c 0619 0064 1019  .....t.|.|...d..
-00000550: 0064 1119 0083 0118 0064 299c 067d 0c7c  .d.......d)..}.|
-00000560: 0864 0e19 0064 086b 0290 0272 877c 0864  .d...d.k...r.|.d
-00000570: 0919 0064 086b 0290 0272 877c 0864 2519  ...d.k...r.|.d%.
-00000580: 0064 0a6b 0290 0272 8774 0d7c 027c 0619  .d.k...r.t.|.|..
-00000590: 0064 1019 0064 1119 0083 0164 266b 0590  .d...d.....d&k..
-000005a0: 0272 8774 0d7c 027c 0619 0064 2719 0083  .r.t.|.|...d'...
-000005b0: 0164 286b 0290 0272 8774 07a0 07a1 0074  .d(k...r.t.....t
-000005c0: 087c 027c 0619 0064 1019 0064 1119 0083  .|.|...d...d....
-000005d0: 0118 007d 0b7c 0b64 2a6b 0590 0272 8774  ...}.|.d*k...r.t
-000005e0: 0c64 2b7c 0669 0183 0101 007a 087c 027c  .d+|.i.....z.|.|
-000005f0: 0619 0064 1319 007d 0857 006e 0c04 0074  ...d...}.W.n...t
-00000600: 0390 0279 6201 0001 0001 0064 147d 0859  ...yb......d.}.Y
-00000610: 006e 0177 007c 0664 2c67 007c 0864 0764  .n.w.|.d,g.|.d.d
-00000620: 2d9c 057c 0064 0219 007c 0619 0064 173c  -..|.d...|...d.<
-00000630: 0064 187c 0064 0219 007c 0619 0064 1919  .d.|.d...|...d..
-00000640: 0064 063c 007c 0064 0219 007c 0619 0064  .d.<.|.d...|...d
-00000650: 0619 0064 0619 00a0 09a1 0001 0057 006e  ...d.........W.n
-00000660: 1804 0074 0390 0279 a001 007d 0a01 007a  ...t...y...}...z
-00000670: 0b74 0464 2e7c 0a83 0201 0057 0059 0064  .t.d.|.....W.Y.d
-00000680: 007d 0a7e 0a6e 0564 007d 0a7e 0a77 0177  .}.~.n.d.}.~.w.w
-00000690: 0009 007a 367c 0864 0e19 0064 086b 0290  ...z6|.d...d.k..
-000006a0: 0272 d77c 0864 0f19 0064 086b 0290 0272  .r.|.d...d.k...r
-000006b0: d77c 0864 2519 0064 0a6b 0290 0272 d77c  .|.d%..d.k...r.|
-000006c0: 0864 0919 0064 086b 0390 0272 d77c 0664  .d...d.k...r.|.d
-000006d0: 2f67 007c 0864 0764 169c 057c 0064 0219  /g.|.d.d...|.d..
-000006e0: 007c 0619 0064 173c 0064 187c 0064 0219  .|...d.<.d.|.d..
-000006f0: 007c 0619 0064 1919 0064 063c 0057 006e  .|...d...d.<.W.n
-00000700: 1a04 0074 0390 0279 f201 007d 0a01 007a  ...t...y...}...z
-00000710: 0d74 0464 3074 0aa0 0ba1 0083 0201 0057  .t.d0t.........W
-00000720: 0059 0064 007d 0a7e 0a6e 0564 007d 0a7e  .Y.d.}.~.n.d.}.~
-00000730: 0a77 0177 0009 0009 007a 287c 0864 0919  .w.w.....z(|.d..
-00000740: 0064 0a6b 0290 0372 1c7c 0864 0e19 0064  .d.k...r.|.d...d
-00000750: 086b 0290 0372 1c7c 0864 2519 0064 086b  .k...r.|.d%..d.k
-00000760: 0290 0372 1c7c 0864 3119 0064 086b 0290  ...r.|.d1..d.k..
-00000770: 0372 1c64 187c 0064 0219 007c 0619 0064  .r.d.|.d...|...d
-00000780: 1919 0064 063c 0057 0071 1704 0074 0390  ...d.<.W.q...t..
-00000790: 0379 3701 007d 0a01 007a 0d74 0464 3074  .y7..}...z.t.d0t
-000007a0: 0aa0 0ba1 0083 0201 0057 0059 0064 007d  .........W.Y.d.}
-000007b0: 0a7e 0a71 1764 007d 0a7e 0a77 0177 007c  .~.q.d.}.~.w.w.|
-000007c0: 0244 005d 1a7d 067c 027c 0619 0064 1919  .D.].}.|.|...d..
-000007d0: 0064 0619 0064 186b 0390 0372 537c 05a0  .d...d.k...rS|..
-000007e0: 0e7c 067c 0064 0219 007c 0619 0064 329c  .|.|.d...|...d2.
-000007f0: 02a1 0101 0090 0371 3a7c 0553 0029 334e  .......q:|.S.)3N
-00000800: da0d 7265 636f 7264 735f 6c65 7665 6cda  ..records_level.
-00000810: 1169 6e74 6572 6e61 6c5f 7374 6174 7573  .internal_status
-00000820: 6573 da0f 696e 7472 6f5f 7661 7269 6162  es..intro_variab
-00000830: 6c65 73da 0a74 696d 655f 6c69 6d69 74da  les..time_limit.
-00000840: 0b6f 6363 7572 7265 6e63 6573 da07 7072  .occurrences..pr
-00000850: 6f63 6573 7354 da03 7965 737a 1573 6361  ocessT..yesz.sca
-00000860: 6e20 7072 6f63 6573 7320 6973 2061 6c69  n process is ali
-00000870: 7665 da02 6e6f 7a1e 7072 6f63 6573 7320  ve..noz.process 
-00000880: 616c 6976 6520 6368 6563 6b20 6578 6365  alive check exce
-00000890: 7074 696f 6e3a da07 756e 6b6e 6f77 6e7a  ption:..unknownz
-000008a0: 1c73 6361 6e20 7072 6f63 6573 7320 7665  .scan process ve
-000008b0: 6e74 7572 6520 7374 6172 7465 647a 1473  nture startedz.s
-000008c0: 6361 6e20 7072 6f63 6573 7320 7374 6172  can process star
-000008d0: 7465 647a 2073 6361 6e20 7072 6f63 6573  tedz scan proces
-000008e0: 7320 6e6f 7469 6669 6564 2061 6767 7265  s notified aggre
-000008f0: 6761 746f 72da 0574 696d 6573 7a0f 7665  gator..timesz.ve
-00000900: 6e74 7572 6520 7374 6172 7465 64e9 1e00  nture started...
-00000910: 0000 da0a 6f63 6375 7265 6e63 6573 7a09  ....occurencesz.
-00000920: 6e6f 7420 666f 756e 647a 6741 6674 6572  not foundzgAfter
-00000930: 2033 3020 7365 636f 6e64 732c 2074 6865   30 seconds, the
-00000940: 2061 6674 6572 2070 726f 6365 7373 206c   after process l
-00000950: 696e 6520 7761 7320 6e6f 7420 7265 6163  ine was not reac
-00000960: 6865 6420 616e 6420 7468 6520 7072 6f63  hed and the proc
-00000970: 6573 7320 6469 6420 6e6f 7420 6e6f 7469  ess did not noti
-00000980: 6679 2074 6865 2061 6767 7265 6761 746f  fy the aggregato
-00000990: 722e 2905 da04 7061 7468 da05 616c 6172  r.)...path..alar
-000009a0: 6dfa 0b61 6c61 726d 206e 6f74 6573 720d  m..alarm notesr.
-000009b0: 0000 00da 0665 7869 7465 64da 0f72 6573  .....exited..res
-000009c0: 756c 7473 5f6f 665f 7363 616e da04 646f  ults_of_scan..do
-000009d0: 6e65 da06 7374 6174 7573 7a3a 5468 6520  ne..statusz:The 
-000009e0: 7072 6f63 6573 7320 6469 646e 2774 206e  process didn't n
-000009f0: 6f74 6966 7920 7468 6520 6167 6772 6567  otify the aggreg
-00000a00: 6174 6f72 2077 6974 6869 6e20 3520 7365  ator within 5 se
-00000a10: 636f 6e64 732e 7a10 646f 6e65 2072 6561  conds.z.done rea
-00000a20: 736f 6e20 6769 7665 7a23 7072 6f63 6573  son givez#proces
-00000a30: 7320 6e6f 6e2d 6e6f 7469 6669 6361 7469  s non-notificati
-00000a40: 6f6e 2065 7863 6570 7469 6f6e 3a7a 1473  on exception:z.s
-00000a50: 6361 6e20 7072 6f63 6573 7320 7374 6f70  can process stop
-00000a60: 7065 647a 1c73 6361 6e20 7072 6f63 6565  pedz.scan procee
-00000a70: 6473 2077 6572 6520 7265 7472 6965 7665  ds were retrieve
-00000a80: 64e9 0f00 0000 7a5d 5468 6520 7363 616e  d.....z]The scan
-00000a90: 2070 726f 6365 7373 2077 6173 2073 746f   process was sto
-00000aa0: 7070 6564 2c20 6275 7420 3135 2073 6563  pped, but 15 sec
-00000ab0: 6f6e 6473 2068 6176 6520 7061 7373 6564  onds have passed
-00000ac0: 2061 6e64 2074 6865 2070 726f 6365 6564   and the proceed
-00000ad0: 7320 7765 7265 206e 6f74 2072 6574 7269  s were not retri
-00000ae0: 6576 6564 2e29 0472 1500 0000 7216 0000  eved.).r....r...
-00000af0: 0072 1700 0000 720d 0000 00e9 1400 0000  .r....r.........
-00000b00: 7a50 4166 7465 7220 3230 2073 6563 6f6e  zPAfter 20 secon
-00000b10: 6473 2c20 7468 6520 7072 6f63 6573 7320  ds, the process 
-00000b20: 6469 6420 6e6f 7420 6e6f 7469 6679 2074  did not notify t
-00000b30: 6865 2061 6767 7265 6761 746f 7220 7468  he aggregator th
-00000b40: 6174 2069 7420 6861 6420 7374 6172 7465  at it had starte
-00000b50: 642e 7a18 7072 6f63 6573 7320 6d61 7920  d.z.process may 
-00000b60: 6861 7665 2073 746f 7070 6564 7a18 7363  have stoppedz.sc
-00000b70: 616e 2070 726f 6365 7373 2077 6173 2073  an process was s
-00000b80: 746f 7070 6564 7203 0000 00da 0772 6563  toppedr......rec
-00000b90: 6f72 6473 7201 0000 0029 06da 0131 da01  ordsr....)...1..
-00000ba0: 32da 0133 da01 34da 0136 da01 37e9 0a00  2..3..4..6..7...
-00000bb0: 0000 7a2b 7265 636f 7264 7320 7765 7265  ..z+records were
-00000bc0: 206e 6f74 2072 6574 7269 6576 6564 2061   not retrieved a
-00000bd0: 6674 6572 2031 3020 7365 636f 6e64 737a  fter 10 secondsz
-00000be0: 2d41 6674 6572 2031 3020 7365 636f 6e64  -After 10 second
-00000bf0: 732c 206e 6f20 7072 6f63 6573 7320 6c6f  s, no process lo
-00000c00: 6773 2077 6572 6520 666f 756e 642e 2905  gs were found.).
-00000c10: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00000c20: 1400 0000 7218 0000 007a 2870 726f 6365  ....r....z(proce
-00000c30: 7373 206c 6f67 7320 7469 6d65 206c 696d  ss logs time lim
-00000c40: 6974 2063 6865 636b 2065 7863 6570 7469  it check excepti
-00000c50: 6f6e 3a7a 3054 6865 2070 726f 6365 7373  on:z0The process
-00000c60: 2065 7869 7465 6420 6265 666f 7265 2072   exited before r
-00000c70: 6573 756c 7473 2063 6f75 6c64 2062 6520  esults could be 
-00000c80: 7365 6e74 2e7a 1a70 6172 7365 2061 6e64  sent.z.parse and
-00000c90: 2063 6865 636b 2065 7863 6570 7469 6f6e   check exception
-00000ca0: 3a7a 1b73 6361 6e20 7265 636f 7264 7320  :z.scan records 
-00000cb0: 7765 7265 2072 6574 7269 6576 6564 2902  were retrieved).
-00000cc0: 7215 0000 00da 0969 6e74 6572 6e61 6c73  r......internals
-00000cd0: 290f 7202 0000 00da 0474 7970 65da 0869  ).r......type..i
-00000ce0: 735f 616c 6976 65da 0945 7863 6570 7469  s_alive..Excepti
-00000cf0: 6f6e da05 7072 696e 7472 0400 0000 7205  on..printr....r.
-00000d00: 0000 00da 0474 696d 65da 0566 6c6f 6174  .....time..float
-00000d10: da09 7465 726d 696e 6174 65da 0974 7261  ..terminate..tra
-00000d20: 6365 6261 636b da0a 666f 726d 6174 5f65  ceback..format_e
-00000d30: 7863 7207 0000 00da 036c 656e da06 6170  xcr......len..ap
-00000d40: 7065 6e64 290d da14 6167 6772 6567 6174  pend)...aggregat
-00000d50: 6f72 5f76 6172 6961 626c 6573 7209 0000  or_variablesr...
-00000d60: 0072 0a00 0000 720c 0000 00da 0873 7461  .r....r......sta
-00000d70: 7475 7365 73da 0a75 6e66 696e 6973 6865  tuses..unfinishe
-00000d80: 64da 0b73 7461 7475 735f 7061 7468 da0e  d..status_path..
-00000d90: 7374 6174 7573 5f6f 665f 7061 7468 720d  status_of_pathr.
-00000da0: 0000 00da 0561 6c69 7665 da01 45da 0765  .....alive..E..e
-00000db0: 6c61 7073 6564 da05 646f 6f72 73a9 0072  lapsed..doors..r
-00000dc0: 3b00 0000 fa71 2f62 696f 7465 6368 2f76  ;....q/biotech/v
-00000dd0: 656e 7565 732f 7374 6167 6573 2f62 696f  enues/stages/bio
-00000de0: 7465 6368 2f70 726f 6365 6475 7265 732f  tech/procedures/
-00000df0: 6167 6772 6567 6174 6f72 5f70 726f 6365  aggregator_proce
-00000e00: 6475 7265 2f70 726f 6365 7373 2f6d 6f76  dure/process/mov
-00000e10: 6573 2f73 7461 7475 735f 6368 6563 6b5f  es/status_check_
-00000e20: 6d6f 6e69 746f 722f 7468 655f 7068 7973  monitor/the_phys
-00000e30: 6963 616c 2e70 79da 2470 6172 7365 5f61  ical.py.$parse_a
-00000e40: 6e64 5f63 6865 636b 5f69 735f 616c 6976  nd_check_is_aliv
-00000e50: 655f 6f66 5f73 7461 7475 7365 7321 0000  e_of_statuses!..
-00000e60: 0073 6401 0000 0601 0802 0801 0c01 0402  .sd.............
-00000e70: 0401 0a01 0802 0801 0202 0204 1001 1801  ................
-00000e80: 1401 0801 0a01 0802 0480 0e02 0a01 1401  ................
-00000e90: 0880 02fe 0805 0803 0205 020c 0c02 0c01  ................
-00000ea0: 0c01 1c02 0802 0201 1001 0c01 0801 02ff  ................
-00000eb0: 0204 0202 0201 0202 0202 12f8 140b 1401  ................
-00000ec0: 1802 0480 0e03 0e01 0c01 0880 02fe 0205  ................
-00000ed0: 0206 0e02 0e01 1c02 0a02 0202 0202 0201  ................
-00000ee0: 0202 12fa 1409 0480 1002 0a01 0c01 0880  ................
-00000ef0: 02fe 0205 0208 0e02 0e01 1c02 0a02 0201  ................
-00000f00: 1001 0e01 0801 02ff 0204 0202 0201 0202  ................
-00000f10: 0202 12f8 140b 1401 1801 0202 0401 06ff  ................
-00000f20: 0480 1003 0e01 0c01 0880 02fe 0205 0212  ................
-00000f30: 0a02 0a01 0a01 1601 1201 1a01 06fa 0e0b  ................
-00000f40: 0e01 0e01 1a01 1602 1c02 0a02 0201 0401  ................
-00000f50: 06ff 0204 1001 0e01 0801 02ff 0204 0202  ................
-00000f60: 0201 0202 0202 12f8 140b 1801 0480 1004  ................
-00000f70: 0a01 0c01 0880 02fe 0206 020c 0e02 0e01  ................
-00000f80: 0e02 0e02 0203 0202 0201 0201 0202 12f9  ................
-00000f90: 140a 0480 1002 0e01 0c01 0880 02fe 0205  ................
-00000fa0: 0208 0203 0e02 0e02 0e01 0e02 1402 0480  ................
-00000fb0: 1002 0e01 0c01 0880 02fe 0806 1601 0401  ................
-00000fc0: 0201 0a01 08fe 0480 0406 723d 0000 0029  ..........r=...)
-00000fd0: 0fda 3962 696f 7465 6368 2e70 726f 6365  ..9biotech.proce
-00000fe0: 6475 7265 732e 6167 6772 6567 6174 6f72  dures.aggregator
-00000ff0: 5f70 726f 6365 6475 7265 2e70 726f 6365  _procedure.proce
-00001000: 7373 2e76 6172 6961 626c 6573 7202 0000  ss.variablesr...
-00001010: 0072 1e00 0000 7204 0000 00da 2761 6c61  .r....r.....'ala
-00001020: 726d 5f63 6865 636b 732e 676c 6f62 616c  rm_checks.global
-00001030: 5f74 696d 655f 6c69 6d69 745f 6578 6365  _time_limit_exce
-00001040: 6564 6564 7205 0000 00da 3062 696f 7465  ededr.....0biote
-00001050: 6368 2e74 6f70 6963 732e 7072 6f63 6573  ch.topics.proces
-00001060: 735f 6f6e 2e70 5f65 7870 6563 742e 7061  s_on.p_expect.pa
-00001070: 7273 655f 7265 636f 7264 7372 0600 0000  rse_recordsr....
-00001080: da1c 6269 6f74 6563 682e 746f 7069 6373  ..biotech.topics
-00001090: 2e73 686f 772e 7661 7269 6162 6c65 7207  .show.variabler.
-000010a0: 0000 0072 0800 0000 722b 0000 0072 2e00  ...r....r+...r..
-000010b0: 0000 da04 7269 6368 723d 0000 0072 3b00  ....richr=...r;.
-000010c0: 0000 723b 0000 0072 3b00 0000 723c 0000  ..r;...r;...r<..
-000010d0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000010e0: 1600 0000 0c07 0c03 0c02 0c02 0c01 0c03  ................
-000010f0: 0801 0801 0803 0205 0c04                 ..........
+00000020: 0002 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
+00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
+00000050: 0100 6404 6405 6c05 6d06 5a06 0100 6404  ..d.d.l.m.Z...d.
+00000060: 6406 6c07 6d08 5a08 0100 6400 6407 6c09  d.l.m.Z...d.d.l.
+00000070: 6d0a 5a0a 0100 6400 6408 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
+00000080: 0100 6400 6409 6c0d 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
+00000090: 640a 6c0e 5a0e 6400 640a 6c0f 5a0f 6400  d.l.Z.d.d.l.Z.d.
+000000a0: 640a 6c10 5a10 0900 640b 640c 8400 5a11  d.l.Z...d.d...Z.
+000000b0: 640a 5300 290d e900 0000 0029 01da 1272  d.S.)......)...r
+000000c0: 6574 7269 6576 655f 7661 7269 6162 6c65  etrieve_variable
+000000d0: 7329 01da 0b61 6464 5f61 6e6f 6d61 6c79  s)...add_anomaly
+000000e0: 2901 da0f 7061 7273 655f 6578 6365 7074  )...parse_except
+000000f0: 696f 6ee9 0100 0000 2901 da0e 6174 7461  ion.....)...atta
+00000100: 6368 5f72 6563 6f72 6473 2901 da27 6c65  ch_records)..'le
+00000110: 6172 6e5f 6966 5f67 6c6f 6261 6c5f 7469  arn_if_global_ti
+00000120: 6d65 5f6c 696d 6974 5f77 6173 5f65 7863  me_limit_was_exc
+00000130: 6565 6465 6429 01da 1670 6172 7365 5f70  eeded)...parse_p
+00000140: 5f65 7870 6563 745f 7265 636f 7264 7329  _expect_records)
+00000150: 01da 0d73 686f 775f 7661 7269 6162 6c65  ...show_variable
+00000160: 2901 da06 7070 7269 6e74 4e63 0000 0000  )...pprintNc....
+00000170: 0000 0000 0000 0000 0b00 0000 0b00 0000  ................
+00000180: 4300 0000 7330 0500 0074 0083 007d 007c  C...s0...t...}.|
+00000190: 0064 0119 007d 017c 0064 0219 007d 027c  .d...}.|.d...}.|
+000001a0: 0064 0319 0064 0419 007d 0369 007d 0467  .d...d...}.i.}.g
+000001b0: 007d 057c 0244 0090 025d 607d 067c 027c  .}.|.D...]`}.|.|
+000001c0: 0619 007d 077c 0764 0519 007d 0809 007a  ...}.|.d...}...z
+000001d0: 2664 067c 027c 0619 0076 0072 4874 017c  &d.|.|...v.rHt.|
+000001e0: 027c 0619 0064 0619 0083 0174 026b 0272  .|...d.....t.k.r
+000001f0: 4764 067c 027c 0619 0064 0619 0076 0072  Gd.|.|...d...v.r
+00000200: 477c 027c 0619 0064 0619 0064 0719 0083  G|.|...d...d....
+00000210: 007c 0864 083c 0009 0057 006e 2004 0074  .|.d.<...W.n ..t
+00000220: 0379 6901 007d 0901 007a 1474 0464 097c  .yi..}...z.t.d.|
+00000230: 0674 057c 0983 0164 0a9c 0383 0101 0064  .t.|...d.......d
+00000240: 0b7c 0864 083c 0057 0059 0064 007d 097e  .|.d.<.W.Y.d.}.~
+00000250: 096e 0564 007d 097e 0977 0177 0074 067c  .n.d.}.~.w.w.t.|
+00000260: 0683 0101 0074 077c 0683 0101 0009 007a  .....t.|.......z
+00000270: 687c 0864 0c19 0064 0d6b 0272 da7c 0864  h|.d...d.k.r.|.d
+00000280: 0e19 0064 0f6b 0272 da7c 0864 1019 0064  ...d.k.r.|.d...d
+00000290: 0f6b 0272 da74 08a0 08a1 0074 097c 027c  .k.r.t.....t.|.|
+000002a0: 0619 0064 1119 0064 1219 0083 0118 007d  ...d...d.......}
+000002b0: 0a7c 0a64 136b 0572 da7a 087c 027c 0619  .|.d.k.r.z.|.|..
+000002c0: 0064 1419 007d 0857 006e 0b04 0074 0379  .d...}.W.n...t.y
+000002d0: ab01 0001 0001 0064 157d 0859 006e 0177  .......d.}.Y.n.w
+000002e0: 007c 0664 1667 007c 0864 1764 189c 057c  .|.d.g.|.d.d...|
+000002f0: 0064 0219 007c 0619 0064 193c 0064 1a7c  .d...|...d.<.d.|
+00000300: 0064 0219 007c 0619 0064 1b19 0064 063c  .d...|...d...d.<
+00000310: 0064 1c7c 0064 0219 007c 0619 0064 0519  .d.|.d...|...d..
+00000320: 0064 1d3c 007c 0064 0219 007c 0619 0064  .d.<.|.d...|...d
+00000330: 0619 0064 0619 00a0 0aa1 0001 0057 006e  ...d.........W.n
+00000340: 1c04 0074 0379 f701 007d 0901 007a 1074  ...t.y...}...z.t
+00000350: 0464 1e7c 0674 057c 0983 0164 0a9c 0383  .d.|.t.|...d....
+00000360: 0101 0057 0059 0064 007d 097e 096e 0564  ...W.Y.d.}.~.n.d
+00000370: 007d 097e 0977 0177 0009 007a 3a7c 0864  .}.~.w.w...z:|.d
+00000380: 1f19 0064 0d6b 0290 0172 327c 0864 2019  ...d.k...r2|.d .
+00000390: 0064 0f6b 0290 0172 3274 08a0 08a1 0074  .d.k...r2t.....t
+000003a0: 097c 027c 0619 0064 1119 0064 1219 0083  .|.|...d...d....
+000003b0: 0118 007d 0a7c 0a64 216b 0590 0172 327c  ...}.|.d!k...r2|
+000003c0: 0664 2267 007c 0864 239c 047c 0064 0219  .d"g.|.d#..|.d..
+000003d0: 007c 0619 0064 193c 0064 1a7c 0064 0219  .|...d.<.d.|.d..
+000003e0: 007c 0619 0064 1b19 0064 063c 0057 006e  .|...d...d.<.W.n
+000003f0: 1d04 0074 0390 0179 5001 007d 0901 007a  ...t...yP..}...z
+00000400: 1074 0464 247c 0674 057c 0983 0164 0a9c  .t.d$|.t.|...d..
+00000410: 0383 0101 0057 0059 0064 007d 097e 096e  .....W.Y.d.}.~.n
+00000420: 0564 007d 097e 0977 0177 0009 007a 6c7c  .d.}.~.w.w...zl|
+00000430: 0864 0e19 0064 0d6b 0290 0172 bd7c 0864  .d...d.k...r.|.d
+00000440: 1019 0064 0f6b 0290 0172 bd74 08a0 08a1  ...d.k...r.t....
+00000450: 0074 097c 027c 0619 0064 1119 0064 1219  .t.|.|...d...d..
+00000460: 0083 0118 007d 0a7c 0a64 256b 0590 0172  .....}.|.d%k...r
+00000470: bd7a 087c 027c 0619 0064 1419 007d 0857  .z.|.|...d...}.W
+00000480: 006e 0c04 0074 0390 0179 8801 0001 0001  .n...t...y......
+00000490: 0064 157d 0859 006e 0177 007c 0664 2667  .d.}.Y.n.w.|.d&g
+000004a0: 007c 0864 1764 189c 057c 0064 0219 007c  .|.d.d...|.d...|
+000004b0: 0619 0064 193c 0064 1a7c 0064 0219 007c  ...d.<.d.|.d...|
+000004c0: 0619 0064 1b19 0064 063c 0064 1c7c 0064  ...d...d.<.d.|.d
+000004d0: 0219 007c 0619 0064 0519 0064 1d3c 007c  ...|...d...d.<.|
+000004e0: 0064 0219 007c 0619 0064 0619 0064 0619  .d...|...d...d..
+000004f0: 00a0 0aa1 0001 0074 0b64 277c 0669 0183  .......t.d'|.i..
+00000500: 0101 0057 006e 1d04 0074 0390 0179 db01  ...W.n...t...y..
+00000510: 007d 0901 007a 1074 0464 287c 0674 057c  .}...z.t.d(|.t.|
+00000520: 0983 0164 0a9c 0383 0101 0057 0059 0064  ...d.......W.Y.d
+00000530: 007d 097e 096e 0564 007d 097e 0977 0177  .}.~.n.d.}.~.w.w
+00000540: 0009 007a 367c 0864 0e19 0064 0d6b 0290  ...z6|.d...d.k..
+00000550: 0272 127c 0864 1019 0064 0d6b 0290 0272  .r.|.d...d.k...r
+00000560: 127c 0864 1f19 0064 0f6b 0290 0272 127c  .|.d...d.k...r.|
+00000570: 0864 0819 0064 0d6b 0390 0272 127c 0664  .d...d.k...r.|.d
+00000580: 2967 007c 0864 1764 189c 057c 0064 0219  )g.|.d.d...|.d..
+00000590: 007c 0619 0064 193c 0064 1a7c 0064 0219  .|...d.<.d.|.d..
+000005a0: 007c 0619 0064 1b19 0064 063c 0057 006e  .|...d...d.<.W.n
+000005b0: 1d04 0074 0390 0279 3001 007d 0901 007a  ...t...y0..}...z
+000005c0: 1074 0464 2a7c 0674 057c 0983 0164 0a9c  .t.d*|.t.|...d..
+000005d0: 0383 0101 0057 0059 0064 007d 097e 096e  .....W.Y.d.}.~.n
+000005e0: 0564 007d 097e 0977 0177 0009 0009 007a  .d.}.~.w.w.....z
+000005f0: 287c 0864 0819 0064 0f6b 0290 0272 5a7c  (|.d...d.k...rZ|
+00000600: 0864 0e19 0064 0d6b 0290 0272 5a7c 0864  .d...d.k...rZ|.d
+00000610: 1f19 0064 0d6b 0290 0272 5a7c 0864 2b19  ...d.k...rZ|.d+.
+00000620: 0064 0d6b 0290 0272 5a64 1a7c 0064 0219  .d.k...rZd.|.d..
+00000630: 007c 0619 0064 1b19 0064 063c 0057 0071  .|...d...d.<.W.q
+00000640: 1704 0074 0390 0279 7801 007d 0901 007a  ...t...yx..}...z
+00000650: 1074 0464 2c7c 0674 057c 0983 0164 0a9c  .t.d,|.t.|...d..
+00000660: 0383 0101 0057 0059 0064 007d 097e 0971  .....W.Y.d.}.~.q
+00000670: 1764 007d 097e 0977 0177 007c 0244 005d  .d.}.~.w.w.|.D.]
+00000680: 1a7d 067c 027c 0619 0064 1b19 0064 0619  .}.|.|...d...d..
+00000690: 0064 1a6b 0390 0272 947c 05a0 0c7c 067c  .d.k...r.|...|.|
+000006a0: 0064 0219 007c 0619 0064 2d9c 02a1 0101  .d...|...d-.....
+000006b0: 0090 0271 7b7c 0553 0029 2e4e da0d 7265  ...q{|.S.).N..re
+000006c0: 636f 7264 735f 6c65 7665 6cda 1169 6e74  cords_level..int
+000006d0: 6572 6e61 6c5f 7374 6174 7573 6573 da0f  ernal_statuses..
+000006e0: 696e 7472 6f5f 7661 7269 6162 6c65 73da  intro_variables.
+000006f0: 0a74 696d 655f 6c69 6d69 74da 0b6f 6363  .time_limit..occ
+00000700: 7572 7265 6e63 6573 da07 7072 6f63 6573  urrences..proces
+00000710: 73da 0869 735f 676f 696e 677a 1573 6361  s..is_goingz.sca
+00000720: 6e20 7072 6f63 6573 7320 6973 2061 6c69  n process is ali
+00000730: 7665 7a27 7068 7973 6963 616c 3a20 7072  vez'physical: pr
+00000740: 6f63 6573 7320 616c 6976 6520 6368 6563  ocess alive chec
+00000750: 6b20 6578 6365 7074 696f 6e29 03da 0761  k exception)...a
+00000760: 6e6f 6d61 6c79 da0b 7374 6174 7573 5f70  nomaly..status_p
+00000770: 6174 68da 0965 7863 6570 7469 6f6e da07  ath..exception..
+00000780: 756e 6b6e 6f77 6e7a 1c73 6361 6e20 7072  unknownz.scan pr
+00000790: 6f63 6573 7320 7665 6e74 7572 6520 7374  ocess venture st
+000007a0: 6172 7465 64da 0379 6573 7a14 7363 616e  arted..yesz.scan
+000007b0: 2070 726f 6365 7373 2073 7461 7274 6564   process started
+000007c0: da02 6e6f 7a20 7363 616e 2070 726f 6365  ..noz scan proce
+000007d0: 7373 206e 6f74 6966 6965 6420 6167 6772  ss notified aggr
+000007e0: 6567 6174 6f72 da05 7469 6d65 737a 0f76  egator..timesz.v
+000007f0: 656e 7475 7265 2073 7461 7274 6564 e91e  enture started..
+00000800: 0000 00da 0a6f 6363 7572 656e 6365 737a  .....occurencesz
+00000810: 096e 6f74 2066 6f75 6e64 7a67 4166 7465  .not foundzgAfte
+00000820: 7220 3330 2073 6563 6f6e 6473 2c20 7468  r 30 seconds, th
+00000830: 6520 6166 7465 7220 7072 6f63 6573 7320  e after process 
+00000840: 6c69 6e65 2077 6173 206e 6f74 2072 6561  line was not rea
+00000850: 6368 6564 2061 6e64 2074 6865 2070 726f  ched and the pro
+00000860: 6365 7373 2064 6964 206e 6f74 206e 6f74  cess did not not
+00000870: 6966 7920 7468 6520 6167 6772 6567 6174  ify the aggregat
+00000880: 6f72 2e54 2905 da04 7061 7468 da05 616c  or.T)...path..al
+00000890: 6172 6dfa 0b61 6c61 726d 206e 6f74 6573  arm..alarm notes
+000008a0: 720f 0000 00da 0665 7869 7465 64da 0f72  r......exited..r
+000008b0: 6573 756c 7473 5f6f 665f 7363 616e da04  esults_of_scan..
+000008c0: 646f 6e65 da06 7374 6174 7573 7a3a 5468  done..statusz:Th
+000008d0: 6520 7072 6f63 6573 7320 6469 646e 2774  e process didn't
+000008e0: 206e 6f74 6966 7920 7468 6520 6167 6772   notify the aggr
+000008f0: 6567 6174 6f72 2077 6974 6869 6e20 3520  egator within 5 
+00000900: 7365 636f 6e64 732e 7a10 646f 6e65 2072  seconds.z.done r
+00000910: 6561 736f 6e20 6769 7665 7a32 7068 7973  eason givez2phys
+00000920: 6963 616c 3a20 7072 6f63 6573 7320 7072  ical: process pr
+00000930: 6f63 6565 6420 6e6f 2073 7461 7274 2063  oceed no start c
+00000940: 6865 636b 2065 7863 6570 7469 6f6e 7a18  heck exceptionz.
+00000950: 7363 616e 2070 726f 6365 7373 2077 6173  scan process was
+00000960: 2073 746f 7070 6564 7a1c 7363 616e 2070   stoppedz.scan p
+00000970: 726f 6365 6564 7320 7765 7265 2072 6574  roceeds were ret
+00000980: 7269 6576 6564 e90f 0000 007a 5d54 6865  rieved.....z]The
+00000990: 2073 6361 6e20 7072 6f63 6573 7320 7761   scan process wa
+000009a0: 7320 7374 6f70 7065 642c 2062 7574 2031  s stopped, but 1
+000009b0: 3520 7365 636f 6e64 7320 6861 7665 2070  5 seconds have p
+000009c0: 6173 7365 6420 616e 6420 7468 6520 7072  assed and the pr
+000009d0: 6f63 6565 6473 2077 6572 6520 6e6f 7420  oceeds were not 
+000009e0: 7265 7472 6965 7665 642e 2904 721b 0000  retrieved.).r...
+000009f0: 0072 1c00 0000 721d 0000 0072 0f00 0000  .r....r....r....
+00000a00: 7a37 7068 7973 6963 616c 3a20 7072 6f63  z7physical: proc
+00000a10: 6573 7320 7072 6f63 6565 6420 6e6f 7420  ess proceed not 
+00000a20: 7265 7472 6965 7665 6420 6368 6563 6b20  retrieved check 
+00000a30: 6578 6365 7074 696f 6ee9 1400 0000 7a50  exception.....zP
+00000a40: 4166 7465 7220 3230 2073 6563 6f6e 6473  After 20 seconds
+00000a50: 2c20 7468 6520 7072 6f63 6573 7320 6469  , the process di
+00000a60: 6420 6e6f 7420 6e6f 7469 6679 2074 6865  d not notify the
+00000a70: 2061 6767 7265 6761 746f 7220 7468 6174   aggregator that
+00000a80: 2069 7420 6861 6420 7374 6172 7465 642e   it had started.
+00000a90: 7a18 7072 6f63 6573 7320 6d61 7920 6861  z.process may ha
+00000aa0: 7665 2073 746f 7070 6564 7a39 7068 7973  ve stoppedz9phys
+00000ab0: 6963 616c 3a20 7072 6f63 6573 7320 7072  ical: process pr
+00000ac0: 6f63 6565 6420 6e6f 206e 6f74 6966 6963  oceed no notific
+00000ad0: 6174 696f 6e20 6368 6563 6b20 6578 6365  ation check exce
+00000ae0: 7074 696f 6e7a 3054 6865 2070 726f 6365  ptionz0The proce
+00000af0: 7373 2065 7869 7465 6420 6265 666f 7265  ss exited before
+00000b00: 2072 6573 756c 7473 2063 6f75 6c64 2062   results could b
+00000b10: 6520 7365 6e74 2e7a 2b70 6879 7369 6361  e sent.z+physica
+00000b20: 6c3a 2070 726f 6365 7373 2070 6172 7365  l: process parse
+00000b30: 2061 6e64 2063 6865 636b 2065 7863 6570   and check excep
+00000b40: 7469 6f6e 7a1b 7363 616e 2072 6563 6f72  tionz.scan recor
+00000b50: 6473 2077 6572 6520 7265 7472 6965 7665  ds were retrieve
+00000b60: 647a 3270 6879 7369 6361 6c3a 2070 726f  dz2physical: pro
+00000b70: 6365 7373 2069 7320 646f 6e65 206e 6f72  cess is done nor
+00000b80: 6d61 6c6c 7920 6368 6563 6b20 6578 6365  mally check exce
+00000b90: 7074 696f 6e29 0272 1b00 0000 da09 696e  ption).r......in
+00000ba0: 7465 726e 616c 7329 0d72 0200 0000 da04  ternals).r......
+00000bb0: 7479 7065 da04 6469 6374 da09 4578 6365  type..dict..Exce
+00000bc0: 7074 696f 6e72 0300 0000 7204 0000 0072  ptionr....r....r
+00000bd0: 0600 0000 7207 0000 00da 0474 696d 65da  ....r......time.
+00000be0: 0566 6c6f 6174 da09 7465 726d 696e 6174  .float..terminat
+00000bf0: 6572 0900 0000 da06 6170 7065 6e64 290b  er......append).
+00000c00: da14 6167 6772 6567 6174 6f72 5f76 6172  ..aggregator_var
+00000c10: 6961 626c 6573 720b 0000 0072 0c00 0000  iablesr....r....
+00000c20: 720e 0000 00da 0873 7461 7475 7365 73da  r......statuses.
+00000c30: 0a75 6e66 696e 6973 6865 6472 1300 0000  .unfinishedr....
+00000c40: da0e 7374 6174 7573 5f6f 665f 7061 7468  ..status_of_path
+00000c50: 720f 0000 00da 0145 da07 656c 6170 7365  r......E..elapse
+00000c60: 64a9 0072 3200 0000 fa71 2f62 696f 7465  d..r2....q/biote
+00000c70: 6368 2f76 656e 7565 732f 7374 6167 6573  ch/venues/stages
+00000c80: 2f62 696f 7465 6368 2f70 726f 6365 6475  /biotech/procedu
+00000c90: 7265 732f 6167 6772 6567 6174 6f72 5f70  res/aggregator_p
+00000ca0: 726f 6365 6475 7265 2f70 726f 6365 7373  rocedure/process
+00000cb0: 2f6d 6f76 6573 2f73 7461 7475 735f 6368  /moves/status_ch
+00000cc0: 6563 6b5f 6d6f 6e69 746f 722f 7468 655f  eck_monitor/the_
+00000cd0: 7068 7973 6963 616c 2e70 79da 2470 6172  physical.py.$par
+00000ce0: 7365 5f61 6e64 5f63 6865 636b 5f69 735f  se_and_check_is_
+00000cf0: 616c 6976 655f 6f66 5f73 7461 7475 7365  alive_of_statuse
+00000d00: 7322 0000 0073 4601 0000 0601 0802 0801  s"...sF.........
+00000d10: 0c01 0402 0401 0a01 0802 0801 0202 0204  ................
+00000d20: 0c01 1402 1001 1602 0202 0480 0e0d 0201  ................
+00000d30: 0201 0201 0601 08fd 1406 0880 02f9 080a  ................
+00000d40: 0802 0205 020c 0c02 0c01 0c01 1c02 0802  ................
+00000d50: 0201 1001 0c01 0801 02ff 0204 0202 0201  ................
+00000d60: 0202 0202 12f8 140b 1401 1802 0480 0e03  ................
+00000d70: 0201 0201 0201 0601 08fd 0c06 0880 02f9  ................
+00000d80: 020a 0206 0e02 0e01 1c02 0a02 0202 0202  ................
+00000d90: 0201 0202 12fa 1409 0480 1002 0201 0201  ................
+00000da0: 0201 0601 08fd 0c06 0880 02f9 020a 0208  ................
+00000db0: 0e02 0e01 1c02 0a02 0201 1001 0e01 0801  ................
+00000dc0: 02ff 0204 0202 0201 0202 0202 12f8 140b  ................
+00000dd0: 1401 1801 0202 0401 06ff 0480 1003 0201  ................
+00000de0: 0201 0201 0601 08fd 0c06 0880 02f9 020e  ................
+00000df0: 020c 0e02 0e01 0e02 0e02 0203 0202 0201  ................
+00000e00: 0201 0202 12f9 140a 0480 1002 0201 0201  ................
+00000e10: 0201 0601 08fd 0c06 0880 02f9 020a 0208  ................
+00000e20: 0203 0e02 0e02 0e01 0e02 1402 0480 1002  ................
+00000e30: 0201 0201 0201 0601 08fd 0c05 0880 02fa  ................
+00000e40: 080a 1601 0401 0201 0a01 08fe 0480 0406  ................
+00000e50: 7234 0000 0029 12da 3962 696f 7465 6368  r4...)..9biotech
+00000e60: 2e70 726f 6365 6475 7265 732e 6167 6772  .procedures.aggr
+00000e70: 6567 6174 6f72 5f70 726f 6365 6475 7265  egator_procedure
+00000e80: 2e70 726f 6365 7373 2e76 6172 6961 626c  .process.variabl
+00000e90: 6573 7202 0000 0072 0300 0000 da19 6269  esr....r......bi
+00000ea0: 6f74 6563 682e 746f 7069 6373 2e65 7863  otech.topics.exc
+00000eb0: 6570 7469 6f6e 7372 0400 0000 da07 7265  eptionsr......re
+00000ec0: 636f 7264 7372 0600 0000 da27 616c 6172  cordsr.....'alar
+00000ed0: 6d5f 6368 6563 6b73 2e67 6c6f 6261 6c5f  m_checks.global_
+00000ee0: 7469 6d65 5f6c 696d 6974 5f65 7863 6565  time_limit_excee
+00000ef0: 6465 6472 0700 0000 da30 6269 6f74 6563  dedr.....0biotec
+00000f00: 682e 746f 7069 6373 2e70 726f 6365 7373  h.topics.process
+00000f10: 5f6f 6e2e 705f 6578 7065 6374 2e70 6172  _on.p_expect.par
+00000f20: 7365 5f72 6563 6f72 6473 7208 0000 00da  se_recordsr.....
+00000f30: 1c62 696f 7465 6368 2e74 6f70 6963 732e  .biotech.topics.
+00000f40: 7368 6f77 2e76 6172 6961 626c 6572 0900  show.variabler..
+00000f50: 0000 720a 0000 0072 2800 0000 da09 7472  ..r....r(.....tr
+00000f60: 6163 6562 6163 6bda 0472 6963 6872 3400  aceback..richr4.
+00000f70: 0000 7232 0000 0072 3200 0000 7232 0000  ..r2...r2...r2..
+00000f80: 0072 3300 0000 da08 3c6d 6f64 756c 653e  .r3.....<module>
+00000f90: 0100 0000 731a 0000 000c 070c 010c 010c  ....s...........
+00000fa0: 020c 020c 020c 010c 0308 0108 0108 0302  ................
+00000fb0: 050c 04                                  ...
```

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 
 
 from biotech.procedures.aggregator_procedure.process.variables import retrieve_variables
+from biotech.procedures.aggregator_procedure.process.variables import add_anomaly
 from ...done_with_scan import done_with_scan_move
 
+from biotech.topics.exceptions import parse_exception
+
 import time
 
 def learn_if_global_time_limit_was_exceeded (status_path):
 	try:
 		aggregator_variables = retrieve_variables ()
 		time_limit = aggregator_variables ["intro_variables"] ["time_limit"]
 		internal_statuses = aggregator_variables ["internal_statuses"]
@@ -20,37 +23,36 @@
 			occurrences ["scan process is alive"] == "yes" and
 			occurrences ["scan process notified aggregator"] == "yes" and
 			occurrences ["scan process was stopped"] == "no" and
 			len (internal_statuses [ status_path ] ["times"] ["started"]) >= 1
 		):	
 		'''
 		
-		if (time.time () - float (internal_statuses [ status_path ] ["times"] ["started"]) >= float (time_limit)):	
-		
-			try:
-				the_scan_records = internal_statuses [ status_path ] ["records"]
-			except Exception:
-				the_scan_records = "not found"
+		started_at = internal_statuses [ status_path ] ["times"] ["started"]
 		
-			done_with_scan_move ({
-				"path": status_path,
-				"result":{
-					"alarm": "time limit exceeded",
-					"the records": the_scan_records
-				}
-			})
-					
+		if (len (started_at) >= 1):
+			if (time.time () - float (started_at) >= float (time_limit)):	
+				try:
+					the_scan_records = internal_statuses [ status_path ] ["records"]
+				except Exception:
+					the_scan_records = "not found"
+			
+				done_with_scan_move ({
+					"path": status_path,
+					"result":{
+						"alarm": "time limit exceeded",
+						"the records": the_scan_records
+					}
+				})
+						
 	except Exception as E1:
-		print ("time limit check exception:", E1)
-	
-		try:
-			aggregator_variables ["anomalies"].append ({
-				"anomaly": "time limit check exception",
-				"exception": E1
-			})
-		except Exception as E2:
-			pass;
+		add_anomaly ({
+			"anomaly": "physical: time limit check exception",
+			"status_path": status_path,
+			"exception": parse_exception (E1)
+		})
+
```

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 
 
 
 #----
 #
 from biotech.procedures.aggregator_procedure.process.variables import retrieve_variables
-
+from biotech.procedures.aggregator_procedure.process.variables import add_anomaly
+from biotech.topics.exceptions import parse_exception
 #
 from .records import attach_records
 #
 from .alarm_checks.global_time_limit_exceeded import learn_if_global_time_limit_was_exceeded
 #
 from biotech.topics.process_on.p_expect.parse_records import parse_p_expect_records
 from biotech.topics.show.variable import show_variable
@@ -45,30 +46,46 @@
 		occurrences = status_of_path ["occurrences"]
 		
 		'''
 			This checks if the pexpect 
 			process is alive.
 		'''
 		try:
-			if ("process" in internal_statuses [ status_path ] ["process"]):
-				if (type (internal_statuses [ status_path ] ["process"] ["process"]) != None):
-					alive = internal_statuses [ status_path ] ["process"] ["process"].is_alive ()
-					if (alive == True):
-						occurrences ["scan process is alive"] = "yes"
-					else:
-						occurrences ["scan process is alive"] = "no"
+			if ("process" in internal_statuses [ status_path ]):
+				if (
+					type (internal_statuses [ status_path ] ["process"]) == dict and
+					"process" in internal_statuses [ status_path ] ["process"]
+				):
+					occurrences ["scan process is alive"] = internal_statuses [ status_path ] ["process"] ["is_going"] ()
+				
+				'''
+				if (
+					type (internal_statuses [ status_path ] ["process"]) == dict and
+					"process" in internal_statuses [ status_path ] ["process"]
+				):
+					if (type (internal_statuses [ status_path ] ["process"] ["process"]) != None):
+						alive = internal_statuses [ status_path ] ["process"] ["process"].is_alive ()
+						if (alive == True):
+							occurrences ["scan process is alive"] = "yes"
+						else:
+							occurrences ["scan process is alive"] = "no"
+				'''
 				
 		except Exception as E:
-			print ("process alive check exception:", E)
+			add_anomaly ({
+				"anomaly": "physical: process alive check exception",
+				"status_path": status_path,
+				"exception": parse_exception (E)
+			})
+		
 			occurrences ["scan process is alive"] = "unknown"		
 		
 		
 		attach_records (status_path)
 		
-		
 		learn_if_global_time_limit_was_exceeded (status_path)
 		
 
 
 		
 		'''
 			This checks if a perhaps non started process didn't 
@@ -110,27 +127,32 @@
 					aggregator_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
 					aggregator_variables ["internal_statuses"] [ status_path ] ["occurrences"] ["done reason give"] = "The process didn't notify the aggregator within 5 seconds."
 					
 					aggregator_variables ["internal_statuses"] [ status_path ] ["process"] ["process"].terminate ()
 					
 
 		except Exception as E:
-			print ("process non-notification exception:", traceback.format_exc ())
+			add_anomaly ({
+				"anomaly": "physical: process proceed no start check exception",
+				"status_path": status_path,
+				"exception": parse_exception (E)
+			})
+		
 			pass;
 			
 		
 		'''
 			objective:
 				The scan process was stopped, 
 				but 10 seconds have passed
 				and the proceeds were not retrieved.
 		'''
 		try:
 			if (
-				occurrences ["scan process stopped"] == "yes" and
+				occurrences ["scan process was stopped"] == "yes" and
 				occurrences ["scan proceeds were retrieved"] == "no"
 			):
 				elapsed = time.time () - float (internal_statuses [ status_path ] ["times"] ["venture started"]);
 				
 				if (elapsed >= 15):	
 					aggregator_variables ["internal_statuses"] [ status_path ] ["results_of_scan"] = {
 						"path": status_path,
@@ -140,21 +162,26 @@
 						
 						"occurrences": occurrences
 					}
 				
 					aggregator_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
 
 		except Exception as E:
-			print ("process non-notification exception:", E)
+			add_anomaly ({
+				"anomaly": "physical: process proceed not retrieved check exception",
+				"status_path": status_path,
+				"exception": parse_exception (E)
+			})
+			
 			pass;
 		
 		
 		'''
 			This checks if a started process didn't 
-			notify the aggregator within 10 seconds.
+			notify the aggregator within 20 seconds.
 		
 				scan process started == "yes"
 				scan process notified aggregator == "no"
 				10 seconds elapsed
 		'''
 		try:
 			if (
@@ -184,86 +211,24 @@
 					aggregator_variables ["internal_statuses"] [ status_path ] ["occurrences"] ["done reason give"] = "The process didn't notify the aggregator within 5 seconds."
 					aggregator_variables ["internal_statuses"] [ status_path ] ["process"] ["process"].terminate ()
 					
 					show_variable ({
 						"process may have stopped": status_path
 					})
 		except Exception as E:
-			print ("process non-notification exception:", traceback.format_exc ())
+			add_anomaly ({
+				"anomaly": "physical: process proceed no notification check exception",
+				"status_path": status_path,
+				"exception": parse_exception (E)
+			})
+		
 			pass;
 		
 		
-		'''
-			A live process that is indicating that
-			it is infinite loop, when it is not.
-			
-			Therefore if after 5 seconds the records are
-			empty, then therer was mostly likely 
-			a problem starting the process.
-		
-				'scan process venture started': 'yes',
-				'scan process started': 'yes',
-				'scan process notified aggregator': 'yes',
-				'scan process is alive': 'yes',
-
-
-				'scan process was stopped': 'no',
-				'scan returned proceeds': 'no',
-				'scan records were retrieved': 'no'
-		'''
-		try:				
-			doors = {
-				"1": occurrences ["scan process started"] == "yes",
-				"2": occurrences ["scan process is alive"] == "yes",
-				"3": occurrences ["scan process was stopped"] == "no",
-				"4": len (internal_statuses [ status_path ] ["times"] ["venture started"]) >= 1,
-				"6": len (internal_statuses [ status_path ] ["records"]) == 0,
-				"7": time.time () - float (internal_statuses [ status_path ] ["times"] ["venture started"])
-			}
-			
 		
-			if (
-				occurrences ["scan process started"] == "yes" and
-				occurrences ["scan process is alive"] == "yes" and
-				occurrences ["scan process was stopped"] == "no" and
-				len (internal_statuses [ status_path ] ["times"] ["venture started"]) >= 1 and
-				
-				len (internal_statuses [ status_path ] ["records"]) == 0
-			):
-				elapsed = time.time () - float (internal_statuses [ status_path ] ["times"] ["venture started"]);
-			
-				if (elapsed >= 10):			
-					show_variable ({
-						"records were not retrieved after 10 seconds": status_path
-					})
-					
-					try:
-						occurrences = internal_statuses [ status_path ] ["occurences"];
-					except Exception:
-						occurrences = "not found"
-					
-					aggregator_variables ["internal_statuses"] [ status_path ] ["results_of_scan"] = {
-						"path": status_path,
-						
-						"alarm": "After 10 seconds, no process logs were found.",
-						"alarm notes": [],
-						
-						"occurences": occurrences,
-						
-						"exited": True
-					}
-				
-					aggregator_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
-					aggregator_variables ["internal_statuses"] [ status_path ] ["process"] ["process"].terminate ()
-					
-					
-						
-		except Exception as E:
-			print ("process logs time limit check exception:", E)
-			pass;
 		
 		
 		
 		'''
 			Alarm Possibility: 
 				"The process exited before results could be sent."
 		
@@ -293,15 +258,20 @@
 					
 					"exited": True
 				}
 			
 				aggregator_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
 
 		except Exception as E:
-			print ("parse and check exception:", traceback.format_exc ())
+			add_anomaly ({
+				"anomaly": "physical: process parse and check exception",
+				"status_path": status_path,
+				"exception": parse_exception (E)
+			})
+			
 			pass;
 		
 		
 		'''
 			objective:
 				This stops the process if:
 					the process is alive, but unresponsive?
@@ -320,15 +290,19 @@
 				occurrences ["scan process was stopped"] == "yes" and
 				
 				occurrences ["scan records were retrieved"] == "yes"
 			):				
 				aggregator_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
 
 		except Exception as E:
-			print ("parse and check exception:", traceback.format_exc ())
+			add_anomaly ({
+				"anomaly": "physical: process is done normally check exception",
+				"status_path": status_path,
+				"exception": parse_exception (E)
+			})
 			pass;
 		
 
 	
 	for status_path in internal_statuses:
 		if (internal_statuses [ status_path ] ["status"] ["process"] != "done"):
 			unfinished.append ({
```

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,25 @@
 
 '''
 	from biotech.procedures.aggregator_procedure.process.variables import retrieve_aggregator_variables
 '''
 
 '''
 	from biotech.procedures.aggregator_procedure.process.variables import add_anomaly
-	add_anomaly ()
+	from biotech.topics.exceptions import parse_exception
+	add_anomaly ({
+		"anomaly": "",
+		"exception": parse_exception (E)
+	})
 '''
 
 from biotech.procedures.aggregator_procedure.process.moves.format_path import format_path
+from biotech.topics.show.variable import show_variable
 
+import json
 
 '''
 	paths_statuses = [{
 		"path": path,
 		** scan_status
 	}]
 '''
@@ -61,25 +67,29 @@
 	"internal_statuses": {},
 	"internal_statuses_built": "no",
 	
 	"anomalies": []
 }
 
 def add_anomaly (anomaly):
+	print ("add_anomaly?", anomaly)
+
 	try:
 		is_JSON = json.dumps (anomaly)
 	
-		aggregator_variables.append (anomaly)
+		aggregator_variables ["anomalies"].append (anomaly)
 		
 		show_variable ({
 			"anomaly": anomaly
 		})
 		
-	except Exception:
+	except Exception as E:
 		show_variable ("An anomaly couldn't be added.")
+		print ("exception:", E)
+
 
 def setup_internal_statuses (
 	status_check_paths,
 	relative_path
 ):
 	for status_check_path in status_check_paths:		
 		aggregator_variables ["internal_statuses"] [
```

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 23:03:08 2024 UTC, .py size: 3303 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,127 +1,137 @@
-00000000: 6f0d 0d0a 0000 0000 2cf8 2266 e70c 0000  o.......,."f....
+00000000: 6f0d 0d0a 0000 0000 d20a 2366 e90d 0000  o.........#f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
+00000020: 0008 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 5a00 0900 6401 6402 6c01 6d02 5a02 0100  Z...d.d.l.m.Z...
-00000040: 0900 0900 6403 6404 6405 9c02 6406 6900  ....d.d.d...d.i.
-00000050: 6407 6900 6408 6700 6409 9c07 5a03 640a  d.i.d.g.d...Z.d.
-00000060: 640b 8400 5a04 640c 640d 8400 5a05 640e  d...Z.d.d...Z.d.
-00000070: 640f 8400 5a06 6410 6411 8400 5a07 6412  d...Z.d.d...Z.d.
-00000080: 6413 8400 5a08 6414 6415 8400 5a09 6416  d...Z.d.d...Z.d.
-00000090: 5300 2917 7a66 0a09 6672 6f6d 2062 696f  S.).zf..from bio
-000000a0: 7465 6368 2e70 726f 6365 6475 7265 732e  tech.procedures.
-000000b0: 6167 6772 6567 6174 6f72 5f70 726f 6365  aggregator_proce
-000000c0: 6475 7265 2e70 726f 6365 7373 2e76 6172  dure.process.var
-000000d0: 6961 626c 6573 2069 6d70 6f72 7420 7265  iables import re
-000000e0: 7472 6965 7665 5f61 6767 7265 6761 746f  trieve_aggregato
-000000f0: 725f 7661 7269 6162 6c65 730a e900 0000  r_variables.....
-00000100: 0029 01da 0b66 6f72 6d61 745f 7061 7468  .)...format_path
-00000110: 7a07 302e 302e 302e 30da 0029 02da 0468  z.0.0.0.0..)...h
-00000120: 6f73 74da 0470 6f72 74e9 0300 0000 e902  ost..port.......
-00000130: 0000 00da 026e 6f29 07da 0c69 6e74 726f  .....no)...intro
-00000140: 5f68 6172 626f 72da 0d72 6563 6f72 6473  _harbor..records
-00000150: 5f6c 6576 656c da0f 696e 7472 6f5f 7661  _level..intro_va
-00000160: 7269 6162 6c65 73da 0764 6574 6169 6c73  riables..details
-00000170: da11 696e 7465 726e 616c 5f73 7461 7475  ..internal_statu
-00000180: 7365 73da 1769 6e74 6572 6e61 6c5f 7374  ses..internal_st
-00000190: 6174 7573 6573 5f62 7569 6c74 da09 616e  atuses_built..an
-000001a0: 6f6d 616c 6965 7363 0100 0000 0000 0000  omaliesc........
-000001b0: 0000 0000 0200 0000 0800 0000 4300 0000  ............C...
-000001c0: 7344 0000 007a 1374 00a0 017c 00a1 017d  sD...z.t...|...}
-000001d0: 0174 02a0 037c 00a1 0101 0074 0464 017c  .t...|.....t.d.|
-000001e0: 0069 0183 0101 0057 0064 0053 0004 0074  .i.....W.d.S...t
-000001f0: 0579 2101 0001 0001 0074 0464 0283 0101  .y!......t.d....
-00000200: 0059 0064 0053 0077 0029 034e da07 616e  .Y.d.S.w.).N..an
-00000210: 6f6d 616c 797a 1d41 6e20 616e 6f6d 616c  omalyz.An anomal
-00000220: 7920 636f 756c 646e 2774 2062 6520 6164  y couldn't be ad
-00000230: 6465 642e 2906 da04 6a73 6f6e da05 6475  ded.)...json..du
-00000240: 6d70 73da 1461 6767 7265 6761 746f 725f  mps..aggregator_
-00000250: 7661 7269 6162 6c65 73da 0661 7070 656e  variables..appen
-00000260: 64da 0d73 686f 775f 7661 7269 6162 6c65  d..show_variable
-00000270: da09 4578 6365 7074 696f 6e29 0272 1000  ..Exception).r..
-00000280: 0000 da07 6973 5f4a 534f 4ea9 0072 1800  ....is_JSON..r..
-00000290: 0000 fa5c 2f62 696f 7465 6368 2f76 656e  ...\/biotech/ven
-000002a0: 7565 732f 7374 6167 6573 2f62 696f 7465  ues/stages/biote
-000002b0: 6368 2f70 726f 6365 6475 7265 732f 6167  ch/procedures/ag
-000002c0: 6772 6567 6174 6f72 5f70 726f 6365 6475  gregator_procedu
-000002d0: 7265 2f70 726f 6365 7373 2f76 6172 6961  re/process/varia
-000002e0: 626c 6573 2f5f 5f69 6e69 745f 5f2e 7079  bles/__init__.py
-000002f0: da0b 6164 645f 616e 6f6d 616c 7943 0000  ..add_anomalyC..
-00000300: 0073 1200 0000 0201 0a01 0a02 0202 0401  .s..............
-00000310: 0cff 0c04 0e01 02ff 721a 0000 0063 0200  ........r....c..
-00000320: 0000 0000 0000 0000 0000 0300 0000 0a00  ................
-00000330: 0000 4300 0000 734e 0000 007c 0044 005d  ..C...sN...|.D.]
-00000340: 227d 0264 0164 0164 0164 0164 0264 0164  "}.d.d.d.d.d.d.d
-00000350: 0164 0364 049c 0864 0564 0669 0164 0364  .d.d...d.d.i.d.d
-00000360: 0364 0364 0364 079c 0467 0064 0064 0064  .d.d.d...g.d.d.d
-00000370: 089c 0674 0064 0919 0074 017c 027c 0183  ...t.d...t.|.|..
-00000380: 023c 0071 0264 0053 0029 0a4e 7208 0000  .<.q.d.S.).Nr...
-00000390: 00da 0775 6e6b 6e6f 776e 7203 0000 0029  ...unknownr....)
-000003a0: 087a 1c73 6361 6e20 7072 6f63 6573 7320  .z.scan process 
-000003b0: 7665 6e74 7572 6520 7374 6172 7465 647a  venture startedz
-000003c0: 1473 6361 6e20 7072 6f63 6573 7320 7374  .scan process st
-000003d0: 6172 7465 647a 2073 6361 6e20 7072 6f63  artedz scan proc
-000003e0: 6573 7320 6e6f 7469 6669 6564 2061 6767  ess notified agg
-000003f0: 7265 6761 746f 727a 1873 6361 6e20 7072  regatorz.scan pr
-00000400: 6f63 6573 7320 7761 7320 7374 6f70 7065  ocess was stoppe
-00000410: 647a 1573 6361 6e20 7072 6f63 6573 7320  dz.scan process 
-00000420: 6973 2061 6c69 7665 7a1c 7363 616e 2070  is alivez.scan p
-00000430: 726f 6365 6564 7320 7765 7265 2072 6574  roceeds were ret
-00000440: 7269 6576 6564 7a1b 7363 616e 2072 6563  rievedz.scan rec
-00000450: 6f72 6473 2077 6572 6520 7265 7472 6965  ords were retrie
-00000460: 7665 647a 1064 6f6e 6520 7265 6173 6f6e  vedz.done reason
-00000470: 2067 6976 65da 0770 726f 6365 7373 da07   give..process..
-00000480: 7065 6e64 696e 6729 04da 0773 7461 7274  pending)...start
-00000490: 6564 da05 656e 6465 64da 0765 6c61 7073  ed..ended..elaps
-000004a0: 6564 7a11 7265 636f 7264 7320 7265 7472  edz.records retr
-000004b0: 6965 7661 6c29 06da 0b6f 6363 7572 7265  ieval)...occurre
-000004c0: 6e63 6573 da06 7374 6174 7573 da05 7469  nces..status..ti
-000004d0: 6d65 73da 0772 6563 6f72 6473 721c 0000  mes..recordsr...
-000004e0: 00da 0f72 6573 756c 7473 5f6f 665f 7363  ...results_of_sc
-000004f0: 616e 720d 0000 0029 0272 1300 0000 7202  anr....).r....r.
-00000500: 0000 0029 03da 1273 7461 7475 735f 6368  ...)...status_ch
-00000510: 6563 6b5f 7061 7468 73da 0d72 656c 6174  eck_paths..relat
-00000520: 6976 655f 7061 7468 da11 7374 6174 7573  ive_path..status
-00000530: 5f63 6865 636b 5f70 6174 6872 1800 0000  _check_pathr....
-00000540: 7218 0000 0072 1900 0000 da17 7365 7475  r....r......setu
-00000550: 705f 696e 7465 726e 616c 5f73 7461 7475  p_internal_statu
-00000560: 7365 7350 0000 0073 3200 0000 0804 020c  sesP...s2.......
-00000570: 0207 0208 0207 0207 0208 0207 0207 04c5  ................
-00000580: 0441 02ff 0206 0201 0201 0201 04fc 0207  .A..............
-00000590: 0202 0201 04b0 06fe 0801 04ff 0456 7229  .............Vr)
-000005a0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000005b0: 0000 0000 0100 0000 4300 0000 7304 0000  ........C...s...
-000005c0: 0064 0053 00a9 014e 7218 0000 0072 1800  .d.S...Nr....r..
-000005d0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-000005e0: 00da 0663 6861 6e67 65ad 0000 00f3 0200  ...change.......
-000005f0: 0000 0401 722b 0000 0063 0000 0000 0000  ....r+...c......
-00000600: 0000 0000 0000 0000 0000 0100 0000 4300  ..............C.
-00000610: 0000 f304 0000 0074 0053 0072 2a00 0000  .......t.S.r*...
-00000620: a901 7213 0000 0072 1800 0000 7218 0000  ..r....r....r...
-00000630: 0072 1800 0000 7219 0000 00da 1272 6574  .r....r......ret
-00000640: 7269 6576 655f 7661 7269 6162 6c65 73b0  rieve_variables.
-00000650: 0000 0072 2c00 0000 722f 0000 0063 0000  ...r,...r/...c..
-00000660: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-00000670: 0000 4300 0000 722d 0000 0072 2a00 0000  ..C...r-...r*...
-00000680: 722e 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000690: 1800 0000 7219 0000 00da 1d72 6574 7269  ....r......retri
-000006a0: 6576 655f 6167 6772 6567 6174 6f72 5f76  eve_aggregator_v
-000006b0: 6172 6961 626c 6573 b300 0000 722c 0000  ariables....r,..
-000006c0: 0072 3000 0000 6300 0000 0000 0000 0000  .r0...c.........
-000006d0: 0000 0000 0000 0001 0000 0043 0000 0072  ...........C...r
-000006e0: 2d00 0000 722a 0000 0072 2e00 0000 7218  -...r*...r....r.
-000006f0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00000700: 0000 da08 7265 7472 6965 7665 b600 0000  ....retrieve....
-00000710: 722c 0000 0072 3100 0000 4e29 0ada 075f  r,...r1...N)..._
-00000720: 5f64 6f63 5f5f da41 6269 6f74 6563 682e  _doc__.Abiotech.
-00000730: 7072 6f63 6564 7572 6573 2e61 6767 7265  procedures.aggre
-00000740: 6761 746f 725f 7072 6f63 6564 7572 652e  gator_procedure.
-00000750: 7072 6f63 6573 732e 6d6f 7665 732e 666f  process.moves.fo
-00000760: 726d 6174 5f70 6174 6872 0200 0000 7213  rmat_pathr....r.
-00000770: 0000 0072 1a00 0000 7229 0000 0072 2b00  ...r....r)...r+.
-00000780: 0000 722f 0000 0072 3000 0000 7231 0000  ..r/...r0...r1..
-00000790: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
-000007a0: 7219 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000007b0: 0000 0073 2a00 0000 0402 0204 0c05 0203  ...s*...........
-000007c0: 0207 0215 0201 04fe 0205 0202 0207 0205  ................
-000007d0: 0201 0202 06e9 081a 080d 085d 0803 0803  ...........]....
-000007e0: 0c03                                     ..
+00000040: 6401 6403 6c03 6d04 5a04 0100 6401 6404  d.d.l.m.Z...d.d.
+00000050: 6c05 5a05 0900 0900 6405 6406 6407 9c02  l.Z.....d.d.d...
+00000060: 6408 6900 6409 6900 640a 6700 640b 9c07  d.i.d.i.d.g.d...
+00000070: 5a06 640c 640d 8400 5a07 640e 640f 8400  Z.d.d...Z.d.d...
+00000080: 5a08 6410 6411 8400 5a09 6412 6413 8400  Z.d.d...Z.d.d...
+00000090: 5a0a 6414 6415 8400 5a0b 6416 6417 8400  Z.d.d...Z.d.d...
+000000a0: 5a0c 6404 5300 2918 7a66 0a09 6672 6f6d  Z.d.S.).zf..from
+000000b0: 2062 696f 7465 6368 2e70 726f 6365 6475   biotech.procedu
+000000c0: 7265 732e 6167 6772 6567 6174 6f72 5f70  res.aggregator_p
+000000d0: 726f 6365 6475 7265 2e70 726f 6365 7373  rocedure.process
+000000e0: 2e76 6172 6961 626c 6573 2069 6d70 6f72  .variables impor
+000000f0: 7420 7265 7472 6965 7665 5f61 6767 7265  t retrieve_aggre
+00000100: 6761 746f 725f 7661 7269 6162 6c65 730a  gator_variables.
+00000110: e900 0000 0029 01da 0b66 6f72 6d61 745f  .....)...format_
+00000120: 7061 7468 2901 da0d 7368 6f77 5f76 6172  path)...show_var
+00000130: 6961 626c 654e 7a07 302e 302e 302e 30da  iableNz.0.0.0.0.
+00000140: 0029 02da 0468 6f73 74da 0470 6f72 74e9  .)...host..port.
+00000150: 0300 0000 e902 0000 00da 026e 6f29 07da  ...........no)..
+00000160: 0c69 6e74 726f 5f68 6172 626f 72da 0d72  .intro_harbor..r
+00000170: 6563 6f72 6473 5f6c 6576 656c da0f 696e  ecords_level..in
+00000180: 7472 6f5f 7661 7269 6162 6c65 73da 0764  tro_variables..d
+00000190: 6574 6169 6c73 da11 696e 7465 726e 616c  etails..internal
+000001a0: 5f73 7461 7475 7365 73da 1769 6e74 6572  _statuses..inter
+000001b0: 6e61 6c5f 7374 6174 7573 6573 5f62 7569  nal_statuses_bui
+000001c0: 6c74 da09 616e 6f6d 616c 6965 7363 0100  lt..anomaliesc..
+000001d0: 0000 0000 0000 0000 0000 0300 0000 0a00  ................
+000001e0: 0000 4300 0000 736e 0000 0074 0064 017c  ..C...sn...t.d.|
+000001f0: 0083 0201 007a 1574 01a0 027c 00a1 017d  .....z.t...|...}
+00000200: 0174 0364 0219 00a0 047c 00a1 0101 0074  .t.d.....|.....t
+00000210: 0564 037c 0069 0183 0101 0057 0064 0053  .d.|.i.....W.d.S
+00000220: 0004 0074 0679 3601 007d 0201 007a 1074  ...t.y6..}...z.t
+00000230: 0564 0483 0101 0074 0064 057c 0283 0201  .d.....t.d.|....
+00000240: 0057 0059 0064 007d 027e 0264 0053 0064  .W.Y.d.}.~.d.S.d
+00000250: 007d 027e 0277 0177 0029 064e 7a0c 6164  .}.~.w.w.).Nz.ad
+00000260: 645f 616e 6f6d 616c 793f 7210 0000 00da  d_anomaly?r.....
+00000270: 0761 6e6f 6d61 6c79 7a1d 416e 2061 6e6f  .anomalyz.An ano
+00000280: 6d61 6c79 2063 6f75 6c64 6e27 7420 6265  maly couldn't be
+00000290: 2061 6464 6564 2e7a 0a65 7863 6570 7469   added.z.excepti
+000002a0: 6f6e 3a29 07da 0570 7269 6e74 da04 6a73  on:)...print..js
+000002b0: 6f6e da05 6475 6d70 73da 1461 6767 7265  on..dumps..aggre
+000002c0: 6761 746f 725f 7661 7269 6162 6c65 73da  gator_variables.
+000002d0: 0661 7070 656e 6472 0300 0000 da09 4578  .appendr......Ex
+000002e0: 6365 7074 696f 6e29 0372 1100 0000 da07  ception).r......
+000002f0: 6973 5f4a 534f 4eda 0145 a900 721a 0000  is_JSON..E..r...
+00000300: 00fa 5c2f 6269 6f74 6563 682f 7665 6e75  ..\/biotech/venu
+00000310: 6573 2f73 7461 6765 732f 6269 6f74 6563  es/stages/biotec
+00000320: 682f 7072 6f63 6564 7572 6573 2f61 6767  h/procedures/agg
+00000330: 7265 6761 746f 725f 7072 6f63 6564 7572  regator_procedur
+00000340: 652f 7072 6f63 6573 732f 7661 7269 6162  e/process/variab
+00000350: 6c65 732f 5f5f 696e 6974 5f5f 2e70 79da  les/__init__.py.
+00000360: 0b61 6464 5f61 6e6f 6d61 6c79 4900 0000  .add_anomalyI...
+00000370: 7318 0000 000a 0102 020a 010e 0202 0204  s...............
+00000380: 010c ff0e 0408 0118 0108 8002 fe72 1c00  .............r..
+00000390: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
+000003a0: 0000 000a 0000 0043 0000 0073 4e00 0000  .......C...sN...
+000003b0: 7c00 4400 5d22 7d02 6401 6401 6401 6401  |.D.]"}.d.d.d.d.
+000003c0: 6402 6401 6401 6403 6404 9c08 6405 6406  d.d.d.d.d...d.d.
+000003d0: 6901 6403 6403 6403 6403 6407 9c04 6700  i.d.d.d.d.d...g.
+000003e0: 6400 6400 6408 9c06 7400 6409 1900 7401  d.d.d...t.d...t.
+000003f0: 7c02 7c01 8302 3c00 7102 6400 5300 290a  |.|...<.q.d.S.).
+00000400: 4e72 0900 0000 da07 756e 6b6e 6f77 6e72  Nr......unknownr
+00000410: 0400 0000 2908 7a1c 7363 616e 2070 726f  ....).z.scan pro
+00000420: 6365 7373 2076 656e 7475 7265 2073 7461  cess venture sta
+00000430: 7274 6564 7a14 7363 616e 2070 726f 6365  rtedz.scan proce
+00000440: 7373 2073 7461 7274 6564 7a20 7363 616e  ss startedz scan
+00000450: 2070 726f 6365 7373 206e 6f74 6966 6965   process notifie
+00000460: 6420 6167 6772 6567 6174 6f72 7a18 7363  d aggregatorz.sc
+00000470: 616e 2070 726f 6365 7373 2077 6173 2073  an process was s
+00000480: 746f 7070 6564 7a15 7363 616e 2070 726f  toppedz.scan pro
+00000490: 6365 7373 2069 7320 616c 6976 657a 1c73  cess is alivez.s
+000004a0: 6361 6e20 7072 6f63 6565 6473 2077 6572  can proceeds wer
+000004b0: 6520 7265 7472 6965 7665 647a 1b73 6361  e retrievedz.sca
+000004c0: 6e20 7265 636f 7264 7320 7765 7265 2072  n records were r
+000004d0: 6574 7269 6576 6564 7a10 646f 6e65 2072  etrievedz.done r
+000004e0: 6561 736f 6e20 6769 7665 da07 7072 6f63  eason give..proc
+000004f0: 6573 73da 0770 656e 6469 6e67 2904 da07  ess..pending)...
+00000500: 7374 6172 7465 64da 0565 6e64 6564 da07  started..ended..
+00000510: 656c 6170 7365 647a 1172 6563 6f72 6473  elapsedz.records
+00000520: 2072 6574 7269 6576 616c 2906 da0b 6f63   retrieval)...oc
+00000530: 6375 7272 656e 6365 73da 0673 7461 7475  currences..statu
+00000540: 73da 0574 696d 6573 da07 7265 636f 7264  s..times..record
+00000550: 7372 1e00 0000 da0f 7265 7375 6c74 735f  sr......results_
+00000560: 6f66 5f73 6361 6e72 0e00 0000 2902 7215  of_scanr....).r.
+00000570: 0000 0072 0200 0000 2903 da12 7374 6174  ...r....)...stat
+00000580: 7573 5f63 6865 636b 5f70 6174 6873 da0d  us_check_paths..
+00000590: 7265 6c61 7469 7665 5f70 6174 68da 1173  relative_path..s
+000005a0: 7461 7475 735f 6368 6563 6b5f 7061 7468  tatus_check_path
+000005b0: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
+000005c0: 1773 6574 7570 5f69 6e74 6572 6e61 6c5f  .setup_internal_
+000005d0: 7374 6174 7573 6573 5a00 0000 7332 0000  statusesZ...s2..
+000005e0: 0008 0402 0c02 0702 0802 0702 0702 0802  ................
+000005f0: 0702 0704 c504 4102 ff02 0602 0102 0102  ......A.........
+00000600: 0104 fc02 0702 0202 0104 b006 fe08 0104  ................
+00000610: ff04 5672 2b00 0000 6300 0000 0000 0000  ..Vr+...c.......
+00000620: 0000 0000 0000 0000 0001 0000 0043 0000  .............C..
+00000630: 0073 0400 0000 6400 5300 a901 4e72 1a00  .s....d.S...Nr..
+00000640: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+00000650: 0072 1b00 0000 da06 6368 616e 6765 b700  .r......change..
+00000660: 0000 f302 0000 0004 0172 2d00 0000 6300  .........r-...c.
+00000670: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00000680: 0000 0043 0000 00f3 0400 0000 7400 5300  ...C........t.S.
+00000690: 722c 0000 00a9 0172 1500 0000 721a 0000  r,.....r....r...
+000006a0: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
+000006b0: da12 7265 7472 6965 7665 5f76 6172 6961  ..retrieve_varia
+000006c0: 626c 6573 ba00 0000 722e 0000 0072 3100  bles....r....r1.
+000006d0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000006e0: 0000 0001 0000 0043 0000 0072 2f00 0000  .......C...r/...
+000006f0: 722c 0000 0072 3000 0000 721a 0000 0072  r,...r0...r....r
+00000700: 1a00 0000 721a 0000 0072 1b00 0000 da1d  ....r....r......
+00000710: 7265 7472 6965 7665 5f61 6767 7265 6761  retrieve_aggrega
+00000720: 746f 725f 7661 7269 6162 6c65 73bd 0000  tor_variables...
+00000730: 0072 2e00 0000 7232 0000 0063 0000 0000  .r....r2...c....
+00000740: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00000750: 4300 0000 722f 0000 0072 2c00 0000 7230  C...r/...r,...r0
+00000760: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+00000770: 0000 721b 0000 00da 0872 6574 7269 6576  ..r......retriev
+00000780: 65c0 0000 0072 2e00 0000 7233 0000 0029  e....r....r3...)
+00000790: 0dda 075f 5f64 6f63 5f5f da41 6269 6f74  ...__doc__.Abiot
+000007a0: 6563 682e 7072 6f63 6564 7572 6573 2e61  ech.procedures.a
+000007b0: 6767 7265 6761 746f 725f 7072 6f63 6564  ggregator_proced
+000007c0: 7572 652e 7072 6f63 6573 732e 6d6f 7665  ure.process.move
+000007d0: 732e 666f 726d 6174 5f70 6174 6872 0200  s.format_pathr..
+000007e0: 0000 da1c 6269 6f74 6563 682e 746f 7069  ....biotech.topi
+000007f0: 6373 2e73 686f 772e 7661 7269 6162 6c65  cs.show.variable
+00000800: 7203 0000 0072 1300 0000 7215 0000 0072  r....r....r....r
+00000810: 1c00 0000 722b 0000 0072 2d00 0000 7231  ....r+...r-...r1
+00000820: 0000 0072 3200 0000 7233 0000 0072 1a00  ...r2...r3...r..
+00000830: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000840: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000850: 2e00 0000 0402 0204 0c09 0c01 0802 0202  ................
+00000860: 0207 0215 0201 04fe 0205 0202 0207 0205  ................
+00000870: 0201 0202 06e9 081a 0811 085d 0803 0803  ...........]....
+00000880: 0c03                                     ..
```

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py` & `biotech-1.1.5/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 22:29:36 2024 UTC, .py size: 500 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-00000000: 6f0d 0d0a 0000 0000 50f0 2266 f401 0000  o.......P."f....
+00000000: 6f0d 0d0a 0000 0000 7d3a 2366 b802 0000  o.......}:#f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
+00000020: 0003 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 0903 0903 0903 6407 6404  m.Z.........d.d.
-00000050: 6405 8401 5a04 6406 5300 2908 e900 0000  d...Z.d.S.).....
-00000060: 0029 01da 1370 726f 6365 7373 5f6f 6e5f  .)...process_on_
-00000070: 696d 706c 6963 6974 2901 da0d 7368 6f77  implicit)...show
-00000080: 5f76 6172 6961 626c 65da 0063 0300 0000  _variable..c....
-00000090: 0000 0000 0000 0000 0500 0000 0500 0000  ................
-000000a0: 4300 0000 732c 0000 0064 017c 0017 007d  C...s,...d.|...}
-000000b0: 0374 007c 037c 0164 029c 0283 0101 0074  .t.|.|.d.......t
-000000c0: 0164 017c 0017 007c 017c 0264 038d 037d  .d.|...|.|.d...}
-000000d0: 047c 0453 0029 044e 7a08 7079 7468 6f6e  .|.S.).Nz.python
-000000e0: 3320 2902 7a07 7363 7269 7074 3a7a 0465  3 ).z.script:z.e
-000000f0: 6e76 3a29 02da 0365 6e76 da04 6e61 6d65  nv:)...env..name
-00000100: 2902 7203 0000 0072 0200 0000 2905 da0c  ).r....r....)...
-00000110: 7072 6f63 6573 735f 7061 7468 7205 0000  process_pathr...
-00000120: 0072 0600 0000 da06 7363 7269 7074 da10  .r......script..
-00000130: 7468 655f 6865 616c 7468 5f63 6865 636b  the_health_check
-00000140: a900 720a 0000 00fa 452f 6269 6f74 6563  ..r.....E/biotec
-00000150: 682f 7665 6e75 6573 2f73 7461 6765 732f  h/venues/stages/
-00000160: 6269 6f74 6563 682f 7072 6f63 6564 7572  biotech/procedur
-00000170: 6573 2f68 6561 6c74 685f 7363 616e 2f64  es/health_scan/d
-00000180: 796e 616d 6963 5f70 6f72 742e 7079 da0c  ynamic_port.py..
-00000190: 6479 6e61 6d69 635f 706f 7274 0600 0000  dynamic_port....
-000001a0: 7316 0000 0008 0602 0202 0102 0108 fe02  s...............
-000001b0: 0506 0102 0302 0106 fb04 0972 0c00 0000  ...........r....
-000001c0: 4e29 0372 0400 0000 7204 0000 0072 0400  N).r....r....r..
-000001d0: 0000 2905 da2b 6269 6f74 6563 682e 746f  ..)..+biotech.to
-000001e0: 7069 6373 2e70 726f 6365 7373 5f6f 6e2e  pics.process_on.
-000001f0: 705f 6578 7065 6374 2e69 6d70 6c69 6369  p_expect.implici
-00000200: 7472 0200 0000 da1c 6269 6f74 6563 682e  tr......biotech.
-00000210: 746f 7069 6373 2e73 686f 772e 7661 7269  topics.show.vari
-00000220: 6162 6c65 7203 0000 0072 0c00 0000 720a  abler....r....r.
-00000230: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
-00000240: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000250: 730c 0000 000c 020c 0102 0302 0202 010e  s...............
-00000260: fc                                       .
+00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000050: 0100 0904 0904 0904 6408 6405 6406 8401  ........d.d.d...
+00000060: 5a06 6407 5300 2909 e900 0000 0029 01da  Z.d.S.)......)..
+00000070: 1370 726f 6365 7373 5f6f 6e5f 696d 706c  .process_on_impl
+00000080: 6963 6974 2901 da0d 7368 6f77 5f76 6172  icit)...show_var
+00000090: 6961 626c 6529 01da 1770 726f 6365 7373  iable)...process
+000000a0: 5f6f 6e5f 7375 625f 696d 706c 6963 6974  _on_sub_implicit
+000000b0: da00 6303 0000 0000 0000 0000 0000 0005  ..c.............
+000000c0: 0000 0004 0000 0043 0000 0073 2c00 0000  .......C...s,...
+000000d0: 6401 7c00 1700 7d03 7400 7c03 7c01 6402  d.|...}.t.|.|.d.
+000000e0: 9c02 8301 0100 0900 7401 6401 7c00 1700  ........t.d.|...
+000000f0: 7c01 6403 8d02 7d04 7c04 5300 2904 4e7a  |.d...}.|.S.).Nz
+00000100: 0870 7974 686f 6e33 2029 027a 0773 6372  .python3 ).z.scr
+00000110: 6970 743a 7a04 656e 763a 2901 da03 656e  ipt:z.env:)...en
+00000120: 7629 0272 0300 0000 7204 0000 0029 05da  v).r....r....)..
+00000130: 0c70 726f 6365 7373 5f70 6174 6872 0600  .process_pathr..
+00000140: 0000 da04 6e61 6d65 da06 7363 7269 7074  ....name..script
+00000150: da10 7468 655f 6865 616c 7468 5f63 6865  ..the_health_che
+00000160: 636b a900 720b 0000 00fa 452f 6269 6f74  ck..r.....E/biot
+00000170: 6563 682f 7665 6e75 6573 2f73 7461 6765  ech/venues/stage
+00000180: 732f 6269 6f74 6563 682f 7072 6f63 6564  s/biotech/proced
+00000190: 7572 6573 2f68 6561 6c74 685f 7363 616e  ures/health_scan
+000001a0: 2f64 796e 616d 6963 5f70 6f72 742e 7079  /dynamic_port.py
+000001b0: da0c 6479 6e61 6d69 635f 706f 7274 0900  ..dynamic_port..
+000001c0: 0000 7316 0000 0008 0602 0202 0102 0108  ..s.............
+000001d0: fe02 0502 0a06 0102 0306 fc04 0872 0d00  .............r..
+000001e0: 0000 4e29 0372 0500 0000 7205 0000 0072  ..N).r....r....r
+000001f0: 0500 0000 2907 da2b 6269 6f74 6563 682e  ....)..+biotech.
+00000200: 746f 7069 6373 2e70 726f 6365 7373 5f6f  topics.process_o
+00000210: 6e2e 705f 6578 7065 6374 2e69 6d70 6c69  n.p_expect.impli
+00000220: 6369 7472 0200 0000 da1c 6269 6f74 6563  citr......biotec
+00000230: 682e 746f 7069 6373 2e73 686f 772e 7661  h.topics.show.va
+00000240: 7269 6162 6c65 7203 0000 00da 2662 696f  riabler.....&bio
+00000250: 7465 6368 2e74 6f70 6963 732e 7072 6f63  tech.topics.proc
+00000260: 6573 735f 6f6e 2e73 7562 2e69 6d70 6c69  ess_on.sub.impli
+00000270: 6369 7472 0400 0000 720d 0000 0072 0b00  citr....r....r..
+00000280: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
+00000290: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000002a0: 0e00 0000 0c02 0c01 0c02 0204 0202 0201  ................
+000002b0: 0efc                                     ..
```

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/on.py` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py` & `biotech-1.1.5/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/intro/on.py` & `biotech-1.1.5/venues/stages/biotech/procedures/intro/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/adventure.py` & `biotech-1.1.5/venues/stages/biotech/procedures/intro/process/adventure.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py` & `biotech-1.1.5/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py` & `biotech-1.1.5/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/keg/__init__.py` & `biotech-1.1.5/venues/stages/biotech/procedures/intro/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar 18 22:01:24 2024 UTC, .py size: 403 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,59 @@
-00000000: 6f0d 0d0a 0000 0000 b4b9 f865 9301 0000  o..........e....
+00000000: 6f0d 0d0a 0000 0000 5c08 2366 fc02 0000  o.......\.#f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
-00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 5a02 6401 6402 6c03 5a03 6403 6504 6404  Z.d.d.l.Z.d.e.d.
-00000050: 6505 6604 6405 6406 8404 5a06 6402 5300  e.f.d.d...Z.d.S.
-00000060: 2907 7a31 0a69 6d70 6f72 7420 766f 6c74  ).z1.import volt
-00000070: 732e 746f 7069 6373 2e65 7863 6570 7469  s.topics.excepti
-00000080: 6f6e 7320 6173 2062 735f 6578 6365 7074  ons as bs_except
-00000090: 696f 6e73 0ae9 0000 0000 4eda 0965 7863  ions......N..exc
-000000a0: 6570 7469 6f6e da06 7265 7475 726e 6301  eption..returnc.
-000000b0: 0000 0000 0000 0000 0000 0002 0000 0008  ................
-000000c0: 0000 0043 0000 0073 4000 0000 7a15 7400  ...C...s@...z.t.
-000000d0: a001 a100 7d01 7402 6a03 7c00 7c01 6401  ....}.t.j.|.|.d.
-000000e0: 8d02 0100 7c01 a004 a100 a005 a100 a006  ....|...........
-000000f0: 6402 a101 5700 5300 0400 7407 791f 0100  d...W.S...t.y...
-00000100: 0100 0100 5900 6403 5300 7700 2904 4e29  ....Y.d.S.w.).N)
-00000110: 01da 0466 696c 65da 010a 7a2e 416e 2065  ...file...z.An e
-00000120: 7863 6570 7469 6f6e 206f 6363 7572 7265  xception occurre
-00000130: 6420 7768 696c 6520 6361 6c63 756c 6174  d while calculat
-00000140: 696e 6720 7472 6163 652e 2908 da02 696f  ing trace.)...io
-00000150: da08 5374 7269 6e67 494f da09 7472 6163  ..StringIO..trac
-00000160: 6562 6163 6bda 0f70 7269 6e74 5f65 7863  eback..print_exc
-00000170: 6570 7469 6f6e da08 6765 7476 616c 7565  eption..getvalue
-00000180: da06 7273 7472 6970 da05 7370 6c69 74da  ..rstrip..split.
-00000190: 0945 7863 6570 7469 6f6e 2902 7202 0000  .Exception).r...
-000001a0: 0072 0400 0000 a900 720e 0000 00fa 6d2f  .r......r.....m/
-000001b0: 6d65 6469 612f 6361 6c63 756c 6174 6f72  media/calculator
-000001c0: 2f77 6174 6572 2f73 7461 7475 7336 3030  /water/status600
-000001d0: 2e63 6f6d 2f47 4c2f 7374 6174 7573 3630  .com/GL/status60
-000001e0: 302f 636c 696d 6174 6573 2f76 6f6c 7473  0/climates/volts
-000001f0: 2f73 7472 7563 7475 7265 732f 6465 636f  /structures/deco
-00000200: 722f 766f 6c74 732f 746f 7069 6373 2f65  r/volts/topics/e
-00000210: 7863 6570 7469 6f6e 732e 7079 da0a 6669  xceptions.py..fi
-00000220: 6e64 5f74 7261 6365 0a00 0000 7310 0000  nd_trace....s...
-00000230: 0002 0108 010e 0114 040c 0102 0104 0202  ................
-00000240: fd72 1000 0000 2907 da07 5f5f 646f 635f  .r....)...__doc_
-00000250: 5f72 0600 0000 da03 7379 7372 0800 0000  _r......sysr....
-00000260: 720d 0000 00da 0373 7472 7210 0000 0072  r......strr....r
-00000270: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
-00000280: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000290: 0073 0a00 0000 0402 0804 0801 0801 1601  .s..............
+00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
+00000030: 5a00 0900 6401 6402 6c01 5a01 6401 6402  Z...d.d.l.Z.d.d.
+00000040: 6c02 5a02 6401 6402 6c03 5a03 6403 6504  l.Z.d.d.l.Z.d.e.
+00000050: 6404 6505 6604 6405 6406 8404 5a06 6407  d.e.f.d.d...Z.d.
+00000060: 6408 8400 5a07 6402 5300 2909 7a33 0a69  d...Z.d.S.).z3.i
+00000070: 6d70 6f72 7420 6269 6f74 6563 682e 746f  mport biotech.to
+00000080: 7069 6373 2e65 7863 6570 7469 6f6e 7320  pics.exceptions 
+00000090: 6173 2062 735f 6578 6365 7074 696f 6e73  as bs_exceptions
+000000a0: 0ae9 0000 0000 4eda 0965 7863 6570 7469  ......N..excepti
+000000b0: 6f6e da06 7265 7475 726e 6301 0000 0000  on..returnc.....
+000000c0: 0000 0000 0000 0002 0000 0008 0000 0043  ...............C
+000000d0: 0000 0073 4000 0000 7a15 7400 a001 a100  ...s@...z.t.....
+000000e0: 7d01 7402 6a03 7c00 7c01 6401 8d02 0100  }.t.j.|.|.d.....
+000000f0: 7c01 a004 a100 a005 a100 a006 6402 a101  |...........d...
+00000100: 5700 5300 0400 7407 791f 0100 0100 0100  W.S...t.y.......
+00000110: 5900 6403 5300 7700 2904 4e29 01da 0466  Y.d.S.w.).N)...f
+00000120: 696c 65da 010a 7a2e 416e 2065 7863 6570  ile...z.An excep
+00000130: 7469 6f6e 206f 6363 7572 7265 6420 7768  tion occurred wh
+00000140: 696c 6520 6361 6c63 756c 6174 696e 6720  ile calculating 
+00000150: 7472 6163 652e 2908 da02 696f da08 5374  trace.)...io..St
+00000160: 7269 6e67 494f da09 7472 6163 6562 6163  ringIO..tracebac
+00000170: 6bda 0f70 7269 6e74 5f65 7863 6570 7469  k..print_excepti
+00000180: 6f6e da08 6765 7476 616c 7565 da06 7273  on..getvalue..rs
+00000190: 7472 6970 da05 7370 6c69 74da 0945 7863  trip..split..Exc
+000001a0: 6570 7469 6f6e 2902 7202 0000 0072 0400  eption).r....r..
+000001b0: 0000 a900 720e 0000 00fa 332f 6269 6f74  ....r.....3/biot
+000001c0: 6563 682f 7665 6e75 6573 2f73 7461 6765  ech/venues/stage
+000001d0: 732f 6269 6f74 6563 682f 746f 7069 6373  s/biotech/topics
+000001e0: 2f65 7863 6570 7469 6f6e 732e 7079 da0a  /exceptions.py..
+000001f0: 6669 6e64 5f74 7261 6365 0e00 0000 7310  find_trace....s.
+00000200: 0000 0002 0108 010e 0114 040c 0102 0104  ................
+00000210: 0202 fd72 1000 0000 6301 0000 0000 0000  ...r....c.......
+00000220: 0000 0000 0002 0000 0008 0000 0043 0000  .............C..
+00000230: 0073 3e00 0000 7a10 7400 a001 7402 7c00  .s>...z.t...t.|.
+00000240: 8301 7c00 7c00 6a03 a103 7d01 6401 a004  ..|.|.j...}.d...
+00000250: 7c01 a101 5700 5300 0400 7405 791e 0100  |...W.S...t.y...
+00000260: 0100 0100 7406 6402 8301 0100 5900 6403  ....t.d.....Y.d.
+00000270: 5300 7700 2904 4eda 007a 1863 6f75 6c64  S.w.).N..z.could
+00000280: 6e27 7420 7061 7273 6520 6578 6365 7074  n't parse except
+00000290: 696f 6e7a 1963 6f75 6c64 206e 6f74 2070  ionz.could not p
+000002a0: 6172 7365 2065 7863 6570 7469 6f6e 2907  arse exception).
+000002b0: 7208 0000 00da 1066 6f72 6d61 745f 6578  r......format_ex
+000002c0: 6365 7074 696f 6eda 0474 7970 65da 0d5f  ception..type.._
+000002d0: 5f74 7261 6365 6261 636b 5f5f da04 6a6f  _traceback__..jo
+000002e0: 696e 720d 0000 00da 0570 7269 6e74 2902  inr......print).
+000002f0: da01 65da 1165 7863 6570 7469 6f6e 5f6d  ..e..exception_m
+00000300: 6573 7361 6765 720e 0000 0072 0e00 0000  essager....r....
+00000310: 720f 0000 00da 0f70 6172 7365 5f65 7863  r......parse_exc
+00000320: 6570 7469 6f6e 1c00 0000 730e 0000 0002  eption....s.....
+00000330: 0114 020c 010c 020a 0104 0202 fd72 1900  .............r..
+00000340: 0000 2908 da07 5f5f 646f 635f 5f72 0600  ..)...__doc__r..
+00000350: 0000 da03 7379 7372 0800 0000 720d 0000  ....sysr....r...
+00000360: 00da 0373 7472 7210 0000 0072 1900 0000  ...strr....r....
+00000370: 720e 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000380: 0f00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000390: 0000 730e 0000 0004 0202 0408 0408 0108  ..s.............
+000003a0: 0112 010c 0e                             .....
```

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/aggregate/__init__.py` & `biotech-1.1.5/venues/stages/biotech/topics/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/alarm_parser/__init__.py` & `biotech-1.1.5/venues/stages/biotech/topics/alarm_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__init__.py` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__init__.py` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/basin/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/treasury.py` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/basin/treasury.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/shares.s.HTML` & `biotech-1.1.5/venues/stages/biotech/topics/help_documentation/shares.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/implicit/proc/__init__.py` & `biotech-1.1.5/venues/stages/biotech/topics/implicit/proc/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/implicit/thread/__init__.py` & `biotech-1.1.5/venues/stages/biotech/topics/implicit/thread/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/printout/passes.py` & `biotech-1.1.5/venues/stages/biotech/topics/printout/passes.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__init__.py` & `biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 23:27:54 2024 UTC, .py size: 1586 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,114 +1,137 @@
-00000000: 6f0d 0d0a 0000 0000 fafd 2266 3206 0000  o........."f2...
+00000000: 6f0d 0d0a 0000 0000 cd38 2366 a407 0000  o........8#f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
+00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6401 6403 6c06 5a06 6401  m.Z...d.d.l.Z.d.
-00000070: 6403 6c09 5a09 6405 6406 8400 5a0a 6403  d.l.Z.d.d...Z.d.
-00000080: 6403 6900 6407 6604 6408 6409 8401 5a0b  d.i.d.f.d.d...Z.
-00000090: 6403 5300 290a 6144 0100 000a 0966 726f  d.S.).aD.....fro
-000000a0: 6d20 6269 6f74 6563 682e 746f 7069 6373  m biotech.topics
-000000b0: 2e70 726f 6365 7373 5f6f 6e2e 705f 6578  .process_on.p_ex
-000000c0: 7065 6374 2e69 6d70 6c69 6369 7420 696d  pect.implicit im
-000000d0: 706f 7274 2070 726f 6365 7373 5f6f 6e5f  port process_on_
-000000e0: 696d 706c 6963 6974 0a09 0a09 7665 6e74  implicit....vent
-000000f0: 7572 6520 3d20 7072 6f63 6573 735f 6f6e  ure = process_on
-00000100: 5f69 6d70 6c69 6369 7420 280a 0909 2727  _implicit (...''
-00000110: 2c0a 0909 0a09 0943 5744 203d 204e 6f6e  ,......CWD = Non
-00000120: 652c 0a09 0965 6e76 203d 207b 7d0a 0929  e,...env = {}..)
-00000130: 0a09 0a09 230a 0923 2073 7461 7475 730a  ....#..# status.
-00000140: 0923 0a09 230a 0970 7269 6e74 2028 2773  .#..#..print ('s
-00000150: 7461 7475 733a 272c 2076 656e 7475 7265  tatus:', venture
-00000160: 205b 2270 726f 6365 7373 225d 2e69 735f   ["process"].is_
-00000170: 616c 6976 6520 2829 290a 090a 0923 0a09  alive ())....#..
-00000180: 2309 7374 6f70 2074 6865 2070 726f 6365  #.stop the proce
-00000190: 7373 0a09 230a 0923 0a09 7665 6e74 7572  ss..#..#..ventur
-000001a0: 6520 5b22 7072 6f63 6573 7322 5d2e 7465  e ["process"].te
-000001b0: 726d 696e 6174 6520 2829 0a09 0a09 7265  rminate ()....re
-000001c0: 636f 7264 7320 3d20 7665 6e74 7572 6520  cords = venture 
-000001d0: 5b22 7265 636f 7264 7322 5d20 2829 0ae9  ["records"] ()..
-000001e0: 0000 0000 2901 da0a 7072 6f63 6573 735f  ....)...process_
-000001f0: 6f6e 4e29 02da 0750 726f 6365 7373 da05  onN)...Process..
-00000200: 5175 6575 6563 0100 0000 0000 0000 0000  Queuec..........
-00000210: 0000 0200 0000 0a00 0000 4300 0000 7348  ..........C...sH
-00000220: 0000 007a 0b74 0064 0183 0101 007c 00a0  ...z.t.d.....|..
-00000230: 01a1 0001 0057 0064 0053 0004 0074 0279  .....W.d.S...t.y
-00000240: 2301 007d 0101 007a 0c74 0064 027c 0183  #..}...z.t.d.|..
-00000250: 0201 0057 0059 0064 007d 017e 0164 0053  ...W.Y.d.}.~.d.S
-00000260: 0064 007d 017e 0177 0177 0029 034e 7a33  .d.}.~.w.w.).Nz3
-00000270: 0a09 090a 0909 0961 7474 656d 7069 6e67  .......attemping
-00000280: 2074 6f20 7374 6f70 2074 6865 2069 6d70   to stop the imp
-00000290: 6c69 6369 7420 7665 6e74 7572 650a 0909  licit venture...
-000002a0: 0a09 097a 1f76 656e 7475 7265 2069 6d70  ...z.venture imp
-000002b0: 6c69 6369 7420 6f66 6620 6578 6365 7074  licit off except
-000002c0: 696f 6e3a 2903 da05 7072 696e 74da 0974  ion:)...print..t
-000002d0: 6572 6d69 6e61 7465 da09 4578 6365 7074  erminate..Except
-000002e0: 696f 6e29 02da 1069 6d70 6c69 6369 745f  ion)...implicit_
-000002f0: 7072 6f63 6573 73da 0145 a900 720a 0000  process..E..r...
-00000300: 00fa 452f 6269 6f74 6563 682f 7665 6e75  ..E/biotech/venu
-00000310: 6573 2f73 7461 6765 732f 6269 6f74 6563  es/stages/biotec
-00000320: 682f 746f 7069 6373 2f70 726f 6365 7373  h/topics/process
-00000330: 5f6f 6e2f 705f 6578 7065 6374 2f69 6d70  _on/p_expect/imp
-00000340: 6c69 6369 742e 7079 da03 6f66 6625 0000  licit.py..off%..
-00000350: 0073 1000 0000 0201 0801 0e05 0e01 0a01  .s..............
-00000360: 0e02 0880 02fd 720c 0000 00da 0770 726f  ......r......pro
-00000370: 6365 7373 6305 0000 0000 0000 0000 0000  cessc...........
-00000380: 0008 0000 0009 0000 0003 0000 0073 6200  .............sb.
-00000390: 0000 7400 8300 8901 7401 a002 a100 8900  ..t.....t.......
-000003a0: 7403 7404 7c00 6701 8801 7c02 7c03 7c04  t.t.|.g...|.|.|.
-000003b0: 8800 6401 9c05 6402 8d03 7d05 7c05 a005  ..d...d...}.|...
-000003c0: a100 0100 8701 6601 6403 6404 8408 7d06  ......f.d.d...}.
-000003d0: 8700 6601 6405 6406 8408 7d07 7406 a007  ..f.d.d...}.t...
-000003e0: 7408 7c05 a102 0100 7c05 7c06 7c07 6407  t.|.....|.|.|.d.
-000003f0: 9c03 5300 2908 4e29 05da 0974 6865 5f71  ..S.).N)...the_q
-00000400: 7565 7565 da03 4357 44da 0365 6e76 da04  ueue..CWD..env..
-00000410: 6e61 6d65 da0a 7374 6f70 5f65 7665 6e74  name..stop_event
-00000420: 2903 da06 7461 7267 6574 da04 6172 6773  )...target..args
-00000430: da06 6b77 6172 6773 6300 0000 0000 0000  ..kwargsc.......
-00000440: 0000 0000 0001 0000 0004 0000 0013 0000  ................
-00000450: 0073 2600 0000 6700 7d00 8800 a000 a100  .s&...g.}.......
-00000460: 7311 7c00 a001 8800 a002 a100 a101 0100  s.|.............
-00000470: 8800 a000 a100 7206 7c00 5300 a901 4e29  ......r.|.S...N)
-00000480: 03da 0565 6d70 7479 da06 6170 7065 6e64  ...empty..append
-00000490: da03 6765 7429 01da 0870 726f 6365 6564  ..get)...proceed
-000004a0: 7329 0172 0e00 0000 720a 0000 0072 0b00  s).r....r....r..
-000004b0: 0000 da0b 7061 7273 655f 7175 6575 6556  ....parse_queueV
-000004c0: 0000 0073 0a00 0000 0401 0801 0e01 08ff  ...s............
-000004d0: 0403 7a28 7072 6f63 6573 735f 6f6e 5f69  ..z(process_on_i
-000004e0: 6d70 6c69 6369 742e 3c6c 6f63 616c 733e  mplicit.<locals>
-000004f0: 2e70 6172 7365 5f71 7565 7565 6300 0000  .parse_queuec...
-00000500: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-00000510: 0013 0000 0073 0c00 0000 8800 a000 a100  .....s..........
-00000520: 0100 6400 5300 7216 0000 0029 01da 0373  ..d.S.r....)...s
-00000530: 6574 720a 0000 0029 0172 1200 0000 720a  etr....).r....r.
-00000540: 0000 0072 0b00 0000 da05 6f66 665f 315d  ...r......off_1]
-00000550: 0000 0073 0200 0000 0c02 7a22 7072 6f63  ...s......z"proc
-00000560: 6573 735f 6f6e 5f69 6d70 6c69 6369 742e  ess_on_implicit.
-00000570: 3c6c 6f63 616c 733e 2e6f 6666 5f31 2903  <locals>.off_1).
-00000580: 720d 0000 00da 0772 6563 6f72 6473 720c  r......recordsr.
-00000590: 0000 0029 0972 0400 0000 da0f 6d75 6c74  ...).r......mult
-000005a0: 6970 726f 6365 7373 696e 67da 0545 7665  iprocessing..Eve
-000005b0: 6e74 7203 0000 0072 0200 0000 da05 7374  ntr....r......st
-000005c0: 6172 74da 0661 7465 7869 74da 0872 6567  art..atexit..reg
-000005d0: 6973 7465 7272 0c00 0000 2908 da0e 7072  isterr....)...pr
-000005e0: 6f63 6573 735f 7374 7269 6e67 720e 0000  ocess_stringr...
-000005f0: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
-00000600: 7208 0000 0072 1b00 0000 721d 0000 0072  r....r....r....r
-00000610: 0a00 0000 2902 7212 0000 0072 0e00 0000  ....).r....r....
-00000620: 720b 0000 00da 1370 726f 6365 7373 5f6f  r......process_o
-00000630: 6e5f 696d 706c 6963 6974 3200 0000 732a  n_implicit2...s*
-00000640: 0000 0006 0908 0202 0202 0102 0302 ff02  ................
-00000650: 0502 0102 0102 0102 0204 fa06 f908 110c  ................
-00000660: 060c 070c 0402 0302 0102 0506 f972 2500  .............r%.
-00000670: 0000 290c da07 5f5f 646f 635f 5fda 2262  ..)...__doc__."b
-00000680: 696f 7465 6368 2e74 6f70 6963 732e 7072  iotech.topics.pr
-00000690: 6f63 6573 735f 6f6e 2e70 5f65 7870 6563  ocess_on.p_expec
-000006a0: 7472 0200 0000 da07 7065 7870 6563 74da  tr......pexpect.
-000006b0: 0472 6963 68da 026f 7372 1f00 0000 7203  .rich..osr....r.
-000006c0: 0000 0072 0400 0000 7222 0000 0072 0c00  ...r....r"...r..
-000006d0: 0000 7225 0000 0072 0a00 0000 720a 0000  ..r%...r....r...
-000006e0: 0072 0a00 0000 720b 0000 00da 083c 6d6f  .r....r......<mo
-000006f0: 6475 6c65 3e01 0000 0073 1c00 0000 0401  dule>....s......
-00000700: 0c19 0802 0801 0802 1001 0801 0801 0802  ................
-00000710: 0210 0201 0201 0202 0ef9                 ..........
+00000070: 6403 6c09 5a09 6401 6403 6c0a 5a0a 6405  d.l.Z.d.d.l.Z.d.
+00000080: 6406 8400 5a0b 6403 6403 6900 6407 6604  d...Z.d.d.i.d.f.
+00000090: 6408 6409 8401 5a0c 6403 5300 290a 6155  d.d...Z.d.S.).aU
+000000a0: 0100 000a 0966 726f 6d20 6269 6f74 6563  .....from biotec
+000000b0: 682e 746f 7069 6373 2e70 726f 6365 7373  h.topics.process
+000000c0: 5f6f 6e2e 705f 6578 7065 6374 2e69 6d70  _on.p_expect.imp
+000000d0: 6c69 6369 7420 696d 706f 7274 2070 726f  licit import pro
+000000e0: 6365 7373 5f6f 6e5f 696d 706c 6963 6974  cess_on_implicit
+000000f0: 0a09 0a09 7665 6e74 7572 6520 3d20 7072  ....venture = pr
+00000100: 6f63 6573 735f 6f6e 5f69 6d70 6c69 6369  ocess_on_implici
+00000110: 7420 280a 0909 2770 7974 686f 6e33 2073  t (...'python3 s
+00000120: 6572 7665 722e 7079 272c 0a09 090a 0909  erver.py',......
+00000130: 4357 4420 3d20 4e6f 6e65 2c0a 0909 656e  CWD = None,...en
+00000140: 7620 3d20 7b7d 0a09 290a 0976 656e 7475  v = {}..)..ventu
+00000150: 7265 205b 2270 726f 6365 7373 225d 2e74  re ["process"].t
+00000160: 6572 6d69 6e61 7465 2028 290a 090a 0923  erminate ()....#
+00000170: 0a09 2320 7374 6174 7573 0a09 230a 0923  ..# status..#..#
+00000180: 0a09 7072 696e 7420 2827 7374 6174 7573  ..print ('status
+00000190: 3a27 2c20 7665 6e74 7572 6520 5b22 7072  :', venture ["pr
+000001a0: 6f63 6573 7322 5d2e 6973 5f61 6c69 7665  ocess"].is_alive
+000001b0: 2028 2929 0a09 0a09 230a 0923 0973 746f   ())....#..#.sto
+000001c0: 7020 7468 6520 7072 6f63 6573 730a 0923  p the process..#
+000001d0: 0a09 230a 090a 0972 6563 6f72 6473 203d  ..#....records =
+000001e0: 2076 656e 7475 7265 205b 2272 6563 6f72   venture ["recor
+000001f0: 6473 225d 2028 290a e900 0000 0029 01da  ds"] ()......)..
+00000200: 0a70 726f 6365 7373 5f6f 6e4e 2902 da07  .process_onN)...
+00000210: 5072 6f63 6573 73da 0551 7565 7565 6301  Process..Queuec.
+00000220: 0000 0000 0000 0000 0000 0002 0000 000a  ................
+00000230: 0000 0043 0000 0073 4800 0000 7a0b 7400  ...C...sH...z.t.
+00000240: 6401 8301 0100 7c00 a001 a100 0100 5700  d.....|.......W.
+00000250: 6400 5300 0400 7402 7923 0100 7d01 0100  d.S...t.y#..}...
+00000260: 7a0c 7400 6402 7c01 8302 0100 5700 5900  z.t.d.|.....W.Y.
+00000270: 6400 7d01 7e01 6400 5300 6400 7d01 7e01  d.}.~.d.S.d.}.~.
+00000280: 7701 7700 2903 4e7a 330a 0909 0a09 0909  w.w.).Nz3.......
+00000290: 6174 7465 6d70 696e 6720 746f 2073 746f  attemping to sto
+000002a0: 7020 7468 6520 696d 706c 6963 6974 2076  p the implicit v
+000002b0: 656e 7475 7265 0a09 090a 0909 7a1f 7665  enture......z.ve
+000002c0: 6e74 7572 6520 696d 706c 6963 6974 206f  nture implicit o
+000002d0: 6666 2065 7863 6570 7469 6f6e 3a29 03da  ff exception:)..
+000002e0: 0570 7269 6e74 da09 7465 726d 696e 6174  .print..terminat
+000002f0: 65da 0945 7863 6570 7469 6f6e 2902 da10  e..Exception)...
+00000300: 696d 706c 6963 6974 5f70 726f 6365 7373  implicit_process
+00000310: da01 45a9 0072 0a00 0000 fa45 2f62 696f  ..E..r.....E/bio
+00000320: 7465 6368 2f76 656e 7565 732f 7374 6167  tech/venues/stag
+00000330: 6573 2f62 696f 7465 6368 2f74 6f70 6963  es/biotech/topic
+00000340: 732f 7072 6f63 6573 735f 6f6e 2f70 5f65  s/process_on/p_e
+00000350: 7870 6563 742f 696d 706c 6963 6974 2e70  xpect/implicit.p
+00000360: 79da 036f 6666 2600 0000 7310 0000 0002  y..off&...s.....
+00000370: 0108 010e 050e 010a 010e 0208 8002 fd72  ...............r
+00000380: 0c00 0000 da07 7072 6f63 6573 7363 0500  ......processc..
+00000390: 0000 0000 0000 0000 0000 0800 0000 0900  ................
+000003a0: 0000 0300 0000 7370 0000 0074 0083 0089  ......sp...t....
+000003b0: 0274 01a0 02a1 007d 0574 0374 047c 0067  .t.....}.t.t.|.g
+000003c0: 0188 027c 027c 037c 047c 0564 019c 0564  ...|.|.|.|.d...d
+000003d0: 028d 0389 0088 00a0 05a1 0001 0087 0266  ...............f
+000003e0: 0164 0364 0484 087d 0687 0066 0164 0564  .d.d...}...f.d.d
+000003f0: 0684 0889 0187 0087 0166 0264 0764 0884  .........f.d.d..
+00000400: 087d 0774 06a0 077c 07a1 0101 0088 007c  .}.t...|.......|
+00000410: 067c 0788 0164 099c 0453 0029 0a4e 2905  .|...d...S.).N).
+00000420: da09 7468 655f 7175 6575 65da 0343 5744  ..the_queue..CWD
+00000430: da03 656e 76da 046e 616d 65da 0a73 746f  ..env..name..sto
+00000440: 705f 6576 656e 7429 03da 0674 6172 6765  p_event)...targe
+00000450: 74da 0461 7267 73da 066b 7761 7267 7363  t..args..kwargsc
+00000460: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00000470: 0400 0000 1300 0000 7326 0000 0067 007d  ........s&...g.}
+00000480: 0088 00a0 00a1 0073 117c 00a0 0188 00a0  .......s.|......
+00000490: 02a1 00a1 0101 0088 00a0 00a1 0072 067c  .............r.|
+000004a0: 0053 0029 014e 2903 da05 656d 7074 79da  .S.).N)...empty.
+000004b0: 0661 7070 656e 64da 0367 6574 2901 da08  .append..get)...
+000004c0: 7072 6f63 6565 6473 2901 720e 0000 0072  proceeds).r....r
+000004d0: 0a00 0000 720b 0000 00da 0b70 6172 7365  ....r......parse
+000004e0: 5f71 7565 7565 5700 0000 730a 0000 0004  _queueW...s.....
+000004f0: 0108 010e 0108 ff04 037a 2870 726f 6365  .........z(proce
+00000500: 7373 5f6f 6e5f 696d 706c 6963 6974 2e3c  ss_on_implicit.<
+00000510: 6c6f 6361 6c73 3e2e 7061 7273 655f 7175  locals>.parse_qu
+00000520: 6575 6563 0000 0000 0000 0000 0000 0000  euec............
+00000530: 0000 0000 0800 0000 1300 0000 7338 0000  ............s8..
+00000540: 007a 0c88 00a0 00a1 0064 016b 0272 0a57  .z.......d.k.r.W
+00000550: 0064 0253 0057 0064 0353 0004 0074 0179  .d.S.W.d.S...t.y
+00000560: 1b01 0001 0001 0074 0264 0474 0383 0201  .......t.d.t....
+00000570: 0059 0064 0553 0077 0029 064e 54da 0379  .Y.d.S.w.).NT..y
+00000580: 6573 da02 6e6f 7a0a 6578 6365 7074 696f  es..noz.exceptio
+00000590: 6e3a da07 756e 6b6e 6f77 6e29 04da 0869  n:..unknown)...i
+000005a0: 735f 616c 6976 6572 0700 0000 7205 0000  s_aliver....r...
+000005b0: 0072 0900 0000 720a 0000 0029 0172 0800  .r....r....).r..
+000005c0: 0000 720a 0000 0072 0b00 0000 da08 6973  ..r....r......is
+000005d0: 5f67 6f69 6e67 5e00 0000 7310 0000 0002  _going^...s.....
+000005e0: 030c 0106 0106 020c 020c 0104 0202 fd7a  ...............z
+000005f0: 2570 726f 6365 7373 5f6f 6e5f 696d 706c  %process_on_impl
+00000600: 6963 6974 2e3c 6c6f 6361 6c73 3e2e 6973  icit.<locals>.is
+00000610: 5f67 6f69 6e67 6300 0000 0000 0000 0000  _goingc.........
+00000620: 0000 0000 0000 0003 0000 0013 0000 0073  ...............s
+00000630: 2e00 0000 8800 a000 a100 0100 8801 8300  ................
+00000640: 6401 6b02 7215 7401 a002 6402 a101 0100  d.k.r.t...d.....
+00000650: 8801 8300 6401 6b02 7309 6400 5300 6400  ....d.k.s.d.S.d.
+00000660: 5300 2903 4e72 1b00 0000 679a 9999 9999  S.).Nr....g.....
+00000670: 99b9 3f29 0372 0600 0000 da04 7469 6d65  ..?).r......time
+00000680: da05 736c 6565 7072 0a00 0000 2902 7208  ..sleepr....).r.
+00000690: 0000 0072 1f00 0000 720a 0000 0072 0b00  ...r....r....r..
+000006a0: 0000 da04 7374 6f70 6c00 0000 7308 0000  ....stopl...s...
+000006b0: 0008 030a 020a 0112 ff7a 2170 726f 6365  .........z!proce
+000006c0: 7373 5f6f 6e5f 696d 706c 6963 6974 2e3c  ss_on_implicit.<
+000006d0: 6c6f 6361 6c73 3e2e 7374 6f70 2904 720d  locals>.stop).r.
+000006e0: 0000 00da 0772 6563 6f72 6473 7222 0000  .....recordsr"..
+000006f0: 0072 1f00 0000 2908 7204 0000 00da 0f6d  .r....).r......m
+00000700: 756c 7469 7072 6f63 6573 7369 6e67 da05  ultiprocessing..
+00000710: 4576 656e 7472 0300 0000 7202 0000 00da  Eventr....r.....
+00000720: 0573 7461 7274 da06 6174 6578 6974 da08  .start..atexit..
+00000730: 7265 6769 7374 6572 2908 da0e 7072 6f63  register)...proc
+00000740: 6573 735f 7374 7269 6e67 720e 0000 0072  ess_stringr....r
+00000750: 0f00 0000 7210 0000 0072 1100 0000 7212  ....r....r....r.
+00000760: 0000 0072 1a00 0000 7222 0000 0072 0a00  ...r....r"...r..
+00000770: 0000 2903 7208 0000 0072 1f00 0000 720e  ..).r....r....r.
+00000780: 0000 0072 0b00 0000 da13 7072 6f63 6573  ...r......proces
+00000790: 735f 6f6e 5f69 6d70 6c69 6369 7433 0000  s_on_implicit3..
+000007a0: 0073 2e00 0000 0609 0802 0202 0201 0203  .s..............
+000007b0: 02ff 0205 0201 0201 0201 0202 04fa 06f9  ................
+000007c0: 0811 0c06 0c07 0e0e 0a0b 0203 0201 0205  ................
+000007d0: 0201 06f8 722a 0000 0029 0dda 075f 5f64  ....r*...)...__d
+000007e0: 6f63 5f5f da22 6269 6f74 6563 682e 746f  oc__."biotech.to
+000007f0: 7069 6373 2e70 726f 6365 7373 5f6f 6e2e  pics.process_on.
+00000800: 705f 6578 7065 6374 7202 0000 00da 0770  p_expectr......p
+00000810: 6578 7065 6374 da04 7269 6368 da02 6f73  expect..rich..os
+00000820: 7224 0000 0072 0300 0000 7204 0000 0072  r$...r....r....r
+00000830: 2700 0000 7220 0000 0072 0c00 0000 722a  '...r ...r....r*
+00000840: 0000 0072 0a00 0000 720a 0000 0072 0a00  ...r....r....r..
+00000850: 0000 720b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000860: 3e01 0000 0073 1e00 0000 0401 0c19 0802  >....s..........
+00000870: 0801 0802 1001 0801 0801 0801 0802 0210  ................
+00000880: 0201 0201 0202 0ef9                      ........
```

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/implicit.py` & `biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/implicit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 
 '''
 	from biotech.topics.process_on.p_expect.implicit import process_on_implicit
 	
 	venture = process_on_implicit (
-		'',
+		'python3 server.py',
 		
 		CWD = None,
 		env = {}
 	)
+	venture ["process"].terminate ()
 	
 	#
 	# status
 	#
 	#
 	print ('status:', venture ["process"].is_alive ())
 	
 	#
 	#	stop the process
 	#
 	#
-	venture ["process"].terminate ()
 	
 	records = venture ["records"] ()
 '''
 
 from biotech.topics.process_on.p_expect import process_on
 
 import pexpect
 import rich
 
 import os
 from multiprocessing import Process, Queue
 import multiprocessing
 import atexit
+import time
 
 def off (implicit_process):
 	try:
 		print ("""
 		
 			attemping to stop the implicit venture
 		
@@ -86,24 +87,46 @@
 	def parse_queue ():
 		proceeds = []
 		while not the_queue.empty ():
 			proceeds.append (the_queue.get ())
 	
 		return proceeds;
 	
-	def off_1 ():
-		nonlocal stop_event;
-		stop_event.set ()
+	def is_going ():
+		nonlocal implicit_process;
+		
+		try:
+			if (implicit_process.is_alive () == True):
+				return "yes"
+			
+			return "no"
+		
+		except Exception:
+			print ("exception:", E)
+			
+		return "unknown"
+	
+	def stop ():
+		nonlocal implicit_process;
+		
+		implicit_process.terminate ();
+		
+		while is_going () == "yes":
+			time.sleep (.1)
+	
+		#nonlocal stop_event;
+		#stop_event.set ()
 	
-	atexit.register (off, implicit_process)
+	atexit.register (stop)
 	
 	return {
 		"process": implicit_process,
 		"records": parse_queue,
 		
 		#
 		#	This might not do anything
 		#
-		"off": off_1
+		"stop": stop,
+		"is_going": is_going
 	}
```

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/parse_records.py` & `biotech-1.1.5/venues/stages/biotech/topics/process_on/p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/quay/garage.py` & `biotech-1.1.5/venues/stages/biotech/topics/quay/garage.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_1.py` & `biotech-1.1.5/venues/stages/biotech/topics/quay/implicit_process_test_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_2.py` & `biotech-1.1.5/venues/stages/biotech/topics/quay/implicit_process_test_2.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_3.py` & `biotech-1.1.5/venues/stages/biotech/topics/quay/implicit_process_test_3.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_4.py` & `biotech-1.1.5/venues/stages/biotech/topics/quay/implicit_process_test_4.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py` & `biotech-1.1.5/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/show/variable.py` & `biotech-1.1.5/venues/stages/biotech/topics/show/variable.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc` & `biotech-1.1.5/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/venues/stages/biotech/topics/start--/simultaneously.py` & `biotech-1.1.5/venues/stages/biotech/topics/start--/simultaneously.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.4/PKG-INFO` & `biotech-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotech
-Version: 1.1.4
+Version: 1.1.5
 Summary: A health monitoring stack
 License: GPL-3.0-only
 Keywords: alarms,screening,monitors,cybernetics,neurons,nervous system,bioelectric,homeostasis,reliability,consistency,integrity,guarantees,vows,oaths,assurances,insurances,ensurances,speed,calmness,education,augmentation,enhancement,improvements
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

