# Comparing `tmp/biotech-1.1.2.tar.gz` & `tmp/biotech-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotech-1.1.2.tar", max compression
+gzip compressed data, was "biotech-1.1.3.tar", max compression
```

## Comparing `biotech-1.1.2.tar` & `biotech-1.1.3.tar`

### file list

```diff
@@ -1,766 +1,766 @@
--rwxr-xr-x   0        0        0      211 2024-04-16 02:07:59.993436 biotech-1.1.2/license.S.HTML
--rwxr-xr-x   0        0        0     1145 2024-04-19 22:47:27.763896 biotech-1.1.2/pyproject.toml
--rwxr-xr-x   0        0        0     3866 2024-04-16 20:53:30.034757 biotech-1.1.2/readme.md
--rwxr-xr-x   0        0        0     2331 2024-04-19 15:34:34.407444 biotech-1.1.2/venue.S.HTML
--rwxr-xr-x   0        0        0   838272 2024-04-16 02:03:26.700967 biotech-1.1.2/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
--rwxr-xr-x   0        0        0     1270 2024-04-17 22:22:59.944800 biotech-1.1.2/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
--rwxr-xr-x   0        0        0     4079 2024-04-16 20:48:34.871383 biotech-1.1.2/venues/stages/biotech/___itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0      645 2024-04-16 20:48:34.875383 biotech-1.1.2/venues/stages/biotech/___itinerary/maybes.s.HTML
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout/script.py
--rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout/start.py
--rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
--rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
--rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
--rwxr-xr-x   0        0        0      385 2024-04-17 18:49:44.656786 biotech-1.1.2/venues/stages/biotech/__glossary/biotech_1
--rwxr-xr-x   0        0        0      114 2024-04-17 18:45:06.744254 biotech-1.1.2/venues/stages/biotech/__glossary/glossary.S.HTML
--rwxr-xr-x   0        0        0      130 2024-04-19 16:49:02.311131 biotech-1.1.2/venues/stages/biotech/__init__.py
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 biotech-1.1.2/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0     1252 2024-04-16 20:48:34.867383 biotech-1.1.2/venues/stages/biotech/_book/advanced tutorial.s.HTML
--rwxr-xr-x   0        0        0     1786 2024-04-16 20:48:34.867383 biotech-1.1.2/venues/stages/biotech/_book/book.s.HTML
--rwxr-xr-x   0        0        0      542 2024-04-16 20:48:34.867383 biotech-1.1.2/venues/stages/biotech/_book/relevant.s.HTML
--rwxr-xr-x   0        0        0     2129 2024-04-17 19:24:51.191926 biotech-1.1.2/venues/stages/biotech/_clique/__init__.py
--rwxr-xr-x   0        0        0     2493 2024-04-17 19:24:52.839918 biotech-1.1.2/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 biotech-1.1.2/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 biotech-1.1.2/venues/stages/biotech/_clique/group/__init__.py
--rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 biotech-1.1.2/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 biotech-1.1.2/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0  1401783 2024-04-19 22:46:46.716354 biotech-1.1.2/venues/stages/biotech/_status/DB/records.json
--rw-r--r--   0        0        0     1172 2024-04-19 22:15:38.920875 biotech-1.1.2/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
--rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 biotech-1.1.2/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
--rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 biotech-1.1.2/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
--rwxr-xr-x   0        0        0     1487 2024-04-19 22:15:36.412903 biotech-1.1.2/venues/stages/biotech/_status/establish.py
--rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416142 biotech-1.1.2/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 biotech-1.1.2/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      720 2024-04-16 20:48:34.887383 biotech-1.1.2/venues/stages/biotech/_status/monitors/-01_start/status_1.py
--rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 biotech-1.1.2/venues/stages/biotech/_status/monitors/00_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 biotech-1.1.2/venues/stages/biotech/_status/monitors/00_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      793 2024-04-16 20:48:34.883383 biotech-1.1.2/venues/stages/biotech/_status/monitors/00_start/status_1.py
--rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708148 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/path_1_health.py
--rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/path_2_health.py
--rwxr-xr-x   0        0        0     1161 2024-04-16 20:48:34.903383 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/status_1.py
--rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/1_health.py
--rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/2_health.py
--rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/modules/MODULE_1.py
--rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1214 2024-04-16 20:48:34.899383 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/status_1.py
--rwxr-xr-x   0        0        0      794 2024-04-16 20:48:34.891383 biotech-1.1.2/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py
--rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 biotech-1.1.2/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 biotech-1.1.2/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      939 2024-04-16 20:48:34.887383 biotech-1.1.2/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py
--rwxr-xr-x   0        0        0      289 2024-04-16 00:28:17.871373 biotech-1.1.2/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      517 2024-04-16 00:32:46.948536 biotech-1.1.2/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      942 2024-04-16 20:48:34.883383 biotech-1.1.2/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py
--rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py
--rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      867 2024-04-16 20:48:34.891383 biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/status_1.py
--rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/1_health.py
--rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/2_health.py
--rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/3_health.py
--rw-r--r--   0        0        0     1036 2024-04-19 19:54:47.501752 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/1_health.cpython-310.pyc
--rw-r--r--   0        0        0      183 2024-04-19 19:54:47.501752 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/2_health.cpython-310.pyc
--rw-r--r--   0        0        0      169 2024-04-19 19:54:47.505751 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/3_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      955 2024-04-19 22:40:42.880411 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/status_1.py
--rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 biotech-1.1.2/venues/stages/biotech/_status/monitors/07/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 biotech-1.1.2/venues/stages/biotech/_status/monitors/07/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0      809 2024-04-16 20:48:34.907383 biotech-1.1.2/venues/stages/biotech/_status/monitors/07/status_1.py
--rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 biotech-1.1.2/venues/stages/biotech/_status/monitors/08_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 biotech-1.1.2/venues/stages/biotech/_status/monitors/08_DB/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0     1561 2024-04-19 19:13:07.956368 biotech-1.1.2/venues/stages/biotech/_status/monitors/08_DB/status_1.py
--rwxr-xr-x   0        0        0    93689 2024-04-19 22:46:21.516636 biotech-1.1.2/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_2.py
--rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_3.py
--rwxr-xr-x   0        0        0     1442 2024-04-19 22:43:25.306602 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py
--rwxr-xr-x   0        0        0      367 2024-04-16 03:23:58.043895 biotech-1.1.2/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 biotech-1.1.2/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1189 2024-04-19 21:55:08.998787 biotech-1.1.2/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
--rw-r--r--   0        0        0      316 2024-04-19 18:57:32.516036 biotech-1.1.2/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       77 2024-04-19 18:57:24.196146 biotech-1.1.2/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1250 2024-04-19 21:55:16.358703 biotech-1.1.2/venues/stages/biotech/_status/monitors/11/status_1.py
--rwxr-xr-x   0        0        0      984 2024-04-18 03:32:30.971629 biotech-1.1.2/venues/stages/biotech/_status/status.proc.py
--rwxr-xr-x   0        0        0      256 2024-04-16 20:48:34.875383 biotech-1.1.2/venues/stages/biotech/_status/status.s.HTML
--rwxr-xr-x   0        0        0     1483 2024-04-16 20:48:34.851384 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
--rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
--rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
--rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 biotech-1.1.2/venues/stages/biotech/_status_advanced/status.proc.py
--rwxr-xr-x   0        0        0     1779 2024-04-16 20:48:34.575388 biotech-1.1.2/venues/stages/biotech/architecture.s.HTML
--rwxr-xr-x   0        0        0      241 2024-04-16 20:53:18.546926 biotech-1.1.2/venues/stages/biotech/emojis.S.HTML
--rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 biotech-1.1.2/venues/stages/biotech/license.S.HTML
--rwxr-xr-x   0        0        0     3068 2024-04-16 20:48:34.543389 biotech-1.1.2/venues/stages/biotech/module.s.HTML
--rw-r--r--   0        0        0     1596 2024-04-19 21:12:05.931720 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      640 2024-04-19 16:26:52.595637 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      259 2024-04-19 16:20:24.028904 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
--rwxr-xr-x   0        0        0     1478 2024-04-19 21:11:18.368263 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.648116 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/paths.py
--rwxr-xr-x   0        0        0      666 2024-04-19 21:46:15.516790 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
--rwxr-xr-x   0        0        0      562 2024-04-17 21:48:05.111704 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
--rwxr-xr-x   0        0        0     1163 2024-04-17 21:49:49.362841 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2023 2024-04-19 20:54:28.011750 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
--rw-r--r--   0        0        0     2447 2024-04-19 20:54:32.867695 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      999 2024-04-19 20:57:55.937395 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0     2881 2024-04-19 21:20:39.102102 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
--rw-r--r--   0        0        0     1152 2024-04-19 21:06:40.923425 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      653 2024-04-19 20:56:23.606442 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
--rwxr-xr-x   0        0        0     3572 2024-04-19 21:20:33.674162 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
--rwxr-xr-x   0        0        0      769 2024-04-19 21:06:33.619508 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
--rwxr-xr-x   0        0        0     2031 2024-04-19 16:27:13.563375 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
--rwxr-xr-x   0        0        0     1282 2024-04-15 20:31:31.342880 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0     1916 2024-04-19 22:44:37.277799 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      418 2024-04-17 20:03:55.692458 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      687 2024-04-15 22:21:10.822989 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
--rwxr-xr-x   0        0        0     3455 2024-04-17 21:41:59.150872 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
--rw-r--r--   0        0        0      728 2024-04-19 20:59:04.160621 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
--rwxr-xr-x   0        0        0      849 2024-04-17 20:12:15.035804 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
--rwxr-xr-x   0        0        0      933 2024-04-15 23:20:20.086332 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
--rwxr-xr-x   0        0        0     3451 2024-04-19 16:26:14.724115 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
--rwxr-xr-x   0        0        0     2917 2024-04-19 22:44:35.329821 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
--rwxr-xr-x   0        0        0      193 2024-04-17 20:02:37.661229 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
--rwxr-xr-x   0        0        0      514 2024-04-19 20:59:00.568662 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
--rwxr-xr-x   0        0        0     1834 2024-04-19 18:55:07.129933 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
--rw-r--r--   0        0        0     1851 2024-04-19 18:55:11.397883 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      799 2024-04-19 16:27:13.563375 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
--rw-r--r--   0        0        0     3986 2024-04-19 22:42:08.999452 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
--rw-r--r--   0        0        0     1513 2024-04-19 20:34:02.861444 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc
--rw-r--r--   0        0        0     1478 2024-04-19 20:33:58.205499 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py
--rwxr-xr-x   0        0        0      754 2024-04-18 00:33:41.120405 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
--rw-r--r--   0        0        0     1826 2024-04-19 18:56:22.468973 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-19 18:56:27.160910 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      996 2024-04-19 16:26:14.764114 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
--rwxr-xr-x   0        0        0     9007 2024-04-19 22:42:04.947497 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
--rwxr-xr-x   0        0        0     3137 2024-04-19 22:45:07.077467 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
--rw-r--r--   0        0        0     1985 2024-04-19 22:45:12.801403 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      834 2024-04-16 20:48:34.547389 biotech-1.1.2/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
--rwxr-xr-x   0        0        0      951 2024-04-16 20:49:56.266040 biotech-1.1.2/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      609 2024-04-19 22:29:43.435688 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
--rw-r--r--   0        0        0     1904 2024-04-19 22:33:09.357432 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      500 2024-04-19 22:29:36.979758 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/dynamic_port.py
--rwxr-xr-x   0        0        0     2161 2024-04-19 22:31:07.314772 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/on.py
--rwxr-xr-x   0        0        0     2200 2024-04-19 22:24:22.967141 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
--rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
--rwxr-xr-x   0        0        0     1441 2024-04-18 02:04:22.961501 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
--rwxr-xr-x   0        0        0      774 2024-04-16 20:48:34.555389 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
--rwxr-xr-x   0        0        0     1336 2024-04-15 21:13:32.676638 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      309 2024-04-17 23:41:26.722721 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      562 2024-04-17 23:41:26.734721 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      525 2024-04-17 23:09:55.764639 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      908 2024-04-19 20:05:11.362609 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0      636 2024-04-18 01:15:59.039315 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      289 2024-04-17 23:05:28.138584 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
--rwxr-xr-x   0        0        0      803 2024-04-19 20:05:09.858629 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
--rwxr-xr-x   0        0        0      378 2024-04-18 01:13:51.928249 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
--rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
--rwxr-xr-x   0        0        0     2182 2024-04-18 01:57:52.896535 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
--rwxr-xr-x   0        0        0     2125 2024-04-18 01:58:34.052216 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1828 2024-04-19 21:04:56.668613 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0     2295 2024-04-19 21:04:32.800884 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
--rw-r--r--   0        0        0        2 2024-04-19 22:32:11.666067 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/start.py
--rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
--rwxr-xr-x   0        0        0      152 2024-04-19 16:48:50.419277 biotech-1.1.2/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4699 2024-04-19 22:17:01.343942 biotech-1.1.2/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.2/venues/stages/biotech/procedures/intro/intro.S.HTML
--rwxr-xr-x   0        0        0     6305 2024-04-19 22:16:54.188023 biotech-1.1.2/venues/stages/biotech/procedures/intro/on.py
--rw-r--r--   0        0        0     2906 2024-04-19 21:43:07.254923 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
--rw-r--r--   0        0        0     4000 2024-04-19 21:42:57.331035 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/adventure.py
--rw-r--r--   0        0        0     1330 2024-04-19 21:12:05.939720 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      905 2024-04-19 16:56:52.013564 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      959 2024-04-19 21:11:59.243796 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      614 2024-04-19 16:56:41.273688 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
--rwxr-xr-x   0        0        0      138 2024-04-19 17:33:23.717242 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/intro.proc.py
--rwxr-xr-x   0        0        0     3084 2024-04-19 21:01:52.394709 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/keg/__init__.py
--rw-r--r--   0        0        0     3068 2024-04-19 21:01:58.358642 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/variables/__init__.py
--rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321766 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      172 2024-04-16 20:48:34.551389 biotech-1.1.2/venues/stages/biotech/procedures/procedures.S.HTML
--rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 biotech-1.1.2/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
--rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 biotech-1.1.2/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
--rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 biotech-1.1.2/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 biotech-1.1.2/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 biotech-1.1.2/venues/stages/biotech/topics/aggregate/__init__.py
--rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 biotech-1.1.2/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 biotech-1.1.2/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      708 2024-04-16 20:48:34.591388 biotech-1.1.2/venues/stages/biotech/topics/alarm_parser/__init__.py
--rwxr-xr-x   0        0        0      673 2024-04-16 20:49:28.126498 biotech-1.1.2/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 biotech-1.1.2/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      405 2024-04-16 20:48:34.579388 biotech-1.1.2/venues/stages/biotech/topics/exceptions.py
--rwxr-xr-x   0        0        0     1190 2024-01-27 05:31:08.525189 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
--rwxr-xr-x   0        0        0     2446 2024-04-17 19:24:25.140060 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__init__.py
--rwxr-xr-x   0        0        0     2491 2024-04-17 19:24:52.839918 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4471 2024-02-01 06:11:56.801715 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1050 2024-04-16 06:10:03.111579 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     1920 2024-01-31 18:50:23.812071 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
--rwxr-xr-x   0        0        0       24 2024-01-26 17:38:56.558087 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
--rwxr-xr-x   0        0        0       24 2024-01-26 17:38:52.854129 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
--rwxr-xr-x   0        0        0      751 2024-04-17 19:16:04.226583 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
--rwxr-xr-x   0        0        0     1981 2024-04-17 19:25:47.591625 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__init__.py
--rwxr-xr-x   0        0        0     2283 2024-04-17 19:25:53.011595 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4019 2024-01-31 18:51:47.652157 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     3843 2024-04-17 19:25:53.099595 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
--rwxr-xr-x   0        0        0     4426 2024-01-27 06:34:32.979965 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
--rwxr-xr-x   0        0        0     3559 2024-04-17 19:25:22.227762 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/treasury.py
--rwxr-xr-x   0        0        0     1727 2024-04-17 19:15:19.882965 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/shares.s.HTML
--rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 biotech-1.1.2/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1558 2024-04-18 05:22:02.832642 biotech-1.1.2/venues/stages/biotech/topics/implicit/proc/__init__.py
--rwxr-xr-x   0        0        0     1158 2024-04-19 21:23:01.800513 biotech-1.1.2/venues/stages/biotech/topics/implicit/thread/__init__.py
--rw-r--r--   0        0        0      855 2024-04-19 21:23:28.056219 biotech-1.1.2/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       90 2024-04-17 22:51:08.968798 biotech-1.1.2/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 22:33:48.860256 biotech-1.1.2/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
--rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 biotech-1.1.2/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
--rwxr-xr-x   0        0        0      470 2024-04-17 23:02:14.419990 biotech-1.1.2/venues/stages/biotech/topics/printout/bracket.py
--rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 biotech-1.1.2/venues/stages/biotech/topics/printout/passes.py
--rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 biotech-1.1.2/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2166 2024-04-19 22:38:28.357906 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__init__.py
--rw-r--r--   0        0        0     1997 2024-04-19 22:38:43.137742 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
--rw-r--r--   0        0        0     1818 2024-04-19 18:54:33.250328 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-18 01:45:27.254200 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1766 2024-04-19 18:53:11.523281 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-18 01:48:34.504806 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-18 01:45:24.082223 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
--rwxr-xr-x   0        0        0      195 2024-04-16 22:50:54.515336 biotech-1.1.2/venues/stages/biotech/topics/process_on/process_on.S.HTML
--rwxr-xr-x   0        0        0     1470 2024-04-18 04:12:56.845888 biotech-1.1.2/venues/stages/biotech/topics/quay/garage.py
--rwxr-xr-x   0        0        0     2546 2024-04-18 04:38:41.478278 biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_1.py
--rwxr-xr-x   0        0        0     1612 2024-04-18 04:54:58.414971 biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_2.py
--rwxr-xr-x   0        0        0      551 2024-04-18 05:20:40.701113 biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_3.py
--rwxr-xr-x   0        0        0     1083 2024-04-18 05:19:11.645613 biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_4.py
--rwxr-xr-x   0        0        0     1448 2024-04-19 22:40:22.232641 biotech-1.1.2/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
--rw-r--r--   0        0        0     1464 2024-04-19 22:41:14.292061 biotech-1.1.2/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 biotech-1.1.2/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
--rw-r--r--   0        0        0      246 2024-04-19 21:18:20.963631 biotech-1.1.2/venues/stages/biotech/topics/report_formats/report_formats.S.HTML
--rw-r--r--   0        0        0     1772 2024-04-19 20:59:56.440027 biotech-1.1.2/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0      461 2024-04-17 23:59:06.614967 biotech-1.1.2/venues/stages/biotech/topics/show/show.S.HTML
--rwxr-xr-x   0        0        0     2295 2024-04-19 20:59:53.444061 biotech-1.1.2/venues/stages/biotech/topics/show/variable.py
--rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
--rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
--rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
--rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
--rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
--rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
--rwxr-xr-x   0        0        0      273 2024-04-16 20:48:34.583388 biotech-1.1.2/venues/stages/biotech/topics/start--/one.py
--rwxr-xr-x   0        0        0      406 2024-04-16 20:48:34.587388 biotech-1.1.2/venues/stages/biotech/topics/start--/sequentially.py
--rwxr-xr-x   0        0        0      532 2024-04-16 20:48:34.587388 biotech-1.1.2/venues/stages/biotech/topics/start--/simultaneously.py
--rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 biotech-1.1.2/venues/stages/biotech/topics/topics.S.HTML
--rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 biotech-1.1.2/venues/stages/biotech/variables/__init__.py
--rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0      211 2024-04-16 02:07:59.993436 biotech-1.1.3/license.S.HTML
+-rwxr-xr-x   0        0        0     1145 2024-04-19 23:11:17.385428 biotech-1.1.3/pyproject.toml
+-rwxr-xr-x   0        0        0     3866 2024-04-16 20:53:30.034757 biotech-1.1.3/readme.md
+-rwxr-xr-x   0        0        0     2331 2024-04-19 15:34:34.407444 biotech-1.1.3/venue.S.HTML
+-rwxr-xr-x   0        0        0   838272 2024-04-16 02:03:26.700967 biotech-1.1.3/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
+-rwxr-xr-x   0        0        0     1270 2024-04-17 22:22:59.944800 biotech-1.1.3/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
+-rwxr-xr-x   0        0        0     4079 2024-04-16 20:48:34.871383 biotech-1.1.3/venues/stages/biotech/___itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      645 2024-04-16 20:48:34.875383 biotech-1.1.3/venues/stages/biotech/___itinerary/maybes.s.HTML
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout/script.py
+-rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout/start.py
+-rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
+-rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
+-rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
+-rwxr-xr-x   0        0        0      385 2024-04-17 18:49:44.656786 biotech-1.1.3/venues/stages/biotech/__glossary/biotech_1
+-rwxr-xr-x   0        0        0      114 2024-04-17 18:45:06.744254 biotech-1.1.3/venues/stages/biotech/__glossary/glossary.S.HTML
+-rwxr-xr-x   0        0        0      130 2024-04-19 16:49:02.311131 biotech-1.1.3/venues/stages/biotech/__init__.py
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 biotech-1.1.3/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0     1252 2024-04-16 20:48:34.867383 biotech-1.1.3/venues/stages/biotech/_book/advanced tutorial.s.HTML
+-rwxr-xr-x   0        0        0     1786 2024-04-16 20:48:34.867383 biotech-1.1.3/venues/stages/biotech/_book/book.s.HTML
+-rwxr-xr-x   0        0        0      542 2024-04-16 20:48:34.867383 biotech-1.1.3/venues/stages/biotech/_book/relevant.s.HTML
+-rwxr-xr-x   0        0        0     2129 2024-04-17 19:24:51.191926 biotech-1.1.3/venues/stages/biotech/_clique/__init__.py
+-rwxr-xr-x   0        0        0     2493 2024-04-17 19:24:52.839918 biotech-1.1.3/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 biotech-1.1.3/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 biotech-1.1.3/venues/stages/biotech/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 biotech-1.1.3/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 biotech-1.1.3/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0  1404986 2024-04-19 23:11:01.025598 biotech-1.1.3/venues/stages/biotech/_status/DB/records.json
+-rw-r--r--   0        0        0     1172 2024-04-19 22:15:38.920875 biotech-1.1.3/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 biotech-1.1.3/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 biotech-1.1.3/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1487 2024-04-19 22:15:36.412903 biotech-1.1.3/venues/stages/biotech/_status/establish.py
+-rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416142 biotech-1.1.3/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 biotech-1.1.3/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      720 2024-04-16 20:48:34.887383 biotech-1.1.3/venues/stages/biotech/_status/monitors/-01_start/status_1.py
+-rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 biotech-1.1.3/venues/stages/biotech/_status/monitors/00_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 biotech-1.1.3/venues/stages/biotech/_status/monitors/00_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      793 2024-04-16 20:48:34.883383 biotech-1.1.3/venues/stages/biotech/_status/monitors/00_start/status_1.py
+-rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708148 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/path_1_health.py
+-rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/path_2_health.py
+-rwxr-xr-x   0        0        0     1161 2024-04-16 20:48:34.903383 biotech-1.1.3/venues/stages/biotech/_status/monitors/01/status_1.py
+-rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/1_health.py
+-rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/2_health.py
+-rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/modules/MODULE_1.py
+-rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1214 2024-04-16 20:48:34.899383 biotech-1.1.3/venues/stages/biotech/_status/monitors/02/status_1.py
+-rwxr-xr-x   0        0        0      794 2024-04-16 20:48:34.891383 biotech-1.1.3/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py
+-rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 biotech-1.1.3/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 biotech-1.1.3/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      939 2024-04-16 20:48:34.887383 biotech-1.1.3/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      289 2024-04-16 00:28:17.871373 biotech-1.1.3/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      517 2024-04-16 00:32:46.948536 biotech-1.1.3/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      942 2024-04-16 20:48:34.883383 biotech-1.1.3/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py
+-rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      867 2024-04-16 20:48:34.891383 biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/status_1.py
+-rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/1_health.py
+-rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/2_health.py
+-rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/3_health.py
+-rw-r--r--   0        0        0     1036 2024-04-19 19:54:47.501752 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/1_health.cpython-310.pyc
+-rw-r--r--   0        0        0      183 2024-04-19 19:54:47.501752 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/2_health.cpython-310.pyc
+-rw-r--r--   0        0        0      169 2024-04-19 19:54:47.505751 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/3_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      955 2024-04-19 22:40:42.880411 biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/status_1.py
+-rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 biotech-1.1.3/venues/stages/biotech/_status/monitors/07/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 biotech-1.1.3/venues/stages/biotech/_status/monitors/07/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0      809 2024-04-16 20:48:34.907383 biotech-1.1.3/venues/stages/biotech/_status/monitors/07/status_1.py
+-rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 biotech-1.1.3/venues/stages/biotech/_status/monitors/08_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 biotech-1.1.3/venues/stages/biotech/_status/monitors/08_DB/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0     1561 2024-04-19 19:13:07.956368 biotech-1.1.3/venues/stages/biotech/_status/monitors/08_DB/status_1.py
+-rwxr-xr-x   0        0        0    96037 2024-04-19 23:10:35.809859 biotech-1.1.3/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_2.py
+-rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_3.py
+-rwxr-xr-x   0        0        0     1442 2024-04-19 22:43:25.306602 biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py
+-rwxr-xr-x   0        0        0      367 2024-04-16 03:23:58.043895 biotech-1.1.3/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 biotech-1.1.3/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1189 2024-04-19 21:55:08.998787 biotech-1.1.3/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
+-rw-r--r--   0        0        0      316 2024-04-19 18:57:32.516036 biotech-1.1.3/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.3/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       77 2024-04-19 18:57:24.196146 biotech-1.1.3/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1250 2024-04-19 21:55:16.358703 biotech-1.1.3/venues/stages/biotech/_status/monitors/11/status_1.py
+-rwxr-xr-x   0        0        0      984 2024-04-18 03:32:30.971629 biotech-1.1.3/venues/stages/biotech/_status/status.proc.py
+-rwxr-xr-x   0        0        0      256 2024-04-16 20:48:34.875383 biotech-1.1.3/venues/stages/biotech/_status/status.s.HTML
+-rwxr-xr-x   0        0        0     1483 2024-04-16 20:48:34.851384 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
+-rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
+-rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 biotech-1.1.3/venues/stages/biotech/_status_advanced/status.proc.py
+-rwxr-xr-x   0        0        0     1779 2024-04-16 20:48:34.575388 biotech-1.1.3/venues/stages/biotech/architecture.s.HTML
+-rwxr-xr-x   0        0        0      241 2024-04-16 20:53:18.546926 biotech-1.1.3/venues/stages/biotech/emojis.S.HTML
+-rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 biotech-1.1.3/venues/stages/biotech/license.S.HTML
+-rwxr-xr-x   0        0        0     3068 2024-04-16 20:48:34.543389 biotech-1.1.3/venues/stages/biotech/module.s.HTML
+-rw-r--r--   0        0        0     1596 2024-04-19 21:12:05.931720 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      640 2024-04-19 16:26:52.595637 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      259 2024-04-19 16:20:24.028904 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
+-rwxr-xr-x   0        0        0     1478 2024-04-19 21:11:18.368263 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.648116 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/paths.py
+-rwxr-xr-x   0        0        0      666 2024-04-19 21:46:15.516790 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
+-rwxr-xr-x   0        0        0      562 2024-04-17 21:48:05.111704 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
+-rwxr-xr-x   0        0        0     1163 2024-04-17 21:49:49.362841 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2023 2024-04-19 20:54:28.011750 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
+-rw-r--r--   0        0        0     2447 2024-04-19 20:54:32.867695 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0      999 2024-04-19 20:57:55.937395 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0     2881 2024-04-19 21:20:39.102102 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
+-rw-r--r--   0        0        0     1152 2024-04-19 21:06:40.923425 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      653 2024-04-19 20:56:23.606442 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
+-rwxr-xr-x   0        0        0     3572 2024-04-19 21:20:33.674162 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
+-rwxr-xr-x   0        0        0      769 2024-04-19 21:06:33.619508 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
+-rwxr-xr-x   0        0        0     2031 2024-04-19 16:27:13.563375 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1282 2024-04-15 20:31:31.342880 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0     2159 2024-04-19 23:06:58.868088 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      418 2024-04-17 20:03:55.692458 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      687 2024-04-15 22:21:10.822989 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3455 2024-04-17 21:41:59.150872 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
+-rw-r--r--   0        0        0      728 2024-04-19 20:59:04.160621 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0      849 2024-04-17 20:12:15.035804 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
+-rwxr-xr-x   0        0        0      933 2024-04-15 23:20:20.086332 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3451 2024-04-19 16:26:14.724115 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
+-rwxr-xr-x   0        0        0     3235 2024-04-19 23:04:19.789690 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
+-rwxr-xr-x   0        0        0      193 2024-04-17 20:02:37.661229 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
+-rwxr-xr-x   0        0        0      514 2024-04-19 20:59:00.568662 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
+-rwxr-xr-x   0        0        0     1834 2024-04-19 18:55:07.129933 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
+-rw-r--r--   0        0        0     1851 2024-04-19 18:55:11.397883 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      799 2024-04-19 16:27:13.563375 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
+-rw-r--r--   0        0        0     4350 2024-04-19 23:06:58.868088 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
+-rw-r--r--   0        0        0     1268 2024-04-19 23:09:27.226569 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc
+-rw-r--r--   0        0        0     1489 2024-04-19 23:09:22.198620 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py
+-rwxr-xr-x   0        0        0      754 2024-04-18 00:33:41.120405 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
+-rw-r--r--   0        0        0     1826 2024-04-19 18:56:22.468973 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-19 18:56:27.160910 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      996 2024-04-19 16:26:14.764114 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
+-rwxr-xr-x   0        0        0     9847 2024-04-19 23:06:53.300145 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
+-rwxr-xr-x   0        0        0     3303 2024-04-19 23:03:08.158399 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
+-rw-r--r--   0        0        0     2018 2024-04-19 23:06:58.864088 biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      834 2024-04-16 20:48:34.547389 biotech-1.1.3/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
+-rwxr-xr-x   0        0        0      951 2024-04-16 20:49:56.266040 biotech-1.1.3/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      609 2024-04-19 22:29:43.435688 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
+-rw-r--r--   0        0        0     1904 2024-04-19 22:33:09.357432 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      500 2024-04-19 22:29:36.979758 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/dynamic_port.py
+-rwxr-xr-x   0        0        0     2161 2024-04-19 22:31:07.314772 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/on.py
+-rwxr-xr-x   0        0        0     2200 2024-04-19 22:24:22.967141 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
+-rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
+-rwxr-xr-x   0        0        0     1441 2024-04-18 02:04:22.961501 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
+-rwxr-xr-x   0        0        0      774 2024-04-16 20:48:34.555389 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
+-rwxr-xr-x   0        0        0     1336 2024-04-15 21:13:32.676638 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      309 2024-04-17 23:41:26.722721 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      562 2024-04-17 23:41:26.734721 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      525 2024-04-17 23:09:55.764639 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      908 2024-04-19 20:05:11.362609 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      636 2024-04-18 01:15:59.039315 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      289 2024-04-17 23:05:28.138584 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
+-rwxr-xr-x   0        0        0      803 2024-04-19 20:05:09.858629 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
+-rwxr-xr-x   0        0        0      378 2024-04-18 01:13:51.928249 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
+-rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
+-rwxr-xr-x   0        0        0     2182 2024-04-18 01:57:52.896535 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
+-rwxr-xr-x   0        0        0     2125 2024-04-18 01:58:34.052216 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1828 2024-04-19 21:04:56.668613 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2295 2024-04-19 21:04:32.800884 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
+-rw-r--r--   0        0        0        2 2024-04-19 22:32:11.666067 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/start.py
+-rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
+-rwxr-xr-x   0        0        0      152 2024-04-19 16:48:50.419277 biotech-1.1.3/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4699 2024-04-19 22:17:01.343942 biotech-1.1.3/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.3/venues/stages/biotech/procedures/intro/intro.S.HTML
+-rwxr-xr-x   0        0        0     6305 2024-04-19 22:16:54.188023 biotech-1.1.3/venues/stages/biotech/procedures/intro/on.py
+-rw-r--r--   0        0        0     2906 2024-04-19 21:43:07.254923 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
+-rw-r--r--   0        0        0     4000 2024-04-19 21:42:57.331035 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/adventure.py
+-rw-r--r--   0        0        0     1330 2024-04-19 21:12:05.939720 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      905 2024-04-19 16:56:52.013564 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      959 2024-04-19 21:11:59.243796 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      614 2024-04-19 16:56:41.273688 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
+-rwxr-xr-x   0        0        0      138 2024-04-19 17:33:23.717242 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/intro.proc.py
+-rwxr-xr-x   0        0        0     3084 2024-04-19 21:01:52.394709 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/keg/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-19 21:01:58.358642 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/variables/__init__.py
+-rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321766 biotech-1.1.3/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      172 2024-04-16 20:48:34.551389 biotech-1.1.3/venues/stages/biotech/procedures/procedures.S.HTML
+-rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 biotech-1.1.3/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 biotech-1.1.3/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
+-rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 biotech-1.1.3/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 biotech-1.1.3/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 biotech-1.1.3/venues/stages/biotech/topics/aggregate/__init__.py
+-rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 biotech-1.1.3/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 biotech-1.1.3/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      708 2024-04-16 20:48:34.591388 biotech-1.1.3/venues/stages/biotech/topics/alarm_parser/__init__.py
+-rwxr-xr-x   0        0        0      673 2024-04-16 20:49:28.126498 biotech-1.1.3/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 biotech-1.1.3/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      405 2024-04-16 20:48:34.579388 biotech-1.1.3/venues/stages/biotech/topics/exceptions.py
+-rwxr-xr-x   0        0        0     1190 2024-01-27 05:31:08.525189 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
+-rwxr-xr-x   0        0        0     2446 2024-04-17 19:24:25.140060 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__init__.py
+-rwxr-xr-x   0        0        0     2491 2024-04-17 19:24:52.839918 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4471 2024-02-01 06:11:56.801715 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1050 2024-04-16 06:10:03.111579 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1920 2024-01-31 18:50:23.812071 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
+-rwxr-xr-x   0        0        0       24 2024-01-26 17:38:56.558087 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
+-rwxr-xr-x   0        0        0       24 2024-01-26 17:38:52.854129 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
+-rwxr-xr-x   0        0        0      751 2024-04-17 19:16:04.226583 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
+-rwxr-xr-x   0        0        0     1981 2024-04-17 19:25:47.591625 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__init__.py
+-rwxr-xr-x   0        0        0     2283 2024-04-17 19:25:53.011595 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4019 2024-01-31 18:51:47.652157 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3843 2024-04-17 19:25:53.099595 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4426 2024-01-27 06:34:32.979965 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3559 2024-04-17 19:25:22.227762 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/treasury.py
+-rwxr-xr-x   0        0        0     1727 2024-04-17 19:15:19.882965 biotech-1.1.3/venues/stages/biotech/topics/help_documentation/shares.s.HTML
+-rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 biotech-1.1.3/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1558 2024-04-18 05:22:02.832642 biotech-1.1.3/venues/stages/biotech/topics/implicit/proc/__init__.py
+-rwxr-xr-x   0        0        0     1158 2024-04-19 21:23:01.800513 biotech-1.1.3/venues/stages/biotech/topics/implicit/thread/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-19 21:23:28.056219 biotech-1.1.3/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       90 2024-04-17 22:51:08.968798 biotech-1.1.3/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 22:33:48.860256 biotech-1.1.3/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
+-rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 biotech-1.1.3/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
+-rwxr-xr-x   0        0        0      470 2024-04-17 23:02:14.419990 biotech-1.1.3/venues/stages/biotech/topics/printout/bracket.py
+-rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 biotech-1.1.3/venues/stages/biotech/topics/printout/passes.py
+-rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 biotech-1.1.3/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2166 2024-04-19 22:38:28.357906 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__init__.py
+-rw-r--r--   0        0        0     1997 2024-04-19 22:38:43.137742 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
+-rw-r--r--   0        0        0     1818 2024-04-19 18:54:33.250328 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-18 01:45:27.254200 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1766 2024-04-19 18:53:11.523281 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-18 01:48:34.504806 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-18 01:45:24.082223 biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
+-rwxr-xr-x   0        0        0      195 2024-04-16 22:50:54.515336 biotech-1.1.3/venues/stages/biotech/topics/process_on/process_on.S.HTML
+-rwxr-xr-x   0        0        0     1470 2024-04-18 04:12:56.845888 biotech-1.1.3/venues/stages/biotech/topics/quay/garage.py
+-rwxr-xr-x   0        0        0     2546 2024-04-18 04:38:41.478278 biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_1.py
+-rwxr-xr-x   0        0        0     1612 2024-04-18 04:54:58.414971 biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_2.py
+-rwxr-xr-x   0        0        0      551 2024-04-18 05:20:40.701113 biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_3.py
+-rwxr-xr-x   0        0        0     1083 2024-04-18 05:19:11.645613 biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_4.py
+-rwxr-xr-x   0        0        0     1448 2024-04-19 22:40:22.232641 biotech-1.1.3/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
+-rw-r--r--   0        0        0     1464 2024-04-19 22:41:14.292061 biotech-1.1.3/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 biotech-1.1.3/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-19 21:18:20.963631 biotech-1.1.3/venues/stages/biotech/topics/report_formats/report_formats.S.HTML
+-rw-r--r--   0        0        0     1772 2024-04-19 20:59:56.440027 biotech-1.1.3/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0      461 2024-04-17 23:59:06.614967 biotech-1.1.3/venues/stages/biotech/topics/show/show.S.HTML
+-rwxr-xr-x   0        0        0     2295 2024-04-19 20:59:53.444061 biotech-1.1.3/venues/stages/biotech/topics/show/variable.py
+-rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
+-rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
+-rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
+-rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
+-rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
+-rwxr-xr-x   0        0        0      273 2024-04-16 20:48:34.583388 biotech-1.1.3/venues/stages/biotech/topics/start--/one.py
+-rwxr-xr-x   0        0        0      406 2024-04-16 20:48:34.587388 biotech-1.1.3/venues/stages/biotech/topics/start--/sequentially.py
+-rwxr-xr-x   0        0        0      532 2024-04-16 20:48:34.587388 biotech-1.1.3/venues/stages/biotech/topics/start--/simultaneously.py
+-rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 biotech-1.1.3/venues/stages/biotech/topics/topics.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 biotech-1.1.3/venues/stages/biotech/variables/__init__.py
+-rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.3/PKG-INFO
```

### Comparing `biotech-1.1.2/pyproject.toml` & `biotech-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 [tool.poetry]
 name = "biotech"
