# Comparing `tmp/biotech-1.1.3.tar.gz` & `tmp/biotech-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotech-1.1.3.tar", max compression
+gzip compressed data, was "biotech-1.1.4.tar", max compression
```

## Comparing `biotech-1.1.3.tar` & `biotech-1.1.4.tar`

### file list

```diff
@@ -1,766 +1,761 @@
--rwxr-xr-x   0        0        0      211 2024-04-16 02:07:59.993436 biotech-1.1.3/license.S.HTML
--rwxr-xr-x   0        0        0     1145 2024-04-19 23:11:17.385428 biotech-1.1.3/pyproject.toml
--rwxr-xr-x   0        0        0     3866 2024-04-16 20:53:30.034757 biotech-1.1.3/readme.md
--rwxr-xr-x   0        0        0     2331 2024-04-19 15:34:34.407444 biotech-1.1.3/venue.S.HTML
--rwxr-xr-x   0        0        0   838272 2024-04-16 02:03:26.700967 biotech-1.1.3/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
--rwxr-xr-x   0        0        0     1270 2024-04-17 22:22:59.944800 biotech-1.1.3/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
--rwxr-xr-x   0        0        0     4079 2024-04-16 20:48:34.871383 biotech-1.1.3/venues/stages/biotech/___itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0      645 2024-04-16 20:48:34.875383 biotech-1.1.3/venues/stages/biotech/___itinerary/maybes.s.HTML
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout/script.py
--rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout/start.py
--rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
--rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
--rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
--rwxr-xr-x   0        0        0      385 2024-04-17 18:49:44.656786 biotech-1.1.3/venues/stages/biotech/__glossary/biotech_1
--rwxr-xr-x   0        0        0      114 2024-04-17 18:45:06.744254 biotech-1.1.3/venues/stages/biotech/__glossary/glossary.S.HTML
--rwxr-xr-x   0        0        0      130 2024-04-19 16:49:02.311131 biotech-1.1.3/venues/stages/biotech/__init__.py
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 biotech-1.1.3/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0     1252 2024-04-16 20:48:34.867383 biotech-1.1.3/venues/stages/biotech/_book/advanced tutorial.s.HTML
--rwxr-xr-x   0        0        0     1786 2024-04-16 20:48:34.867383 biotech-1.1.3/venues/stages/biotech/_book/book.s.HTML
--rwxr-xr-x   0        0        0      542 2024-04-16 20:48:34.867383 biotech-1.1.3/venues/stages/biotech/_book/relevant.s.HTML
--rwxr-xr-x   0        0        0     2129 2024-04-17 19:24:51.191926 biotech-1.1.3/venues/stages/biotech/_clique/__init__.py
--rwxr-xr-x   0        0        0     2493 2024-04-17 19:24:52.839918 biotech-1.1.3/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 biotech-1.1.3/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 biotech-1.1.3/venues/stages/biotech/_clique/group/__init__.py
--rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 biotech-1.1.3/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 biotech-1.1.3/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0  1404986 2024-04-19 23:11:01.025598 biotech-1.1.3/venues/stages/biotech/_status/DB/records.json
--rw-r--r--   0        0        0     1172 2024-04-19 22:15:38.920875 biotech-1.1.3/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
--rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 biotech-1.1.3/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
--rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 biotech-1.1.3/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
--rwxr-xr-x   0        0        0     1487 2024-04-19 22:15:36.412903 biotech-1.1.3/venues/stages/biotech/_status/establish.py
--rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416142 biotech-1.1.3/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 biotech-1.1.3/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      720 2024-04-16 20:48:34.887383 biotech-1.1.3/venues/stages/biotech/_status/monitors/-01_start/status_1.py
--rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 biotech-1.1.3/venues/stages/biotech/_status/monitors/00_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 biotech-1.1.3/venues/stages/biotech/_status/monitors/00_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      793 2024-04-16 20:48:34.883383 biotech-1.1.3/venues/stages/biotech/_status/monitors/00_start/status_1.py
--rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708148 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/path_1_health.py
--rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/path_2_health.py
--rwxr-xr-x   0        0        0     1161 2024-04-16 20:48:34.903383 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/status_1.py
--rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/1_health.py
--rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/2_health.py
--rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/modules/MODULE_1.py
--rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1214 2024-04-16 20:48:34.899383 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/status_1.py
--rwxr-xr-x   0        0        0      794 2024-04-16 20:48:34.891383 biotech-1.1.3/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py
--rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 biotech-1.1.3/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 biotech-1.1.3/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      939 2024-04-16 20:48:34.887383 biotech-1.1.3/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py
--rwxr-xr-x   0        0        0      289 2024-04-16 00:28:17.871373 biotech-1.1.3/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      517 2024-04-16 00:32:46.948536 biotech-1.1.3/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      942 2024-04-16 20:48:34.883383 biotech-1.1.3/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py
--rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py
--rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      867 2024-04-16 20:48:34.891383 biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/status_1.py
--rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/1_health.py
--rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/2_health.py
--rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/3_health.py
--rw-r--r--   0        0        0     1036 2024-04-19 19:54:47.501752 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/1_health.cpython-310.pyc
--rw-r--r--   0        0        0      183 2024-04-19 19:54:47.501752 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/2_health.cpython-310.pyc
--rw-r--r--   0        0        0      169 2024-04-19 19:54:47.505751 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/3_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      955 2024-04-19 22:40:42.880411 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/status_1.py
--rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 biotech-1.1.3/venues/stages/biotech/_status/monitors/07/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 biotech-1.1.3/venues/stages/biotech/_status/monitors/07/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0      809 2024-04-16 20:48:34.907383 biotech-1.1.3/venues/stages/biotech/_status/monitors/07/status_1.py
--rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 biotech-1.1.3/venues/stages/biotech/_status/monitors/08_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 biotech-1.1.3/venues/stages/biotech/_status/monitors/08_DB/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0     1561 2024-04-19 19:13:07.956368 biotech-1.1.3/venues/stages/biotech/_status/monitors/08_DB/status_1.py
--rwxr-xr-x   0        0        0    96037 2024-04-19 23:10:35.809859 biotech-1.1.3/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_2.py
--rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_3.py
--rwxr-xr-x   0        0        0     1442 2024-04-19 22:43:25.306602 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py
--rwxr-xr-x   0        0        0      367 2024-04-16 03:23:58.043895 biotech-1.1.3/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 biotech-1.1.3/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1189 2024-04-19 21:55:08.998787 biotech-1.1.3/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
--rw-r--r--   0        0        0      316 2024-04-19 18:57:32.516036 biotech-1.1.3/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       77 2024-04-19 18:57:24.196146 biotech-1.1.3/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1250 2024-04-19 21:55:16.358703 biotech-1.1.3/venues/stages/biotech/_status/monitors/11/status_1.py
--rwxr-xr-x   0        0        0      984 2024-04-18 03:32:30.971629 biotech-1.1.3/venues/stages/biotech/_status/status.proc.py
--rwxr-xr-x   0        0        0      256 2024-04-16 20:48:34.875383 biotech-1.1.3/venues/stages/biotech/_status/status.s.HTML
--rwxr-xr-x   0        0        0     1483 2024-04-16 20:48:34.851384 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
--rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
--rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
--rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 biotech-1.1.3/venues/stages/biotech/_status_advanced/status.proc.py
--rwxr-xr-x   0        0        0     1779 2024-04-16 20:48:34.575388 biotech-1.1.3/venues/stages/biotech/architecture.s.HTML
--rwxr-xr-x   0        0        0      241 2024-04-16 20:53:18.546926 biotech-1.1.3/venues/stages/biotech/emojis.S.HTML
--rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 biotech-1.1.3/venues/stages/biotech/license.S.HTML
--rwxr-xr-x   0        0        0     3068 2024-04-16 20:48:34.543389 biotech-1.1.3/venues/stages/biotech/module.s.HTML
--rw-r--r--   0        0        0     1596 2024-04-19 21:12:05.931720 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      640 2024-04-19 16:26:52.595637 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      259 2024-04-19 16:20:24.028904 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
--rwxr-xr-x   0        0        0     1478 2024-04-19 21:11:18.368263 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.648116 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/paths.py
--rwxr-xr-x   0        0        0      666 2024-04-19 21:46:15.516790 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
--rwxr-xr-x   0        0        0      562 2024-04-17 21:48:05.111704 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
--rwxr-xr-x   0        0        0     1163 2024-04-17 21:49:49.362841 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2023 2024-04-19 20:54:28.011750 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
--rw-r--r--   0        0        0     2447 2024-04-19 20:54:32.867695 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      999 2024-04-19 20:57:55.937395 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0     2881 2024-04-19 21:20:39.102102 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
--rw-r--r--   0        0        0     1152 2024-04-19 21:06:40.923425 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      653 2024-04-19 20:56:23.606442 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
--rwxr-xr-x   0        0        0     3572 2024-04-19 21:20:33.674162 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
--rwxr-xr-x   0        0        0      769 2024-04-19 21:06:33.619508 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
--rwxr-xr-x   0        0        0     2031 2024-04-19 16:27:13.563375 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
--rwxr-xr-x   0        0        0     1282 2024-04-15 20:31:31.342880 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0     2159 2024-04-19 23:06:58.868088 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      418 2024-04-17 20:03:55.692458 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      687 2024-04-15 22:21:10.822989 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
--rwxr-xr-x   0        0        0     3455 2024-04-17 21:41:59.150872 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
--rw-r--r--   0        0        0      728 2024-04-19 20:59:04.160621 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
--rwxr-xr-x   0        0        0      849 2024-04-17 20:12:15.035804 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
--rwxr-xr-x   0        0        0      933 2024-04-15 23:20:20.086332 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
--rwxr-xr-x   0        0        0     3451 2024-04-19 16:26:14.724115 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
--rwxr-xr-x   0        0        0     3235 2024-04-19 23:04:19.789690 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
--rwxr-xr-x   0        0        0      193 2024-04-17 20:02:37.661229 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
--rwxr-xr-x   0        0        0      514 2024-04-19 20:59:00.568662 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
--rwxr-xr-x   0        0        0     1834 2024-04-19 18:55:07.129933 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
--rw-r--r--   0        0        0     1851 2024-04-19 18:55:11.397883 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      799 2024-04-19 16:27:13.563375 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
--rw-r--r--   0        0        0     4350 2024-04-19 23:06:58.868088 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
--rw-r--r--   0        0        0     1268 2024-04-19 23:09:27.226569 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc
--rw-r--r--   0        0        0     1489 2024-04-19 23:09:22.198620 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py
--rwxr-xr-x   0        0        0      754 2024-04-18 00:33:41.120405 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
--rw-r--r--   0        0        0     1826 2024-04-19 18:56:22.468973 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-19 18:56:27.160910 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      996 2024-04-19 16:26:14.764114 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
--rwxr-xr-x   0        0        0     9847 2024-04-19 23:06:53.300145 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
--rwxr-xr-x   0        0        0     3303 2024-04-19 23:03:08.158399 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
--rw-r--r--   0        0        0     2018 2024-04-19 23:06:58.864088 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      834 2024-04-16 20:48:34.547389 biotech-1.1.3/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
--rwxr-xr-x   0        0        0      951 2024-04-16 20:49:56.266040 biotech-1.1.3/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      609 2024-04-19 22:29:43.435688 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
--rw-r--r--   0        0        0     1904 2024-04-19 22:33:09.357432 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      500 2024-04-19 22:29:36.979758 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/dynamic_port.py
--rwxr-xr-x   0        0        0     2161 2024-04-19 22:31:07.314772 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/on.py
--rwxr-xr-x   0        0        0     2200 2024-04-19 22:24:22.967141 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
--rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
--rwxr-xr-x   0        0        0     1441 2024-04-18 02:04:22.961501 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
--rwxr-xr-x   0        0        0      774 2024-04-16 20:48:34.555389 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
--rwxr-xr-x   0        0        0     1336 2024-04-15 21:13:32.676638 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      309 2024-04-17 23:41:26.722721 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      562 2024-04-17 23:41:26.734721 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      525 2024-04-17 23:09:55.764639 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      908 2024-04-19 20:05:11.362609 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0      636 2024-04-18 01:15:59.039315 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      289 2024-04-17 23:05:28.138584 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
--rwxr-xr-x   0        0        0      803 2024-04-19 20:05:09.858629 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
--rwxr-xr-x   0        0        0      378 2024-04-18 01:13:51.928249 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
--rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
--rwxr-xr-x   0        0        0     2182 2024-04-18 01:57:52.896535 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
--rwxr-xr-x   0        0        0     2125 2024-04-18 01:58:34.052216 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1828 2024-04-19 21:04:56.668613 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0     2295 2024-04-19 21:04:32.800884 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
--rw-r--r--   0        0        0        2 2024-04-19 22:32:11.666067 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/start.py
--rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
--rwxr-xr-x   0        0        0      152 2024-04-19 16:48:50.419277 biotech-1.1.3/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4699 2024-04-19 22:17:01.343942 biotech-1.1.3/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.3/venues/stages/biotech/procedures/intro/intro.S.HTML
--rwxr-xr-x   0        0        0     6305 2024-04-19 22:16:54.188023 biotech-1.1.3/venues/stages/biotech/procedures/intro/on.py
--rw-r--r--   0        0        0     2906 2024-04-19 21:43:07.254923 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
--rw-r--r--   0        0        0     4000 2024-04-19 21:42:57.331035 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/adventure.py
--rw-r--r--   0        0        0     1330 2024-04-19 21:12:05.939720 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      905 2024-04-19 16:56:52.013564 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      959 2024-04-19 21:11:59.243796 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      614 2024-04-19 16:56:41.273688 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
--rwxr-xr-x   0        0        0      138 2024-04-19 17:33:23.717242 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/intro.proc.py
--rwxr-xr-x   0        0        0     3084 2024-04-19 21:01:52.394709 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/keg/__init__.py
--rw-r--r--   0        0        0     3068 2024-04-19 21:01:58.358642 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/variables/__init__.py
--rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321766 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      172 2024-04-16 20:48:34.551389 biotech-1.1.3/venues/stages/biotech/procedures/procedures.S.HTML
--rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 biotech-1.1.3/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
--rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 biotech-1.1.3/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
--rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 biotech-1.1.3/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 biotech-1.1.3/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 biotech-1.1.3/venues/stages/biotech/topics/aggregate/__init__.py
--rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 biotech-1.1.3/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 biotech-1.1.3/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      708 2024-04-16 20:48:34.591388 biotech-1.1.3/venues/stages/biotech/topics/alarm_parser/__init__.py
--rwxr-xr-x   0        0        0      673 2024-04-16 20:49:28.126498 biotech-1.1.3/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 biotech-1.1.3/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      405 2024-04-16 20:48:34.579388 biotech-1.1.3/venues/stages/biotech/topics/exceptions.py
--rwxr-xr-x   0        0        0     1190 2024-01-27 05:31:08.525189 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
--rwxr-xr-x   0        0        0     2446 2024-04-17 19:24:25.140060 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__init__.py
--rwxr-xr-x   0        0        0     2491 2024-04-17 19:24:52.839918 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4471 2024-02-01 06:11:56.801715 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1050 2024-04-16 06:10:03.111579 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     1920 2024-01-31 18:50:23.812071 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
--rwxr-xr-x   0        0        0       24 2024-01-26 17:38:56.558087 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
--rwxr-xr-x   0        0        0       24 2024-01-26 17:38:52.854129 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
--rwxr-xr-x   0        0        0      751 2024-04-17 19:16:04.226583 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
--rwxr-xr-x   0        0        0     1981 2024-04-17 19:25:47.591625 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__init__.py
--rwxr-xr-x   0        0        0     2283 2024-04-17 19:25:53.011595 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4019 2024-01-31 18:51:47.652157 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     3843 2024-04-17 19:25:53.099595 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
--rwxr-xr-x   0        0        0     4426 2024-01-27 06:34:32.979965 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
--rwxr-xr-x   0        0        0     3559 2024-04-17 19:25:22.227762 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/treasury.py
--rwxr-xr-x   0        0        0     1727 2024-04-17 19:15:19.882965 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/shares.s.HTML
--rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 biotech-1.1.3/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1558 2024-04-18 05:22:02.832642 biotech-1.1.3/venues/stages/biotech/topics/implicit/proc/__init__.py
--rwxr-xr-x   0        0        0     1158 2024-04-19 21:23:01.800513 biotech-1.1.3/venues/stages/biotech/topics/implicit/thread/__init__.py
--rw-r--r--   0        0        0      855 2024-04-19 21:23:28.056219 biotech-1.1.3/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       90 2024-04-17 22:51:08.968798 biotech-1.1.3/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 22:33:48.860256 biotech-1.1.3/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
--rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 biotech-1.1.3/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
--rwxr-xr-x   0        0        0      470 2024-04-17 23:02:14.419990 biotech-1.1.3/venues/stages/biotech/topics/printout/bracket.py
--rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 biotech-1.1.3/venues/stages/biotech/topics/printout/passes.py
--rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 biotech-1.1.3/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2166 2024-04-19 22:38:28.357906 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__init__.py
--rw-r--r--   0        0        0     1997 2024-04-19 22:38:43.137742 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
--rw-r--r--   0        0        0     1818 2024-04-19 18:54:33.250328 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-18 01:45:27.254200 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1766 2024-04-19 18:53:11.523281 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-18 01:48:34.504806 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-18 01:45:24.082223 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
--rwxr-xr-x   0        0        0      195 2024-04-16 22:50:54.515336 biotech-1.1.3/venues/stages/biotech/topics/process_on/process_on.S.HTML
--rwxr-xr-x   0        0        0     1470 2024-04-18 04:12:56.845888 biotech-1.1.3/venues/stages/biotech/topics/quay/garage.py
--rwxr-xr-x   0        0        0     2546 2024-04-18 04:38:41.478278 biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_1.py
--rwxr-xr-x   0        0        0     1612 2024-04-18 04:54:58.414971 biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_2.py
--rwxr-xr-x   0        0        0      551 2024-04-18 05:20:40.701113 biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_3.py
--rwxr-xr-x   0        0        0     1083 2024-04-18 05:19:11.645613 biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_4.py
--rwxr-xr-x   0        0        0     1448 2024-04-19 22:40:22.232641 biotech-1.1.3/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
--rw-r--r--   0        0        0     1464 2024-04-19 22:41:14.292061 biotech-1.1.3/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 biotech-1.1.3/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
--rw-r--r--   0        0        0      246 2024-04-19 21:18:20.963631 biotech-1.1.3/venues/stages/biotech/topics/report_formats/report_formats.S.HTML
--rw-r--r--   0        0        0     1772 2024-04-19 20:59:56.440027 biotech-1.1.3/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0      461 2024-04-17 23:59:06.614967 biotech-1.1.3/venues/stages/biotech/topics/show/show.S.HTML
--rwxr-xr-x   0        0        0     2295 2024-04-19 20:59:53.444061 biotech-1.1.3/venues/stages/biotech/topics/show/variable.py
--rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
--rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
--rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
--rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
--rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
--rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
--rwxr-xr-x   0        0        0      273 2024-04-16 20:48:34.583388 biotech-1.1.3/venues/stages/biotech/topics/start--/one.py
--rwxr-xr-x   0        0        0      406 2024-04-16 20:48:34.587388 biotech-1.1.3/venues/stages/biotech/topics/start--/sequentially.py
--rwxr-xr-x   0        0        0      532 2024-04-16 20:48:34.587388 biotech-1.1.3/venues/stages/biotech/topics/start--/simultaneously.py
--rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 biotech-1.1.3/venues/stages/biotech/topics/topics.S.HTML
--rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 biotech-1.1.3/venues/stages/biotech/variables/__init__.py
--rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0      211 2024-04-16 02:07:59.993436 biotech-1.1.4/license.S.HTML
+-rwxr-xr-x   0        0        0     1145 2024-04-19 23:43:10.476201 biotech-1.1.4/pyproject.toml
+-rwxr-xr-x   0        0        0     3866 2024-04-16 20:53:30.034757 biotech-1.1.4/readme.md
+-rwxr-xr-x   0        0        0     2331 2024-04-19 15:34:34.407444 biotech-1.1.4/venue.S.HTML
+-rwxr-xr-x   0        0        0   838272 2024-04-16 02:03:26.700967 biotech-1.1.4/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
+-rwxr-xr-x   0        0        0     1270 2024-04-17 22:22:59.944800 biotech-1.1.4/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
+-rwxr-xr-x   0        0        0     4079 2024-04-16 20:48:34.871383 biotech-1.1.4/venues/stages/biotech/___itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      645 2024-04-16 20:48:34.875383 biotech-1.1.4/venues/stages/biotech/___itinerary/maybes.s.HTML
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout/script.py
+-rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout/start.py
+-rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
+-rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
+-rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
+-rwxr-xr-x   0        0        0      385 2024-04-17 18:49:44.656786 biotech-1.1.4/venues/stages/biotech/__glossary/biotech_1
+-rwxr-xr-x   0        0        0      114 2024-04-17 18:45:06.744254 biotech-1.1.4/venues/stages/biotech/__glossary/glossary.S.HTML
+-rwxr-xr-x   0        0        0      130 2024-04-19 16:49:02.311131 biotech-1.1.4/venues/stages/biotech/__init__.py
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 biotech-1.1.4/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0     1252 2024-04-16 20:48:34.867383 biotech-1.1.4/venues/stages/biotech/_book/advanced tutorial.s.HTML
+-rwxr-xr-x   0        0        0     1786 2024-04-16 20:48:34.867383 biotech-1.1.4/venues/stages/biotech/_book/book.s.HTML
+-rwxr-xr-x   0        0        0      542 2024-04-16 20:48:34.867383 biotech-1.1.4/venues/stages/biotech/_book/relevant.s.HTML
+-rwxr-xr-x   0        0        0     2129 2024-04-17 19:24:51.191926 biotech-1.1.4/venues/stages/biotech/_clique/__init__.py
+-rwxr-xr-x   0        0        0     2493 2024-04-17 19:24:52.839918 biotech-1.1.4/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 biotech-1.1.4/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 biotech-1.1.4/venues/stages/biotech/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 biotech-1.1.4/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 biotech-1.1.4/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0  1411387 2024-04-19 23:40:10.090237 biotech-1.1.4/venues/stages/biotech/_status/DB/records.json
+-rw-r--r--   0        0        0     1172 2024-04-19 22:15:38.920875 biotech-1.1.4/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 biotech-1.1.4/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 biotech-1.1.4/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1487 2024-04-19 22:15:36.412903 biotech-1.1.4/venues/stages/biotech/_status/establish.py
+-rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416142 biotech-1.1.4/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 biotech-1.1.4/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      720 2024-04-16 20:48:34.887383 biotech-1.1.4/venues/stages/biotech/_status/monitors/-01_start/status_1.py
+-rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 biotech-1.1.4/venues/stages/biotech/_status/monitors/00_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 biotech-1.1.4/venues/stages/biotech/_status/monitors/00_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      793 2024-04-16 20:48:34.883383 biotech-1.1.4/venues/stages/biotech/_status/monitors/00_start/status_1.py
+-rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708148 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/path_1_health.py
+-rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/path_2_health.py
+-rwxr-xr-x   0        0        0     1161 2024-04-16 20:48:34.903383 biotech-1.1.4/venues/stages/biotech/_status/monitors/01/status_1.py
+-rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/1_health.py
+-rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/2_health.py
+-rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/modules/MODULE_1.py
+-rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1214 2024-04-16 20:48:34.899383 biotech-1.1.4/venues/stages/biotech/_status/monitors/02/status_1.py
+-rwxr-xr-x   0        0        0      794 2024-04-16 20:48:34.891383 biotech-1.1.4/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py
+-rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 biotech-1.1.4/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 biotech-1.1.4/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      939 2024-04-16 20:48:34.887383 biotech-1.1.4/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      289 2024-04-16 00:28:17.871373 biotech-1.1.4/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      517 2024-04-16 00:32:46.948536 biotech-1.1.4/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      942 2024-04-16 20:48:34.883383 biotech-1.1.4/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py
+-rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      867 2024-04-16 20:48:34.891383 biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/status_1.py
+-rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/stasis/1_health.py
+-rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/stasis/2_health.py
+-rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/stasis/3_health.py
+-rw-r--r--   0        0        0     1036 2024-04-19 19:54:47.501752 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/1_health.cpython-310.pyc
+-rw-r--r--   0        0        0      183 2024-04-19 19:54:47.501752 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/2_health.cpython-310.pyc
+-rw-r--r--   0        0        0      169 2024-04-19 19:54:47.505751 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/3_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      955 2024-04-19 22:40:42.880411 biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/status_1.py
+-rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 biotech-1.1.4/venues/stages/biotech/_status/monitors/07/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 biotech-1.1.4/venues/stages/biotech/_status/monitors/07/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0      809 2024-04-16 20:48:34.907383 biotech-1.1.4/venues/stages/biotech/_status/monitors/07/status_1.py
+-rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 biotech-1.1.4/venues/stages/biotech/_status/monitors/08_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 biotech-1.1.4/venues/stages/biotech/_status/monitors/08_DB/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0     1561 2024-04-19 19:13:07.956368 biotech-1.1.4/venues/stages/biotech/_status/monitors/08_DB/status_1.py
+-rwxr-xr-x   0        0        0    98385 2024-04-19 23:39:44.894524 biotech-1.1.4/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_2.py
+-rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_3.py
+-rwxr-xr-x   0        0        0     1442 2024-04-19 22:43:25.306602 biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py
+-rwxr-xr-x   0        0        0      367 2024-04-16 03:23:58.043895 biotech-1.1.4/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 biotech-1.1.4/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1189 2024-04-19 21:55:08.998787 biotech-1.1.4/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
+-rw-r--r--   0        0        0      316 2024-04-19 18:57:32.516036 biotech-1.1.4/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.4/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       77 2024-04-19 18:57:24.196146 biotech-1.1.4/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1250 2024-04-19 21:55:16.358703 biotech-1.1.4/venues/stages/biotech/_status/monitors/11/status_1.py
+-rwxr-xr-x   0        0        0      984 2024-04-18 03:32:30.971629 biotech-1.1.4/venues/stages/biotech/_status/status.proc.py
+-rwxr-xr-x   0        0        0      256 2024-04-16 20:48:34.875383 biotech-1.1.4/venues/stages/biotech/_status/status.s.HTML
+-rwxr-xr-x   0        0        0     1483 2024-04-16 20:48:34.851384 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
+-rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
+-rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 biotech-1.1.4/venues/stages/biotech/_status_advanced/status.proc.py
+-rwxr-xr-x   0        0        0     1779 2024-04-16 20:48:34.575388 biotech-1.1.4/venues/stages/biotech/architecture.s.HTML
+-rwxr-xr-x   0        0        0      241 2024-04-16 20:53:18.546926 biotech-1.1.4/venues/stages/biotech/emojis.S.HTML
+-rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 biotech-1.1.4/venues/stages/biotech/license.S.HTML
+-rwxr-xr-x   0        0        0     3068 2024-04-16 20:48:34.543389 biotech-1.1.4/venues/stages/biotech/module.s.HTML
+-rw-r--r--   0        0        0     1596 2024-04-19 21:12:05.931720 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      640 2024-04-19 16:26:52.595637 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      259 2024-04-19 16:20:24.028904 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
+-rwxr-xr-x   0        0        0     1478 2024-04-19 21:11:18.368263 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.648116 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/paths.py
+-rwxr-xr-x   0        0        0      666 2024-04-19 21:46:15.516790 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
+-rwxr-xr-x   0        0        0      562 2024-04-17 21:48:05.111704 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
+-rwxr-xr-x   0        0        0     1163 2024-04-17 21:49:49.362841 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3193 2024-04-19 23:42:26.432696 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
+-rw-r--r--   0        0        0     3137 2024-04-19 23:42:29.804658 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0      999 2024-04-19 20:57:55.937395 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0     2881 2024-04-19 21:20:39.102102 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
+-rw-r--r--   0        0        0     1152 2024-04-19 21:06:40.923425 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      653 2024-04-19 20:56:23.606442 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
+-rwxr-xr-x   0        0        0     3572 2024-04-19 21:20:33.674162 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
+-rwxr-xr-x   0        0        0      769 2024-04-19 21:06:33.619508 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
+-rw-r--r--   0        0        0     2031 2024-04-19 23:33:27.678892 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
+-rw-r--r--   0        0        0     2159 2024-04-19 23:33:27.678892 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      420 2024-04-19 23:33:27.678892 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
+-rw-r--r--   0        0        0      728 2024-04-19 23:33:27.682892 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3451 2024-04-19 16:26:14.724115 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
+-rwxr-xr-x   0        0        0     3235 2024-04-19 23:04:19.789690 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
+-rwxr-xr-x   0        0        0      193 2024-04-17 20:02:37.661229 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
+-rwxr-xr-x   0        0        0      514 2024-04-19 20:59:00.568662 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
+-rwxr-xr-x   0        0        0     1830 2024-04-19 23:29:07.554044 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
+-rw-r--r--   0        0        0     1851 2024-04-19 23:33:27.678892 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      799 2024-04-19 16:27:13.563375 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
+-rw-r--r--   0        0        0     4346 2024-04-19 23:33:27.682892 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
+-rw-r--r--   0        0        0     1268 2024-04-19 23:09:27.226569 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc
+-rw-r--r--   0        0        0     1489 2024-04-19 23:09:22.198620 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py
+-rwxr-xr-x   0        0        0      754 2024-04-18 00:33:41.120405 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
+-rw-r--r--   0        0        0     1826 2024-04-19 18:56:22.468973 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-19 18:56:27.160910 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      996 2024-04-19 16:26:14.764114 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
+-rwxr-xr-x   0        0        0     9825 2024-04-19 23:33:20.738974 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
+-rwxr-xr-x   0        0        0     3303 2024-04-19 23:03:08.158399 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
+-rw-r--r--   0        0        0     2018 2024-04-19 23:06:58.864088 biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      834 2024-04-16 20:48:34.547389 biotech-1.1.4/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
+-rwxr-xr-x   0        0        0      951 2024-04-16 20:49:56.266040 biotech-1.1.4/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      609 2024-04-19 22:29:43.435688 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
+-rw-r--r--   0        0        0     1904 2024-04-19 22:33:09.357432 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      500 2024-04-19 22:29:36.979758 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/dynamic_port.py
+-rwxr-xr-x   0        0        0     2161 2024-04-19 22:31:07.314772 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/on.py
+-rwxr-xr-x   0        0        0     2200 2024-04-19 22:24:22.967141 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
+-rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
+-rwxr-xr-x   0        0        0     1441 2024-04-18 02:04:22.961501 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
+-rwxr-xr-x   0        0        0      774 2024-04-16 20:48:34.555389 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
+-rwxr-xr-x   0        0        0     1336 2024-04-15 21:13:32.676638 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      309 2024-04-17 23:41:26.722721 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      562 2024-04-17 23:41:26.734721 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      525 2024-04-17 23:09:55.764639 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      908 2024-04-19 20:05:11.362609 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      636 2024-04-18 01:15:59.039315 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      289 2024-04-17 23:05:28.138584 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
+-rwxr-xr-x   0        0        0      803 2024-04-19 20:05:09.858629 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
+-rwxr-xr-x   0        0        0      378 2024-04-18 01:13:51.928249 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
+-rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
+-rwxr-xr-x   0        0        0     2182 2024-04-18 01:57:52.896535 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
+-rwxr-xr-x   0        0        0     2125 2024-04-18 01:58:34.052216 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1828 2024-04-19 21:04:56.668613 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2295 2024-04-19 21:04:32.800884 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
+-rw-r--r--   0        0        0        2 2024-04-19 22:32:11.666067 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/start.py
+-rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
+-rwxr-xr-x   0        0        0      152 2024-04-19 16:48:50.419277 biotech-1.1.4/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4699 2024-04-19 22:17:01.343942 biotech-1.1.4/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.4/venues/stages/biotech/procedures/intro/intro.S.HTML
+-rwxr-xr-x   0        0        0     6305 2024-04-19 22:16:54.188023 biotech-1.1.4/venues/stages/biotech/procedures/intro/on.py
+-rw-r--r--   0        0        0     2906 2024-04-19 21:43:07.254923 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
+-rw-r--r--   0        0        0     4000 2024-04-19 21:42:57.331035 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/adventure.py
+-rw-r--r--   0        0        0     1330 2024-04-19 21:12:05.939720 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      905 2024-04-19 16:56:52.013564 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      959 2024-04-19 21:11:59.243796 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      614 2024-04-19 16:56:41.273688 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
+-rwxr-xr-x   0        0        0      138 2024-04-19 17:33:23.717242 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/intro.proc.py
+-rwxr-xr-x   0        0        0     3084 2024-04-19 21:01:52.394709 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/keg/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-19 21:01:58.358642 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/variables/__init__.py
+-rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321766 biotech-1.1.4/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      172 2024-04-16 20:48:34.551389 biotech-1.1.4/venues/stages/biotech/procedures/procedures.S.HTML
+-rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 biotech-1.1.4/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 biotech-1.1.4/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
+-rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 biotech-1.1.4/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 biotech-1.1.4/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 biotech-1.1.4/venues/stages/biotech/topics/aggregate/__init__.py
+-rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 biotech-1.1.4/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 biotech-1.1.4/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      708 2024-04-16 20:48:34.591388 biotech-1.1.4/venues/stages/biotech/topics/alarm_parser/__init__.py
+-rwxr-xr-x   0        0        0      673 2024-04-16 20:49:28.126498 biotech-1.1.4/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 biotech-1.1.4/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      405 2024-04-16 20:48:34.579388 biotech-1.1.4/venues/stages/biotech/topics/exceptions.py
+-rwxr-xr-x   0        0        0     1190 2024-01-27 05:31:08.525189 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
+-rwxr-xr-x   0        0        0     2446 2024-04-17 19:24:25.140060 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__init__.py
+-rwxr-xr-x   0        0        0     2491 2024-04-17 19:24:52.839918 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4471 2024-02-01 06:11:56.801715 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1050 2024-04-16 06:10:03.111579 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1920 2024-01-31 18:50:23.812071 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
+-rwxr-xr-x   0        0        0       24 2024-01-26 17:38:56.558087 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
+-rwxr-xr-x   0        0        0       24 2024-01-26 17:38:52.854129 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
+-rwxr-xr-x   0        0        0      751 2024-04-17 19:16:04.226583 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
+-rwxr-xr-x   0        0        0     1981 2024-04-17 19:25:47.591625 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__init__.py
+-rwxr-xr-x   0        0        0     2283 2024-04-17 19:25:53.011595 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4019 2024-01-31 18:51:47.652157 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3843 2024-04-17 19:25:53.099595 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4426 2024-01-27 06:34:32.979965 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3559 2024-04-17 19:25:22.227762 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/treasury.py
+-rwxr-xr-x   0        0        0     1727 2024-04-17 19:15:19.882965 biotech-1.1.4/venues/stages/biotech/topics/help_documentation/shares.s.HTML
+-rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 biotech-1.1.4/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1558 2024-04-18 05:22:02.832642 biotech-1.1.4/venues/stages/biotech/topics/implicit/proc/__init__.py
+-rwxr-xr-x   0        0        0     1158 2024-04-19 21:23:01.800513 biotech-1.1.4/venues/stages/biotech/topics/implicit/thread/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-19 21:23:28.056219 biotech-1.1.4/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       90 2024-04-17 22:51:08.968798 biotech-1.1.4/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 22:33:48.860256 biotech-1.1.4/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
+-rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 biotech-1.1.4/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
+-rwxr-xr-x   0        0        0      470 2024-04-17 23:02:14.419990 biotech-1.1.4/venues/stages/biotech/topics/printout/bracket.py
+-rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 biotech-1.1.4/venues/stages/biotech/topics/printout/passes.py
+-rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 biotech-1.1.4/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2166 2024-04-19 22:38:28.357906 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__init__.py
+-rw-r--r--   0        0        0     1997 2024-04-19 22:38:43.137742 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
+-rw-r--r--   0        0        0     1818 2024-04-19 23:33:25.614916 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-18 01:45:27.254200 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1586 2024-04-19 23:27:54.158868 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-18 01:48:34.504806 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-18 01:45:24.082223 biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
+-rwxr-xr-x   0        0        0      195 2024-04-16 22:50:54.515336 biotech-1.1.4/venues/stages/biotech/topics/process_on/process_on.S.HTML
+-rwxr-xr-x   0        0        0     1470 2024-04-18 04:12:56.845888 biotech-1.1.4/venues/stages/biotech/topics/quay/garage.py
+-rwxr-xr-x   0        0        0     2546 2024-04-18 04:38:41.478278 biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_1.py
+-rwxr-xr-x   0        0        0     1612 2024-04-18 04:54:58.414971 biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_2.py
+-rwxr-xr-x   0        0        0      551 2024-04-18 05:20:40.701113 biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_3.py
+-rwxr-xr-x   0        0        0     1083 2024-04-18 05:19:11.645613 biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_4.py
+-rwxr-xr-x   0        0        0     1448 2024-04-19 22:40:22.232641 biotech-1.1.4/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
+-rw-r--r--   0        0        0     1464 2024-04-19 22:41:14.292061 biotech-1.1.4/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 biotech-1.1.4/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-19 21:18:20.963631 biotech-1.1.4/venues/stages/biotech/topics/report_formats/report_formats.S.HTML
+-rw-r--r--   0        0        0     1772 2024-04-19 20:59:56.440027 biotech-1.1.4/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0      461 2024-04-17 23:59:06.614967 biotech-1.1.4/venues/stages/biotech/topics/show/show.S.HTML
+-rwxr-xr-x   0        0        0     2295 2024-04-19 20:59:53.444061 biotech-1.1.4/venues/stages/biotech/topics/show/variable.py
+-rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
+-rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
+-rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
+-rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
+-rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
+-rwxr-xr-x   0        0        0      273 2024-04-16 20:48:34.583388 biotech-1.1.4/venues/stages/biotech/topics/start--/one.py
+-rwxr-xr-x   0        0        0      406 2024-04-16 20:48:34.587388 biotech-1.1.4/venues/stages/biotech/topics/start--/sequentially.py
+-rwxr-xr-x   0        0        0      532 2024-04-16 20:48:34.587388 biotech-1.1.4/venues/stages/biotech/topics/start--/simultaneously.py
+-rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 biotech-1.1.4/venues/stages/biotech/topics/topics.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 biotech-1.1.4/venues/stages/biotech/variables/__init__.py
+-rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.4/PKG-INFO
```

### Comparing `biotech-1.1.3/pyproject.toml` & `biotech-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 [tool.poetry]
 name = "biotech"