-version = "1.1.2"
+version = "1.1.3"
 description = "A health monitoring stack"
 authors = []
 readme = "readme.md"
 
 packages = [
     { include = "biotech", from = "venues/stages" }
 ]
```

### Comparing `biotech-1.1.2/readme.md` & `biotech-1.1.3/readme.md`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venue.S.HTML` & `biotech-1.1.3/venue.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg` & `biotech-1.1.3/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML` & `biotech-1.1.3/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/___itinerary/itinerary.S.HTML` & `biotech-1.1.3/venues/stages/biotech/___itinerary/itinerary.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/___itinerary/maybes.s.HTML` & `biotech-1.1.3/venues/stages/biotech/___itinerary/maybes.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout/start.py` & `biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout_v2/start.py` & `biotech-1.1.3/venues/stages/biotech/___itinerary/processes/errout_v2/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/__license/options/gpl-3.0-standalone.html` & `biotech-1.1.3/venues/stages/biotech/__license/options/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_book/advanced tutorial.s.HTML` & `biotech-1.1.3/venues/stages/biotech/_book/advanced tutorial.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_book/book.s.HTML` & `biotech-1.1.3/venues/stages/biotech/_book/book.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_book/relevant.s.HTML` & `biotech-1.1.3/venues/stages/biotech/_book/relevant.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_clique/__init__.py` & `biotech-1.1.3/venues/stages/biotech/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/DB/records.json` & `biotech-1.1.3/venues/stages/biotech/_status/DB/records.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987244897959184%*

 * *Differences: {"'_default'": "{'392': OrderedDict([('paths', [OrderedDict([('path', "*

 * *               "'_status/monitors/-01_start/status_1.py'), ('empty', False), ('parsed', True), "*

 * *               "('stats', OrderedDict([('passes', 1), ('alarms', 0)])), ('checks', "*

 * *               "[OrderedDict([('check', 'check 1'), ('passed', True), ('elapsed', "*

 * *               "[6.048765312996693, 'seconds'])])])]), OrderedDict([('path', "*

 * *               "'_status/monitors/00_start/status_1.py'), ('empty', False), ('parsed', True), " […]*

```diff
@@ -52260,14 +52260,293 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 14
                 },
                 "empty": 0
             }
         },