-version = "1.1.3"
+version = "1.1.4"
 description = "A health monitoring stack"
 authors = []
 readme = "readme.md"
 
 packages = [
     { include = "biotech", from = "venues/stages" }
 ]
```

### Comparing `biotech-1.1.3/readme.md` & `biotech-1.1.4/readme.md`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venue.S.HTML` & `biotech-1.1.4/venue.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg` & `biotech-1.1.4/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML` & `biotech-1.1.4/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/___itinerary/itinerary.S.HTML` & `biotech-1.1.4/venues/stages/biotech/___itinerary/itinerary.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/___itinerary/maybes.s.HTML` & `biotech-1.1.4/venues/stages/biotech/___itinerary/maybes.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout/start.py` & `biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout_v2/start.py` & `biotech-1.1.4/venues/stages/biotech/___itinerary/processes/errout_v2/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/__license/options/gpl-3.0-standalone.html` & `biotech-1.1.4/venues/stages/biotech/__license/options/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_book/advanced tutorial.s.HTML` & `biotech-1.1.4/venues/stages/biotech/_book/advanced tutorial.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_book/book.s.HTML` & `biotech-1.1.4/venues/stages/biotech/_book/book.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_book/relevant.s.HTML` & `biotech-1.1.4/venues/stages/biotech/_book/relevant.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_clique/__init__.py` & `biotech-1.1.4/venues/stages/biotech/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/DB/records.json` & `biotech-1.1.4/venues/stages/biotech/_status/DB/records.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974619289340101%*

 * *Differences: {"'_default'": "{'393': OrderedDict([('paths', [OrderedDict([('path', "*

 * *               "'_status/monitors/-01_start/status_1.py'), ('empty', False), ('parsed', True), "*

 * *               "('stats', OrderedDict([('passes', 1), ('alarms', 0)])), ('checks', "*

 * *               "[OrderedDict([('check', 'check 1'), ('passed', True), ('elapsed', "*

 * *               "[6.0906080289969395, 'seconds'])])])]), OrderedDict([('path', "*

 * *               "'_status/monitors/00_start/status_1.py'), ('empty', False), ('parsed', True),  […]*

```diff
@@ -52539,14 +52539,572 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 14
                 },
                 "empty": 0
             }
         },
+        "393": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.0906080289969395,
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
+                                6.072293995999644,
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
+                                6.160357748001843,
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
+                                6.067098220999469,
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
+                                4.152753874001064,
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
+                                6.068201549998776,
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
+                                6.079794304998359,
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
+                                6.126444256999093,
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
+                                6.082427370001824,
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
+                                6.123411993001355,
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
+                                6.23630679100097,
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
+                                6.107790165999177,
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
+                                10.09284376299911,
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
+                                6.087700168001902,
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
+        "394": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.081707201003155,
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
+                                6.070731929998146,
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
+                                6.132641017000424,
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
+                                6.102444821000972,
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
+                                4.159180358001322,
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
+                                6.069372066998767,
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
+                                6.083376340000541,
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
+                                6.127884724999603,
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
+                                6.091530325997155,
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
+                                6.186807818998204,
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
+                                6.2011516589991516,
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
+                                6.12531683600173,
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
+                                10.116770153999823,
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
+                                6.090978301999712,
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

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/establish.py` & `biotech-1.1.4/venues/stages/biotech/_status/establish.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/-01_start/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/-01_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/00_start/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/00_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_1_health.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/01/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/01/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/02/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/02/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/05__file__/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/06_various/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/07/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/07/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/08_DB/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/08_DB/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9957627118644068%*

 * *Differences: {"'_default'": "{'235': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [1.8255999748362228e-05, 'seconds']), ('passed', "*

 * *               "True)])]), ('empty', False), ('parsed', True), ('path', 'guarantee_1.py'), "*

 * *               "('records', ['proceeds None\\r\\n', 'checks in module True\\r\\n', 'check "*

 * *               '1\\r\\n\', \'{\\r\\n\', \'  "variable": {\\r\\n\', \'    "pid": 14559,\\r\\n\', '*

 * *               '\'    "proceeds": {\\r\\ […]*

```diff
@@ -5601,14 +5601,146 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 1
                 },
                 "empty": 0
             }
         },
+        "235": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.8255999748362228e-05,
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
+                        "    \"pid\": 14559,\r\n",
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
+                        "            1.8255999748362228e-05,\r\n",
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
+        "236": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.896000508684665e-06,
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
+                        "    \"pid\": 15018,\r\n",
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
+                        "            8.896000508684665e-06,\r\n",
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
         "24": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
```

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/monitors/11/status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status/monitors/11/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status/status.proc.py` & `biotech-1.1.4/venues/stages/biotech/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py` & `biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json` & `biotech-1.1.4/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/_status_advanced/status.proc.py` & `biotech-1.1.4/venues/stages/biotech/_status_advanced/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/architecture.s.HTML` & `biotech-1.1.4/venues/stages/biotech/architecture.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/module.s.HTML` & `biotech-1.1.4/venues/stages/biotech/module.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/on.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -64,21 +64,68 @@
 		return "yes"
 		
 	@app.route ("/anomalies", methods = [ 'GET' ])
 	def on_anomalies ():	
 		try:
 			aggregator_variables = retrieve_aggregator_variables ()
 			
-			return jsonify (aggregator_variables ["anomalies"])
+			return {
+				"anomalies": jsonify (aggregator_variables ["anomalies"])
+			}
 			
 		except Exception:
 			pass;
 			
 		return "not parseable"
 
+
+	@app.route ("/waiting_for", methods = [ 'GET' ])
+	def on_waiting_for ():	
+		try:
+			aggregator_variables = retrieve_aggregator_variables ()
+			internal_statuses = aggregator_variables ["internal_statuses"]
+
+			
+			waiting_for = []
+			for status_path in internal_statuses:
+				occurrences = "not parseable"
+				try:
+					occurrences = aggregator_variables ["internal_statuses"] [ status_path ] ["occurrences"]
+				except Exception:
+					pass;
+					
+				records = "not parseable"
+				try:
+					records = aggregator_variables ["internal_statuses"] [ status_path ] ["records"]
+				except Exception:
+					pass;
+					
+				times = "not parseable"
+				try:
+					times = aggregator_variables ["internal_statuses"] [ status_path ] ["times"]
+				except Exception:
+					pass;
+			
+				if (internal_statuses [ status_path ] ["status"] ["process"] != "done"):
+					waiting_for.append ({
+						"path": status_path,
+						"occurrences": occurrences,
+						"records": records,
+						"times": times
+					})
+			
+			return jsonify ({
+				"waiting_for": waiting_for
+			})
+			
+		except Exception as E:
+			print ("exception:", E)
+			pass;
+			
+		return "not parseable"
 		
 	@app.route ('/health_scans/paths', methods = [ 'GET' ])
 	def on__get__health_scans__paths ():	
 		aggregator_variables = retrieve_aggregator_variables ()
 		
 		the_paths = {}
```

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 20:54:28 2024 UTC, .py size: 2023 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 04da 2266 e707 0000  o........."f....
+00000000: 6f0d 0d0a 0000 0000 6201 2366 790c 0000  o.......b.#fy...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6405 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 6407 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6405 6408 6c0d 5a0d 6405  m.Z...d.d.l.Z.d.
@@ -24,130 +24,174 @@
 00000170: 616c 7468 5f73 6361 6e5f 7374 6172 7465  alth_scan_starte
 00000180: 64e9 0000 0000 2901 da1d 7265 7472 6965  d.....)...retrie
 00000190: 7665 5f61 6767 7265 6761 746f 725f 7661  ve_aggregator_va
 000001a0: 7269 6162 6c65 7329 03da 0546 6c61 736b  riables)...Flask
 000001b0: da07 7265 7175 6573 74da 076a 736f 6e69  ..request..jsoni
 000001c0: 6679 4e29 03da 0764 6972 6e61 6d65 da04  fyN)...dirname..
 000001d0: 6a6f 696e da08 6e6f 726d 7061 7468 6302  join..normpathc.
-000001e0: 0000 0000 0000 0000 0000 0008 0000 0005  ................
-000001f0: 0000 0043 0000 0073 c400 0000 7c01 6401  ...C...s....|.d.
+000001e0: 0000 0000 0000 0000 0000 0009 0000 0005  ................
+000001f0: 0000 0043 0000 0073 dc00 0000 7c01 6401  ...C...s....|.d.
 00000200: 6b05 7209 7400 6402 7c00 8302 0100 7401  k.r.t.d.|.....t.
 00000210: 6403 8301 7d02 0900 7402 7c02 7c00 6404  d...}...t.|.|.d.
 00000220: 8d02 0100 7c02 6a03 6405 6406 6701 6407  ....|.j.d.d.g.d.
 00000230: 8d02 6408 6409 8400 8301 7d03 7c02 6a03  ..d.d.....}.|.j.
 00000240: 640a 6406 6701 6407 8d02 640b 640c 8400  d.d.g.d...d.d...
 00000250: 8301 7d04 7c02 6a03 640d 6406 6701 6407  ..}.|.j.d.d.g.d.
 00000260: 8d02 640e 640f 8400 8301 7d05 7c02 6a03  ..d.d.....}.|.j.
 00000270: 6410 6406 6701 6407 8d02 6411 6412 8400  d.d.g.d...d.d...
 00000280: 8301 7d06 7c02 6a03 6413 6406 6701 6407  ..}.|.j.d.d.g.d.
-00000290: 8d02 6414 6415 8400 8301 7d07 7404 7c02  ..d.d.....}.t.|.
-000002a0: 8301 0100 7405 7c02 8301 0100 7c02 6a06  ....t.|.....|.j.
-000002b0: 6416 7c00 6417 6418 8d03 0100 6400 5300  d.|.d.d.....d.S.
-000002c0: 2919 4e72 0100 0000 7a21 6f70 656e 696e  ).Nr....z!openin
-000002d0: 6720 7363 616e 2070 726f 6365 7373 206b  g scan process k
-000002e0: 6567 206f 6e20 706f 7274 3a7a 1161 6767  eg on port:z.agg
-000002f0: 7265 6761 746f 7220 6861 7262 6f72 2901  regator harbor).
-00000300: da19 6167 6772 6567 6174 6f72 5f70 726f  ..aggregator_pro
-00000310: 6365 6475 7265 5f70 6f72 74fa 012f da03  cedure_port../..
-00000320: 4745 5429 01da 076d 6574 686f 6473 6300  GET)...methodsc.
-00000330: 0000 0000 0000 0000 0000 0000 0000 0006  ................
-00000340: 0000 0053 0000 0073 1a00 0000 7400 6401  ...S...s....t.d.
-00000350: 6701 6401 6701 6401 6701 6401 6701 6402  g.d.g.d.g.d.g.d.
-00000360: 9c04 8301 5300 2903 4eda 0367 6574 2904  ....S.).N..get).
-00000370: fa24 2f68 6561 6c74 685f 7363 616e 2f3c  .$/health_scan/<
-00000380: 7061 7468 3a68 6561 6c74 685f 7363 616e  path:health_scan
-00000390: 5f70 6174 683e fa13 2f68 6561 6c74 685f  _path>../health_
-000003a0: 7363 616e 732f 7061 7468 73fa 032f 6f6e  scans/paths../on
-000003b0: fa0a 2f61 6e6f 6d61 6c69 6573 2901 7209  ../anomalies).r.
-000003c0: 0000 00a9 0072 1600 0000 7216 0000 00fa  .....r....r.....
-000003d0: 562f 6269 6f74 6563 682f 7665 6e75 6573  V/biotech/venues
-000003e0: 2f73 7461 6765 732f 6269 6f74 6563 682f  /stages/biotech/
-000003f0: 7072 6f63 6564 7572 6573 2f61 6767 7265  procedures/aggre
-00000400: 6761 746f 725f 7072 6f63 6564 7572 652f  gator_procedure/
-00000410: 7072 6f63 6573 732f 6b65 672f 5f5f 696e  process/keg/__in
-00000420: 6974 5f5f 2e70 79da 0868 6f6d 655f 6765  it__.py..home_ge
-00000430: 7434 0000 0073 0c00 0000 0202 0401 0401  t4...s..........
-00000440: 0401 0401 08fc 7a1d 6f70 656e 5f68 6172  ......z.open_har
-00000450: 626f 722e 3c6c 6f63 616c 733e 2e68 6f6d  bor.<locals>.hom
-00000460: 655f 6765 7472 1400 0000 6300 0000 0000  e_getr....c.....
-00000470: 0000 0000 0000 0000 0000 0001 0000 0053  ...............S
-00000480: 0000 00f3 0400 0000 6401 5300 a902 4eda  ........d.S...N.
-00000490: 0379 6573 7216 0000 0072 1600 0000 7216  .yesr....r....r.
-000004a0: 0000 0072 1600 0000 7217 0000 00da 066f  ...r....r......o
-000004b0: 6e5f 6765 743e 0000 00f3 0200 0000 0402  n_get>..........
-000004c0: 7a1b 6f70 656e 5f68 6172 626f 722e 3c6c  z.open_harbor.<l
-000004d0: 6f63 616c 733e 2e6f 6e5f 6765 7472 1500  ocals>.on_getr..
-000004e0: 0000 6300 0000 0000 0000 0000 0000 0001  ..c.............
-000004f0: 0000 0008 0000 0053 0000 0073 2a00 0000  .......S...s*...
-00000500: 7a0a 7400 8300 7d00 7401 7c00 6401 1900  z.t...}.t.|.d...
-00000510: 8301 5700 5300 0400 7402 7914 0100 0100  ..W.S...t.y.....
-00000520: 0100 5900 6402 5300 7700 2903 4eda 0961  ..Y.d.S.w.).N..a
-00000530: 6e6f 6d61 6c69 6573 7a0d 6e6f 7420 7061  nomaliesz.not pa
-00000540: 7273 6561 626c 6529 0372 0600 0000 7209  rseable).r....r.
-00000550: 0000 00da 0945 7863 6570 7469 6f6e 2901  .....Exception).
-00000560: da14 6167 6772 6567 6174 6f72 5f76 6172  ..aggregator_var
-00000570: 6961 626c 6573 7216 0000 0072 1600 0000  iablesr....r....
-00000580: 7217 0000 00da 0c6f 6e5f 616e 6f6d 616c  r......on_anomal
-00000590: 6965 7342 0000 0073 0e00 0000 0202 0601  iesB...s........
-000005a0: 0e02 0c02 0201 0402 02fd 7a21 6f70 656e  ..........z!open
-000005b0: 5f68 6172 626f 722e 3c6c 6f63 616c 733e  _harbor.<locals>
-000005c0: 2e6f 6e5f 616e 6f6d 616c 6965 7372 1300  .on_anomaliesr..
-000005d0: 0000 6300 0000 0000 0000 0000 0000 0003  ..c.............
-000005e0: 0000 0004 0000 0053 0000 0073 2800 0000  .......S...s(...
-000005f0: 7400 8300 7d00 6900 7d01 7c00 6401 1900  t...}.i.}.|.d...
-00000600: 4400 5d06 7d02 6402 7c01 7c02 3c00 7109  D.].}.d.|.|.<.q.
-00000610: 7401 7c01 8301 5300 2903 4eda 1169 6e74  t.|...S.).N..int
-00000620: 6572 6e61 6c5f 7374 6174 7573 6573 da00  ernal_statuses..
-00000630: 2902 7206 0000 0072 0900 0000 2903 7220  ).r....r....).r 
-00000640: 0000 00da 0974 6865 5f70 6174 6873 da04  .....the_paths..
-00000650: 7061 7468 7216 0000 0072 1600 0000 7217  pathr....r....r.
-00000660: 0000 00da 1c6f 6e5f 5f67 6574 5f5f 6865  .....on__get__he
-00000670: 616c 7468 5f73 6361 6e73 5f5f 7061 7468  alth_scans__path
-00000680: 734f 0000 0073 0a00 0000 0602 0402 0c02  sO...s..........
-00000690: 0a01 0802 7a31 6f70 656e 5f68 6172 626f  ....z1open_harbo
-000006a0: 722e 3c6c 6f63 616c 733e 2e6f 6e5f 5f67  r.<locals>.on__g
-000006b0: 6574 5f5f 6865 616c 7468 5f73 6361 6e73  et__health_scans
-000006c0: 5f5f 7061 7468 7372 1200 0000 6301 0000  __pathsr....c...
-000006d0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-000006e0: 0053 0000 0072 1900 0000 721a 0000 0072  .S...r....r....r
-000006f0: 1600 0000 2901 da10 6865 616c 7468 5f73  ....)...health_s
-00000700: 6361 6e5f 7061 7468 7216 0000 0072 1600  can_pathr....r..
-00000710: 0000 7217 0000 00da 1a6f 6e5f 5f67 6574  ..r......on__get
-00000720: 5f5f 6865 616c 7468 5f73 6361 6e5f 5f70  __health_scan__p
-00000730: 6174 685a 0000 0072 1d00 0000 7a2f 6f70  athZ...r....z/op
-00000740: 656e 5f68 6172 626f 722e 3c6c 6f63 616c  en_harbor.<local
-00000750: 733e 2e6f 6e5f 5f67 6574 5f5f 6865 616c  s>.on__get__heal
-00000760: 7468 5f73 6361 6e5f 5f70 6174 687a 0730  th_scan__pathz.0
-00000770: 2e30 2e30 2e30 4629 02da 0470 6f72 74da  .0.0.0F)...port.
-00000780: 0564 6562 7567 2907 da05 7072 696e 7472  .debug)...printr
-00000790: 0700 0000 7203 0000 00da 0572 6f75 7465  ....r......route
-000007a0: 7204 0000 0072 0200 0000 da03 7275 6e29  r....r......run)
-000007b0: 0872 2900 0000 da07 7265 636f 7264 73da  .r).....records.
-000007c0: 0361 7070 7218 0000 0072 1c00 0000 7221  .appr....r....r!
-000007d0: 0000 0072 2600 0000 7228 0000 0072 1600  ...r&...r(...r..
-000007e0: 0000 7216 0000 0072 1700 0000 da0b 6f70  ..r....r......op
-000007f0: 656e 5f68 6172 626f 7224 0000 0073 2c00  en_harbor$...s,.
-00000800: 0000 0804 0a01 0804 0202 0c03 0e02 0a01  ................
-00000810: 0e09 0a01 0e03 0a01 0e0c 0a01 0e0a 0a01  ................
-00000820: 0804 0802 0404 0201 0201 0201 0afd 7230  ..............r0
-00000830: 0000 0029 0272 0500 0000 7205 0000 0029  ...).r....r....)
-00000840: 19da 075f 5f64 6f63 5f5f da15 7370 6163  ...__doc__..spac
-00000850: 6573 2e64 6f6e 655f 7769 7468 5f73 6361  es.done_with_sca
-00000860: 6e72 0200 0000 da12 7370 6163 6573 2e70  nr......spaces.p
-00000870: 6174 6873 5f70 6174 6368 7203 0000 00da  aths_patchr.....
-00000880: 1e73 7061 6365 732e 7468 655f 6865 616c  .spaces.the_heal
-00000890: 7468 5f73 6361 6e5f 7374 6172 7465 6472  th_scan_startedr
-000008a0: 0400 0000 da39 6269 6f74 6563 682e 7072  .....9biotech.pr
-000008b0: 6f63 6564 7572 6573 2e61 6767 7265 6761  ocedures.aggrega
-000008c0: 746f 725f 7072 6f63 6564 7572 652e 7072  tor_procedure.pr
-000008d0: 6f63 6573 732e 7661 7269 6162 6c65 7372  ocess.variablesr
-000008e0: 0600 0000 da05 666c 6173 6b72 0700 0000  ......flaskr....
-000008f0: 7208 0000 0072 0900 0000 da04 7269 6368  r....r......rich
-00000900: da04 6a73 6f6e da07 7061 7468 6c69 62da  ..json..pathlib.
-00000910: 026f 73da 076f 732e 7061 7468 720a 0000  .os..os.pathr...
-00000920: 0072 0b00 0000 720c 0000 00da 0373 7973  .r....r......sys
-00000930: da09 7468 7265 6164 696e 67da 0474 696d  ..threading..tim
-00000940: 6572 3000 0000 7216 0000 0072 1600 0000  er0...r....r....
-00000950: 7216 0000 0072 1700 0000 da08 3c6d 6f64  r....r......<mod
-00000960: 756c 653e 0100 0000 7322 0000 0004 020c  ule>....s"......
-00000970: 0c0c 010c 010c 0214 0308 0108 0308 0108  ................
-00000980: 0114 0108 0108 0108 0102 0502 010e fe    ...............
+00000290: 8d02 6414 6415 8400 8301 7d07 7c02 6a03  ..d.d.....}.|.j.
+000002a0: 6416 6406 6701 6407 8d02 6417 6418 8400  d.d.g.d...d.d...
+000002b0: 8301 7d08 7404 7c02 8301 0100 7405 7c02  ..}.t.|.....t.|.
+000002c0: 8301 0100 7c02 6a06 6419 7c00 641a 641b  ....|.j.d.|.d.d.
+000002d0: 8d03 0100 6400 5300 291c 4e72 0100 0000  ....d.S.).Nr....
+000002e0: 7a21 6f70 656e 696e 6720 7363 616e 2070  z!opening scan p
+000002f0: 726f 6365 7373 206b 6567 206f 6e20 706f  rocess keg on po
+00000300: 7274 3a7a 1161 6767 7265 6761 746f 7220  rt:z.aggregator 
+00000310: 6861 7262 6f72 2901 da19 6167 6772 6567  harbor)...aggreg
+00000320: 6174 6f72 5f70 726f 6365 6475 7265 5f70  ator_procedure_p
+00000330: 6f72 74fa 012f da03 4745 5429 01da 076d  ort../..GET)...m
+00000340: 6574 686f 6473 6300 0000 0000 0000 0000  ethodsc.........
+00000350: 0000 0000 0000 0006 0000 0053 0000 0073  ...........S...s
+00000360: 1a00 0000 7400 6401 6701 6401 6701 6401  ....t.d.g.d.g.d.
+00000370: 6701 6401 6701 6402 9c04 8301 5300 2903  g.d.g.d.....S.).
+00000380: 4eda 0367 6574 2904 fa24 2f68 6561 6c74  N..get)..$/healt
+00000390: 685f 7363 616e 2f3c 7061 7468 3a68 6561  h_scan/<path:hea
+000003a0: 6c74 685f 7363 616e 5f70 6174 683e fa13  lth_scan_path>..
+000003b0: 2f68 6561 6c74 685f 7363 616e 732f 7061  /health_scans/pa
+000003c0: 7468 73fa 032f 6f6e fa0a 2f61 6e6f 6d61  ths../on../anoma
+000003d0: 6c69 6573 2901 7209 0000 00a9 0072 1600  lies).r......r..
+000003e0: 0000 7216 0000 00fa 562f 6269 6f74 6563  ..r.....V/biotec
+000003f0: 682f 7665 6e75 6573 2f73 7461 6765 732f  h/venues/stages/
+00000400: 6269 6f74 6563 682f 7072 6f63 6564 7572  biotech/procedur
+00000410: 6573 2f61 6767 7265 6761 746f 725f 7072  es/aggregator_pr
+00000420: 6f63 6564 7572 652f 7072 6f63 6573 732f  ocedure/process/
+00000430: 6b65 672f 5f5f 696e 6974 5f5f 2e70 79da  keg/__init__.py.
+00000440: 0868 6f6d 655f 6765 7434 0000 0073 0c00  .home_get4...s..
+00000450: 0000 0202 0401 0401 0401 0401 08fc 7a1d  ..............z.
+00000460: 6f70 656e 5f68 6172 626f 722e 3c6c 6f63  open_harbor.<loc
+00000470: 616c 733e 2e68 6f6d 655f 6765 7472 1400  als>.home_getr..
+00000480: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000490: 0000 0001 0000 0053 0000 00f3 0400 0000  .......S........
+000004a0: 6401 5300 a902 4eda 0379 6573 7216 0000  d.S...N..yesr...
+000004b0: 0072 1600 0000 7216 0000 0072 1600 0000  .r....r....r....
+000004c0: 7217 0000 00da 066f 6e5f 6765 743e 0000  r......on_get>..
+000004d0: 00f3 0200 0000 0402 7a1b 6f70 656e 5f68  ........z.open_h
+000004e0: 6172 626f 722e 3c6c 6f63 616c 733e 2e6f  arbor.<locals>.o
+000004f0: 6e5f 6765 7472 1500 0000 6300 0000 0000  n_getr....c.....
+00000500: 0000 0000 0000 0001 0000 0008 0000 0053  ...............S
+00000510: 0000 0073 2e00 0000 7a0c 7400 8300 7d00  ...s....z.t...}.
+00000520: 6401 7401 7c00 6401 1900 8301 6901 5700  d.t.|.d.....i.W.
+00000530: 5300 0400 7402 7916 0100 0100 0100 5900  S...t.y.......Y.
+00000540: 6402 5300 7700 2903 4eda 0961 6e6f 6d61  d.S.w.).N..anoma
+00000550: 6c69 6573 fa0d 6e6f 7420 7061 7273 6561  lies..not parsea
+00000560: 626c 6529 0372 0600 0000 7209 0000 00da  ble).r....r.....
+00000570: 0945 7863 6570 7469 6f6e 2901 da14 6167  .Exception)...ag
+00000580: 6772 6567 6174 6f72 5f76 6172 6961 626c  gregator_variabl
+00000590: 6573 7216 0000 0072 1600 0000 7217 0000  esr....r....r...
+000005a0: 00da 0c6f 6e5f 616e 6f6d 616c 6965 7342  ...on_anomaliesB
+000005b0: 0000 0073 1000 0000 0202 0601 0c03 06ff  ...s............
+000005c0: 0c04 0201 0402 02fd 7a21 6f70 656e 5f68  ........z!open_h
+000005d0: 6172 626f 722e 3c6c 6f63 616c 733e 2e6f  arbor.<locals>.o
+000005e0: 6e5f 616e 6f6d 616c 6965 737a 0c2f 7761  n_anomaliesz./wa
+000005f0: 6974 696e 675f 666f 7263 0000 0000 0000  iting_forc......
+00000600: 0000 0000 0000 0800 0000 0a00 0000 5300  ..............S.
+00000610: 0000 7308 0100 007a 6b74 0083 007d 007c  ..s....zkt...}.|
+00000620: 0064 0119 007d 0167 007d 027c 0144 005d  .d...}.g.}.|.D.]
+00000630: 587d 0364 027d 047a 0a7c 0064 0119 007c  X}.d.}.z.|.d...|
+00000640: 0319 0064 0319 007d 0457 006e 0904 0074  ...d...}.W.n...t
+00000650: 0179 2301 0001 0001 0059 006e 0177 0064  .y#......Y.n.w.d
+00000660: 027d 057a 0a7c 0064 0119 007c 0319 0064  .}.z.|.d...|...d
+00000670: 0419 007d 0557 006e 0904 0074 0179 3901  ...}.W.n...t.y9.
+00000680: 0001 0001 0059 006e 0177 0064 027d 067a  .....Y.n.w.d.}.z
+00000690: 0a7c 0064 0119 007c 0319 0064 0519 007d  .|.d...|...d...}
+000006a0: 0657 006e 0904 0074 0179 4f01 0001 0001  .W.n...t.yO.....
+000006b0: 0059 006e 0177 007c 017c 0319 0064 0619  .Y.n.w.|.|...d..
+000006c0: 0064 0719 0064 086b 0372 647c 02a0 027c  .d...d.k.rd|...|
+000006d0: 037c 047c 057c 0664 099c 04a1 0101 0071  .|.|.|.d.......q
+000006e0: 0c74 0364 0a7c 0269 0183 0157 0053 0004  .t.d.|.i...W.S..
+000006f0: 0074 0179 8301 007d 0701 007a 0c74 0464  .t.y...}...z.t.d
+00000700: 0b7c 0783 0201 0057 0059 0064 007d 077e  .|.....W.Y.d.}.~
+00000710: 0764 0253 0064 007d 077e 0777 0177 0029  .d.S.d.}.~.w.w.)
+00000720: 0c4e da11 696e 7465 726e 616c 5f73 7461  .N..internal_sta
+00000730: 7475 7365 7372 1f00 0000 da0b 6f63 6375  tusesr......occu
+00000740: 7272 656e 6365 73da 0772 6563 6f72 6473  rrences..records
+00000750: da05 7469 6d65 73da 0673 7461 7475 73da  ..times..status.
+00000760: 0770 726f 6365 7373 da04 646f 6e65 2904  .process..done).
+00000770: da04 7061 7468 7224 0000 0072 2500 0000  ..pathr$...r%...
+00000780: 7226 0000 00da 0b77 6169 7469 6e67 5f66  r&.....waiting_f
+00000790: 6f72 7a0a 6578 6365 7074 696f 6e3a 2905  orz.exception:).
+000007a0: 7206 0000 0072 2000 0000 da06 6170 7065  r....r .....appe
+000007b0: 6e64 7209 0000 00da 0570 7269 6e74 2908  ndr......print).
+000007c0: 7221 0000 0072 2300 0000 722b 0000 00da  r!...r#...r+....
+000007d0: 0b73 7461 7475 735f 7061 7468 7224 0000  .status_pathr$..
+000007e0: 0072 2500 0000 7226 0000 00da 0145 7216  .r%...r&.....Er.
+000007f0: 0000 0072 1600 0000 7217 0000 00da 0e6f  ...r....r......o
+00000800: 6e5f 7761 6974 696e 675f 666f 7251 0000  n_waiting_forQ..
+00000810: 0073 5000 0000 0202 0601 0801 0403 0801  .sP.............
+00000820: 0401 0201 1401 0c01 0401 02ff 0403 0201  ................
+00000830: 1401 0c01 0401 02ff 0403 0201 1401 0c01  ................
+00000840: 0401 02ff 1403 0401 0201 0201 0201 0201  ................
+00000850: 08fc 0280 0207 0401 08ff 0e04 0a01 0a01  ................
+00000860: 0402 0880 02fc 7a23 6f70 656e 5f68 6172  ......z#open_har
+00000870: 626f 722e 3c6c 6f63 616c 733e 2e6f 6e5f  bor.<locals>.on_
+00000880: 7761 6974 696e 675f 666f 7272 1300 0000  waiting_forr....
+00000890: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
+000008a0: 0004 0000 0053 0000 0073 2800 0000 7400  .....S...s(...t.
+000008b0: 8300 7d00 6900 7d01 7c00 6401 1900 4400  ..}.i.}.|.d...D.
+000008c0: 5d06 7d02 6402 7c01 7c02 3c00 7109 7401  ].}.d.|.|.<.q.t.
+000008d0: 7c01 8301 5300 2903 4e72 2300 0000 da00  |...S.).Nr#.....
+000008e0: 2902 7206 0000 0072 0900 0000 2903 7221  ).r....r....).r!
+000008f0: 0000 00da 0974 6865 5f70 6174 6873 722a  .....the_pathsr*
+00000900: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00000910: 0000 da1c 6f6e 5f5f 6765 745f 5f68 6561  ....on__get__hea
+00000920: 6c74 685f 7363 616e 735f 5f70 6174 6873  lth_scans__paths
+00000930: 7e00 0000 730a 0000 0006 0204 020c 020a  ~...s...........
+00000940: 0108 027a 316f 7065 6e5f 6861 7262 6f72  ...z1open_harbor
+00000950: 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f5f 6765  .<locals>.on__ge
+00000960: 745f 5f68 6561 6c74 685f 7363 616e 735f  t__health_scans_
+00000970: 5f70 6174 6873 7212 0000 0063 0100 0000  _pathsr....c....
+00000980: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00000990: 5300 0000 7219 0000 0072 1a00 0000 7216  S...r....r....r.
+000009a0: 0000 0029 01da 1068 6561 6c74 685f 7363  ...)...health_sc
+000009b0: 616e 5f70 6174 6872 1600 0000 7216 0000  an_pathr....r...
+000009c0: 0072 1700 0000 da1a 6f6e 5f5f 6765 745f  .r......on__get_
+000009d0: 5f68 6561 6c74 685f 7363 616e 5f5f 7061  _health_scan__pa
+000009e0: 7468 8900 0000 721d 0000 007a 2f6f 7065  th....r....z/ope
+000009f0: 6e5f 6861 7262 6f72 2e3c 6c6f 6361 6c73  n_harbor.<locals
+00000a00: 3e2e 6f6e 5f5f 6765 745f 5f68 6561 6c74  >.on__get__healt
+00000a10: 685f 7363 616e 5f5f 7061 7468 7a07 302e  h_scan__pathz.0.
+00000a20: 302e 302e 3046 2902 da04 706f 7274 da05  0.0.0F)...port..
+00000a30: 6465 6275 6729 0772 2d00 0000 7207 0000  debug).r-...r...
+00000a40: 0072 0300 0000 da05 726f 7574 6572 0400  .r......router..
+00000a50: 0000 7202 0000 00da 0372 756e 2909 7236  ..r......run).r6
+00000a60: 0000 0072 2500 0000 da03 6170 7072 1800  ...r%.....appr..
+00000a70: 0000 721c 0000 0072 2200 0000 7230 0000  ..r....r"...r0..
+00000a80: 0072 3300 0000 7235 0000 0072 1600 0000  .r3...r5...r....
+00000a90: 7216 0000 0072 1700 0000 da0b 6f70 656e  r....r......open
+00000aa0: 5f68 6172 626f 7224 0000 0073 3000 0000  _harbor$...s0...
+00000ab0: 0804 0a01 0804 0202 0c03 0e02 0a01 0e09  ................
+00000ac0: 0a01 0e03 0a01 0e0e 0a01 0e2c 0a01 0e0a  ...........,....
+00000ad0: 0a01 0804 0802 0404 0201 0201 0201 0afd  ................
+00000ae0: 723b 0000 0029 0272 0500 0000 7205 0000  r;...).r....r...
+00000af0: 0029 19da 075f 5f64 6f63 5f5f da15 7370  .)...__doc__..sp
+00000b00: 6163 6573 2e64 6f6e 655f 7769 7468 5f73  aces.done_with_s
+00000b10: 6361 6e72 0200 0000 da12 7370 6163 6573  canr......spaces
+00000b20: 2e70 6174 6873 5f70 6174 6368 7203 0000  .paths_patchr...
+00000b30: 00da 1e73 7061 6365 732e 7468 655f 6865  ...spaces.the_he
+00000b40: 616c 7468 5f73 6361 6e5f 7374 6172 7465  alth_scan_starte
+00000b50: 6472 0400 0000 da39 6269 6f74 6563 682e  dr.....9biotech.
+00000b60: 7072 6f63 6564 7572 6573 2e61 6767 7265  procedures.aggre
+00000b70: 6761 746f 725f 7072 6f63 6564 7572 652e  gator_procedure.
+00000b80: 7072 6f63 6573 732e 7661 7269 6162 6c65  process.variable
+00000b90: 7372 0600 0000 da05 666c 6173 6b72 0700  sr......flaskr..
+00000ba0: 0000 7208 0000 0072 0900 0000 da04 7269  ..r....r......ri
+00000bb0: 6368 da04 6a73 6f6e da07 7061 7468 6c69  ch..json..pathli
+00000bc0: 62da 026f 73da 076f 732e 7061 7468 720a  b..os..os.pathr.
+00000bd0: 0000 0072 0b00 0000 720c 0000 00da 0373  ...r....r......s
+00000be0: 7973 da09 7468 7265 6164 696e 67da 0474  ys..threading..t
+00000bf0: 696d 6572 3b00 0000 7216 0000 0072 1600  imer;...r....r..
+00000c00: 0000 7216 0000 0072 1700 0000 da08 3c6d  ..r....r......<m
+00000c10: 6f64 756c 653e 0100 0000 7322 0000 0004  odule>....s"....
+00000c20: 020c 0c0c 010c 010c 0214 0308 0108 0308  ................
+00000c30: 0108 0114 0108 0108 0108 0102 0502 010e  ................
+00000c40: fe                                       .
```

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 				print_waiting_for (unfinished, time_limit)
 			
 			result = send_done_if_finished (unfinished)
 			if (result == "sent"):
 				break;
 			
 			
-			
 			cycle += 1
 			if (cycle == 3):
 				cycle = 0
 			
 			time.sleep (1)
```

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 18:55:07 2024 UTC, .py size: 1834 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0bbe 2266 2a07 0000  o........."f*...
+00000000: 6f0d 0d0a 0000 0000 43fe 2266 2607 0000  o.......C."f&...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
 00000040: 6404 6c03 6d03 5a03 0100 6403 6405 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6406 6407 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6406 6408 6c08 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6409 6c09 6d0a 5a0a 0100 6401 640a 6c0b  d.l.m.Z...d.d.l.
@@ -78,24 +78,24 @@
 000004d0: 6d65 da05 736c 6565 7029 05da 0a73 746f  me..sleep)...sto
 000004e0: 705f 6576 656e 74da 0563 7963 6c65 720e  p_event..cycler.
 000004f0: 0000 00da 0a75 6e66 696e 6973 6865 64da  .....unfinished.
 00000500: 0672 6573 756c 7472 1500 0000 7215 0000  .resultr....r...
 00000510: 0072 1600 0000 da04 7461 736b 3500 0000  .r......task5...
 00000520: 7324 0000 0004 0108 020c 010e 0104 020c  s$..............
 00000530: 0702 0106 0208 020a 0108 0208 0104 0108  ................
-00000540: 0408 0104 010a 0210 e37a 2273 7461 7475  .........z"statu
+00000540: 0308 0104 010a 0210 e47a 2273 7461 7475  .........z"statu
 00000550: 735f 6368 6563 6b5f 6d6f 6e69 746f 722e  s_check_monitor.
 00000560: 3c6c 6f63 616c 733e 2e74 6173 6b29 0172  <locals>.task).r
 00000570: 2600 0000 da02 6f6e 2901 4e29 0272 0200  &.....on).N).r..
 00000580: 0000 7209 0000 0029 0372 1800 0000 7226  ..r....).r....r&
 00000590: 0000 00da 0874 6865 5f74 6173 6b72 1500  .....the_taskr..
 000005a0: 0000 7215 0000 0072 1600 0000 da14 7374  ..r....r......st
 000005b0: 6174 7573 5f63 6865 636b 5f6d 6f6e 6974  atus_check_monit
 000005c0: 6f72 3200 0000 730c 0000 0008 010a 0202  or2...s.........
-000005d0: 2502 0106 ff0e 0372 2900 0000 2914 da07  %......r)...)...
+000005d0: 2402 0106 ff0e 0372 2900 0000 2914 da07  $......r)...)...
 000005e0: 5f5f 646f 635f 5fda 3962 696f 7465 6368  __doc__.9biotech
 000005f0: 2e70 726f 6365 6475 7265 732e 6167 6772  .procedures.aggr
 00000600: 6567 6174 6f72 5f70 726f 6365 6475 7265  egator_procedure
 00000610: 2e70 726f 6365 7373 2e76 6172 6961 626c  .process.variabl
 00000620: 6573 7202 0000 0072 0400 0000 da0e 646f  esr....r......do
 00000630: 6e65 5f77 6974 685f 7363 616e 7205 0000  ne_with_scanr...
 00000640: 00da 0c74 6865 5f70 6879 7369 6361 6c72  ...the_physicalr
```

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 23:06:53 2024 UTC, .py size: 9847 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0df9 2266 7726 0000  o........."fw&..
+00000000: 6f0d 0d0a 0000 0000 40ff 2266 6126 0000  o.......@."fa&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6405 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6400 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6408 6c0b 5a0b 6400  m.Z...d.d.l.Z.d.
@@ -14,19 +14,19 @@
 000000d0: 2901 da27 6c65 6172 6e5f 6966 5f67 6c6f  )..'learn_if_glo
 000000e0: 6261 6c5f 7469 6d65 5f6c 696d 6974 5f77  bal_time_limit_w
 000000f0: 6173 5f65 7863 6565 6465 6429 01da 1670  as_exceeded)...p
 00000100: 6172 7365 5f70 5f65 7870 6563 745f 7265  arse_p_expect_re
 00000110: 636f 7264 7329 01da 0d73 686f 775f 7661  cords)...show_va
 00000120: 7269 6162 6c65 2901 da06 7070 7269 6e74  riable)...pprint
 00000130: 4e63 0000 0000 0000 0000 0000 0000 0d00  Nc..............