+        "392": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.048765312996693,
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
+                                6.103876150998985,
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
+                                6.1730756430006295,
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
+                                6.097779736999655,
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
+                                4.136612875998253,
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
+                                6.089650953999808,
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
+                                6.0989780700001575,
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
+                                6.1668213220000325,
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
+                                6.111853198999597,
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
+                                6.130437919000542,
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
+                                6.184211400999629,
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
+                                6.133905479000532,
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
+                                10.08989692799878,
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
+                                6.072280407999642,
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

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/establish.py` & `biotech-1.1.3/venues/stages/biotech/_status/establish.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/-01_start/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/-01_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/00_start/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/00_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_1_health.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/01/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/01/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/02/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/02/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/05__file__/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/06_various/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/07/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/07/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/08_DB/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/08_DB/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9957264957264957%*

 * *Differences: {"'_default'": "{'233': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [1.2728000001516193e-05, 'seconds']), ('passed', "*

 * *               "True)])]), ('empty', False), ('parsed', True), ('path', 'guarantee_1.py'), "*

 * *               "('records', ['proceeds None\\r\\n', 'checks in module True\\r\\n', 'check "*

 * *               '1\\r\\n\', \'{\\r\\n\', \'  "variable": {\\r\\n\', \'    "pid": 13379,\\r\\n\', '*

 * *               '\'    "proceeds": {\\r\\ […]*

```diff
@@ -5469,14 +5469,146 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 1
                 },
                 "empty": 0
             }
         },
+        "233": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.2728000001516193e-05,
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
+                        "    \"pid\": 13379,\r\n",
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
+                        "            1.2728000001516193e-05,\r\n",
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
+        "234": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.092999006388709e-06,
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
+                        "    \"pid\": 13769,\r\n",
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
+                        "            4.092999006388709e-06,\r\n",
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

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/monitors/11/status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status/monitors/11/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status/status.proc.py` & `biotech-1.1.3/venues/stages/biotech/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py` & `biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json` & `biotech-1.1.3/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/_status_advanced/status.proc.py` & `biotech-1.1.3/venues/stages/biotech/_status_advanced/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/architecture.s.HTML` & `biotech-1.1.3/venues/stages/biotech/architecture.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/module.s.HTML` & `biotech-1.1.3/venues/stages/biotech/module.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/on.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 #----
 #
 from ..variables import aggregator_variables
 from .aggregate_stats import aggregate_stats
 #
 from biotech.topics.process_on.p_expect.parse_records import parse_p_expect_records
 from biotech.topics.show.variable import show_variable
+from biotech.procedures.aggregator_procedure.process.variables import add_anomaly
 #
 #
 import rich
 #
 #
 import time
 #
@@ -58,56 +59,67 @@
 	
 	#print ('turning off scan process with pid:', the_pid)
 	#os.kill (the_pid, 9)
 	#
 	#----
 	
 
-	
+	'''
+		records
+	'''
 	try:
-		aggregator_variables ["internal_statuses"] [ the_path ] ["records"] = parse_p_expect_records (
-			records = aggregator_variables ["internal_statuses"] [ the_path ] ["process"] ["records"] (),
-			format = "UTF8"
-		)
+		try:
+			aggregator_variables ["internal_statuses"] [ the_path ] ["records"] = parse_p_expect_records (
+				records = aggregator_variables ["internal_statuses"] [ the_path ] ["process"] ["records"] (),
+				format = "UTF8"
+			)
+		except Exception:
+			add_anomaly ("The records could not be parsed!")
+		
+		
 	except Exception:
-		show_variable ("The records could not be parsed!")
+		add_anomaly ("The records could not be added to the results packet!")
+		
+	aggregator_variables ["internal_statuses"] [ the_path ] ["occurrences"] ["scan records were retrieved"] = "yes"
+	aggregator_variables ["internal_statuses"] [ the_path ] ["times"] ["records retrieval"] = str (time.time ());
+	
 	
 	
 	
 	'''
 		This sets the results packet
 	'''
 	try:
 		the_results_packet = {
 			"path": the_path
 		}
-	
+		
 		try:
 			the_results_packet ["records"] = aggregator_variables ["internal_statuses"] [ the_path ] ["records"]
 		except Exception:
-			show_variable ("The records could not be added to the results packet!")
+			add_anomaly ("The records could not be added to the result!")
 		
 		try:
 			for result in the_result:
 				the_results_packet [ result ] = the_result [ result ]
 		except Exception:
-			show_variable ("A result in the results could not be added!")
+			add_anomaly ("A result in the results could not be added!")
 			
 		try:
 			aggregator_variables ["internal_statuses"] [ the_path ] ["results_of_scan"] = the_results_packet	
 		except Exception:
-			show_variable ("The results packet could not be added.")
+			add_anomaly ("The results packet could not be added.")
+			
+		aggregator_variables ["internal_statuses"] [ the_path ] ["occurrences"] ["scan proceeds were retrieved"] = "yes"	
 			
 	except Exception:
-		show_variable ("An exception occurred while building the results.")
+		add_anomaly ("An exception occurred while building the results.")
 	
 	
 	
-	aggregator_variables ["internal_statuses"] [ the_path ] ["occurrences"] ["scan records were retrieved"] = "yes"
-	aggregator_variables ["internal_statuses"] [ the_path ] ["times"] ["records retrieval"] = str (time.time ());
 	
 	time.sleep (1)
 	
 	'''
 		This is only variable that is waited on.
 	'''
 	aggregator_variables ["internal_statuses"] [ the_path ] ["status"] ["process"] = "done"
```

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 22:42:04 2024 UTC, .py size: 9007 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3cf3 2266 2f23 0000  o.......<."f/#..
+00000000: 6f0d 0d0a 0000 0000 0df9 2266 7726 0000  o........."fw&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6405 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6400 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6408 6c0b 5a0b 6400  m.Z...d.d.l.Z.d.
@@ -14,237 +14,259 @@
 000000d0: 2901 da27 6c65 6172 6e5f 6966 5f67 6c6f  )..'learn_if_glo
 000000e0: 6261 6c5f 7469 6d65 5f6c 696d 6974 5f77  bal_time_limit_w
 000000f0: 6173 5f65 7863 6565 6465 6429 01da 1670  as_exceeded)...p
 00000100: 6172 7365 5f70 5f65 7870 6563 745f 7265  arse_p_expect_re
 00000110: 636f 7264 7329 01da 0d73 686f 775f 7661  cords)...show_va
 00000120: 7269 6162 6c65 2901 da06 7070 7269 6e74  riable)...pprint
 00000130: 4e63 0000 0000 0000 0000 0000 0000 0d00  Nc..............
-00000140: 0000 0b00 0000 4300 0000 7312 0600 0074  ......C...s....t
+00000140: 0000 0b00 0000 4300 0000 73b2 0600 0074  ......C...s....t
 00000150: 0083 007d 007c 0064 0119 007d 017c 0064  ...}.|.d...}.|.d
 00000160: 0219 007d 027c 0064 0319 0064 0419 007d  ...}.|.d...d...}
-00000170: 0369 007d 0467 007d 057c 0244 0090 025d  .i.}.g.}.|.D...]
-00000180: d17d 067c 027c 0619 007d 077c 0764 0519  .}.|.|...}.|.d..
+00000170: 0369 007d 0467 007d 057c 0244 0090 035d  .i.}.g.}.|.D...]
+00000180: 217d 067c 027c 0619 007d 077c 0764 0519  !}.|.|...}.|.d..
 00000190: 007d 0809 007a 2d64 067c 027c 0619 0064  .}...z-d.|.|...d
 000001a0: 0619 0076 0072 4f74 017c 027c 0619 0064  ...v.rOt.|.|...d
 000001b0: 0619 0064 0619 0083 0164 006b 0372 4f7c  ...d.....d.k.rO|
 000001c0: 027c 0619 0064 0619 0064 0619 00a0 02a1  .|...d...d......
 000001d0: 007d 097c 0964 076b 0272 4b64 087c 0864  .}.|.d.k.rKd.|.d
 000001e0: 093c 006e 0464 0a7c 0864 093c 0057 006e  .<.n.d.|.d.<.W.n
 000001f0: 1b04 0074 0379 6b01 007d 0a01 007a 0f74  ...t.yk..}...z.t
 00000200: 0464 0b7c 0a83 0201 0064 0c7c 0864 093c  .d.|.....d.|.d.<
 00000210: 0057 0059 0064 007d 0a7e 0a6e 0564 007d  .W.Y.d.}.~.n.d.}
 00000220: 0a7e 0a77 0177 0074 057c 0683 0101 0074  .~.w.w.t.|.....t
-00000230: 067c 0683 0101 0009 007a 6e7c 0864 0d19  .|.......zn|.d..
-00000240: 0064 086b 0272 e27c 0864 0e19 0064 0a6b  .d.k.r.|.d...d.k
-00000250: 0272 e27c 0864 0f19 0064 0a6b 0272 e274  .r.|.d...d.k.r.t
+00000230: 067c 0683 0101 0009 007a 687c 0864 0d19  .|.......zh|.d..
+00000240: 0064 086b 0272 dc7c 0864 0e19 0064 0a6b  .d.k.r.|.d...d.k
+00000250: 0272 dc7c 0864 0f19 0064 0a6b 0272 dc74  .r.|.d...d.k.r.t
 00000260: 07a0 07a1 0074 087c 027c 0619 0064 1019  .....t.|.|...d..
 00000270: 0064 1119 0083 0118 007d 0b7c 0b64 126b  .d.......}.|.d.k
-00000280: 0572 e27a 087c 027c 0619 0064 1319 007d  .r.z.|.|...d...}
+00000280: 0572 dc7a 087c 027c 0619 0064 1319 007d  .r.z.|.|...d...}
 00000290: 0857 006e 0b04 0074 0379 ad01 0001 0001  .W.n...t.y......
 000002a0: 0064 147d 0859 006e 0177 007c 0664 1567  .d.}.Y.n.w.|.d.g
 000002b0: 007c 0864 0764 169c 057c 0064 0219 007c  .|.d.d...|.d...|
 000002c0: 0619 0064 173c 0064 187c 0064 0219 007c  ...d.<.d.|.d...|
 000002d0: 0619 0064 1919 0064 063c 0064 1a7c 0064  ...d...d.<.d.|.d
 000002e0: 0219 007c 0619 0064 0519 0064 1b3c 007c  ...|...d...d.<.|
 000002f0: 0064 0219 007c 0619 0064 0619 0064 0619  .d...|...d...d..