-00000140: 0000 0b00 0000 4300 0000 73b2 0600 0074  ......C...s....t
+00000140: 0000 0b00 0000 4300 0000 73ae 0600 0074  ......C...s....t
 00000150: 0083 007d 007c 0064 0119 007d 017c 0064  ...}.|.d...}.|.d
 00000160: 0219 007d 027c 0064 0319 0064 0419 007d  ...}.|.d...d...}
 00000170: 0369 007d 0467 007d 057c 0244 0090 035d  .i.}.g.}.|.D...]
-00000180: 217d 067c 027c 0619 007d 077c 0764 0519  !}.|.|...}.|.d..
+00000180: 1f7d 067c 027c 0619 007d 077c 0764 0519  .}.|.|...}.|.d..
 00000190: 007d 0809 007a 2d64 067c 027c 0619 0064  .}...z-d.|.|...d
 000001a0: 0619 0076 0072 4f74 017c 027c 0619 0064  ...v.rOt.|.|...d
 000001b0: 0619 0064 0619 0083 0164 006b 0372 4f7c  ...d.....d.k.rO|
 000001c0: 027c 0619 0064 0619 0064 0619 00a0 02a1  .|...d...d......
 000001d0: 007d 097c 0964 076b 0272 4b64 087c 0864  .}.|.d.k.rKd.|.d
 000001e0: 093c 006e 0464 0a7c 0864 093c 0057 006e  .<.n.d.|.d.<.W.n
 000001f0: 1b04 0074 0379 6b01 007d 0a01 007a 0f74  ...t.yk..}...z.t
@@ -53,220 +53,220 @@
 00000340: 3a7c 0864 1d19 0064 086b 0290 0172 317c  :|.d...d.k...r1|
 00000350: 0864 1e19 0064 0a6b 0290 0172 3174 07a0  .d...d.k...r1t..
 00000360: 07a1 0074 087c 027c 0619 0064 1019 0064  ...t.|.|...d...d
 00000370: 1119 0083 0118 007d 0b7c 0b64 1f6b 0590  .......}.|.d.k..
 00000380: 0172 317c 0664 2067 007c 0864 219c 047c  .r1|.d g.|.d!..|
 00000390: 0064 0219 007c 0619 0064 173c 0064 187c  .d...|...d.<.d.|
 000003a0: 0064 0219 007c 0619 0064 1919 0064 063c  .d...|...d...d.<
-000003b0: 0057 006e 1a04 0074 0390 0179 4c01 007d  .W.n...t...yL..}
-000003c0: 0a01 007a 0d74 0464 1c74 0aa0 0ba1 0083  ...z.t.d.t......
-000003d0: 0201 0057 0059 0064 007d 0a7e 0a6e 0564  ...W.Y.d.}.~.n.d
-000003e0: 007d 0a7e 0a77 0177 0009 007a 6c7c 0864  .}.~.w.w...zl|.d
-000003f0: 0e19 0064 086b 0290 0172 b97c 0864 0f19  ...d.k...r.|.d..
-00000400: 0064 0a6b 0290 0172 b974 07a0 07a1 0074  .d.k...r.t.....t
-00000410: 087c 027c 0619 0064 1019 0064 1119 0083  .|.|...d...d....
-00000420: 0118 007d 0b7c 0b64 226b 0590 0172 b97a  ...}.|.d"k...r.z
-00000430: 087c 027c 0619 0064 1319 007d 0857 006e  .|.|...d...}.W.n
-00000440: 0c04 0074 0390 0179 8401 0001 0001 0064  ...t...y.......d
-00000450: 147d 0859 006e 0177 007c 0664 2367 007c  .}.Y.n.w.|.d#g.|
-00000460: 0864 0764 169c 057c 0064 0219 007c 0619  .d.d...|.d...|..
-00000470: 0064 173c 0064 187c 0064 0219 007c 0619  .d.<.d.|.d...|..
-00000480: 0064 1919 0064 063c 0064 1a7c 0064 0219  .d...d.<.d.|.d..
-00000490: 007c 0619 0064 0519 0064 1b3c 007c 0064  .|...d...d.<.|.d
-000004a0: 0219 007c 0619 0064 0619 0064 0619 00a0  ...|...d...d....
-000004b0: 09a1 0001 0074 0c64 247c 0669 0183 0101  .....t.d$|.i....
-000004c0: 0057 006e 1a04 0074 0390 0179 d401 007d  .W.n...t...y...}
-000004d0: 0a01 007a 0d74 0464 1c74 0aa0 0ba1 0083  ...z.t.d.t......
-000004e0: 0201 0057 0059 0064 007d 0a7e 0a6e 0564  ...W.Y.d.}.~.n.d
-000004f0: 007d 0a7e 0a77 0177 0009 007a b47c 0864  .}.~.w.w...z.|.d
-00000500: 0e19 0064 086b 027c 0864 0919 0064 086b  ...d.k.|.d...d.k
-00000510: 027c 0864 2519 0064 0a6b 0274 0d7c 027c  .|.d%..d.k.t.|.|
-00000520: 0619 0064 1019 0064 1119 0083 0164 266b  ...d...d.....d&k
-00000530: 0574 0d7c 027c 0619 0064 2719 0083 0164  .t.|.|...d'....d
-00000540: 286b 0274 07a0 07a1 0074 087c 027c 0619  (k.t.....t.|.|..
-00000550: 0064 1019 0064 1119 0083 0118 0064 299c  .d...d.......d).
-00000560: 067d 0c7c 0864 0e19 0064 086b 0290 0272  .}.|.d...d.k...r
-00000570: 897c 0864 0919 0064 086b 0290 0272 897c  .|.d...d.k...r.|
-00000580: 0864 2519 0064 0a6b 0290 0272 8974 0d7c  .d%..d.k...r.t.|
-00000590: 027c 0619 0064 1019 0064 1119 0083 0164  .|...d...d.....d
-000005a0: 266b 0590 0272 8974 0d7c 027c 0619 0064  &k...r.t.|.|...d
-000005b0: 2719 0083 0164 286b 0290 0272 8974 07a0  '....d(k...r.t..
-000005c0: 07a1 0074 087c 027c 0619 0064 1019 0064  ...t.|.|...d...d
-000005d0: 1119 0083 0118 007d 0b7c 0b64 2a6b 0590  .......}.|.d*k..
-000005e0: 0272 8974 0c64 2b7c 0669 0183 0101 007a  .r.t.d+|.i.....z
-000005f0: 087c 027c 0619 0064 1319 007d 0857 006e  .|.|...d...}.W.n
-00000600: 0c04 0074 0390 0279 6401 0001 0001 0064  ...t...yd......d
-00000610: 147d 0859 006e 0177 007c 0664 2c67 007c  .}.Y.n.w.|.d,g.|
-00000620: 0864 0764 2d9c 057c 0064 0219 007c 0619  .d.d-..|.d...|..
-00000630: 0064 173c 0064 187c 0064 0219 007c 0619  .d.<.d.|.d...|..
-00000640: 0064 1919 0064 063c 007c 0064 0219 007c  .d...d.<.|.d...|
-00000650: 0619 0064 0619 0064 0619 00a0 09a1 0001  ...d...d........
-00000660: 0057 006e 1804 0074 0390 0279 a201 007d  .W.n...t...y...}
-00000670: 0a01 007a 0b74 0464 2e7c 0a83 0201 0057  ...z.t.d.|.....W
-00000680: 0059 0064 007d 0a7e 0a6e 0564 007d 0a7e  .Y.d.}.~.n.d.}.~
-00000690: 0a77 0177 0009 007a 367c 0864 0e19 0064  .w.w...z6|.d...d
-000006a0: 086b 0290 0272 d97c 0864 0f19 0064 086b  .k...r.|.d...d.k
-000006b0: 0290 0272 d97c 0864 2519 0064 0a6b 0290  ...r.|.d%..d.k..
-000006c0: 0272 d97c 0864 0919 0064 086b 0390 0272  .r.|.d...d.k...r
-000006d0: d97c 0664 2f67 007c 0864 0764 169c 057c  .|.d/g.|.d.d...|
-000006e0: 0064 0219 007c 0619 0064 173c 0064 187c  .d...|...d.<.d.|
-000006f0: 0064 0219 007c 0619 0064 1919 0064 063c  .d...|...d...d.<
-00000700: 0057 006e 1a04 0074 0390 0279 f401 007d  .W.n...t...y...}
-00000710: 0a01 007a 0d74 0464 3074 0aa0 0ba1 0083  ...z.t.d0t......
-00000720: 0201 0057 0059 0064 007d 0a7e 0a6e 0564  ...W.Y.d.}.~.n.d
-00000730: 007d 0a7e 0a77 0177 0009 0009 007a 287c  .}.~.w.w.....z(|
-00000740: 0864 0919 0064 0a6b 0290 0372 1e7c 0864  .d...d.k...r.|.d
-00000750: 0e19 0064 086b 0290 0372 1e7c 0864 2519  ...d.k...r.|.d%.
-00000760: 0064 086b 0290 0372 1e7c 0864 3119 0064  .d.k...r.|.d1..d
-00000770: 086b 0290 0372 1e64 187c 0064 0219 007c  .k...r.d.|.d...|
-00000780: 0619 0064 1919 0064 063c 0057 0071 1704  ...d...d.<.W.q..
-00000790: 0074 0390 0379 3901 007d 0a01 007a 0d74  .t...y9..}...z.t
-000007a0: 0464 3074 0aa0 0ba1 0083 0201 0057 0059  .d0t.........W.Y
-000007b0: 0064 007d 0a7e 0a71 1764 007d 0a7e 0a77  .d.}.~.q.d.}.~.w
-000007c0: 0177 007c 0244 005d 1a7d 067c 027c 0619  .w.|.D.].}.|.|..
-000007d0: 0064 1919 0064 0619 0064 186b 0390 0372  .d...d...d.k...r
-000007e0: 557c 05a0 0e7c 067c 0064 0219 007c 0619  U|...|.|.d...|..
-000007f0: 0064 329c 02a1 0101 0090 0371 3c7c 0553  .d2........q<|.S
-00000800: 0029 334e da0d 7265 636f 7264 735f 6c65  .)3N..records_le
-00000810: 7665 6cda 1169 6e74 6572 6e61 6c5f 7374  vel..internal_st
-00000820: 6174 7573 6573 da0f 696e 7472 6f5f 7661  atuses..intro_va
-00000830: 7269 6162 6c65 73da 0a74 696d 655f 6c69  riables..time_li
-00000840: 6d69 74da 0b6f 6363 7572 7265 6e63 6573  mit..occurrences
-00000850: da07 7072 6f63 6573 7354 da03 7965 737a  ..processT..yesz
-00000860: 1573 6361 6e20 7072 6f63 6573 7320 6973  .scan process is
-00000870: 2061 6c69 7665 da02 6e6f 7a1e 7072 6f63   alive..noz.proc
-00000880: 6573 7320 616c 6976 6520 6368 6563 6b20  ess alive check 
-00000890: 6578 6365 7074 696f 6e3a da07 756e 6b6e  exception:..unkn
-000008a0: 6f77 6e7a 1c73 6361 6e20 7072 6f63 6573  ownz.scan proces
-000008b0: 7320 7665 6e74 7572 6520 7374 6172 7465  s venture starte
-000008c0: 647a 1473 6361 6e20 7072 6f63 6573 7320  dz.scan process 
-000008d0: 7374 6172 7465 647a 2073 6361 6e20 7072  startedz scan pr
-000008e0: 6f63 6573 7320 6e6f 7469 6669 6564 2061  ocess notified a
-000008f0: 6767 7265 6761 746f 72da 0574 696d 6573  ggregator..times
-00000900: 7a0f 7665 6e74 7572 6520 7374 6172 7465  z.venture starte
-00000910: 64e9 1e00 0000 da0a 6f63 6375 7265 6e63  d.......occurenc
-00000920: 6573 7a09 6e6f 7420 666f 756e 647a 6741  esz.not foundzgA
-00000930: 6674 6572 2033 3020 7365 636f 6e64 732c  fter 30 seconds,
-00000940: 2074 6865 2061 6674 6572 2070 726f 6365   the after proce
-00000950: 7373 206c 696e 6520 7761 7320 6e6f 7420  ss line was not 
-00000960: 7265 6163 6865 6420 616e 6420 7468 6520  reached and the 
-00000970: 7072 6f63 6573 7320 6469 6420 6e6f 7420  process did not 
-00000980: 6e6f 7469 6679 2074 6865 2061 6767 7265  notify the aggre
-00000990: 6761 746f 722e 2905 da04 7061 7468 da05  gator.)...path..
-000009a0: 616c 6172 6dfa 0b61 6c61 726d 206e 6f74  alarm..alarm not
-000009b0: 6573 720d 0000 00da 0665 7869 7465 64da  esr......exited.
-000009c0: 0f72 6573 756c 7473 5f6f 665f 7363 616e  .results_of_scan
-000009d0: da04 646f 6e65 da06 7374 6174 7573 7a3a  ..done..statusz:
-000009e0: 5468 6520 7072 6f63 6573 7320 6469 646e  The process didn
-000009f0: 2774 206e 6f74 6966 7920 7468 6520 6167  't notify the ag
-00000a00: 6772 6567 6174 6f72 2077 6974 6869 6e20  gregator within 
-00000a10: 3520 7365 636f 6e64 732e 7a10 646f 6e65  5 seconds.z.done
-00000a20: 2072 6561 736f 6e20 6769 7665 7a23 7072   reason givez#pr
-00000a30: 6f63 6573 7320 6e6f 6e2d 6e6f 7469 6669  ocess non-notifi
-00000a40: 6361 7469 6f6e 2065 7863 6570 7469 6f6e  cation exception
-00000a50: 3a7a 1473 6361 6e20 7072 6f63 6573 7320  :z.scan process 
-00000a60: 7374 6f70 7065 647a 1c73 6361 6e20 7072  stoppedz.scan pr
-00000a70: 6f63 6565 6473 2077 6572 6520 7265 7472  oceeds were retr
-00000a80: 6965 7665 64e9 0f00 0000 7a5d 5468 6520  ieved.....z]The 
-00000a90: 7363 616e 2070 726f 6365 7373 2077 6173  scan process was
-00000aa0: 2073 746f 7070 6564 2c20 6275 7420 3135   stopped, but 15
-00000ab0: 2073 6563 6f6e 6473 2068 6176 6520 7061   seconds have pa
-00000ac0: 7373 6564 2061 6e64 2074 6865 2070 726f  ssed and the pro
-00000ad0: 6365 6564 7320 7765 7265 206e 6f74 2072  ceeds were not r
-00000ae0: 6574 7269 6576 6564 2e29 0472 1500 0000  etrieved.).r....
-00000af0: 7216 0000 0072 1700 0000 720d 0000 00e9  r....r....r.....
-00000b00: 1400 0000 7a50 4166 7465 7220 3230 2073  ....zPAfter 20 s
-00000b10: 6563 6f6e 6473 2c20 7468 6520 7072 6f63  econds, the proc
-00000b20: 6573 7320 6469 6420 6e6f 7420 6e6f 7469  ess did not noti
-00000b30: 6679 2074 6865 2061 6767 7265 6761 746f  fy the aggregato
-00000b40: 7220 7468 6174 2069 7420 6861 6420 7374  r that it had st
-00000b50: 6172 7465 642e 7a18 7072 6f63 6573 7320  arted.z.process 
-00000b60: 6d61 7920 6861 7665 2073 746f 7070 6564  may have stopped
-00000b70: 7a18 7363 616e 2070 726f 6365 7373 2077  z.scan process w
-00000b80: 6173 2073 746f 7070 6564 7203 0000 00da  as stoppedr.....
-00000b90: 0772 6563 6f72 6473 7201 0000 0029 06da  .recordsr....)..
-00000ba0: 0131 da01 32da 0133 da01 34da 0136 da01  .1..2..3..4..6..
-00000bb0: 37e9 0a00 0000 7a2b 7265 636f 7264 7320  7.....z+records 
-00000bc0: 7765 7265 206e 6f74 2072 6574 7269 6576  were not retriev
-00000bd0: 6564 2061 6674 6572 2031 3020 7365 636f  ed after 10 seco
-00000be0: 6e64 737a 2d41 6674 6572 2031 3020 7365  ndsz-After 10 se
-00000bf0: 636f 6e64 732c 206e 6f20 7072 6f63 6573  conds, no proces
-00000c00: 7320 6c6f 6773 2077 6572 6520 666f 756e  s logs were foun
-00000c10: 642e 2905 7215 0000 0072 1600 0000 7217  d.).r....r....r.
-00000c20: 0000 0072 1400 0000 7218 0000 007a 2870  ...r....r....z(p
-00000c30: 726f 6365 7373 206c 6f67 7320 7469 6d65  rocess logs time
-00000c40: 206c 696d 6974 2063 6865 636b 2065 7863   limit check exc
-00000c50: 6570 7469 6f6e 3a7a 3054 6865 2070 726f  eption:z0The pro
-00000c60: 6365 7373 2065 7869 7465 6420 6265 666f  cess exited befo
-00000c70: 7265 2072 6573 756c 7473 2063 6f75 6c64  re results could
-00000c80: 2062 6520 7365 6e74 2e7a 1a70 6172 7365   be sent.z.parse
-00000c90: 2061 6e64 2063 6865 636b 2065 7863 6570   and check excep
-00000ca0: 7469 6f6e 3a7a 1b73 6361 6e20 7265 636f  tion:z.scan reco
-00000cb0: 7264 7320 7765 7265 2072 6574 7269 6576  rds were retriev
-00000cc0: 6564 2902 7215 0000 00da 0969 6e74 6572  ed).r......inter
-00000cd0: 6e61 6c73 290f 7202 0000 00da 0474 7970  nals).r......typ
-00000ce0: 65da 0869 735f 616c 6976 65da 0945 7863  e..is_alive..Exc
-00000cf0: 6570 7469 6f6e da05 7072 696e 7472 0400  eption..printr..
-00000d00: 0000 7205 0000 00da 0474 696d 65da 0566  ..r......time..f
-00000d10: 6c6f 6174 da09 7465 726d 696e 6174 65da  loat..terminate.
-00000d20: 0974 7261 6365 6261 636b da0a 666f 726d  .traceback..form
-00000d30: 6174 5f65 7863 7207 0000 00da 036c 656e  at_excr......len
-00000d40: da06 6170 7065 6e64 290d da14 6167 6772  ..append)...aggr
-00000d50: 6567 6174 6f72 5f76 6172 6961 626c 6573  egator_variables
-00000d60: 7209 0000 0072 0a00 0000 720c 0000 00da  r....r....r.....
-00000d70: 0873 7461 7475 7365 73da 0a75 6e66 696e  .statuses..unfin
-00000d80: 6973 6865 64da 0b73 7461 7475 735f 7061  ished..status_pa
-00000d90: 7468 da0e 7374 6174 7573 5f6f 665f 7061  th..status_of_pa
-00000da0: 7468 720d 0000 00da 0561 6c69 7665 da01  thr......alive..
-00000db0: 45da 0765 6c61 7073 6564 da05 646f 6f72  E..elapsed..door
-00000dc0: 73a9 0072 3b00 0000 fa71 2f62 696f 7465  s..r;....q/biote
-00000dd0: 6368 2f76 656e 7565 732f 7374 6167 6573  ch/venues/stages
-00000de0: 2f62 696f 7465 6368 2f70 726f 6365 6475  /biotech/procedu
-00000df0: 7265 732f 6167 6772 6567 6174 6f72 5f70  res/aggregator_p
-00000e00: 726f 6365 6475 7265 2f70 726f 6365 7373  rocedure/process
-00000e10: 2f6d 6f76 6573 2f73 7461 7475 735f 6368  /moves/status_ch
-00000e20: 6563 6b5f 6d6f 6e69 746f 722f 7468 655f  eck_monitor/the_
-00000e30: 7068 7973 6963 616c 2e70 79da 2470 6172  physical.py.$par
-00000e40: 7365 5f61 6e64 5f63 6865 636b 5f69 735f  se_and_check_is_
-00000e50: 616c 6976 655f 6f66 5f73 7461 7475 7365  alive_of_statuse
-00000e60: 7321 0000 0073 6401 0000 0601 0802 0801  s!...sd.........
-00000e70: 0c01 0402 0401 0a01 0802 0801 0202 0204  ................
-00000e80: 1001 1801 1401 0801 0a01 0802 0480 0e02  ................
-00000e90: 0a01 1401 0880 02fe 0805 0803 0205 020c  ................
-00000ea0: 0c02 0c01 0c01 1c02 0802 0201 1001 0c01  ................
-00000eb0: 0801 02ff 0204 0202 0201 0202 0202 12f8  ................
-00000ec0: 140b 1401 1802 0480 0e03 0e01 0c01 0880  ................
-00000ed0: 02fe 0205 0206 0e02 0e01 1c02 0a02 0202  ................
-00000ee0: 0202 0201 0202 12fa 1409 0480 1002 0e01  ................
-00000ef0: 0c01 0880 02fe 0205 0208 0e02 0e01 1c02  ................
-00000f00: 0a02 0201 1001 0e01 0801 02ff 0204 0202  ................
-00000f10: 0201 0202 0202 12f8 140b 1401 1801 0202  ................
-00000f20: 0401 06ff 0480 1003 0e01 0c01 0880 02fe  ................
-00000f30: 0205 0212 0a02 0a01 0a01 1601 1201 1a01  ................
-00000f40: 06fa 0e0b 0e01 0e01 1a01 1602 1c02 0a02  ................
-00000f50: 0201 0401 06ff 0204 1001 0e01 0801 02ff  ................
-00000f60: 0204 0202 0201 0202 0202 12f8 140b 1801  ................
-00000f70: 0480 1004 0a01 0c01 0880 02fe 0206 020c  ................
-00000f80: 0e02 0e01 0e02 0e02 0203 0202 0201 0201  ................
-00000f90: 0202 12f9 140a 0480 1002 0e01 0c01 0880  ................
-00000fa0: 02fe 0205 0208 0203 0e02 0e02 0e01 0e02  ................
-00000fb0: 1402 0480 1002 0e01 0c01 0880 02fe 0806  ................
-00000fc0: 1601 0401 0201 0a01 08fe 0480 0406 723d  ..............r=
-00000fd0: 0000 0029 0fda 3962 696f 7465 6368 2e70  ...)..9biotech.p
-00000fe0: 726f 6365 6475 7265 732e 6167 6772 6567  rocedures.aggreg
-00000ff0: 6174 6f72 5f70 726f 6365 6475 7265 2e70  ator_procedure.p
-00001000: 726f 6365 7373 2e76 6172 6961 626c 6573  rocess.variables
-00001010: 7202 0000 0072 1e00 0000 7204 0000 00da  r....r....r.....
-00001020: 2761 6c61 726d 5f63 6865 636b 732e 676c  'alarm_checks.gl
-00001030: 6f62 616c 5f74 696d 655f 6c69 6d69 745f  obal_time_limit_
-00001040: 6578 6365 6564 6564 7205 0000 00da 3062  exceededr.....0b
-00001050: 696f 7465 6368 2e74 6f70 6963 732e 7072  iotech.topics.pr
-00001060: 6f63 6573 735f 6f6e 2e70 5f65 7870 6563  ocess_on.p_expec
-00001070: 742e 7061 7273 655f 7265 636f 7264 7372  t.parse_recordsr
-00001080: 0600 0000 da1c 6269 6f74 6563 682e 746f  ......biotech.to
-00001090: 7069 6373 2e73 686f 772e 7661 7269 6162  pics.show.variab
-000010a0: 6c65 7207 0000 0072 0800 0000 722b 0000  ler....r....r+..
-000010b0: 0072 2e00 0000 da04 7269 6368 723d 0000  .r......richr=..
-000010c0: 0072 3b00 0000 723b 0000 0072 3b00 0000  .r;...r;...r;...
-000010d0: 723c 0000 00da 083c 6d6f 6475 6c65 3e01  r<.....<module>.
-000010e0: 0000 0073 1600 0000 0c07 0c03 0c02 0c02  ...s............
-000010f0: 0c01 0c03 0801 0801 0803 0205 0c04       ..............
+000003b0: 0057 006e 1804 0074 0390 0179 4a01 007d  .W.n...t...yJ..}
+000003c0: 0a01 007a 0b74 0464 1c7c 0a83 0201 0057  ...z.t.d.|.....W
+000003d0: 0059 0064 007d 0a7e 0a6e 0564 007d 0a7e  .Y.d.}.~.n.d.}.~
+000003e0: 0a77 0177 0009 007a 6c7c 0864 0e19 0064  .w.w...zl|.d...d
+000003f0: 086b 0290 0172 b77c 0864 0f19 0064 0a6b  .k...r.|.d...d.k
+00000400: 0290 0172 b774 07a0 07a1 0074 087c 027c  ...r.t.....t.|.|
+00000410: 0619 0064 1019 0064 1119 0083 0118 007d  ...d...d.......}
+00000420: 0b7c 0b64 226b 0590 0172 b77a 087c 027c  .|.d"k...r.z.|.|
+00000430: 0619 0064 1319 007d 0857 006e 0c04 0074  ...d...}.W.n...t
+00000440: 0390 0179 8201 0001 0001 0064 147d 0859  ...y.......d.}.Y
+00000450: 006e 0177 007c 0664 2367 007c 0864 0764  .n.w.|.d#g.|.d.d
+00000460: 169c 057c 0064 0219 007c 0619 0064 173c  ...|.d...|...d.<
+00000470: 0064 187c 0064 0219 007c 0619 0064 1919  .d.|.d...|...d..
+00000480: 0064 063c 0064 1a7c 0064 0219 007c 0619  .d.<.d.|.d...|..
+00000490: 0064 0519 0064 1b3c 007c 0064 0219 007c  .d...d.<.|.d...|
+000004a0: 0619 0064 0619 0064 0619 00a0 09a1 0001  ...d...d........
+000004b0: 0074 0c64 247c 0669 0183 0101 0057 006e  .t.d$|.i.....W.n
+000004c0: 1a04 0074 0390 0179 d201 007d 0a01 007a  ...t...y...}...z
+000004d0: 0d74 0464 1c74 0aa0 0ba1 0083 0201 0057  .t.d.t.........W
+000004e0: 0059 0064 007d 0a7e 0a6e 0564 007d 0a7e  .Y.d.}.~.n.d.}.~
+000004f0: 0a77 0177 0009 007a b47c 0864 0e19 0064  .w.w...z.|.d...d
+00000500: 086b 027c 0864 0919 0064 086b 027c 0864  .k.|.d...d.k.|.d
+00000510: 2519 0064 0a6b 0274 0d7c 027c 0619 0064  %..d.k.t.|.|...d
+00000520: 1019 0064 1119 0083 0164 266b 0574 0d7c  ...d.....d&k.t.|
+00000530: 027c 0619 0064 2719 0083 0164 286b 0274  .|...d'....d(k.t
+00000540: 07a0 07a1 0074 087c 027c 0619 0064 1019  .....t.|.|...d..
+00000550: 0064 1119 0083 0118 0064 299c 067d 0c7c  .d.......d)..}.|
+00000560: 0864 0e19 0064 086b 0290 0272 877c 0864  .d...d.k...r.|.d
+00000570: 0919 0064 086b 0290 0272 877c 0864 2519  ...d.k...r.|.d%.
+00000580: 0064 0a6b 0290 0272 8774 0d7c 027c 0619  .d.k...r.t.|.|..
+00000590: 0064 1019 0064 1119 0083 0164 266b 0590  .d...d.....d&k..
+000005a0: 0272 8774 0d7c 027c 0619 0064 2719 0083  .r.t.|.|...d'...
+000005b0: 0164 286b 0290 0272 8774 07a0 07a1 0074  .d(k...r.t.....t
+000005c0: 087c 027c 0619 0064 1019 0064 1119 0083  .|.|...d...d....
+000005d0: 0118 007d 0b7c 0b64 2a6b 0590 0272 8774  ...}.|.d*k...r.t
+000005e0: 0c64 2b7c 0669 0183 0101 007a 087c 027c  .d+|.i.....z.|.|
+000005f0: 0619 0064 1319 007d 0857 006e 0c04 0074  ...d...}.W.n...t
+00000600: 0390 0279 6201 0001 0001 0064 147d 0859  ...yb......d.}.Y
+00000610: 006e 0177 007c 0664 2c67 007c 0864 0764  .n.w.|.d,g.|.d.d
+00000620: 2d9c 057c 0064 0219 007c 0619 0064 173c  -..|.d...|...d.<
+00000630: 0064 187c 0064 0219 007c 0619 0064 1919  .d.|.d...|...d..
+00000640: 0064 063c 007c 0064 0219 007c 0619 0064  .d.<.|.d...|...d
+00000650: 0619 0064 0619 00a0 09a1 0001 0057 006e  ...d.........W.n
+00000660: 1804 0074 0390 0279 a001 007d 0a01 007a  ...t...y...}...z
+00000670: 0b74 0464 2e7c 0a83 0201 0057 0059 0064  .t.d.|.....W.Y.d
+00000680: 007d 0a7e 0a6e 0564 007d 0a7e 0a77 0177  .}.~.n.d.}.~.w.w
+00000690: 0009 007a 367c 0864 0e19 0064 086b 0290  ...z6|.d...d.k..
+000006a0: 0272 d77c 0864 0f19 0064 086b 0290 0272  .r.|.d...d.k...r
+000006b0: d77c 0864 2519 0064 0a6b 0290 0272 d77c  .|.d%..d.k...r.|
+000006c0: 0864 0919 0064 086b 0390 0272 d77c 0664  .d...d.k...r.|.d
+000006d0: 2f67 007c 0864 0764 169c 057c 0064 0219  /g.|.d.d...|.d..
+000006e0: 007c 0619 0064 173c 0064 187c 0064 0219  .|...d.<.d.|.d..
+000006f0: 007c 0619 0064 1919 0064 063c 0057 006e  .|...d...d.<.W.n
+00000700: 1a04 0074 0390 0279 f201 007d 0a01 007a  ...t...y...}...z
+00000710: 0d74 0464 3074 0aa0 0ba1 0083 0201 0057  .t.d0t.........W
+00000720: 0059 0064 007d 0a7e 0a6e 0564 007d 0a7e  .Y.d.}.~.n.d.}.~
+00000730: 0a77 0177 0009 0009 007a 287c 0864 0919  .w.w.....z(|.d..
+00000740: 0064 0a6b 0290 0372 1c7c 0864 0e19 0064  .d.k...r.|.d...d
+00000750: 086b 0290 0372 1c7c 0864 2519 0064 086b  .k...r.|.d%..d.k
+00000760: 0290 0372 1c7c 0864 3119 0064 086b 0290  ...r.|.d1..d.k..
+00000770: 0372 1c64 187c 0064 0219 007c 0619 0064  .r.d.|.d...|...d
+00000780: 1919 0064 063c 0057 0071 1704 0074 0390  ...d.<.W.q...t..
+00000790: 0379 3701 007d 0a01 007a 0d74 0464 3074  .y7..}...z.t.d0t
+000007a0: 0aa0 0ba1 0083 0201 0057 0059 0064 007d  .........W.Y.d.}
+000007b0: 0a7e 0a71 1764 007d 0a7e 0a77 0177 007c  .~.q.d.}.~.w.w.|
+000007c0: 0244 005d 1a7d 067c 027c 0619 0064 1919  .D.].}.|.|...d..
+000007d0: 0064 0619 0064 186b 0390 0372 537c 05a0  .d...d.k...rS|..
+000007e0: 0e7c 067c 0064 0219 007c 0619 0064 329c  .|.|.d...|...d2.
+000007f0: 02a1 0101 0090 0371 3a7c 0553 0029 334e  .......q:|.S.)3N
+00000800: da0d 7265 636f 7264 735f 6c65 7665 6cda  ..records_level.
+00000810: 1169 6e74 6572 6e61 6c5f 7374 6174 7573  .internal_status
+00000820: 6573 da0f 696e 7472 6f5f 7661 7269 6162  es..intro_variab
+00000830: 6c65 73da 0a74 696d 655f 6c69 6d69 74da  les..time_limit.
+00000840: 0b6f 6363 7572 7265 6e63 6573 da07 7072  .occurrences..pr
+00000850: 6f63 6573 7354 da03 7965 737a 1573 6361  ocessT..yesz.sca
+00000860: 6e20 7072 6f63 6573 7320 6973 2061 6c69  n process is ali
+00000870: 7665 da02 6e6f 7a1e 7072 6f63 6573 7320  ve..noz.process 
+00000880: 616c 6976 6520 6368 6563 6b20 6578 6365  alive check exce
+00000890: 7074 696f 6e3a da07 756e 6b6e 6f77 6e7a  ption:..unknownz
+000008a0: 1c73 6361 6e20 7072 6f63 6573 7320 7665  .scan process ve
+000008b0: 6e74 7572 6520 7374 6172 7465 647a 1473  nture startedz.s
+000008c0: 6361 6e20 7072 6f63 6573 7320 7374 6172  can process star
+000008d0: 7465 647a 2073 6361 6e20 7072 6f63 6573  tedz scan proces
+000008e0: 7320 6e6f 7469 6669 6564 2061 6767 7265  s notified aggre
+000008f0: 6761 746f 72da 0574 696d 6573 7a0f 7665  gator..timesz.ve
+00000900: 6e74 7572 6520 7374 6172 7465 64e9 1e00  nture started...
+00000910: 0000 da0a 6f63 6375 7265 6e63 6573 7a09  ....occurencesz.
+00000920: 6e6f 7420 666f 756e 647a 6741 6674 6572  not foundzgAfter
+00000930: 2033 3020 7365 636f 6e64 732c 2074 6865   30 seconds, the
+00000940: 2061 6674 6572 2070 726f 6365 7373 206c   after process l
+00000950: 696e 6520 7761 7320 6e6f 7420 7265 6163  ine was not reac
+00000960: 6865 6420 616e 6420 7468 6520 7072 6f63  hed and the proc
+00000970: 6573 7320 6469 6420 6e6f 7420 6e6f 7469  ess did not noti
+00000980: 6679 2074 6865 2061 6767 7265 6761 746f  fy the aggregato
+00000990: 722e 2905 da04 7061 7468 da05 616c 6172  r.)...path..alar
+000009a0: 6dfa 0b61 6c61 726d 206e 6f74 6573 720d  m..alarm notesr.
+000009b0: 0000 00da 0665 7869 7465 64da 0f72 6573  .....exited..res
+000009c0: 756c 7473 5f6f 665f 7363 616e da04 646f  ults_of_scan..do
+000009d0: 6e65 da06 7374 6174 7573 7a3a 5468 6520  ne..statusz:The 
+000009e0: 7072 6f63 6573 7320 6469 646e 2774 206e  process didn't n
+000009f0: 6f74 6966 7920 7468 6520 6167 6772 6567  otify the aggreg
+00000a00: 6174 6f72 2077 6974 6869 6e20 3520 7365  ator within 5 se
+00000a10: 636f 6e64 732e 7a10 646f 6e65 2072 6561  conds.z.done rea
+00000a20: 736f 6e20 6769 7665 7a23 7072 6f63 6573  son givez#proces
+00000a30: 7320 6e6f 6e2d 6e6f 7469 6669 6361 7469  s non-notificati
+00000a40: 6f6e 2065 7863 6570 7469 6f6e 3a7a 1473  on exception:z.s
+00000a50: 6361 6e20 7072 6f63 6573 7320 7374 6f70  can process stop
+00000a60: 7065 647a 1c73 6361 6e20 7072 6f63 6565  pedz.scan procee
+00000a70: 6473 2077 6572 6520 7265 7472 6965 7665  ds were retrieve
+00000a80: 64e9 0f00 0000 7a5d 5468 6520 7363 616e  d.....z]The scan
+00000a90: 2070 726f 6365 7373 2077 6173 2073 746f   process was sto
+00000aa0: 7070 6564 2c20 6275 7420 3135 2073 6563  pped, but 15 sec
+00000ab0: 6f6e 6473 2068 6176 6520 7061 7373 6564  onds have passed
+00000ac0: 2061 6e64 2074 6865 2070 726f 6365 6564   and the proceed
+00000ad0: 7320 7765 7265 206e 6f74 2072 6574 7269  s were not retri
+00000ae0: 6576 6564 2e29 0472 1500 0000 7216 0000  eved.).r....r...
+00000af0: 0072 1700 0000 720d 0000 00e9 1400 0000  .r....r.........
+00000b00: 7a50 4166 7465 7220 3230 2073 6563 6f6e  zPAfter 20 secon
+00000b10: 6473 2c20 7468 6520 7072 6f63 6573 7320  ds, the process 
+00000b20: 6469 6420 6e6f 7420 6e6f 7469 6679 2074  did not notify t
+00000b30: 6865 2061 6767 7265 6761 746f 7220 7468  he aggregator th
+00000b40: 6174 2069 7420 6861 6420 7374 6172 7465  at it had starte
+00000b50: 642e 7a18 7072 6f63 6573 7320 6d61 7920  d.z.process may 
+00000b60: 6861 7665 2073 746f 7070 6564 7a18 7363  have stoppedz.sc
+00000b70: 616e 2070 726f 6365 7373 2077 6173 2073  an process was s
+00000b80: 746f 7070 6564 7203 0000 00da 0772 6563  toppedr......rec
+00000b90: 6f72 6473 7201 0000 0029 06da 0131 da01  ordsr....)...1..
+00000ba0: 32da 0133 da01 34da 0136 da01 37e9 0a00  2..3..4..6..7...
+00000bb0: 0000 7a2b 7265 636f 7264 7320 7765 7265  ..z+records were
+00000bc0: 206e 6f74 2072 6574 7269 6576 6564 2061   not retrieved a
+00000bd0: 6674 6572 2031 3020 7365 636f 6e64 737a  fter 10 secondsz
+00000be0: 2d41 6674 6572 2031 3020 7365 636f 6e64  -After 10 second
+00000bf0: 732c 206e 6f20 7072 6f63 6573 7320 6c6f  s, no process lo
+00000c00: 6773 2077 6572 6520 666f 756e 642e 2905  gs were found.).
+00000c10: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000c20: 1400 0000 7218 0000 007a 2870 726f 6365  ....r....z(proce
+00000c30: 7373 206c 6f67 7320 7469 6d65 206c 696d  ss logs time lim
+00000c40: 6974 2063 6865 636b 2065 7863 6570 7469  it check excepti
+00000c50: 6f6e 3a7a 3054 6865 2070 726f 6365 7373  on:z0The process
+00000c60: 2065 7869 7465 6420 6265 666f 7265 2072   exited before r
+00000c70: 6573 756c 7473 2063 6f75 6c64 2062 6520  esults could be 
+00000c80: 7365 6e74 2e7a 1a70 6172 7365 2061 6e64  sent.z.parse and
+00000c90: 2063 6865 636b 2065 7863 6570 7469 6f6e   check exception
+00000ca0: 3a7a 1b73 6361 6e20 7265 636f 7264 7320  :z.scan records 
+00000cb0: 7765 7265 2072 6574 7269 6576 6564 2902  were retrieved).
+00000cc0: 7215 0000 00da 0969 6e74 6572 6e61 6c73  r......internals
+00000cd0: 290f 7202 0000 00da 0474 7970 65da 0869  ).r......type..i
+00000ce0: 735f 616c 6976 65da 0945 7863 6570 7469  s_alive..Excepti
+00000cf0: 6f6e da05 7072 696e 7472 0400 0000 7205  on..printr....r.
+00000d00: 0000 00da 0474 696d 65da 0566 6c6f 6174  .....time..float
+00000d10: da09 7465 726d 696e 6174 65da 0974 7261  ..terminate..tra
+00000d20: 6365 6261 636b da0a 666f 726d 6174 5f65  ceback..format_e
+00000d30: 7863 7207 0000 00da 036c 656e da06 6170  xcr......len..ap
+00000d40: 7065 6e64 290d da14 6167 6772 6567 6174  pend)...aggregat
+00000d50: 6f72 5f76 6172 6961 626c 6573 7209 0000  or_variablesr...
+00000d60: 0072 0a00 0000 720c 0000 00da 0873 7461  .r....r......sta
+00000d70: 7475 7365 73da 0a75 6e66 696e 6973 6865  tuses..unfinishe
+00000d80: 64da 0b73 7461 7475 735f 7061 7468 da0e  d..status_path..
+00000d90: 7374 6174 7573 5f6f 665f 7061 7468 720d  status_of_pathr.
+00000da0: 0000 00da 0561 6c69 7665 da01 45da 0765  .....alive..E..e
+00000db0: 6c61 7073 6564 da05 646f 6f72 73a9 0072  lapsed..doors..r
+00000dc0: 3b00 0000 fa71 2f62 696f 7465 6368 2f76  ;....q/biotech/v
+00000dd0: 656e 7565 732f 7374 6167 6573 2f62 696f  enues/stages/bio
+00000de0: 7465 6368 2f70 726f 6365 6475 7265 732f  tech/procedures/
+00000df0: 6167 6772 6567 6174 6f72 5f70 726f 6365  aggregator_proce
+00000e00: 6475 7265 2f70 726f 6365 7373 2f6d 6f76  dure/process/mov
+00000e10: 6573 2f73 7461 7475 735f 6368 6563 6b5f  es/status_check_
+00000e20: 6d6f 6e69 746f 722f 7468 655f 7068 7973  monitor/the_phys
+00000e30: 6963 616c 2e70 79da 2470 6172 7365 5f61  ical.py.$parse_a
+00000e40: 6e64 5f63 6865 636b 5f69 735f 616c 6976  nd_check_is_aliv
+00000e50: 655f 6f66 5f73 7461 7475 7365 7321 0000  e_of_statuses!..
+00000e60: 0073 6401 0000 0601 0802 0801 0c01 0402  .sd.............
+00000e70: 0401 0a01 0802 0801 0202 0204 1001 1801  ................
+00000e80: 1401 0801 0a01 0802 0480 0e02 0a01 1401  ................
+00000e90: 0880 02fe 0805 0803 0205 020c 0c02 0c01  ................
+00000ea0: 0c01 1c02 0802 0201 1001 0c01 0801 02ff  ................
+00000eb0: 0204 0202 0201 0202 0202 12f8 140b 1401  ................
+00000ec0: 1802 0480 0e03 0e01 0c01 0880 02fe 0205  ................
+00000ed0: 0206 0e02 0e01 1c02 0a02 0202 0202 0201  ................
+00000ee0: 0202 12fa 1409 0480 1002 0a01 0c01 0880  ................
+00000ef0: 02fe 0205 0208 0e02 0e01 1c02 0a02 0201  ................
+00000f00: 1001 0e01 0801 02ff 0204 0202 0201 0202  ................
+00000f10: 0202 12f8 140b 1401 1801 0202 0401 06ff  ................
+00000f20: 0480 1003 0e01 0c01 0880 02fe 0205 0212  ................
+00000f30: 0a02 0a01 0a01 1601 1201 1a01 06fa 0e0b  ................
+00000f40: 0e01 0e01 1a01 1602 1c02 0a02 0201 0401  ................
+00000f50: 06ff 0204 1001 0e01 0801 02ff 0204 0202  ................
+00000f60: 0201 0202 0202 12f8 140b 1801 0480 1004  ................
+00000f70: 0a01 0c01 0880 02fe 0206 020c 0e02 0e01  ................
+00000f80: 0e02 0e02 0203 0202 0201 0201 0202 12f9  ................
+00000f90: 140a 0480 1002 0e01 0c01 0880 02fe 0205  ................
+00000fa0: 0208 0203 0e02 0e02 0e01 0e02 1402 0480  ................
+00000fb0: 1002 0e01 0c01 0880 02fe 0806 1601 0401  ................
+00000fc0: 0201 0a01 08fe 0480 0406 723d 0000 0029  ..........r=...)
+00000fd0: 0fda 3962 696f 7465 6368 2e70 726f 6365  ..9biotech.proce
+00000fe0: 6475 7265 732e 6167 6772 6567 6174 6f72  dures.aggregator
+00000ff0: 5f70 726f 6365 6475 7265 2e70 726f 6365  _procedure.proce
+00001000: 7373 2e76 6172 6961 626c 6573 7202 0000  ss.variablesr...
+00001010: 0072 1e00 0000 7204 0000 00da 2761 6c61  .r....r.....'ala
+00001020: 726d 5f63 6865 636b 732e 676c 6f62 616c  rm_checks.global
+00001030: 5f74 696d 655f 6c69 6d69 745f 6578 6365  _time_limit_exce
+00001040: 6564 6564 7205 0000 00da 3062 696f 7465  ededr.....0biote
+00001050: 6368 2e74 6f70 6963 732e 7072 6f63 6573  ch.topics.proces
+00001060: 735f 6f6e 2e70 5f65 7870 6563 742e 7061  s_on.p_expect.pa
+00001070: 7273 655f 7265 636f 7264 7372 0600 0000  rse_recordsr....
+00001080: da1c 6269 6f74 6563 682e 746f 7069 6373  ..biotech.topics
+00001090: 2e73 686f 772e 7661 7269 6162 6c65 7207  .show.variabler.
+000010a0: 0000 0072 0800 0000 722b 0000 0072 2e00  ...r....r+...r..
+000010b0: 0000 da04 7269 6368 723d 0000 0072 3b00  ....richr=...r;.
+000010c0: 0000 723b 0000 0072 3b00 0000 723c 0000  ..r;...r;...r<..
+000010d0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000010e0: 1600 0000 0c07 0c03 0c02 0c02 0c01 0c03  ................
+000010f0: 0801 0801 0803 0205 0c04                 ..........
```

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 						
 						"occurrences": occurrences
 					}
 				
 					aggregator_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
 
 		except Exception as E:
-			print ("process non-notification exception:", traceback.format_exc ())
+			print ("process non-notification exception:", E)
 			pass;
 		
 		
 		'''
 			This checks if a started process didn't 
 			notify the aggregator within 10 seconds.
```

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py` & `biotech-1.1.4/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/on.py` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py` & `biotech-1.1.4/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/intro/on.py` & `biotech-1.1.4/venues/stages/biotech/procedures/intro/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/adventure.py` & `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/adventure.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py` & `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py` & `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/keg/__init__.py` & `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/aggregate/__init__.py` & `biotech-1.1.4/venues/stages/biotech/topics/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/alarm_parser/__init__.py` & `biotech-1.1.4/venues/stages/biotech/topics/alarm_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__init__.py` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__init__.py` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/treasury.py` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/basin/treasury.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/shares.s.HTML` & `biotech-1.1.4/venues/stages/biotech/topics/help_documentation/shares.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/implicit/proc/__init__.py` & `biotech-1.1.4/venues/stages/biotech/topics/implicit/proc/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/implicit/thread/__init__.py` & `biotech-1.1.4/venues/stages/biotech/topics/implicit/thread/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/printout/passes.py` & `biotech-1.1.4/venues/stages/biotech/topics/printout/passes.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__init__.py` & `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 18:53:11 2024 UTC, .py size: 1766 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 97bd 2266 e606 0000  o........."f....
+00000000: 6f0d 0d0a 0000 0000 fafd 2266 3206 0000  o........."f2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6401 6403 6c06 5a06 6401  m.Z...d.d.l.Z.d.
 00000070: 6403 6c09 5a09 6405 6406 8400 5a0a 6403  d.l.Z.d.d...Z.d.