-00000300: 00a0 09a1 0001 0074 0a64 1c7c 0669 0183  .......t.d.|.i..
-00000310: 0101 0057 006e 1904 0074 0379 fc01 007d  ...W.n...t.y...}
-00000320: 0a01 007a 0d74 0464 1d74 0ba0 0ca1 0083  ...z.t.d.t......
-00000330: 0201 0057 0059 0064 007d 0a7e 0a6e 0564  ...W.Y.d.}.~.n.d
-00000340: 007d 0a7e 0a77 0177 0009 007a 6c7c 0864  .}.~.w.w...zl|.d
-00000350: 0e19 0064 086b 0290 0172 697c 0864 0f19  ...d.k...ri|.d..
-00000360: 0064 0a6b 0290 0172 6974 07a0 07a1 0074  .d.k...rit.....t
-00000370: 087c 027c 0619 0064 1019 0064 1119 0083  .|.|...d...d....
-00000380: 0118 007d 0b7c 0b64 1e6b 0590 0172 697a  ...}.|.d.k...riz
-00000390: 087c 027c 0619 0064 1319 007d 0857 006e  .|.|...d...}.W.n
-000003a0: 0c04 0074 0390 0179 3401 0001 0001 0064  ...t...y4......d
-000003b0: 147d 0859 006e 0177 007c 0664 1f67 007c  .}.Y.n.w.|.d.g.|
-000003c0: 0864 0764 169c 057c 0064 0219 007c 0619  .d.d...|.d...|..
-000003d0: 0064 173c 0064 187c 0064 0219 007c 0619  .d.<.d.|.d...|..
-000003e0: 0064 1919 0064 063c 0064 1a7c 0064 0219  .d...d.<.d.|.d..
-000003f0: 007c 0619 0064 0519 0064 1b3c 007c 0064  .|...d...d.<.|.d
-00000400: 0219 007c 0619 0064 0619 0064 0619 00a0  ...|...d...d....
-00000410: 09a1 0001 0074 0a64 1c7c 0669 0183 0101  .....t.d.|.i....
-00000420: 0057 006e 1a04 0074 0390 0179 8401 007d  .W.n...t...y...}
-00000430: 0a01 007a 0d74 0464 1d74 0ba0 0ca1 0083  ...z.t.d.t......
-00000440: 0201 0057 0059 0064 007d 0a7e 0a6e 0564  ...W.Y.d.}.~.n.d
-00000450: 007d 0a7e 0a77 0177 0009 007a b47c 0864  .}.~.w.w...z.|.d
-00000460: 0e19 0064 086b 027c 0864 0919 0064 086b  ...d.k.|.d...d.k
-00000470: 027c 0864 2019 0064 0a6b 0274 0d7c 027c  .|.d ..d.k.t.|.|
-00000480: 0619 0064 1019 0064 1119 0083 0164 216b  ...d...d.....d!k
-00000490: 0574 0d7c 027c 0619 0064 2219 0083 0164  .t.|.|...d"....d
-000004a0: 236b 0274 07a0 07a1 0074 087c 027c 0619  #k.t.....t.|.|..
-000004b0: 0064 1019 0064 1119 0083 0118 0064 249c  .d...d.......d$.
-000004c0: 067d 0c7c 0864 0e19 0064 086b 0290 0272  .}.|.d...d.k...r
-000004d0: 397c 0864 0919 0064 086b 0290 0272 397c  9|.d...d.k...r9|
-000004e0: 0864 2019 0064 0a6b 0290 0272 3974 0d7c  .d ..d.k...r9t.|
-000004f0: 027c 0619 0064 1019 0064 1119 0083 0164  .|...d...d.....d
-00000500: 216b 0590 0272 3974 0d7c 027c 0619 0064  !k...r9t.|.|...d
-00000510: 2219 0083 0164 236b 0290 0272 3974 07a0  "....d#k...r9t..
-00000520: 07a1 0074 087c 027c 0619 0064 1019 0064  ...t.|.|...d...d
-00000530: 1119 0083 0118 007d 0b7c 0b64 256b 0590  .......}.|.d%k..
-00000540: 0272 3974 0a64 267c 0669 0183 0101 007a  .r9t.d&|.i.....z
-00000550: 087c 027c 0619 0064 1319 007d 0857 006e  .|.|...d...}.W.n
-00000560: 0c04 0074 0390 0279 1401 0001 0001 0064  ...t...y.......d
-00000570: 147d 0859 006e 0177 007c 0664 2767 007c  .}.Y.n.w.|.d'g.|
-00000580: 0864 0764 289c 057c 0064 0219 007c 0619  .d.d(..|.d...|..
-00000590: 0064 173c 0064 187c 0064 0219 007c 0619  .d.<.d.|.d...|..
-000005a0: 0064 1919 0064 063c 007c 0064 0219 007c  .d...d.<.|.d...|
-000005b0: 0619 0064 0619 0064 0619 00a0 09a1 0001  ...d...d........
-000005c0: 0057 006e 1804 0074 0390 0279 5201 007d  .W.n...t...yR..}
-000005d0: 0a01 007a 0b74 0464 297c 0a83 0201 0057  ...z.t.d)|.....W
-000005e0: 0059 0064 007d 0a7e 0a6e 0564 007d 0a7e  .Y.d.}.~.n.d.}.~
-000005f0: 0a77 0177 0009 007a 367c 0864 0e19 0064  .w.w...z6|.d...d
-00000600: 086b 0290 0272 897c 0864 0f19 0064 086b  .k...r.|.d...d.k
-00000610: 0290 0272 897c 0864 2019 0064 0a6b 0290  ...r.|.d ..d.k..
-00000620: 0272 897c 0864 0919 0064 086b 0390 0272  .r.|.d...d.k...r
-00000630: 897c 0664 2a67 007c 0864 0764 169c 057c  .|.d*g.|.d.d...|
-00000640: 0064 0219 007c 0619 0064 173c 0064 187c  .d...|...d.<.d.|
-00000650: 0064 0219 007c 0619 0064 1919 0064 063c  .d...|...d...d.<
-00000660: 0057 006e 1a04 0074 0390 0279 a401 007d  .W.n...t...y...}
-00000670: 0a01 007a 0d74 0464 2b74 0ba0 0ca1 0083  ...z.t.d+t......
-00000680: 0201 0057 0059 0064 007d 0a7e 0a6e 0564  ...W.Y.d.}.~.n.d
-00000690: 007d 0a7e 0a77 0177 0009 0009 007a 287c  .}.~.w.w.....z(|
-000006a0: 0864 0919 0064 0a6b 0290 0272 ce7c 0864  .d...d.k...r.|.d
-000006b0: 0e19 0064 086b 0290 0272 ce7c 0864 2019  ...d.k...r.|.d .
-000006c0: 0064 086b 0290 0272 ce7c 0864 2c19 0064  .d.k...r.|.d,..d
-000006d0: 086b 0290 0272 ce64 187c 0064 0219 007c  .k...r.d.|.d...|
-000006e0: 0619 0064 1919 0064 063c 0057 0071 1704  ...d...d.<.W.q..
-000006f0: 0074 0390 0279 e901 007d 0a01 007a 0d74  .t...y...}...z.t
-00000700: 0464 2b74 0ba0 0ca1 0083 0201 0057 0059  .d+t.........W.Y
-00000710: 0064 007d 0a7e 0a71 1764 007d 0a7e 0a77  .d.}.~.q.d.}.~.w
-00000720: 0177 007c 0244 005d 1a7d 067c 027c 0619  .w.|.D.].}.|.|..
-00000730: 0064 1919 0064 0619 0064 186b 0390 0372  .d...d...d.k...r
-00000740: 057c 05a0 0e7c 067c 0064 0219 007c 0619  .|...|.|.d...|..
-00000750: 0064 2d9c 02a1 0101 0090 0271 ec7c 0553  .d-........q.|.S
-00000760: 0029 2e4e da0d 7265 636f 7264 735f 6c65  .).N..records_le
-00000770: 7665 6cda 1169 6e74 6572 6e61 6c5f 7374  vel..internal_st
-00000780: 6174 7573 6573 da0f 696e 7472 6f5f 7661  atuses..intro_va
-00000790: 7269 6162 6c65 73da 0a74 696d 655f 6c69  riables..time_li
-000007a0: 6d69 74da 0b6f 6363 7572 7265 6e63 6573  mit..occurrences
-000007b0: da07 7072 6f63 6573 7354 da03 7965 737a  ..processT..yesz
-000007c0: 1573 6361 6e20 7072 6f63 6573 7320 6973  .scan process is
-000007d0: 2061 6c69 7665 da02 6e6f 7a1e 7072 6f63   alive..noz.proc
-000007e0: 6573 7320 616c 6976 6520 6368 6563 6b20  ess alive check 
-000007f0: 6578 6365 7074 696f 6e3a da07 756e 6b6e  exception:..unkn
-00000800: 6f77 6e7a 1c73 6361 6e20 7072 6f63 6573  ownz.scan proces
-00000810: 7320 7665 6e74 7572 6520 7374 6172 7465  s venture starte
-00000820: 647a 1473 6361 6e20 7072 6f63 6573 7320  dz.scan process 
-00000830: 7374 6172 7465 647a 2073 6361 6e20 7072  startedz scan pr
-00000840: 6f63 6573 7320 6e6f 7469 6669 6564 2061  ocess notified a
-00000850: 6767 7265 6761 746f 72da 0574 696d 6573  ggregator..times
-00000860: 7a0f 7665 6e74 7572 6520 7374 6172 7465  z.venture starte
-00000870: 64e9 1e00 0000 da0a 6f63 6375 7265 6e63  d.......occurenc
-00000880: 6573 7a09 6e6f 7420 666f 756e 647a 6741  esz.not foundzgA
-00000890: 6674 6572 2033 3020 7365 636f 6e64 732c  fter 30 seconds,
-000008a0: 2074 6865 2061 6674 6572 2070 726f 6365   the after proce
-000008b0: 7373 206c 696e 6520 7761 7320 6e6f 7420  ss line was not 
-000008c0: 7265 6163 6865 6420 616e 6420 7468 6520  reached and the 
-000008d0: 7072 6f63 6573 7320 6469 6420 6e6f 7420  process did not 
-000008e0: 6e6f 7469 6679 2074 6865 2061 6767 7265  notify the aggre
-000008f0: 6761 746f 722e 2905 da04 7061 7468 da05  gator.)...path..
-00000900: 616c 6172 6dfa 0b61 6c61 726d 206e 6f74  alarm..alarm not
-00000910: 6573 720d 0000 00da 0665 7869 7465 64da  esr......exited.
-00000920: 0f72 6573 756c 7473 5f6f 665f 7363 616e  .results_of_scan
-00000930: da04 646f 6e65 da06 7374 6174 7573 7a3a  ..done..statusz:
-00000940: 5468 6520 7072 6f63 6573 7320 6469 646e  The process didn
-00000950: 2774 206e 6f74 6966 7920 7468 6520 6167  't notify the ag
-00000960: 6772 6567 6174 6f72 2077 6974 6869 6e20  gregator within 
-00000970: 3520 7365 636f 6e64 732e 7a10 646f 6e65  5 seconds.z.done
-00000980: 2072 6561 736f 6e20 6769 7665 7a18 7072   reason givez.pr
-00000990: 6f63 6573 7320 6d61 7920 6861 7665 2073  ocess may have s
-000009a0: 746f 7070 6564 7a23 7072 6f63 6573 7320  toppedz#process 
-000009b0: 6e6f 6e2d 6e6f 7469 6669 6361 7469 6f6e  non-notification
-000009c0: 2065 7863 6570 7469 6f6e 3ae9 1400 0000   exception:.....
-000009d0: 7a50 4166 7465 7220 3230 2073 6563 6f6e  zPAfter 20 secon
-000009e0: 6473 2c20 7468 6520 7072 6f63 6573 7320  ds, the process 
-000009f0: 6469 6420 6e6f 7420 6e6f 7469 6679 2074  did not notify t
-00000a00: 6865 2061 6767 7265 6761 746f 7220 7468  he aggregator th
-00000a10: 6174 2069 7420 6861 6420 7374 6172 7465  at it had starte
-00000a20: 642e 7a18 7363 616e 2070 726f 6365 7373  d.z.scan process
-00000a30: 2077 6173 2073 746f 7070 6564 7203 0000   was stoppedr...
-00000a40: 00da 0772 6563 6f72 6473 7201 0000 0029  ...recordsr....)
-00000a50: 06da 0131 da01 32da 0133 da01 34da 0136  ...1..2..3..4..6
-00000a60: da01 37e9 0a00 0000 7a2b 7265 636f 7264  ..7.....z+record
-00000a70: 7320 7765 7265 206e 6f74 2072 6574 7269  s were not retri
-00000a80: 6576 6564 2061 6674 6572 2031 3020 7365  eved after 10 se
-00000a90: 636f 6e64 737a 2d41 6674 6572 2031 3020  condsz-After 10 
-00000aa0: 7365 636f 6e64 732c 206e 6f20 7072 6f63  seconds, no proc
-00000ab0: 6573 7320 6c6f 6773 2077 6572 6520 666f  ess logs were fo
-00000ac0: 756e 642e 2905 7215 0000 0072 1600 0000  und.).r....r....
-00000ad0: 7217 0000 0072 1400 0000 7218 0000 007a  r....r....r....z
-00000ae0: 2870 726f 6365 7373 206c 6f67 7320 7469  (process logs ti
-00000af0: 6d65 206c 696d 6974 2063 6865 636b 2065  me limit check e
-00000b00: 7863 6570 7469 6f6e 3a7a 3054 6865 2070  xception:z0The p
-00000b10: 726f 6365 7373 2065 7869 7465 6420 6265  rocess exited be
-00000b20: 666f 7265 2072 6573 756c 7473 2063 6f75  fore results cou
-00000b30: 6c64 2062 6520 7365 6e74 2e7a 1a70 6172  ld be sent.z.par
-00000b40: 7365 2061 6e64 2063 6865 636b 2065 7863  se and check exc
-00000b50: 6570 7469 6f6e 3a7a 1b73 6361 6e20 7265  eption:z.scan re
-00000b60: 636f 7264 7320 7765 7265 2072 6574 7269  cords were retri
-00000b70: 6576 6564 2902 7215 0000 00da 0969 6e74  eved).r......int
-00000b80: 6572 6e61 6c73 290f 7202 0000 00da 0474  ernals).r......t
-00000b90: 7970 65da 0869 735f 616c 6976 65da 0945  ype..is_alive..E
-00000ba0: 7863 6570 7469 6f6e da05 7072 696e 7472  xception..printr
-00000bb0: 0400 0000 7205 0000 00da 0474 696d 65da  ....r......time.
-00000bc0: 0566 6c6f 6174 da09 7465 726d 696e 6174  .float..terminat
-00000bd0: 6572 0700 0000 da09 7472 6163 6562 6163  er......tracebac
-00000be0: 6bda 0a66 6f72 6d61 745f 6578 63da 036c  k..format_exc..l
-00000bf0: 656e da06 6170 7065 6e64 290d da14 6167  en..append)...ag
-00000c00: 6772 6567 6174 6f72 5f76 6172 6961 626c  gregator_variabl
-00000c10: 6573 7209 0000 0072 0a00 0000 720c 0000  esr....r....r...
-00000c20: 00da 0873 7461 7475 7365 73da 0a75 6e66  ...statuses..unf
-00000c30: 696e 6973 6865 64da 0b73 7461 7475 735f  inished..status_
-00000c40: 7061 7468 da0e 7374 6174 7573 5f6f 665f  path..status_of_
-00000c50: 7061 7468 720d 0000 00da 0561 6c69 7665  pathr......alive
-00000c60: da01 45da 0765 6c61 7073 6564 da05 646f  ..E..elapsed..do
-00000c70: 6f72 73a9 0072 3a00 0000 fa71 2f62 696f  ors..r:....q/bio
-00000c80: 7465 6368 2f76 656e 7565 732f 7374 6167  tech/venues/stag
-00000c90: 6573 2f62 696f 7465 6368 2f70 726f 6365  es/biotech/proce
-00000ca0: 6475 7265 732f 6167 6772 6567 6174 6f72  dures/aggregator
-00000cb0: 5f70 726f 6365 6475 7265 2f70 726f 6365  _procedure/proce
-00000cc0: 7373 2f6d 6f76 6573 2f73 7461 7475 735f  ss/moves/status_
-00000cd0: 6368 6563 6b5f 6d6f 6e69 746f 722f 7468  check_monitor/th
-00000ce0: 655f 7068 7973 6963 616c 2e70 79da 2470  e_physical.py.$p
-00000cf0: 6172 7365 5f61 6e64 5f63 6865 636b 5f69  arse_and_check_i
-00000d00: 735f 616c 6976 655f 6f66 5f73 7461 7475  s_alive_of_statu
-00000d10: 7365 7321 0000 0073 4601 0000 0601 0802  ses!...sF.......
-00000d20: 0801 0c01 0402 0401 0a01 0802 0801 0202  ................
-00000d30: 0204 1001 1801 1401 0801 0a01 0802 0480  ................
-00000d40: 0e02 0a01 1401 0880 02fe 0805 0803 0205  ................
-00000d50: 020d 0c02 0c01 0c01 1c02 0802 0201 1001  ................
-00000d60: 0c01 0801 02ff 0204 0202 0201 0202 0202  ................
-00000d70: 12f8 140b 1401 1802 0202 0401 06ff 0480  ................
-00000d80: 0e03 0e01 0c01 0880 02fe 0205 0208 0e02  ................
-00000d90: 0e01 1c02 0a02 0201 1001 0e01 0801 02ff  ................
-00000da0: 0204 0202 0201 0202 0202 12f8 140b 1401  ................
-00000db0: 1801 0202 0401 06ff 0480 1003 0e01 0c01  ................
-00000dc0: 0880 02fe 0205 0212 0a02 0a01 0a01 1601  ................
-00000dd0: 1201 1a01 06fa 0e0b 0e01 0e01 1a01 1602  ................
-00000de0: 1c02 0a02 0201 0401 06ff 0204 1001 0e01  ................
-00000df0: 0801 02ff 0204 0202 0201 0202 0202 12f8  ................
-00000e00: 140b 1801 0480 1004 0a01 0c01 0880 02fe  ................
-00000e10: 0206 020c 0e02 0e01 0e02 0e02 0203 0202  ................
-00000e20: 0201 0201 0202 12f9 140a 0480 1002 0e01  ................
-00000e30: 0c01 0880 02fe 0205 0208 0203 0e02 0e02  ................
-00000e40: 0e01 0e02 1402 0480 1002 0e01 0c01 0880  ................
-00000e50: 02fe 0806 1601 0401 0201 0a01 08fe 0480  ................
-00000e60: 0406 723c 0000 0029 0fda 3962 696f 7465  ..r<...)..9biote
-00000e70: 6368 2e70 726f 6365 6475 7265 732e 6167  ch.procedures.ag
-00000e80: 6772 6567 6174 6f72 5f70 726f 6365 6475  gregator_procedu
-00000e90: 7265 2e70 726f 6365 7373 2e76 6172 6961  re.process.varia
-00000ea0: 626c 6573 7202 0000 0072 1d00 0000 7204  blesr....r....r.
-00000eb0: 0000 00da 2761 6c61 726d 5f63 6865 636b  ....'alarm_check
-00000ec0: 732e 676c 6f62 616c 5f74 696d 655f 6c69  s.global_time_li
-00000ed0: 6d69 745f 6578 6365 6564 6564 7205 0000  mit_exceededr...
-00000ee0: 00da 3062 696f 7465 6368 2e74 6f70 6963  ..0biotech.topic
-00000ef0: 732e 7072 6f63 6573 735f 6f6e 2e70 5f65  s.process_on.p_e
-00000f00: 7870 6563 742e 7061 7273 655f 7265 636f  xpect.parse_reco
-00000f10: 7264 7372 0600 0000 da1c 6269 6f74 6563  rdsr......biotec
-00000f20: 682e 746f 7069 6373 2e73 686f 772e 7661  h.topics.show.va
-00000f30: 7269 6162 6c65 7207 0000 0072 0800 0000  riabler....r....
-00000f40: 722a 0000 0072 2d00 0000 da04 7269 6368  r*...r-.....rich
-00000f50: 723c 0000 0072 3a00 0000 723a 0000 0072  r<...r:...r:...r
-00000f60: 3a00 0000 723b 0000 00da 083c 6d6f 6475  :...r;.....<modu
-00000f70: 6c65 3e01 0000 0073 1600 0000 0c07 0c03  le>....s........
-00000f80: 0c02 0c02 0c01 0c03 0801 0801 0803 0205  ................
-00000f90: 0c04                                     ..
+00000300: 00a0 09a1 0001 0057 006e 1904 0074 0379  .......W.n...t.y
+00000310: f601 007d 0a01 007a 0d74 0464 1c74 0aa0  ...}...z.t.d.t..
+00000320: 0ba1 0083 0201 0057 0059 0064 007d 0a7e  .......W.Y.d.}.~
+00000330: 0a6e 0564 007d 0a7e 0a77 0177 0009 007a  .n.d.}.~.w.w...z
+00000340: 3a7c 0864 1d19 0064 086b 0290 0172 317c  :|.d...d.k...r1|
+00000350: 0864 1e19 0064 0a6b 0290 0172 3174 07a0  .d...d.k...r1t..
+00000360: 07a1 0074 087c 027c 0619 0064 1019 0064  ...t.|.|...d...d
+00000370: 1119 0083 0118 007d 0b7c 0b64 1f6b 0590  .......}.|.d.k..
+00000380: 0172 317c 0664 2067 007c 0864 219c 047c  .r1|.d g.|.d!..|
+00000390: 0064 0219 007c 0619 0064 173c 0064 187c  .d...|...d.<.d.|
+000003a0: 0064 0219 007c 0619 0064 1919 0064 063c  .d...|...d...d.<
+000003b0: 0057 006e 1a04 0074 0390 0179 4c01 007d  .W.n...t...yL..}
+000003c0: 0a01 007a 0d74 0464 1c74 0aa0 0ba1 0083  ...z.t.d.t......
+000003d0: 0201 0057 0059 0064 007d 0a7e 0a6e 0564  ...W.Y.d.}.~.n.d
+000003e0: 007d 0a7e 0a77 0177 0009 007a 6c7c 0864  .}.~.w.w...zl|.d
+000003f0: 0e19 0064 086b 0290 0172 b97c 0864 0f19  ...d.k...r.|.d..
+00000400: 0064 0a6b 0290 0172 b974 07a0 07a1 0074  .d.k...r.t.....t
+00000410: 087c 027c 0619 0064 1019 0064 1119 0083  .|.|...d...d....
+00000420: 0118 007d 0b7c 0b64 226b 0590 0172 b97a  ...}.|.d"k...r.z
+00000430: 087c 027c 0619 0064 1319 007d 0857 006e  .|.|...d...}.W.n
+00000440: 0c04 0074 0390 0179 8401 0001 0001 0064  ...t...y.......d
+00000450: 147d 0859 006e 0177 007c 0664 2367 007c  .}.Y.n.w.|.d#g.|
+00000460: 0864 0764 169c 057c 0064 0219 007c 0619  .d.d...|.d...|..
+00000470: 0064 173c 0064 187c 0064 0219 007c 0619  .d.<.d.|.d...|..
+00000480: 0064 1919 0064 063c 0064 1a7c 0064 0219  .d...d.<.d.|.d..
+00000490: 007c 0619 0064 0519 0064 1b3c 007c 0064  .|...d...d.<.|.d
+000004a0: 0219 007c 0619 0064 0619 0064 0619 00a0  ...|...d...d....
+000004b0: 09a1 0001 0074 0c64 247c 0669 0183 0101  .....t.d$|.i....
+000004c0: 0057 006e 1a04 0074 0390 0179 d401 007d  .W.n...t...y...}
+000004d0: 0a01 007a 0d74 0464 1c74 0aa0 0ba1 0083  ...z.t.d.t......
+000004e0: 0201 0057 0059 0064 007d 0a7e 0a6e 0564  ...W.Y.d.}.~.n.d
+000004f0: 007d 0a7e 0a77 0177 0009 007a b47c 0864  .}.~.w.w...z.|.d
+00000500: 0e19 0064 086b 027c 0864 0919 0064 086b  ...d.k.|.d...d.k
+00000510: 027c 0864 2519 0064 0a6b 0274 0d7c 027c  .|.d%..d.k.t.|.|
+00000520: 0619 0064 1019 0064 1119 0083 0164 266b  ...d...d.....d&k
+00000530: 0574 0d7c 027c 0619 0064 2719 0083 0164  .t.|.|...d'....d
+00000540: 286b 0274 07a0 07a1 0074 087c 027c 0619  (k.t.....t.|.|..
+00000550: 0064 1019 0064 1119 0083 0118 0064 299c  .d...d.......d).
+00000560: 067d 0c7c 0864 0e19 0064 086b 0290 0272  .}.|.d...d.k...r
+00000570: 897c 0864 0919 0064 086b 0290 0272 897c  .|.d...d.k...r.|
+00000580: 0864 2519 0064 0a6b 0290 0272 8974 0d7c  .d%..d.k...r.t.|
+00000590: 027c 0619 0064 1019 0064 1119 0083 0164  .|...d...d.....d
+000005a0: 266b 0590 0272 8974 0d7c 027c 0619 0064  &k...r.t.|.|...d
+000005b0: 2719 0083 0164 286b 0290 0272 8974 07a0  '....d(k...r.t..
+000005c0: 07a1 0074 087c 027c 0619 0064 1019 0064  ...t.|.|...d...d
+000005d0: 1119 0083 0118 007d 0b7c 0b64 2a6b 0590  .......}.|.d*k..
+000005e0: 0272 8974 0c64 2b7c 0669 0183 0101 007a  .r.t.d+|.i.....z
+000005f0: 087c 027c 0619 0064 1319 007d 0857 006e  .|.|...d...}.W.n
+00000600: 0c04 0074 0390 0279 6401 0001 0001 0064  ...t...yd......d
+00000610: 147d 0859 006e 0177 007c 0664 2c67 007c  .}.Y.n.w.|.d,g.|
+00000620: 0864 0764 2d9c 057c 0064 0219 007c 0619  .d.d-..|.d...|..
+00000630: 0064 173c 0064 187c 0064 0219 007c 0619  .d.<.d.|.d...|..
+00000640: 0064 1919 0064 063c 007c 0064 0219 007c  .d...d.<.|.d...|
+00000650: 0619 0064 0619 0064 0619 00a0 09a1 0001  ...d...d........
+00000660: 0057 006e 1804 0074 0390 0279 a201 007d  .W.n...t...y...}
+00000670: 0a01 007a 0b74 0464 2e7c 0a83 0201 0057  ...z.t.d.|.....W
+00000680: 0059 0064 007d 0a7e 0a6e 0564 007d 0a7e  .Y.d.}.~.n.d.}.~
+00000690: 0a77 0177 0009 007a 367c 0864 0e19 0064  .w.w...z6|.d...d
+000006a0: 086b 0290 0272 d97c 0864 0f19 0064 086b  .k...r.|.d...d.k
+000006b0: 0290 0272 d97c 0864 2519 0064 0a6b 0290  ...r.|.d%..d.k..
+000006c0: 0272 d97c 0864 0919 0064 086b 0390 0272  .r.|.d...d.k...r
+000006d0: d97c 0664 2f67 007c 0864 0764 169c 057c  .|.d/g.|.d.d...|
+000006e0: 0064 0219 007c 0619 0064 173c 0064 187c  .d...|...d.<.d.|
+000006f0: 0064 0219 007c 0619 0064 1919 0064 063c  .d...|...d...d.<
+00000700: 0057 006e 1a04 0074 0390 0279 f401 007d  .W.n...t...y...}
+00000710: 0a01 007a 0d74 0464 3074 0aa0 0ba1 0083  ...z.t.d0t......
+00000720: 0201 0057 0059 0064 007d 0a7e 0a6e 0564  ...W.Y.d.}.~.n.d
+00000730: 007d 0a7e 0a77 0177 0009 0009 007a 287c  .}.~.w.w.....z(|
+00000740: 0864 0919 0064 0a6b 0290 0372 1e7c 0864  .d...d.k...r.|.d
+00000750: 0e19 0064 086b 0290 0372 1e7c 0864 2519  ...d.k...r.|.d%.
+00000760: 0064 086b 0290 0372 1e7c 0864 3119 0064  .d.k...r.|.d1..d
+00000770: 086b 0290 0372 1e64 187c 0064 0219 007c  .k...r.d.|.d...|
+00000780: 0619 0064 1919 0064 063c 0057 0071 1704  ...d...d.<.W.q..
+00000790: 0074 0390 0379 3901 007d 0a01 007a 0d74  .t...y9..}...z.t
+000007a0: 0464 3074 0aa0 0ba1 0083 0201 0057 0059  .d0t.........W.Y
+000007b0: 0064 007d 0a7e 0a71 1764 007d 0a7e 0a77  .d.}.~.q.d.}.~.w
+000007c0: 0177 007c 0244 005d 1a7d 067c 027c 0619  .w.|.D.].}.|.|..
+000007d0: 0064 1919 0064 0619 0064 186b 0390 0372  .d...d...d.k...r
+000007e0: 557c 05a0 0e7c 067c 0064 0219 007c 0619  U|...|.|.d...|..
+000007f0: 0064 329c 02a1 0101 0090 0371 3c7c 0553  .d2........q<|.S
+00000800: 0029 334e da0d 7265 636f 7264 735f 6c65  .)3N..records_le
+00000810: 7665 6cda 1169 6e74 6572 6e61 6c5f 7374  vel..internal_st
+00000820: 6174 7573 6573 da0f 696e 7472 6f5f 7661  atuses..intro_va
+00000830: 7269 6162 6c65 73da 0a74 696d 655f 6c69  riables..time_li
+00000840: 6d69 74da 0b6f 6363 7572 7265 6e63 6573  mit..occurrences
+00000850: da07 7072 6f63 6573 7354 da03 7965 737a  ..processT..yesz
+00000860: 1573 6361 6e20 7072 6f63 6573 7320 6973  .scan process is
+00000870: 2061 6c69 7665 da02 6e6f 7a1e 7072 6f63   alive..noz.proc
+00000880: 6573 7320 616c 6976 6520 6368 6563 6b20  ess alive check 
+00000890: 6578 6365 7074 696f 6e3a da07 756e 6b6e  exception:..unkn
+000008a0: 6f77 6e7a 1c73 6361 6e20 7072 6f63 6573  ownz.scan proces
+000008b0: 7320 7665 6e74 7572 6520 7374 6172 7465  s venture starte
+000008c0: 647a 1473 6361 6e20 7072 6f63 6573 7320  dz.scan process 
+000008d0: 7374 6172 7465 647a 2073 6361 6e20 7072  startedz scan pr
+000008e0: 6f63 6573 7320 6e6f 7469 6669 6564 2061  ocess notified a
+000008f0: 6767 7265 6761 746f 72da 0574 696d 6573  ggregator..times
+00000900: 7a0f 7665 6e74 7572 6520 7374 6172 7465  z.venture starte
+00000910: 64e9 1e00 0000 da0a 6f63 6375 7265 6e63  d.......occurenc
+00000920: 6573 7a09 6e6f 7420 666f 756e 647a 6741  esz.not foundzgA
+00000930: 6674 6572 2033 3020 7365 636f 6e64 732c  fter 30 seconds,
+00000940: 2074 6865 2061 6674 6572 2070 726f 6365   the after proce
+00000950: 7373 206c 696e 6520 7761 7320 6e6f 7420  ss line was not 
+00000960: 7265 6163 6865 6420 616e 6420 7468 6520  reached and the 
+00000970: 7072 6f63 6573 7320 6469 6420 6e6f 7420  process did not 
+00000980: 6e6f 7469 6679 2074 6865 2061 6767 7265  notify the aggre
+00000990: 6761 746f 722e 2905 da04 7061 7468 da05  gator.)...path..
+000009a0: 616c 6172 6dfa 0b61 6c61 726d 206e 6f74  alarm..alarm not
+000009b0: 6573 720d 0000 00da 0665 7869 7465 64da  esr......exited.
+000009c0: 0f72 6573 756c 7473 5f6f 665f 7363 616e  .results_of_scan
+000009d0: da04 646f 6e65 da06 7374 6174 7573 7a3a  ..done..statusz:
+000009e0: 5468 6520 7072 6f63 6573 7320 6469 646e  The process didn
+000009f0: 2774 206e 6f74 6966 7920 7468 6520 6167  't notify the ag
+00000a00: 6772 6567 6174 6f72 2077 6974 6869 6e20  gregator within 
+00000a10: 3520 7365 636f 6e64 732e 7a10 646f 6e65  5 seconds.z.done
+00000a20: 2072 6561 736f 6e20 6769 7665 7a23 7072   reason givez#pr
+00000a30: 6f63 6573 7320 6e6f 6e2d 6e6f 7469 6669  ocess non-notifi
+00000a40: 6361 7469 6f6e 2065 7863 6570 7469 6f6e  cation exception
+00000a50: 3a7a 1473 6361 6e20 7072 6f63 6573 7320  :z.scan process 
+00000a60: 7374 6f70 7065 647a 1c73 6361 6e20 7072  stoppedz.scan pr
+00000a70: 6f63 6565 6473 2077 6572 6520 7265 7472  oceeds were retr
+00000a80: 6965 7665 64e9 0f00 0000 7a5d 5468 6520  ieved.....z]The 
+00000a90: 7363 616e 2070 726f 6365 7373 2077 6173  scan process was
+00000aa0: 2073 746f 7070 6564 2c20 6275 7420 3135   stopped, but 15
+00000ab0: 2073 6563 6f6e 6473 2068 6176 6520 7061   seconds have pa
+00000ac0: 7373 6564 2061 6e64 2074 6865 2070 726f  ssed and the pro
+00000ad0: 6365 6564 7320 7765 7265 206e 6f74 2072  ceeds were not r
+00000ae0: 6574 7269 6576 6564 2e29 0472 1500 0000  etrieved.).r....
+00000af0: 7216 0000 0072 1700 0000 720d 0000 00e9  r....r....r.....
+00000b00: 1400 0000 7a50 4166 7465 7220 3230 2073  ....zPAfter 20 s
+00000b10: 6563 6f6e 6473 2c20 7468 6520 7072 6f63  econds, the proc
+00000b20: 6573 7320 6469 6420 6e6f 7420 6e6f 7469  ess did not noti
+00000b30: 6679 2074 6865 2061 6767 7265 6761 746f  fy the aggregato
+00000b40: 7220 7468 6174 2069 7420 6861 6420 7374  r that it had st
+00000b50: 6172 7465 642e 7a18 7072 6f63 6573 7320  arted.z.process 
+00000b60: 6d61 7920 6861 7665 2073 746f 7070 6564  may have stopped
+00000b70: 7a18 7363 616e 2070 726f 6365 7373 2077  z.scan process w
+00000b80: 6173 2073 746f 7070 6564 7203 0000 00da  as stoppedr.....
+00000b90: 0772 6563 6f72 6473 7201 0000 0029 06da  .recordsr....)..
+00000ba0: 0131 da01 32da 0133 da01 34da 0136 da01  .1..2..3..4..6..
+00000bb0: 37e9 0a00 0000 7a2b 7265 636f 7264 7320  7.....z+records 
+00000bc0: 7765 7265 206e 6f74 2072 6574 7269 6576  were not retriev
+00000bd0: 6564 2061 6674 6572 2031 3020 7365 636f  ed after 10 seco
+00000be0: 6e64 737a 2d41 6674 6572 2031 3020 7365  ndsz-After 10 se
+00000bf0: 636f 6e64 732c 206e 6f20 7072 6f63 6573  conds, no proces
+00000c00: 7320 6c6f 6773 2077 6572 6520 666f 756e  s logs were foun
+00000c10: 642e 2905 7215 0000 0072 1600 0000 7217  d.).r....r....r.
+00000c20: 0000 0072 1400 0000 7218 0000 007a 2870  ...r....r....z(p
+00000c30: 726f 6365 7373 206c 6f67 7320 7469 6d65  rocess logs time
+00000c40: 206c 696d 6974 2063 6865 636b 2065 7863   limit check exc
+00000c50: 6570 7469 6f6e 3a7a 3054 6865 2070 726f  eption:z0The pro
+00000c60: 6365 7373 2065 7869 7465 6420 6265 666f  cess exited befo
+00000c70: 7265 2072 6573 756c 7473 2063 6f75 6c64  re results could
+00000c80: 2062 6520 7365 6e74 2e7a 1a70 6172 7365   be sent.z.parse
+00000c90: 2061 6e64 2063 6865 636b 2065 7863 6570   and check excep
+00000ca0: 7469 6f6e 3a7a 1b73 6361 6e20 7265 636f  tion:z.scan reco
+00000cb0: 7264 7320 7765 7265 2072 6574 7269 6576  rds were retriev
+00000cc0: 6564 2902 7215 0000 00da 0969 6e74 6572  ed).r......inter
+00000cd0: 6e61 6c73 290f 7202 0000 00da 0474 7970  nals).r......typ
+00000ce0: 65da 0869 735f 616c 6976 65da 0945 7863  e..is_alive..Exc
+00000cf0: 6570 7469 6f6e da05 7072 696e 7472 0400  eption..printr..
+00000d00: 0000 7205 0000 00da 0474 696d 65da 0566  ..r......time..f
+00000d10: 6c6f 6174 da09 7465 726d 696e 6174 65da  loat..terminate.
+00000d20: 0974 7261 6365 6261 636b da0a 666f 726d  .traceback..form
+00000d30: 6174 5f65 7863 7207 0000 00da 036c 656e  at_excr......len
+00000d40: da06 6170 7065 6e64 290d da14 6167 6772  ..append)...aggr
+00000d50: 6567 6174 6f72 5f76 6172 6961 626c 6573  egator_variables
+00000d60: 7209 0000 0072 0a00 0000 720c 0000 00da  r....r....r.....
+00000d70: 0873 7461 7475 7365 73da 0a75 6e66 696e  .statuses..unfin
+00000d80: 6973 6865 64da 0b73 7461 7475 735f 7061  ished..status_pa
+00000d90: 7468 da0e 7374 6174 7573 5f6f 665f 7061  th..status_of_pa
+00000da0: 7468 720d 0000 00da 0561 6c69 7665 da01  thr......alive..
+00000db0: 45da 0765 6c61 7073 6564 da05 646f 6f72  E..elapsed..door
+00000dc0: 73a9 0072 3b00 0000 fa71 2f62 696f 7465  s..r;....q/biote
+00000dd0: 6368 2f76 656e 7565 732f 7374 6167 6573  ch/venues/stages
+00000de0: 2f62 696f 7465 6368 2f70 726f 6365 6475  /biotech/procedu
+00000df0: 7265 732f 6167 6772 6567 6174 6f72 5f70  res/aggregator_p
+00000e00: 726f 6365 6475 7265 2f70 726f 6365 7373  rocedure/process
+00000e10: 2f6d 6f76 6573 2f73 7461 7475 735f 6368  /moves/status_ch
+00000e20: 6563 6b5f 6d6f 6e69 746f 722f 7468 655f  eck_monitor/the_
+00000e30: 7068 7973 6963 616c 2e70 79da 2470 6172  physical.py.$par
+00000e40: 7365 5f61 6e64 5f63 6865 636b 5f69 735f  se_and_check_is_
+00000e50: 616c 6976 655f 6f66 5f73 7461 7475 7365  alive_of_statuse
+00000e60: 7321 0000 0073 6401 0000 0601 0802 0801  s!...sd.........
+00000e70: 0c01 0402 0401 0a01 0802 0801 0202 0204  ................
+00000e80: 1001 1801 1401 0801 0a01 0802 0480 0e02  ................
+00000e90: 0a01 1401 0880 02fe 0805 0803 0205 020c  ................
+00000ea0: 0c02 0c01 0c01 1c02 0802 0201 1001 0c01  ................
+00000eb0: 0801 02ff 0204 0202 0201 0202 0202 12f8  ................
+00000ec0: 140b 1401 1802 0480 0e03 0e01 0c01 0880  ................
+00000ed0: 02fe 0205 0206 0e02 0e01 1c02 0a02 0202  ................
+00000ee0: 0202 0201 0202 12fa 1409 0480 1002 0e01  ................
+00000ef0: 0c01 0880 02fe 0205 0208 0e02 0e01 1c02  ................
+00000f00: 0a02 0201 1001 0e01 0801 02ff 0204 0202  ................
+00000f10: 0201 0202 0202 12f8 140b 1401 1801 0202  ................
+00000f20: 0401 06ff 0480 1003 0e01 0c01 0880 02fe  ................
+00000f30: 0205 0212 0a02 0a01 0a01 1601 1201 1a01  ................
+00000f40: 06fa 0e0b 0e01 0e01 1a01 1602 1c02 0a02  ................
+00000f50: 0201 0401 06ff 0204 1001 0e01 0801 02ff  ................
+00000f60: 0204 0202 0201 0202 0202 12f8 140b 1801  ................
+00000f70: 0480 1004 0a01 0c01 0880 02fe 0206 020c  ................
+00000f80: 0e02 0e01 0e02 0e02 0203 0202 0201 0201  ................
+00000f90: 0202 12f9 140a 0480 1002 0e01 0c01 0880  ................
+00000fa0: 02fe 0205 0208 0203 0e02 0e02 0e01 0e02  ................
+00000fb0: 1402 0480 1002 0e01 0c01 0880 02fe 0806  ................
+00000fc0: 1601 0401 0201 0a01 08fe 0480 0406 723d  ..............r=
+00000fd0: 0000 0029 0fda 3962 696f 7465 6368 2e70  ...)..9biotech.p
+00000fe0: 726f 6365 6475 7265 732e 6167 6772 6567  rocedures.aggreg
+00000ff0: 6174 6f72 5f70 726f 6365 6475 7265 2e70  ator_procedure.p
+00001000: 726f 6365 7373 2e76 6172 6961 626c 6573  rocess.variables
+00001010: 7202 0000 0072 1e00 0000 7204 0000 00da  r....r....r.....
+00001020: 2761 6c61 726d 5f63 6865 636b 732e 676c  'alarm_checks.gl
+00001030: 6f62 616c 5f74 696d 655f 6c69 6d69 745f  obal_time_limit_
+00001040: 6578 6365 6564 6564 7205 0000 00da 3062  exceededr.....0b
+00001050: 696f 7465 6368 2e74 6f70 6963 732e 7072  iotech.topics.pr
+00001060: 6f63 6573 735f 6f6e 2e70 5f65 7870 6563  ocess_on.p_expec
+00001070: 742e 7061 7273 655f 7265 636f 7264 7372  t.parse_recordsr
+00001080: 0600 0000 da1c 6269 6f74 6563 682e 746f  ......biotech.to
+00001090: 7069 6373 2e73 686f 772e 7661 7269 6162  pics.show.variab
+000010a0: 6c65 7207 0000 0072 0800 0000 722b 0000  ler....r....r+..
+000010b0: 0072 2e00 0000 da04 7269 6368 723d 0000  .r......richr=..
+000010c0: 0072 3b00 0000 723b 0000 0072 3b00 0000  .r;...r;...r;...
+000010d0: 723c 0000 00da 083c 6d6f 6475 6c65 3e01  r<.....<module>.
+000010e0: 0000 0073 1600 0000 0c07 0c03 0c02 0c02  ...s............
+000010f0: 0c01 0c03 0801 0801 0803 0205 0c04       ..............
```

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 20:33:58 2024 UTC, .py size: 1478 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,80 @@
-00000000: 6f0d 0d0a 0000 0000 36d5 2266 c605 0000  o.......6."f....
+00000000: 6f0d 0d0a 0000 0000 a2f9 2266 d105 0000  o........."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6404 6c04 5a04 6405  m.Z...d.d.l.Z.d.
 00000050: 6406 8400 5a05 6404 5300 2907 e900 0000  d...Z.d.S.).....
 00000060: 0029 01da 1272 6574 7269 6576 655f 7661  .)...retrieve_va
 00000070: 7269 6162 6c65 73e9 0300 0000 2901 da13  riables.....)...
 00000080: 646f 6e65 5f77 6974 685f 7363 616e 5f6d  done_with_scan_m
 00000090: 6f76 654e 6301 0000 0000 0000 0000 0000  oveNc...........
-000000a0: 0009 0000 000d 0000 0043 0000 0073 7a01  .........C...sz.
-000000b0: 0000 7a7e 7400 8300 7d01 7c01 6401 1900  ..z~t...}.|.d...
+000000a0: 0009 0000 000d 0000 0043 0000 0073 1601  .........C...s..
+000000b0: 0000 7a4c 7400 8300 7d01 7c01 6401 1900  ..zLt...}.|.d...
 000000c0: 6402 1900 7d02 7c01 6403 1900 7d03 7c03  d...}.|.d...}.|.
-000000d0: 7c00 1900 7d04 7c04 6404 1900 7d05 7c05  |...}.|.d...}.|.
-000000e0: 6405 1900 6406 6b02 726d 7c05 6407 1900  d...d.k.rm|.d...
-000000f0: 6406 6b02 7270 7c05 6408 1900 6406 6b02  d.k.rp|.d...d.k.
-00000100: 7273 7c05 6409 1900 640a 6b02 7276 7401  rs|.d...d.k.rvt.
-00000110: 7c03 7c00 1900 640b 1900 640c 1900 8301  |.|...d...d.....
-00000120: 640d 6b05 7279 7402 a002 a100 7403 7c03  d.k.ryt.....t.|.
-00000130: 7c00 1900 640b 1900 640c 1900 8301 1800  |...d...d.......
-00000140: 7403 7c02 8301 6b05 727c 7a08 7c03 7c00  t.|...k.r|z.|.|.
-00000150: 1900 640e 1900 7d06 5700 6e0b 0400 7404  ..d...}.W.n...t.
-00000160: 795f 0100 0100 0100 640f 7d06 5900 6e01  y_......d.}.Y.n.
-00000170: 7700 7405 7c00 6410 7c06 6411 9c02 6412  w.t.|.d.|.d...d.
-00000180: 9c02 8301 0100 5700 6400 5300 5700 6400  ......W.d.S.W.d.
-00000190: 5300 5700 6400 5300 5700 6400 5300 5700  S.W.d.S.W.d.S.W.
-000001a0: 6400 5300 5700 6400 5300 5700 6400 5300  d.S.W.d.S.W.d.S.
-000001b0: 0400 7404 79bc 0100 7d07 0100 7a32 7406  ..t.y...}...z2t.
-000001c0: 6413 7407 8302 0100 7a0c 7c01 6414 1900  d.t.....z.|.d...
-000001d0: a008 6415 7c07 6416 9c02 a101 0100 5700  ..d.|.d.......W.
-000001e0: 6e12 0400 7404 79a9 0100 7d08 0100 7a06  n...t.y...}...z.
-000001f0: 5700 5900 6400 7d08 7e08 6e0c 6400 7d08  W.Y.d.}.~.n.d.}.
-00000200: 7e08 7701 7700 5700 5900 6400 7d07 7e07  ~.w.w.W.Y.d.}.~.
-00000210: 6400 5300 5700 5900 6400 7d07 7e07 6400  d.S.W.Y.d.}.~.d.
-00000220: 5300 6400 7d07 7e07 7701 7700 2917 4eda  S.d.}.~.w.w.).N.
-00000230: 0f69 6e74 726f 5f76 6172 6961 626c 6573  .intro_variables
-00000240: da0a 7469 6d65 5f6c 696d 6974 da11 696e  ..time_limit..in
-00000250: 7465 726e 616c 5f73 7461 7475 7365 73da  ternal_statuses.
-00000260: 0b6f 6363 7572 7265 6e63 6573 7a14 7363  .occurrencesz.sc
-00000270: 616e 2070 726f 6365 7373 2073 7461 7274  an process start
-00000280: 6564 da03 7965 737a 1573 6361 6e20 7072  ed..yesz.scan pr
-00000290: 6f63 6573 7320 6973 2061 6c69 7665 7a20  ocess is alivez 
-000002a0: 7363 616e 2070 726f 6365 7373 206e 6f74  scan process not
-000002b0: 6966 6965 6420 6167 6772 6567 6174 6f72  ified aggregator
-000002c0: 7a18 7363 616e 2070 726f 6365 7373 2077  z.scan process w
-000002d0: 6173 2073 746f 7070 6564 da02 6e6f da05  as stopped..no..
-000002e0: 7469 6d65 73da 0773 7461 7274 6564 e901  times..started..
-000002f0: 0000 00da 0772 6563 6f72 6473 7a09 6e6f  .....recordsz.no
-00000300: 7420 666f 756e 647a 1374 696d 6520 6c69  t foundz.time li
-00000310: 6d69 7420 6578 6365 6564 6564 2902 da05  mit exceeded)...
-00000320: 616c 6172 6d7a 0b74 6865 2072 6563 6f72  alarmz.the recor
-00000330: 6473 2902 da04 7061 7468 da06 7265 7375  ds)...path..resu
-00000340: 6c74 7a1b 7469 6d65 206c 696d 6974 2063  ltz.time limit c
-00000350: 6865 636b 2065 7863 6570 7469 6f6e 3ada  heck exception:.
-00000360: 0961 6e6f 6d61 6c69 6573 7a1a 7469 6d65  .anomaliesz.time
-00000370: 206c 696d 6974 2063 6865 636b 2065 7863   limit check exc
-00000380: 6570 7469 6f6e 2902 da07 616e 6f6d 616c  eption)...anomal
-00000390: 79da 0965 7863 6570 7469 6f6e 2909 7202  y..exception).r.
-000003a0: 0000 00da 036c 656e da04 7469 6d65 da05  .....len..time..
-000003b0: 666c 6f61 74da 0945 7863 6570 7469 6f6e  float..Exception
-000003c0: 7204 0000 00da 0570 7269 6e74 da01 45da  r......print..E.
-000003d0: 0661 7070 656e 6429 09da 0b73 7461 7475  .append)...statu
-000003e0: 735f 7061 7468 da14 6167 6772 6567 6174  s_path..aggregat
-000003f0: 6f72 5f76 6172 6961 626c 6573 7206 0000  or_variablesr...
-00000400: 0072 0700 0000 da0e 7374 6174 7573 5f6f  .r......status_o
-00000410: 665f 7061 7468 7208 0000 00da 1074 6865  f_pathr......the
-00000420: 5f73 6361 6e5f 7265 636f 7264 73da 0245  _scan_records..E
-00000430: 31da 0245 32a9 0072 2200 0000 fa8c 2f62  1..E2..r"...../b
-00000440: 696f 7465 6368 2f76 656e 7565 732f 7374  iotech/venues/st
-00000450: 6167 6573 2f62 696f 7465 6368 2f70 726f  ages/biotech/pro
-00000460: 6365 6475 7265 732f 6167 6772 6567 6174  cedures/aggregat
-00000470: 6f72 5f70 726f 6365 6475 7265 2f70 726f  or_procedure/pro
-00000480: 6365 7373 2f6d 6f76 6573 2f73 7461 7475  cess/moves/statu
-00000490: 735f 6368 6563 6b5f 6d6f 6e69 746f 722f  s_check_monitor/
-000004a0: 616c 6172 6d5f 6368 6563 6b73 2f67 6c6f  alarm_checks/glo
-000004b0: 6261 6c5f 7469 6d65 5f6c 696d 6974 5f65  bal_time_limit_e
-000004c0: 7863 6565 6465 642e 7079 da27 6c65 6172  xceeded.py.'lear
-000004d0: 6e5f 6966 5f67 6c6f 6261 6c5f 7469 6d65  n_if_global_time
-000004e0: 5f6c 696d 6974 5f77 6173 5f65 7863 6565  _limit_was_excee
-000004f0: 6465 6408 0000 0073 5800 0000 0201 0601  ded....sX.......
-00000500: 0c01 0801 0802 0801 0c03 0c01 0c01 0c01  ................
-00000510: 1801 2402 0202 1001 0c01 0801 02ff 0203  ..$.............
-00000520: 0201 0202 0201 04fe 0efe 06f3 0601 0601  ................
-00000530: 0601 0601 0602 0e0f 0a01 0202 0801 0201  ................
-00000540: 0201 0cfe 0e04 0c01 0880 02ff 0efc 0e05  ................
-00000550: 0880 02f7 7224 0000 0029 06da 3962 696f  ....r$...)..9bio
-00000560: 7465 6368 2e70 726f 6365 6475 7265 732e  tech.procedures.
-00000570: 6167 6772 6567 6174 6f72 5f70 726f 6365  aggregator_proce
-00000580: 6475 7265 2e70 726f 6365 7373 2e76 6172  dure.process.var
-00000590: 6961 626c 6573 7202 0000 00da 0e64 6f6e  iablesr......don
-000005a0: 655f 7769 7468 5f73 6361 6e72 0400 0000  e_with_scanr....
-000005b0: 7216 0000 0072 2400 0000 7222 0000 0072  r....r$...r"...r
-000005c0: 2200 0000 7222 0000 0072 2300 0000 da08  "...r"...r#.....
-000005d0: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
-000005e0: 000c 020c 0108 020c 02                   .........
+000000d0: 7c00 1900 7d04 7c04 6404 1900 7d05 0900  |...}.|.d...}...
+000000e0: 7401 a001 a100 7402 7c03 7c00 1900 6405  t.....t.|.|...d.
+000000f0: 1900 6406 1900 8301 1800 7402 7c02 8301  ..d.......t.|...
+00000100: 6b05 724a 7a08 7c03 7c00 1900 6407 1900  k.rJz.|.|...d...
+00000110: 7d06 5700 6e0b 0400 7403 793c 0100 0100  }.W.n...t.y<....
+00000120: 0100 6408 7d06 5900 6e01 7700 7404 7c00  ..d.}.Y.n.w.t.|.
+00000130: 6409 7c06 640a 9c02 640b 9c02 8301 0100  d.|.d...d.......
+00000140: 5700 6400 5300 5700 6400 5300 0400 7403  W.d.S.W.d.S...t.
+00000150: 798a 0100 7d07 0100 7a32 7405 640c 7c07  y...}...z2t.d.|.
+00000160: 8302 0100 7a0c 7c01 640d 1900 a006 640e  ....z.|.d.....d.
+00000170: 7c07 640f 9c02 a101 0100 5700 6e12 0400  |.d.......W.n...
+00000180: 7403 7977 0100 7d08 0100 7a06 5700 5900  t.yw..}...z.W.Y.
+00000190: 6400 7d08 7e08 6e0c 6400 7d08 7e08 7701  d.}.~.n.d.}.~.w.
+000001a0: 7700 5700 5900 6400 7d07 7e07 6400 5300  w.W.Y.d.}.~.d.S.
+000001b0: 5700 5900 6400 7d07 7e07 6400 5300 6400  W.Y.d.}.~.d.S.d.
+000001c0: 7d07 7e07 7701 7700 2910 4eda 0f69 6e74  }.~.w.w.).N..int
+000001d0: 726f 5f76 6172 6961 626c 6573 da0a 7469  ro_variables..ti
+000001e0: 6d65 5f6c 696d 6974 da11 696e 7465 726e  me_limit..intern
+000001f0: 616c 5f73 7461 7475 7365 73da 0b6f 6363  al_statuses..occ
+00000200: 7572 7265 6e63 6573 da05 7469 6d65 73da  urrences..times.
+00000210: 0773 7461 7274 6564 da07 7265 636f 7264  .started..record
+00000220: 737a 096e 6f74 2066 6f75 6e64 7a13 7469  sz.not foundz.ti
+00000230: 6d65 206c 696d 6974 2065 7863 6565 6465  me limit exceede
+00000240: 6429 02da 0561 6c61 726d 7a0b 7468 6520  d)...alarmz.the 
+00000250: 7265 636f 7264 7329 02da 0470 6174 68da  records)...path.
+00000260: 0672 6573 756c 747a 1b74 696d 6520 6c69  .resultz.time li
+00000270: 6d69 7420 6368 6563 6b20 6578 6365 7074  mit check except
+00000280: 696f 6e3a da09 616e 6f6d 616c 6965 737a  ion:..anomaliesz
+00000290: 1a74 696d 6520 6c69 6d69 7420 6368 6563  .time limit chec
+000002a0: 6b20 6578 6365 7074 696f 6e29 02da 0761  k exception)...a
+000002b0: 6e6f 6d61 6c79 da09 6578 6365 7074 696f  nomaly..exceptio
+000002c0: 6e29 0772 0200 0000 da04 7469 6d65 da05  n).r......time..
+000002d0: 666c 6f61 74da 0945 7863 6570 7469 6f6e  float..Exception
+000002e0: 7204 0000 00da 0570 7269 6e74 da06 6170  r......print..ap
+000002f0: 7065 6e64 2909 da0b 7374 6174 7573 5f70  pend)...status_p
+00000300: 6174 68da 1461 6767 7265 6761 746f 725f  ath..aggregator_
+00000310: 7661 7269 6162 6c65 7372 0600 0000 7207  variablesr....r.
+00000320: 0000 00da 0e73 7461 7475 735f 6f66 5f70  .....status_of_p
+00000330: 6174 6872 0800 0000 da10 7468 655f 7363  athr......the_sc
+00000340: 616e 5f72 6563 6f72 6473 da02 4531 da02  an_records..E1..
+00000350: 4532 a900 721d 0000 00fa 8c2f 6269 6f74  E2..r....../biot
+00000360: 6563 682f 7665 6e75 6573 2f73 7461 6765  ech/venues/stage
+00000370: 732f 6269 6f74 6563 682f 7072 6f63 6564  s/biotech/proced
+00000380: 7572 6573 2f61 6767 7265 6761 746f 725f  ures/aggregator_
+00000390: 7072 6f63 6564 7572 652f 7072 6f63 6573  procedure/proces
+000003a0: 732f 6d6f 7665 732f 7374 6174 7573 5f63  s/moves/status_c
+000003b0: 6865 636b 5f6d 6f6e 6974 6f72 2f61 6c61  heck_monitor/ala
+000003c0: 726d 5f63 6865 636b 732f 676c 6f62 616c  rm_checks/global
+000003d0: 5f74 696d 655f 6c69 6d69 745f 6578 6365  _time_limit_exce
+000003e0: 6564 6564 2e70 79da 276c 6561 726e 5f69  eded.py.'learn_i
+000003f0: 665f 676c 6f62 616c 5f74 696d 655f 6c69  f_global_time_li
+00000400: 6d69 745f 7761 735f 6578 6365 6564 6564  mit_was_exceeded
+00000410: 0800 0000 7346 0000 0002 0106 010c 0108  ....sF..........
+00000420: 0108 0208 0102 0224 0a02 0210 010c 0108  .......$........
+00000430: 0102 ff02 0302 0102 0202 0104 fe0e fe06  ................
+00000440: f90e 0f0a 0102 0208 0102 0102 010c fe0e  ................
+00000450: 040c 0108 8002 ff0e fc0e 0508 8002 f772  ...............r
+00000460: 1f00 0000 2906 da39 6269 6f74 6563 682e  ....)..9biotech.
+00000470: 7072 6f63 6564 7572 6573 2e61 6767 7265  procedures.aggre
+00000480: 6761 746f 725f 7072 6f63 6564 7572 652e  gator_procedure.
+00000490: 7072 6f63 6573 732e 7661 7269 6162 6c65  process.variable
+000004a0: 7372 0200 0000 da0e 646f 6e65 5f77 6974  sr......done_wit
+000004b0: 685f 7363 616e 7204 0000 0072 1200 0000  h_scanr....r....
+000004c0: 721f 0000 0072 1d00 0000 721d 0000 0072  r....r....r....r
+000004d0: 1d00 0000 721e 0000 00da 083c 6d6f 6475  ....r......<modu
+000004e0: 6c65 3e01 0000 0073 0800 0000 0c02 0c01  le>....s........
+000004f0: 0802 0c02                                ....
```

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,41 +10,47 @@
 		aggregator_variables = retrieve_variables ()
 		time_limit = aggregator_variables ["intro_variables"] ["time_limit"]
 		internal_statuses = aggregator_variables ["internal_statuses"]
 		
 		status_of_path = internal_statuses [ status_path ]
 		occurrences = status_of_path ["occurrences"]
 	
+		'''
 		if (
 			occurrences ["scan process started"] == "yes" and
 			occurrences ["scan process is alive"] == "yes" and
 			occurrences ["scan process notified aggregator"] == "yes" and
 			occurrences ["scan process was stopped"] == "no" and
 			len (internal_statuses [ status_path ] ["times"] ["started"]) >= 1
-		):			
-			if (time.time () - float (internal_statuses [ status_path ] ["times"] ["started"]) >= float (time_limit)):	
-			
-				try:
-					the_scan_records = internal_statuses [ status_path ] ["records"]
-				except Exception:
-					the_scan_records = "not found"
-			
-				done_with_scan_move ({
-					"path": status_path,
-					"result":{
-						"alarm": "time limit exceeded",
-						"the records": the_scan_records
-					}
-				})
+		):	
+		'''
+		
+		if (time.time () - float (internal_statuses [ status_path ] ["times"] ["started"]) >= float (time_limit)):	
+		
+			try:
+				the_scan_records = internal_statuses [ status_path ] ["records"]
+			except Exception:
+				the_scan_records = "not found"
+		
+			done_with_scan_move ({
+				"path": status_path,
+				"result":{
+					"alarm": "time limit exceeded",
+					"the records": the_scan_records
+				}
+			})
 					
 	except Exception as E1:
-		print ("time limit check exception:", E)
+		print ("time limit check exception:", E1)
 	
 		try:
 			aggregator_variables ["anomalies"].append ({
 				"anomaly": "time limit check exception",
 				"exception": E1
 			})
 		except Exception as E2:
 			pass;
+			
+			
+
```

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 		
 			The before process line was reached:
 				scan process venture started == "yes"
 			
 			The after process line was not reached:
 				scan process venture started == "no"
 		
-			
 			30 seconds elapsed
 		'''
 		try:
 			if (
 				occurrences ["scan process venture started"] == "yes" and
 				occurrences ["scan process started"] == "no" and
 				occurrences ["scan process notified aggregator"] == "no"
@@ -109,23 +108,51 @@
 					}
 				
 					aggregator_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
 					aggregator_variables ["internal_statuses"] [ status_path ] ["occurrences"] ["done reason give"] = "The process didn't notify the aggregator within 5 seconds."
 					
 					aggregator_variables ["internal_statuses"] [ status_path ] ["process"] ["process"].terminate ()
 					
-					show_variable ({
-						"process may have stopped": status_path
-					})
+
 		except Exception as E:
 			print ("process non-notification exception:", traceback.format_exc ())
 			pass;
 			
 		
 		'''
+			objective:
+				The scan process was stopped, 
+				but 10 seconds have passed
+				and the proceeds were not retrieved.
+		'''
+		try:
+			if (
+				occurrences ["scan process stopped"] == "yes" and
+				occurrences ["scan proceeds were retrieved"] == "no"
+			):
+				elapsed = time.time () - float (internal_statuses [ status_path ] ["times"] ["venture started"]);
+				
+				if (elapsed >= 15):	
+					aggregator_variables ["internal_statuses"] [ status_path ] ["results_of_scan"] = {
+						"path": status_path,
+						
+						"alarm": "The scan process was stopped, but 15 seconds have passed and the proceeds were not retrieved.",
+						"alarm notes": [],
+						
+						"occurrences": occurrences
+					}
+				
+					aggregator_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
+
+		except Exception as E:
+			print ("process non-notification exception:", traceback.format_exc ())
+			pass;
+		
+		
+		'''
 			This checks if a started process didn't 
 			notify the aggregator within 10 seconds.
 		
 				scan process started == "yes"
 				scan process notified aggregator == "no"
 				10 seconds elapsed
 		'''
```

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 
 
 '''
 	from biotech.procedures.aggregator_procedure.process.variables import retrieve_aggregator_variables
 '''
 