@@ -69,24 +69,24 @@
 00000440: 0000 0000 0001 0000 0004 0000 0013 0000  ................
 00000450: 0073 2600 0000 6700 7d00 8800 a000 a100  .s&...g.}.......
 00000460: 7311 7c00 a001 8800 a002 a100 a101 0100  s.|.............
 00000470: 8800 a000 a100 7206 7c00 5300 a901 4e29  ......r.|.S...N)
 00000480: 03da 0565 6d70 7479 da06 6170 7065 6e64  ...empty..append
 00000490: da03 6765 7429 01da 0870 726f 6365 6564  ..get)...proceed
 000004a0: 7329 0172 0e00 0000 720a 0000 0072 0b00  s).r....r....r..
-000004b0: 0000 da0b 7061 7273 655f 7175 6575 655a  ....parse_queueZ
+000004b0: 0000 da0b 7061 7273 655f 7175 6575 6556  ....parse_queueV
 000004c0: 0000 0073 0a00 0000 0401 0801 0e01 08ff  ...s............
 000004d0: 0403 7a28 7072 6f63 6573 735f 6f6e 5f69  ..z(process_on_i
 000004e0: 6d70 6c69 6369 742e 3c6c 6f63 616c 733e  mplicit.<locals>
 000004f0: 2e70 6172 7365 5f71 7565 7565 6300 0000  .parse_queuec...
 00000500: 0000 0000 0000 0000 0000 0000 0002 0000  ................
 00000510: 0013 0000 0073 0c00 0000 8800 a000 a100  .....s..........
 00000520: 0100 6400 5300 7216 0000 0029 01da 0373  ..d.S.r....)...s
 00000530: 6574 720a 0000 0029 0172 1200 0000 720a  etr....).r....r.