+'''
+	from biotech.procedures.aggregator_procedure.process.variables import add_anomaly
+	add_anomaly ()
+'''
+
 from biotech.procedures.aggregator_procedure.process.moves.format_path import format_path
 
 
 '''
 	paths_statuses = [{
 		"path": path,
 		** scan_status
@@ -60,14 +65,19 @@
 }
 
 def add_anomaly (anomaly):
 	try:
 		is_JSON = json.dumps (anomaly)
 	
 		aggregator_variables.append (anomaly)
+		
+		show_variable ({
+			"anomaly": anomaly
+		})
+		
 	except Exception:
 		show_variable ("An anomaly couldn't be added.")
 
 def setup_internal_statuses (
 	status_check_paths,
 	relative_path
 ):
@@ -116,15 +126,15 @@
 				
 				#
 				#	This indicates if the aggregator received 
 				#	proceeds from the health scan process (by HTTP).
 				#
 				#		options: [ "yes", "no" ]
 				#
-				"scan returned proceeds": "no",
+				"scan proceeds were retrieved": "no",
 				
 				#
 				#	This indicates if the aggregator 
 				#	retrieved the "records" from the
 				#	health scan process (by pexpect).
 				#
 				"scan records were retrieved": "no",
```

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 22:45:07 2024 UTC, .py size: 3137 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,125 +1,127 @@
-00000000: 6f0d 0d0a 0000 0000 f3f3 2266 410c 0000  o........."fA...
+00000000: 6f0d 0d0a 0000 0000 2cf8 2266 e70c 0000  o.......,."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
-00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 0900  Z.d.d.l.m.Z.....
-00000040: 0900 6403 6404 6405 9c02 6406 6900 6407  ..d.d.d...d.i.d.
-00000050: 6900 6408 6700 6409 9c07 5a03 640a 640b  i.d.g.d...Z.d.d.
-00000060: 8400 5a04 640c 640d 8400 5a05 640e 640f  ..Z.d.d...Z.d.d.
-00000070: 8400 5a06 6410 6411 8400 5a07 6412 6413  ..Z.d.d...Z.d.d.
-00000080: 8400 5a08 6414 6415 8400 5a09 6416 5300  ..Z.d.d...Z.d.S.
-00000090: 2917 7a66 0a09 6672 6f6d 2062 696f 7465  ).zf..from biote
-000000a0: 6368 2e70 726f 6365 6475 7265 732e 6167  ch.procedures.ag
-000000b0: 6772 6567 6174 6f72 5f70 726f 6365 6475  gregator_procedu
-000000c0: 7265 2e70 726f 6365 7373 2e76 6172 6961  re.process.varia
-000000d0: 626c 6573 2069 6d70 6f72 7420 7265 7472  bles import retr
-000000e0: 6965 7665 5f61 6767 7265 6761 746f 725f  ieve_aggregator_
-000000f0: 7661 7269 6162 6c65 730a e900 0000 0029  variables......)
-00000100: 01da 0b66 6f72 6d61 745f 7061 7468 7a07  ...format_pathz.
-00000110: 302e 302e 302e 30da 0029 02da 0468 6f73  0.0.0.0..)...hos
-00000120: 74da 0470 6f72 74e9 0300 0000 e902 0000  t..port.........
-00000130: 00da 026e 6f29 07da 0c69 6e74 726f 5f68  ...no)...intro_h
-00000140: 6172 626f 72da 0d72 6563 6f72 6473 5f6c  arbor..records_l
-00000150: 6576 656c da0f 696e 7472 6f5f 7661 7269  evel..intro_vari
-00000160: 6162 6c65 73da 0764 6574 6169 6c73 da11  ables..details..
-00000170: 696e 7465 726e 616c 5f73 7461 7475 7365  internal_statuse
-00000180: 73da 1769 6e74 6572 6e61 6c5f 7374 6174  s..internal_stat
-00000190: 7573 6573 5f62 7569 6c74 da09 616e 6f6d  uses_built..anom
-000001a0: 616c 6965 7363 0100 0000 0000 0000 0000  aliesc..........
-000001b0: 0000 0200 0000 0800 0000 4300 0000 7338  ..........C...s8
-000001c0: 0000 007a 0d74 00a0 017c 00a1 017d 0174  ...z.t...|...}.t
-000001d0: 02a0 037c 00a1 0101 0057 0064 0053 0004  ...|.....W.d.S..
-000001e0: 0074 0479 1b01 0001 0001 0074 0564 0183  .t.y.......t.d..
-000001f0: 0101 0059 0064 0053 0077 0029 024e 7a1d  ...Y.d.S.w.).Nz.
-00000200: 416e 2061 6e6f 6d61 6c79 2063 6f75 6c64  An anomaly could
-00000210: 6e27 7420 6265 2061 6464 6564 2e29 06da  n't be added.)..
-00000220: 046a 736f 6eda 0564 756d 7073 da14 6167  .json..dumps..ag
-00000230: 6772 6567 6174 6f72 5f76 6172 6961 626c  gregator_variabl
-00000240: 6573 da06 6170 7065 6e64 da09 4578 6365  es..append..Exce
-00000250: 7074 696f 6eda 0d73 686f 775f 7661 7269  ption..show_vari
-00000260: 6162 6c65 2902 da07 616e 6f6d 616c 79da  able)...anomaly.
-00000270: 0769 735f 4a53 4f4e a900 7218 0000 00fa  .is_JSON..r.....
-00000280: 5c2f 6269 6f74 6563 682f 7665 6e75 6573  \/biotech/venues
-00000290: 2f73 7461 6765 732f 6269 6f74 6563 682f  /stages/biotech/
-000002a0: 7072 6f63 6564 7572 6573 2f61 6767 7265  procedures/aggre
-000002b0: 6761 746f 725f 7072 6f63 6564 7572 652f  gator_procedure/
-000002c0: 7072 6f63 6573 732f 7661 7269 6162 6c65  process/variable
-000002d0: 732f 5f5f 696e 6974 5f5f 2e70 79da 0b61  s/__init__.py..a
-000002e0: 6464 5f61 6e6f 6d61 6c79 3e00 0000 730c  dd_anomaly>...s.
-000002f0: 0000 0002 010a 0110 020c 010e 0102 ff72  ...............r
-00000300: 1a00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000310: 0003 0000 000a 0000 0043 0000 0073 4e00  .........C...sN.
-00000320: 0000 7c00 4400 5d22 7d02 6401 6401 6401  ..|.D.]"}.d.d.d.
-00000330: 6401 6402 6401 6401 6403 6404 9c08 6405  d.d.d.d.d.d...d.
-00000340: 6406 6901 6403 6403 6403 6403 6407 9c04  d.i.d.d.d.d.d...
-00000350: 6700 6400 6400 6408 9c06 7400 6409 1900  g.d.d.d...t.d...
-00000360: 7401 7c02 7c01 8302 3c00 7102 6400 5300  t.|.|...<.q.d.S.
-00000370: 290a 4e72 0800 0000 da07 756e 6b6e 6f77  ).Nr......unknow
-00000380: 6e72 0300 0000 2908 7a1c 7363 616e 2070  nr....).z.scan p
-00000390: 726f 6365 7373 2076 656e 7475 7265 2073  rocess venture s
-000003a0: 7461 7274 6564 7a14 7363 616e 2070 726f  tartedz.scan pro
-000003b0: 6365 7373 2073 7461 7274 6564 7a20 7363  cess startedz sc
-000003c0: 616e 2070 726f 6365 7373 206e 6f74 6966  an process notif
-000003d0: 6965 6420 6167 6772 6567 6174 6f72 7a18  ied aggregatorz.
-000003e0: 7363 616e 2070 726f 6365 7373 2077 6173  scan process was
-000003f0: 2073 746f 7070 6564 7a15 7363 616e 2070   stoppedz.scan p
-00000400: 726f 6365 7373 2069 7320 616c 6976 657a  rocess is alivez
-00000410: 1673 6361 6e20 7265 7475 726e 6564 2070  .scan returned p
-00000420: 726f 6365 6564 737a 1b73 6361 6e20 7265  roceedsz.scan re
-00000430: 636f 7264 7320 7765 7265 2072 6574 7269  cords were retri
-00000440: 6576 6564 7a10 646f 6e65 2072 6561 736f  evedz.done reaso
-00000450: 6e20 6769 7665 da07 7072 6f63 6573 73da  n give..process.
-00000460: 0770 656e 6469 6e67 2904 da07 7374 6172  .pending)...star
-00000470: 7465 64da 0565 6e64 6564 da07 656c 6170  ted..ended..elap
-00000480: 7365 647a 1172 6563 6f72 6473 2072 6574  sedz.records ret
-00000490: 7269 6576 616c 2906 da0b 6f63 6375 7272  rieval)...occurr
-000004a0: 656e 6365 73da 0673 7461 7475 73da 0574  ences..status..t
-000004b0: 696d 6573 da07 7265 636f 7264 7372 1c00  imes..recordsr..
-000004c0: 0000 da0f 7265 7375 6c74 735f 6f66 5f73  ....results_of_s
-000004d0: 6361 6e72 0d00 0000 2902 7212 0000 0072  canr....).r....r
-000004e0: 0200 0000 2903 da12 7374 6174 7573 5f63  ....)...status_c
-000004f0: 6865 636b 5f70 6174 6873 da0d 7265 6c61  heck_paths..rela
-00000500: 7469 7665 5f70 6174 68da 1173 7461 7475  tive_path..statu
-00000510: 735f 6368 6563 6b5f 7061 7468 7218 0000  s_check_pathr...
-00000520: 0072 1800 0000 7219 0000 00da 1773 6574  .r....r......set
-00000530: 7570 5f69 6e74 6572 6e61 6c5f 7374 6174  up_internal_stat
-00000540: 7573 6573 4600 0000 7332 0000 0008 0402  usesF...s2......
-00000550: 0c02 0702 0802 0702 0702 0802 0702 0704  ................
-00000560: c504 4102 ff02 0602 0102 0102 0104 fc02  ..A.............
-00000570: 0702 0202 0104 b006 fe08 0104 ff04 5672  ..............Vr
-00000580: 2900 0000 6300 0000 0000 0000 0000 0000  )...c...........
-00000590: 0000 0000 0001 0000 0043 0000 0073 0400  .........C...s..
-000005a0: 0000 6400 5300 a901 4e72 1800 0000 7218  ..d.S...Nr....r.
-000005b0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-000005c0: 0000 da06 6368 616e 6765 a300 0000 f302  ....change......
-000005d0: 0000 0004 0172 2b00 0000 6300 0000 0000  .....r+...c.....
-000005e0: 0000 0000 0000 0000 0000 0001 0000 0043  ...............C
-000005f0: 0000 00f3 0400 0000 7400 5300 722a 0000  ........t.S.r*..
-00000600: 00a9 0172 1200 0000 7218 0000 0072 1800  ...r....r....r..
-00000610: 0000 7218 0000 0072 1900 0000 da12 7265  ..r....r......re
-00000620: 7472 6965 7665 5f76 6172 6961 626c 6573  trieve_variables
-00000630: a600 0000 722c 0000 0072 2f00 0000 6300  ....r,...r/...c.
-00000640: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00000650: 0000 0043 0000 0072 2d00 0000 722a 0000  ...C...r-...r*..
-00000660: 0072 2e00 0000 7218 0000 0072 1800 0000  .r....r....r....
-00000670: 7218 0000 0072 1900 0000 da1d 7265 7472  r....r......retr
-00000680: 6965 7665 5f61 6767 7265 6761 746f 725f  ieve_aggregator_
-00000690: 7661 7269 6162 6c65 73a9 0000 0072 2c00  variables....r,.
-000006a0: 0000 7230 0000 0063 0000 0000 0000 0000  ..r0...c........
-000006b0: 0000 0000 0000 0000 0100 0000 4300 0000  ............C...
-000006c0: 722d 0000 0072 2a00 0000 722e 0000 0072  r-...r*...r....r
-000006d0: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
-000006e0: 0000 00da 0872 6574 7269 6576 65ac 0000  .....retrieve...
-000006f0: 0072 2c00 0000 7231 0000 004e 290a da07  .r,...r1...N)...
-00000700: 5f5f 646f 635f 5fda 4162 696f 7465 6368  __doc__.Abiotech
-00000710: 2e70 726f 6365 6475 7265 732e 6167 6772  .procedures.aggr
-00000720: 6567 6174 6f72 5f70 726f 6365 6475 7265  egator_procedure
-00000730: 2e70 726f 6365 7373 2e6d 6f76 6573 2e66  .process.moves.f
-00000740: 6f72 6d61 745f 7061 7468 7202 0000 0072  ormat_pathr....r
-00000750: 1200 0000 721a 0000 0072 2900 0000 722b  ....r....r)...r+
-00000760: 0000 0072 2f00 0000 7230 0000 0072 3100  ...r/...r0...r1.
-00000770: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
-00000780: 0072 1900 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000790: 0100 0000 7328 0000 0004 020c 0402 0302  ....s(..........
-000007a0: 0702 1502 0104 fe02 0502 0202 0702 0502  ................
-000007b0: 0102 0206 e908 1a08 0808 5d08 0308 030c  ..........].....
-000007c0: 03                                       .
+00000020: 0008 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
+00000030: 5a00 0900 6401 6402 6c01 6d02 5a02 0100  Z...d.d.l.m.Z...
+00000040: 0900 0900 6403 6404 6405 9c02 6406 6900  ....d.d.d...d.i.
+00000050: 6407 6900 6408 6700 6409 9c07 5a03 640a  d.i.d.g.d...Z.d.
+00000060: 640b 8400 5a04 640c 640d 8400 5a05 640e  d...Z.d.d...Z.d.
+00000070: 640f 8400 5a06 6410 6411 8400 5a07 6412  d...Z.d.d...Z.d.
+00000080: 6413 8400 5a08 6414 6415 8400 5a09 6416  d...Z.d.d...Z.d.
+00000090: 5300 2917 7a66 0a09 6672 6f6d 2062 696f  S.).zf..from bio
+000000a0: 7465 6368 2e70 726f 6365 6475 7265 732e  tech.procedures.
+000000b0: 6167 6772 6567 6174 6f72 5f70 726f 6365  aggregator_proce
+000000c0: 6475 7265 2e70 726f 6365 7373 2e76 6172  dure.process.var
+000000d0: 6961 626c 6573 2069 6d70 6f72 7420 7265  iables import re
+000000e0: 7472 6965 7665 5f61 6767 7265 6761 746f  trieve_aggregato
+000000f0: 725f 7661 7269 6162 6c65 730a e900 0000  r_variables.....
+00000100: 0029 01da 0b66 6f72 6d61 745f 7061 7468  .)...format_path
+00000110: 7a07 302e 302e 302e 30da 0029 02da 0468  z.0.0.0.0..)...h
+00000120: 6f73 74da 0470 6f72 74e9 0300 0000 e902  ost..port.......
+00000130: 0000 00da 026e 6f29 07da 0c69 6e74 726f  .....no)...intro
+00000140: 5f68 6172 626f 72da 0d72 6563 6f72 6473  _harbor..records
+00000150: 5f6c 6576 656c da0f 696e 7472 6f5f 7661  _level..intro_va
+00000160: 7269 6162 6c65 73da 0764 6574 6169 6c73  riables..details
+00000170: da11 696e 7465 726e 616c 5f73 7461 7475  ..internal_statu
+00000180: 7365 73da 1769 6e74 6572 6e61 6c5f 7374  ses..internal_st
+00000190: 6174 7573 6573 5f62 7569 6c74 da09 616e  atuses_built..an
+000001a0: 6f6d 616c 6965 7363 0100 0000 0000 0000  omaliesc........
+000001b0: 0000 0000 0200 0000 0800 0000 4300 0000  ............C...
+000001c0: 7344 0000 007a 1374 00a0 017c 00a1 017d  sD...z.t...|...}
+000001d0: 0174 02a0 037c 00a1 0101 0074 0464 017c  .t...|.....t.d.|
+000001e0: 0069 0183 0101 0057 0064 0053 0004 0074  .i.....W.d.S...t
+000001f0: 0579 2101 0001 0001 0074 0464 0283 0101  .y!......t.d....
+00000200: 0059 0064 0053 0077 0029 034e da07 616e  .Y.d.S.w.).N..an
+00000210: 6f6d 616c 797a 1d41 6e20 616e 6f6d 616c  omalyz.An anomal
+00000220: 7920 636f 756c 646e 2774 2062 6520 6164  y couldn't be ad
+00000230: 6465 642e 2906 da04 6a73 6f6e da05 6475  ded.)...json..du
+00000240: 6d70 73da 1461 6767 7265 6761 746f 725f  mps..aggregator_
+00000250: 7661 7269 6162 6c65 73da 0661 7070 656e  variables..appen
+00000260: 64da 0d73 686f 775f 7661 7269 6162 6c65  d..show_variable
+00000270: da09 4578 6365 7074 696f 6e29 0272 1000  ..Exception).r..
+00000280: 0000 da07 6973 5f4a 534f 4ea9 0072 1800  ....is_JSON..r..
+00000290: 0000 fa5c 2f62 696f 7465 6368 2f76 656e  ...\/biotech/ven
+000002a0: 7565 732f 7374 6167 6573 2f62 696f 7465  ues/stages/biote
+000002b0: 6368 2f70 726f 6365 6475 7265 732f 6167  ch/procedures/ag
+000002c0: 6772 6567 6174 6f72 5f70 726f 6365 6475  gregator_procedu
+000002d0: 7265 2f70 726f 6365 7373 2f76 6172 6961  re/process/varia
+000002e0: 626c 6573 2f5f 5f69 6e69 745f 5f2e 7079  bles/__init__.py
+000002f0: da0b 6164 645f 616e 6f6d 616c 7943 0000  ..add_anomalyC..
+00000300: 0073 1200 0000 0201 0a01 0a02 0202 0401  .s..............
+00000310: 0cff 0c04 0e01 02ff 721a 0000 0063 0200  ........r....c..
+00000320: 0000 0000 0000 0000 0000 0300 0000 0a00  ................
+00000330: 0000 4300 0000 734e 0000 007c 0044 005d  ..C...sN...|.D.]
+00000340: 227d 0264 0164 0164 0164 0164 0264 0164  "}.d.d.d.d.d.d.d
+00000350: 0164 0364 049c 0864 0564 0669 0164 0364  .d.d...d.d.i.d.d
+00000360: 0364 0364 0364 079c 0467 0064 0064 0064  .d.d.d...g.d.d.d
+00000370: 089c 0674 0064 0919 0074 017c 027c 0183  ...t.d...t.|.|..
+00000380: 023c 0071 0264 0053 0029 0a4e 7208 0000  .<.q.d.S.).Nr...
+00000390: 00da 0775 6e6b 6e6f 776e 7203 0000 0029  ...unknownr....)
+000003a0: 087a 1c73 6361 6e20 7072 6f63 6573 7320  .z.scan process 
+000003b0: 7665 6e74 7572 6520 7374 6172 7465 647a  venture startedz
+000003c0: 1473 6361 6e20 7072 6f63 6573 7320 7374  .scan process st
+000003d0: 6172 7465 647a 2073 6361 6e20 7072 6f63  artedz scan proc
+000003e0: 6573 7320 6e6f 7469 6669 6564 2061 6767  ess notified agg
+000003f0: 7265 6761 746f 727a 1873 6361 6e20 7072  regatorz.scan pr
+00000400: 6f63 6573 7320 7761 7320 7374 6f70 7065  ocess was stoppe
+00000410: 647a 1573 6361 6e20 7072 6f63 6573 7320  dz.scan process 
+00000420: 6973 2061 6c69 7665 7a1c 7363 616e 2070  is alivez.scan p
+00000430: 726f 6365 6564 7320 7765 7265 2072 6574  roceeds were ret
+00000440: 7269 6576 6564 7a1b 7363 616e 2072 6563  rievedz.scan rec
+00000450: 6f72 6473 2077 6572 6520 7265 7472 6965  ords were retrie
+00000460: 7665 647a 1064 6f6e 6520 7265 6173 6f6e  vedz.done reason
+00000470: 2067 6976 65da 0770 726f 6365 7373 da07   give..process..
+00000480: 7065 6e64 696e 6729 04da 0773 7461 7274  pending)...start
+00000490: 6564 da05 656e 6465 64da 0765 6c61 7073  ed..ended..elaps
+000004a0: 6564 7a11 7265 636f 7264 7320 7265 7472  edz.records retr
+000004b0: 6965 7661 6c29 06da 0b6f 6363 7572 7265  ieval)...occurre
+000004c0: 6e63 6573 da06 7374 6174 7573 da05 7469  nces..status..ti
+000004d0: 6d65 73da 0772 6563 6f72 6473 721c 0000  mes..recordsr...
+000004e0: 00da 0f72 6573 756c 7473 5f6f 665f 7363  ...results_of_sc
+000004f0: 616e 720d 0000 0029 0272 1300 0000 7202  anr....).r....r.
+00000500: 0000 0029 03da 1273 7461 7475 735f 6368  ...)...status_ch
+00000510: 6563 6b5f 7061 7468 73da 0d72 656c 6174  eck_paths..relat
+00000520: 6976 655f 7061 7468 da11 7374 6174 7573  ive_path..status
+00000530: 5f63 6865 636b 5f70 6174 6872 1800 0000  _check_pathr....
+00000540: 7218 0000 0072 1900 0000 da17 7365 7475  r....r......setu
+00000550: 705f 696e 7465 726e 616c 5f73 7461 7475  p_internal_statu
+00000560: 7365 7350 0000 0073 3200 0000 0804 020c  sesP...s2.......
+00000570: 0207 0208 0207 0207 0208 0207 0207 04c5  ................
+00000580: 0441 02ff 0206 0201 0201 0201 04fc 0207  .A..............
+00000590: 0202 0201 04b0 06fe 0801 04ff 0456 7229  .............Vr)
+000005a0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000005b0: 0000 0000 0100 0000 4300 0000 7304 0000  ........C...s...
+000005c0: 0064 0053 00a9 014e 7218 0000 0072 1800  .d.S...Nr....r..
+000005d0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+000005e0: 00da 0663 6861 6e67 65ad 0000 00f3 0200  ...change.......
+000005f0: 0000 0401 722b 0000 0063 0000 0000 0000  ....r+...c......
+00000600: 0000 0000 0000 0000 0000 0100 0000 4300  ..............C.
+00000610: 0000 f304 0000 0074 0053 0072 2a00 0000  .......t.S.r*...
+00000620: a901 7213 0000 0072 1800 0000 7218 0000  ..r....r....r...
+00000630: 0072 1800 0000 7219 0000 00da 1272 6574  .r....r......ret
+00000640: 7269 6576 655f 7661 7269 6162 6c65 73b0  rieve_variables.
+00000650: 0000 0072 2c00 0000 722f 0000 0063 0000  ...r,...r/...c..
+00000660: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00000670: 0000 4300 0000 722d 0000 0072 2a00 0000  ..C...r-...r*...
+00000680: 722e 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
+00000690: 1800 0000 7219 0000 00da 1d72 6574 7269  ....r......retri
+000006a0: 6576 655f 6167 6772 6567 6174 6f72 5f76  eve_aggregator_v
+000006b0: 6172 6961 626c 6573 b300 0000 722c 0000  ariables....r,..
+000006c0: 0072 3000 0000 6300 0000 0000 0000 0000  .r0...c.........
+000006d0: 0000 0000 0000 0001 0000 0043 0000 0072  ...........C...r
+000006e0: 2d00 0000 722a 0000 0072 2e00 0000 7218  -...r*...r....r.
+000006f0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+00000700: 0000 da08 7265 7472 6965 7665 b600 0000  ....retrieve....
+00000710: 722c 0000 0072 3100 0000 4e29 0ada 075f  r,...r1...N)..._
+00000720: 5f64 6f63 5f5f da41 6269 6f74 6563 682e  _doc__.Abiotech.
+00000730: 7072 6f63 6564 7572 6573 2e61 6767 7265  procedures.aggre
+00000740: 6761 746f 725f 7072 6f63 6564 7572 652e  gator_procedure.
+00000750: 7072 6f63 6573 732e 6d6f 7665 732e 666f  process.moves.fo
+00000760: 726d 6174 5f70 6174 6872 0200 0000 7213  rmat_pathr....r.
+00000770: 0000 0072 1a00 0000 7229 0000 0072 2b00  ...r....r)...r+.
+00000780: 0000 722f 0000 0072 3000 0000 7231 0000  ..r/...r0...r1..
+00000790: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
+000007a0: 7219 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+000007b0: 0000 0073 2a00 0000 0402 0204 0c05 0203  ...s*...........
+000007c0: 0207 0215 0201 04fe 0205 0202 0207 0205  ................
+000007d0: 0201 0202 06e9 081a 080d 085d 0803 0803  ...........]....
+000007e0: 0c03                                     ..
```

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py` & `biotech-1.1.3/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/on.py` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py` & `biotech-1.1.3/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/intro/on.py` & `biotech-1.1.3/venues/stages/biotech/procedures/intro/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/adventure.py` & `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/adventure.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py` & `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py` & `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/keg/__init__.py` & `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/aggregate/__init__.py` & `biotech-1.1.3/venues/stages/biotech/topics/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/alarm_parser/__init__.py` & `biotech-1.1.3/venues/stages/biotech/topics/alarm_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__init__.py` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__init__.py` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/treasury.py` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/basin/treasury.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/shares.s.HTML` & `biotech-1.1.3/venues/stages/biotech/topics/help_documentation/shares.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/implicit/proc/__init__.py` & `biotech-1.1.3/venues/stages/biotech/topics/implicit/proc/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/implicit/thread/__init__.py` & `biotech-1.1.3/venues/stages/biotech/topics/implicit/thread/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/printout/passes.py` & `biotech-1.1.3/venues/stages/biotech/topics/printout/passes.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__init__.py` & `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/implicit.py` & `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/parse_records.py` & `biotech-1.1.3/venues/stages/biotech/topics/process_on/p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/quay/garage.py` & `biotech-1.1.3/venues/stages/biotech/topics/quay/garage.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_1.py` & `biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_2.py` & `biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_2.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_3.py` & `biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_3.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_4.py` & `biotech-1.1.3/venues/stages/biotech/topics/quay/implicit_process_test_4.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py` & `biotech-1.1.3/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/show/variable.py` & `biotech-1.1.3/venues/stages/biotech/topics/show/variable.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc` & `biotech-1.1.3/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/venues/stages/biotech/topics/start--/simultaneously.py` & `biotech-1.1.3/venues/stages/biotech/topics/start--/simultaneously.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.2/PKG-INFO` & `biotech-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotech
-Version: 1.1.2
+Version: 1.1.3
 Summary: A health monitoring stack
 License: GPL-3.0-only
 Keywords: alarms,screening,monitors,cybernetics,neurons,nervous system,bioelectric,homeostasis,reliability,consistency,integrity,guarantees,vows,oaths,assurances,insurances,ensurances,speed,calmness,education,augmentation,enhancement,improvements
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