-00000540: 0000 0072 0b00 0000 da05 6f66 665f 3163  ...r......off_1c
+00000540: 0000 0072 0b00 0000 da05 6f66 665f 315d  ...r......off_1]
 00000550: 0000 0073 0200 0000 0c02 7a22 7072 6f63  ...s......z"proc
 00000560: 6573 735f 6f6e 5f69 6d70 6c69 6369 742e  ess_on_implicit.
 00000570: 3c6c 6f63 616c 733e 2e6f 6666 5f31 2903  <locals>.off_1).
 00000580: 720d 0000 00da 0772 6563 6f72 6473 720c  r......recordsr.
 00000590: 0000 0029 0972 0400 0000 da0f 6d75 6c74  ...).r......mult
 000005a0: 6970 726f 6365 7373 696e 67da 0545 7665  iprocessing..Eve
 000005b0: 6e74 7203 0000 0072 0200 0000 da05 7374  ntr....r......st
@@ -96,15 +96,15 @@
 000005f0: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
 00000600: 7208 0000 0072 1b00 0000 721d 0000 0072  r....r....r....r
 00000610: 0a00 0000 2902 7212 0000 0072 0e00 0000  ....).r....r....
 00000620: 720b 0000 00da 1370 726f 6365 7373 5f6f  r......process_o
 00000630: 6e5f 696d 706c 6963 6974 3200 0000 732a  n_implicit2...s*
 00000640: 0000 0006 0908 0202 0202 0102 0302 ff02  ................
 00000650: 0502 0102 0102 0102 0204 fa06 f908 110c  ................
-00000660: 0a0c 090c 0402 0302 0102 0506 f972 2500  .............r%.
+00000660: 060c 070c 0402 0302 0102 0506 f972 2500  .............r%.
 00000670: 0000 290c da07 5f5f 646f 635f 5fda 2262  ..)...__doc__."b
 00000680: 696f 7465 6368 2e74 6f70 6963 732e 7072  iotech.topics.pr
 00000690: 6f63 6573 735f 6f6e 2e70 5f65 7870 6563  ocess_on.p_expec
 000006a0: 7472 0200 0000 da07 7065 7870 6563 74da  tr......pexpect.
 000006b0: 0472 6963 68da 026f 7372 1f00 0000 7203  .rich..osr....r.
 000006c0: 0000 0072 0400 0000 7222 0000 0072 0c00  ...r....r"...r..
 000006d0: 0000 7225 0000 0072 0a00 0000 720a 0000  ..r%...r....r...
```

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/implicit.py` & `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/implicit.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,31 +75,25 @@
 			
 			"stop_event": stop_event
 		}
 	)
 	
 	implicit_process.start ()
 	
-	# print ('the process started in the implicit')
-	
 	# if you'd like to await the process
 	# implicit_process.join ()
 	
-	#result = the_queue.get (timeout = 1)
-	#print ("Result from implicit process:", result)
 	
 	def parse_queue ():
 		proceeds = []
 		while not the_queue.empty ():
 			proceeds.append (the_queue.get ())
 	
 		return proceeds;
 	
-		#return the_queue.get (timeout = 1)
-	
 	def off_1 ():
 		nonlocal stop_event;
 		stop_event.set ()
 	
 	atexit.register (off, implicit_process)
 	
 	return {
```

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/parse_records.py` & `biotech-1.1.4/venues/stages/biotech/topics/process_on/p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/quay/garage.py` & `biotech-1.1.4/venues/stages/biotech/topics/quay/garage.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_1.py` & `biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_2.py` & `biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_2.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_3.py` & `biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_3.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_4.py` & `biotech-1.1.4/venues/stages/biotech/topics/quay/implicit_process_test_4.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py` & `biotech-1.1.4/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/show/variable.py` & `biotech-1.1.4/venues/stages/biotech/topics/show/variable.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc` & `biotech-1.1.4/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/venues/stages/biotech/topics/start--/simultaneously.py` & `biotech-1.1.4/venues/stages/biotech/topics/start--/simultaneously.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.3/PKG-INFO` & `biotech-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotech
-Version: 1.1.3
+Version: 1.1.4
 Summary: A health monitoring stack
 License: GPL-3.0-only
 Keywords: alarms,screening,monitors,cybernetics,neurons,nervous system,bioelectric,homeostasis,reliability,consistency,integrity,guarantees,vows,oaths,assurances,insurances,ensurances,speed,calmness,education,augmentation,enhancement,improvements
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

