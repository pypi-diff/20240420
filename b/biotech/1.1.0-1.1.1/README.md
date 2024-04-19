# Comparing `tmp/biotech-1.1.0.tar.gz` & `tmp/biotech-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotech-1.1.0.tar", max compression
+gzip compressed data, was "biotech-1.1.1.tar", max compression
```

## Comparing `biotech-1.1.0.tar` & `biotech-1.1.1.tar`

### file list

```diff
@@ -1,785 +1,786 @@
--rwxr-xr-x   0        0        0      211 2024-04-16 02:07:59.993436 biotech-1.1.0/license.S.HTML
--rwxr-xr-x   0        0        0     1145 2024-04-19 20:06:30.613524 biotech-1.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     3866 2024-04-16 20:53:30.034757 biotech-1.1.0/readme.md
--rwxr-xr-x   0        0        0     2331 2024-04-19 15:34:34.407444 biotech-1.1.0/venue.S.HTML
--rwxr-xr-x   0        0        0   838272 2024-04-16 02:03:26.700967 biotech-1.1.0/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
--rwxr-xr-x   0        0        0     1270 2024-04-17 22:22:59.944800 biotech-1.1.0/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
--rwxr-xr-x   0        0        0     4079 2024-04-16 20:48:34.871383 biotech-1.1.0/venues/stages/biotech/___itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0      645 2024-04-16 20:48:34.875383 biotech-1.1.0/venues/stages/biotech/___itinerary/maybes.s.HTML
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout/script.py
--rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout/start.py
--rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
--rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
--rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
--rwxr-xr-x   0        0        0      385 2024-04-17 18:49:44.656786 biotech-1.1.0/venues/stages/biotech/__glossary/biotech_1
--rwxr-xr-x   0        0        0      114 2024-04-17 18:45:06.744254 biotech-1.1.0/venues/stages/biotech/__glossary/glossary.S.HTML
--rwxr-xr-x   0        0        0      130 2024-04-19 16:49:02.311131 biotech-1.1.0/venues/stages/biotech/__init__.py
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 biotech-1.1.0/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0     1252 2024-04-16 20:48:34.867383 biotech-1.1.0/venues/stages/biotech/_book/advanced tutorial.s.HTML
--rwxr-xr-x   0        0        0     1786 2024-04-16 20:48:34.867383 biotech-1.1.0/venues/stages/biotech/_book/book.s.HTML
--rwxr-xr-x   0        0        0      542 2024-04-16 20:48:34.867383 biotech-1.1.0/venues/stages/biotech/_book/relevant.s.HTML
--rwxr-xr-x   0        0        0     2129 2024-04-17 19:24:51.191926 biotech-1.1.0/venues/stages/biotech/_clique/__init__.py
--rwxr-xr-x   0        0        0     2493 2024-04-17 19:24:52.839918 biotech-1.1.0/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 biotech-1.1.0/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 biotech-1.1.0/venues/stages/biotech/_clique/group/__init__.py
--rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 biotech-1.1.0/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 biotech-1.1.0/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0  1328100 2024-04-19 20:05:41.074199 biotech-1.1.0/venues/stages/biotech/_status/DB/records.json
--rwxr-xr-x   0        0        0     1156 2024-04-19 17:06:33.102985 biotech-1.1.0/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
--rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 biotech-1.1.0/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
--rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 biotech-1.1.0/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
--rwxr-xr-x   0        0        0     1463 2024-04-19 17:05:25.115746 biotech-1.1.0/venues/stages/biotech/_status/establish.py
--rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416142 biotech-1.1.0/venues/stages/biotech/_status/monitors/-1_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 biotech-1.1.0/venues/stages/biotech/_status/monitors/-1_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      720 2024-04-16 20:48:34.887383 biotech-1.1.0/venues/stages/biotech/_status/monitors/-1_start/status_1.py
--rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 biotech-1.1.0/venues/stages/biotech/_status/monitors/0_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 biotech-1.1.0/venues/stages/biotech/_status/monitors/0_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      793 2024-04-16 20:48:34.883383 biotech-1.1.0/venues/stages/biotech/_status/monitors/0_start/status_1.py
--rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708148 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/path_1_health.py
--rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/path_2_health.py
--rwxr-xr-x   0        0        0     1161 2024-04-16 20:48:34.903383 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/status_1.py
--rwxr-xr-x   0        0        0      367 2024-04-16 03:23:58.043895 biotech-1.1.0/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 biotech-1.1.0/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1147 2024-04-19 19:06:56.036882 biotech-1.1.0/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
--rw-r--r--   0        0        0      316 2024-04-19 18:57:32.516036 biotech-1.1.0/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       77 2024-04-19 18:57:24.196146 biotech-1.1.0/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1208 2024-04-19 17:04:46.812176 biotech-1.1.0/venues/stages/biotech/_status/monitors/11/status_1.py
--rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/1_health.py
--rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/2_health.py
--rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/modules/MODULE_1.py
--rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1214 2024-04-16 20:48:34.899383 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/status_1.py
--rwxr-xr-x   0        0        0      794 2024-04-16 20:48:34.891383 biotech-1.1.0/venues/stages/biotech/_status/monitors/3_empty_glob/status_1.py
--rwxr-xr-x   0        0        0      289 2024-04-16 00:28:17.871373 biotech-1.1.0/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      517 2024-04-16 00:32:46.948536 biotech-1.1.0/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      942 2024-04-16 20:48:34.883383 biotech-1.1.0/venues/stages/biotech/_status/monitors/4.1_bad_import/status_1.py
--rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 biotech-1.1.0/venues/stages/biotech/_status/monitors/4_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 biotech-1.1.0/venues/stages/biotech/_status/monitors/4_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      939 2024-04-16 20:48:34.887383 biotech-1.1.0/venues/stages/biotech/_status/monitors/4_bad_import/status_1.py
--rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/1_health.py
--rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      867 2024-04-16 20:48:34.891383 biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/status_1.py
--rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/1_health.py
--rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/2_health.py
--rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/3_health.py
--rw-r--r--   0        0        0     1036 2024-04-19 19:54:47.501752 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc
--rw-r--r--   0        0        0      183 2024-04-19 19:54:47.501752 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/2_health.cpython-310.pyc
--rw-r--r--   0        0        0      169 2024-04-19 19:54:47.505751 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/3_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      926 2024-04-19 19:53:38.302512 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/status_1.py
--rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 biotech-1.1.0/venues/stages/biotech/_status/monitors/7/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 biotech-1.1.0/venues/stages/biotech/_status/monitors/7/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0      809 2024-04-16 20:48:34.907383 biotech-1.1.0/venues/stages/biotech/_status/monitors/7/status_1.py
--rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 biotech-1.1.0/venues/stages/biotech/_status/monitors/8_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 biotech-1.1.0/venues/stages/biotech/_status/monitors/8_DB/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0     1561 2024-04-19 19:13:07.956368 biotech-1.1.0/venues/stages/biotech/_status/monitors/8_DB/status_1.py
--rwxr-xr-x   0        0        0    82190 2024-04-19 20:05:31.254334 biotech-1.1.0/venues/stages/biotech/_status/monitors/8_DB/variable/status_db/records.json
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_2.py
--rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_3.py
--rwxr-xr-x   0        0        0     1402 2024-04-19 19:21:30.822364 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/status_1.py
--rwxr-xr-x   0        0        0      984 2024-04-18 03:32:30.971629 biotech-1.1.0/venues/stages/biotech/_status/status.proc.py
--rwxr-xr-x   0        0        0      256 2024-04-16 20:48:34.875383 biotech-1.1.0/venues/stages/biotech/_status/status.s.HTML
--rwxr-xr-x   0        0        0     1483 2024-04-16 20:48:34.851384 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
--rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
--rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
--rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 biotech-1.1.0/venues/stages/biotech/_status_advanced/status.proc.py
--rwxr-xr-x   0        0        0     1779 2024-04-16 20:48:34.575388 biotech-1.1.0/venues/stages/biotech/architecture.s.HTML
--rwxr-xr-x   0        0        0      241 2024-04-16 20:53:18.546926 biotech-1.1.0/venues/stages/biotech/emojis.S.HTML
--rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 biotech-1.1.0/venues/stages/biotech/license.S.HTML
--rwxr-xr-x   0        0        0     3068 2024-04-16 20:48:34.543389 biotech-1.1.0/venues/stages/biotech/module.s.HTML
--rwxr-xr-x   0        0        0     1615 2024-04-19 16:31:12.412493 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      640 2024-04-19 16:26:52.595637 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      259 2024-04-19 16:20:24.028904 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
--rwxr-xr-x   0        0        0     1461 2024-04-19 16:31:10.152519 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.648116 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/paths.py
--rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.660116 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
--rwxr-xr-x   0        0        0      562 2024-04-17 21:48:05.111704 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
--rwxr-xr-x   0        0        0     1163 2024-04-17 21:49:49.362841 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1734 2024-04-19 16:26:14.672115 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
--rwxr-xr-x   0        0        0     2173 2024-04-19 16:27:13.567375 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      965 2024-04-19 16:27:13.567375 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0     2744 2024-04-19 19:39:17.347586 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0     1137 2024-04-19 16:27:13.567375 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      643 2024-04-19 16:26:14.684115 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
--rwxr-xr-x   0        0        0     3672 2024-04-19 19:29:49.876463 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
--rwxr-xr-x   0        0        0      789 2024-04-19 16:26:14.712115 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
--rwxr-xr-x   0        0        0     2031 2024-04-19 16:27:13.563375 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
--rwxr-xr-x   0        0        0     1282 2024-04-15 20:31:31.342880 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0     1743 2024-04-19 18:03:45.582807 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      418 2024-04-17 20:03:55.692458 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      687 2024-04-15 22:21:10.822989 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
--rwxr-xr-x   0        0        0     3455 2024-04-17 21:41:59.150872 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
--rwxr-xr-x   0        0        0      746 2024-04-17 23:09:52.928659 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
--rwxr-xr-x   0        0        0      849 2024-04-17 20:12:15.035804 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
--rwxr-xr-x   0        0        0      933 2024-04-15 23:20:20.086332 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
--rwxr-xr-x   0        0        0     3451 2024-04-19 16:26:14.724115 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
--rwxr-xr-x   0        0        0     2705 2024-04-19 18:03:38.578879 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
--rwxr-xr-x   0        0        0      193 2024-04-17 20:02:37.661229 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
--rwxr-xr-x   0        0        0      566 2024-04-17 23:09:07.804988 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
--rwxr-xr-x   0        0        0     1834 2024-04-19 18:55:07.129933 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
--rw-r--r--   0        0        0     1851 2024-04-19 18:55:11.397883 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      799 2024-04-19 16:27:13.563375 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
--rw-r--r--   0        0        0     4038 2024-04-19 19:39:17.347586 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
--rwxr-xr-x   0        0        0      754 2024-04-18 00:33:41.120405 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
--rw-r--r--   0        0        0     1826 2024-04-19 18:56:22.468973 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-19 18:56:27.160910 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      996 2024-04-19 16:26:14.764114 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
--rwxr-xr-x   0        0        0     8610 2024-04-19 19:38:19.764145 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
--rwxr-xr-x   0        0        0     1223 2024-04-19 16:26:14.792114 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/venture_finish--.py
--rwxr-xr-x   0        0        0     2910 2024-04-19 16:26:14.804114 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
--rwxr-xr-x   0        0        0     1684 2024-04-19 16:27:13.563375 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      834 2024-04-16 20:48:34.547389 biotech-1.1.0/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
--rwxr-xr-x   0        0        0      951 2024-04-16 20:49:56.266040 biotech-1.1.0/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      479 2024-04-16 20:49:28.130498 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
--rwxr-xr-x   0        0        0     1838 2024-04-19 16:27:13.567375 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      347 2024-04-16 20:48:34.555389 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/dynamic_port.py
--rwxr-xr-x   0        0        0     2105 2024-04-19 16:26:14.612116 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/on.py
--rwxr-xr-x   0        0        0     2201 2024-04-18 02:31:19.570492 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
--rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
--rwxr-xr-x   0        0        0     1441 2024-04-18 02:04:22.961501 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
--rwxr-xr-x   0        0        0      774 2024-04-16 20:48:34.555389 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
--rwxr-xr-x   0        0        0     1336 2024-04-15 21:13:32.676638 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      309 2024-04-17 23:41:26.722721 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      562 2024-04-17 23:41:26.734721 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      525 2024-04-17 23:09:55.764639 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      908 2024-04-19 20:05:11.362609 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0      636 2024-04-18 01:15:59.039315 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      289 2024-04-17 23:05:28.138584 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
--rwxr-xr-x   0        0        0      803 2024-04-19 20:05:09.858629 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
--rwxr-xr-x   0        0        0      378 2024-04-18 01:13:51.928249 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
--rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
--rwxr-xr-x   0        0        0     2182 2024-04-18 01:57:52.896535 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
--rwxr-xr-x   0        0        0     2125 2024-04-18 01:58:34.052216 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1027 2024-04-17 23:41:26.738721 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0     1368 2024-04-17 23:38:58.631806 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
--rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
--rwxr-xr-x   0        0        0      152 2024-04-19 16:48:50.419277 biotech-1.1.0/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3443 2024-04-19 20:02:47.664429 biotech-1.1.0/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.0/venues/stages/biotech/procedures/intro/intro.S.HTML
--rwxr-xr-x   0        0        0     5074 2024-04-19 20:02:38.772528 biotech-1.1.0/venues/stages/biotech/procedures/intro/on.py
--rw-r--r--   0        0        0     2887 2024-04-19 19:04:05.278996 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
--rw-r--r--   0        0        0     3989 2024-04-19 19:03:05.467745 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/adventure.py
--rwxr-xr-x   0        0        0     1267 2024-04-19 16:26:52.599637 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      905 2024-04-19 16:56:52.013564 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      901 2024-04-19 16:26:14.840113 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      614 2024-04-19 16:56:41.273688 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
--rwxr-xr-x   0        0        0      138 2024-04-19 17:33:23.717242 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/intro.proc.py
--rwxr-xr-x   0        0        0     3047 2024-04-19 19:04:01.875038 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/keg/__init__.py
--rw-r--r--   0        0        0     3044 2024-04-19 19:04:05.278996 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/variables/__init__.py
--rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321766 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       33 2024-04-17 22:47:27.362384 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/__init__.py
--rwxr-xr-x   0        0        0      192 2024-04-17 22:47:29.166371 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1930 2024-04-19 16:45:15.609992 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     3212 2024-04-19 16:26:52.583637 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/_ops/__pycache__/start.cpython-310.pyc
--rwxr-xr-x   0        0        0     4487 2024-04-19 16:26:14.828113 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/_ops/start.py
--rwxr-xr-x   0        0        0     1267 2024-04-19 16:26:52.599637 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      855 2024-04-19 16:26:52.631636 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      901 2024-04-19 16:26:14.840113 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      572 2024-04-19 16:26:14.856113 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/send_paths.py
--rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/intro.S.HTML
--rwxr-xr-x   0        0        0     1991 2024-04-18 03:48:25.192521 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/__init__.py
--rwxr-xr-x   0        0        0     1394 2024-04-18 06:18:52.492292 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/__init__v1.py
--rwxr-xr-x   0        0        0     2895 2024-04-18 05:23:09.408255 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1447 2024-04-16 20:48:34.559388 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/quart__init__.py
--rwxr-xr-x   0        0        0     2039 2024-04-19 16:45:13.398021 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/on.py
--rwxr-xr-x   0        0        0     4069 2024-04-19 16:41:30.225039 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/intro.proc.py
--rwxr-xr-x   0        0        0     2819 2024-04-19 16:40:32.337866 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/keg/__init__.py
--rwxr-xr-x   0        0        0     3015 2024-04-19 16:40:36.437807 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3062 2024-04-19 16:26:53.431626 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/moves/__pycache__/adventure.cpython-310.pyc
--rwxr-xr-x   0        0        0     4716 2024-04-19 16:26:14.896113 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/moves/adventure.py
--rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/variables/__init__.py
--rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321765 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      172 2024-04-16 20:48:34.551389 biotech-1.1.0/venues/stages/biotech/procedures/procedures.S.HTML
--rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 biotech-1.1.0/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
--rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 biotech-1.1.0/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
--rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 biotech-1.1.0/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 biotech-1.1.0/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 biotech-1.1.0/venues/stages/biotech/topics/aggregate/__init__.py
--rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 biotech-1.1.0/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 biotech-1.1.0/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      708 2024-04-16 20:48:34.591388 biotech-1.1.0/venues/stages/biotech/topics/alarm_parser/__init__.py
--rwxr-xr-x   0        0        0      673 2024-04-16 20:49:28.126498 biotech-1.1.0/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 biotech-1.1.0/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      405 2024-04-16 20:48:34.579388 biotech-1.1.0/venues/stages/biotech/topics/exceptions.py
--rwxr-xr-x   0        0        0     1190 2024-01-27 05:31:08.525189 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
--rwxr-xr-x   0        0        0     2446 2024-04-17 19:24:25.140060 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__init__.py
--rwxr-xr-x   0        0        0     2491 2024-04-17 19:24:52.839918 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4471 2024-02-01 06:11:56.801715 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1050 2024-04-16 06:10:03.111579 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     1920 2024-01-31 18:50:23.812071 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
--rwxr-xr-x   0        0        0       24 2024-01-26 17:38:56.558087 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
--rwxr-xr-x   0        0        0       24 2024-01-26 17:38:52.854129 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
--rwxr-xr-x   0        0        0      751 2024-04-17 19:16:04.226583 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
--rwxr-xr-x   0        0        0     1981 2024-04-17 19:25:47.591625 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__init__.py
--rwxr-xr-x   0        0        0     2283 2024-04-17 19:25:53.011595 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4019 2024-01-31 18:51:47.652157 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     3843 2024-04-17 19:25:53.099595 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
--rwxr-xr-x   0        0        0     4426 2024-01-27 06:34:32.979965 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
--rwxr-xr-x   0        0        0     3559 2024-04-17 19:25:22.227762 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/treasury.py
--rwxr-xr-x   0        0        0     1727 2024-04-17 19:15:19.882965 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/shares.s.HTML
--rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 biotech-1.1.0/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1558 2024-04-18 05:22:02.832642 biotech-1.1.0/venues/stages/biotech/topics/implicit/proc/__init__.py
--rwxr-xr-x   0        0        0     1155 2024-04-18 05:46:33.436738 biotech-1.1.0/venues/stages/biotech/topics/implicit/thread/__init__.py
--rwxr-xr-x   0        0        0      855 2024-04-18 06:05:23.346518 biotech-1.1.0/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       90 2024-04-17 22:51:08.968798 biotech-1.1.0/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 22:33:48.860256 biotech-1.1.0/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
--rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 biotech-1.1.0/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
--rwxr-xr-x   0        0        0      470 2024-04-17 23:02:14.419990 biotech-1.1.0/venues/stages/biotech/topics/printout/bracket.py
--rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 biotech-1.1.0/venues/stages/biotech/topics/printout/passes.py
--rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 biotech-1.1.0/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2163 2024-04-19 18:50:11.157390 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__init__.py
--rw-r--r--   0        0        0     1997 2024-04-19 18:52:58.595432 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
--rw-r--r--   0        0        0     1818 2024-04-19 18:54:33.250328 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-18 01:45:27.254200 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1766 2024-04-19 18:53:11.523281 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-18 01:48:34.504806 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-18 01:45:24.082223 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
--rwxr-xr-x   0        0        0      195 2024-04-16 22:50:54.515336 biotech-1.1.0/venues/stages/biotech/topics/process_on/process_on.S.HTML
--rwxr-xr-x   0        0        0     1470 2024-04-18 04:12:56.845888 biotech-1.1.0/venues/stages/biotech/topics/quay/garage.py
--rwxr-xr-x   0        0        0     2546 2024-04-18 04:38:41.478278 biotech-1.1.0/venues/stages/biotech/topics/quay/implicit_process_test_1.py
--rwxr-xr-x   0        0        0     1612 2024-04-18 04:54:58.414971 biotech-1.1.0/venues/stages/biotech/topics/quay/implicit_process_test_2.py
--rwxr-xr-x   0        0        0      551 2024-04-18 05:20:40.701113 biotech-1.1.0/venues/stages/biotech/topics/quay/implicit_process_test_3.py
--rwxr-xr-x   0        0        0     1083 2024-04-18 05:19:11.645613 biotech-1.1.0/venues/stages/biotech/topics/quay/implicit_process_test_4.py
--rwxr-xr-x   0        0        0     1442 2024-04-16 20:48:34.591388 biotech-1.1.0/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
--rwxr-xr-x   0        0        0     1464 2024-04-16 20:49:28.126498 biotech-1.1.0/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 biotech-1.1.0/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
--rw-r--r--   0        0        0     1776 2024-04-19 19:50:41.332444 biotech-1.1.0/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0      461 2024-04-17 23:59:06.614967 biotech-1.1.0/venues/stages/biotech/topics/show/show.S.HTML
--rwxr-xr-x   0        0        0     2305 2024-04-19 19:50:39.412465 biotech-1.1.0/venues/stages/biotech/topics/show/variable.py
--rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
--rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
--rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
--rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
--rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
--rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
--rwxr-xr-x   0        0        0      273 2024-04-16 20:48:34.583388 biotech-1.1.0/venues/stages/biotech/topics/start--/one.py
--rwxr-xr-x   0        0        0      406 2024-04-16 20:48:34.587388 biotech-1.1.0/venues/stages/biotech/topics/start--/sequentially.py
--rwxr-xr-x   0        0        0      532 2024-04-16 20:48:34.587388 biotech-1.1.0/venues/stages/biotech/topics/start--/simultaneously.py
--rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 biotech-1.1.0/venues/stages/biotech/topics/topics.S.HTML
--rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 biotech-1.1.0/venues/stages/biotech/variables/__init__.py
--rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0      211 2024-04-16 02:07:59.993436 biotech-1.1.1/license.S.HTML
+-rwxr-xr-x   0        0        0     1145 2024-04-19 20:38:42.426229 biotech-1.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0     3866 2024-04-16 20:53:30.034757 biotech-1.1.1/readme.md
+-rwxr-xr-x   0        0        0     2331 2024-04-19 15:34:34.407444 biotech-1.1.1/venue.S.HTML
+-rwxr-xr-x   0        0        0   838272 2024-04-16 02:03:26.700967 biotech-1.1.1/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
+-rwxr-xr-x   0        0        0     1270 2024-04-17 22:22:59.944800 biotech-1.1.1/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
+-rwxr-xr-x   0        0        0     4079 2024-04-16 20:48:34.871383 biotech-1.1.1/venues/stages/biotech/___itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      645 2024-04-16 20:48:34.875383 biotech-1.1.1/venues/stages/biotech/___itinerary/maybes.s.HTML
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout/script.py
+-rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout/start.py
+-rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
+-rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
+-rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
+-rwxr-xr-x   0        0        0      385 2024-04-17 18:49:44.656786 biotech-1.1.1/venues/stages/biotech/__glossary/biotech_1
+-rwxr-xr-x   0        0        0      114 2024-04-17 18:45:06.744254 biotech-1.1.1/venues/stages/biotech/__glossary/glossary.S.HTML
+-rwxr-xr-x   0        0        0      130 2024-04-19 16:49:02.311131 biotech-1.1.1/venues/stages/biotech/__init__.py
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 biotech-1.1.1/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0     1252 2024-04-16 20:48:34.867383 biotech-1.1.1/venues/stages/biotech/_book/advanced tutorial.s.HTML
+-rwxr-xr-x   0        0        0     1786 2024-04-16 20:48:34.867383 biotech-1.1.1/venues/stages/biotech/_book/book.s.HTML
+-rwxr-xr-x   0        0        0      542 2024-04-16 20:48:34.867383 biotech-1.1.1/venues/stages/biotech/_book/relevant.s.HTML
+-rwxr-xr-x   0        0        0     2129 2024-04-17 19:24:51.191926 biotech-1.1.1/venues/stages/biotech/_clique/__init__.py
+-rwxr-xr-x   0        0        0     2493 2024-04-17 19:24:52.839918 biotech-1.1.1/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 biotech-1.1.1/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 biotech-1.1.1/venues/stages/biotech/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 biotech-1.1.1/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 biotech-1.1.1/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0  1334817 2024-04-19 20:37:52.170777 biotech-1.1.1/venues/stages/biotech/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1156 2024-04-19 17:06:33.102985 biotech-1.1.1/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 biotech-1.1.1/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 biotech-1.1.1/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1463 2024-04-19 17:05:25.115746 biotech-1.1.1/venues/stages/biotech/_status/establish.py
+-rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416142 biotech-1.1.1/venues/stages/biotech/_status/monitors/-1_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 biotech-1.1.1/venues/stages/biotech/_status/monitors/-1_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      720 2024-04-16 20:48:34.887383 biotech-1.1.1/venues/stages/biotech/_status/monitors/-1_start/status_1.py
+-rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 biotech-1.1.1/venues/stages/biotech/_status/monitors/0_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 biotech-1.1.1/venues/stages/biotech/_status/monitors/0_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      793 2024-04-16 20:48:34.883383 biotech-1.1.1/venues/stages/biotech/_status/monitors/0_start/status_1.py
+-rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708148 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/path_1_health.py
+-rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/path_2_health.py
+-rwxr-xr-x   0        0        0     1161 2024-04-16 20:48:34.903383 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/status_1.py
+-rwxr-xr-x   0        0        0      367 2024-04-16 03:23:58.043895 biotech-1.1.1/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 biotech-1.1.1/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1147 2024-04-19 19:06:56.036882 biotech-1.1.1/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
+-rw-r--r--   0        0        0      316 2024-04-19 18:57:32.516036 biotech-1.1.1/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       77 2024-04-19 18:57:24.196146 biotech-1.1.1/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1208 2024-04-19 17:04:46.812176 biotech-1.1.1/venues/stages/biotech/_status/monitors/11/status_1.py
+-rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/1_health.py
+-rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/2_health.py
+-rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/modules/MODULE_1.py
+-rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1214 2024-04-16 20:48:34.899383 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/status_1.py
+-rwxr-xr-x   0        0        0      794 2024-04-16 20:48:34.891383 biotech-1.1.1/venues/stages/biotech/_status/monitors/3_empty_glob/status_1.py
+-rwxr-xr-x   0        0        0      289 2024-04-16 00:28:17.871373 biotech-1.1.1/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      517 2024-04-16 00:32:46.948536 biotech-1.1.1/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      942 2024-04-16 20:48:34.883383 biotech-1.1.1/venues/stages/biotech/_status/monitors/4.1_bad_import/status_1.py
+-rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 biotech-1.1.1/venues/stages/biotech/_status/monitors/4_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 biotech-1.1.1/venues/stages/biotech/_status/monitors/4_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      939 2024-04-16 20:48:34.887383 biotech-1.1.1/venues/stages/biotech/_status/monitors/4_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/1_health.py
+-rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      867 2024-04-16 20:48:34.891383 biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/status_1.py
+-rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/1_health.py
+-rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/2_health.py
+-rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/3_health.py
+-rw-r--r--   0        0        0     1036 2024-04-19 19:54:47.501752 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc
+-rw-r--r--   0        0        0      183 2024-04-19 19:54:47.501752 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/2_health.cpython-310.pyc
+-rw-r--r--   0        0        0      169 2024-04-19 19:54:47.505751 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/3_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      926 2024-04-19 19:53:38.302512 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/status_1.py
+-rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 biotech-1.1.1/venues/stages/biotech/_status/monitors/7/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 biotech-1.1.1/venues/stages/biotech/_status/monitors/7/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0      809 2024-04-16 20:48:34.907383 biotech-1.1.1/venues/stages/biotech/_status/monitors/7/status_1.py
+-rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 biotech-1.1.1/venues/stages/biotech/_status/monitors/8_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 biotech-1.1.1/venues/stages/biotech/_status/monitors/8_DB/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0     1561 2024-04-19 19:13:07.956368 biotech-1.1.1/venues/stages/biotech/_status/monitors/8_DB/status_1.py
+-rwxr-xr-x   0        0        0    84462 2024-04-19 20:37:42.406890 biotech-1.1.1/venues/stages/biotech/_status/monitors/8_DB/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_2.py
+-rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_3.py
+-rwxr-xr-x   0        0        0     1402 2024-04-19 19:21:30.822364 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/status_1.py
+-rwxr-xr-x   0        0        0      984 2024-04-18 03:32:30.971629 biotech-1.1.1/venues/stages/biotech/_status/status.proc.py
+-rwxr-xr-x   0        0        0      256 2024-04-16 20:48:34.875383 biotech-1.1.1/venues/stages/biotech/_status/status.s.HTML
+-rwxr-xr-x   0        0        0     1483 2024-04-16 20:48:34.851384 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
+-rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
+-rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 biotech-1.1.1/venues/stages/biotech/_status_advanced/status.proc.py
+-rwxr-xr-x   0        0        0     1779 2024-04-16 20:48:34.575388 biotech-1.1.1/venues/stages/biotech/architecture.s.HTML
+-rwxr-xr-x   0        0        0      241 2024-04-16 20:53:18.546926 biotech-1.1.1/venues/stages/biotech/emojis.S.HTML
+-rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 biotech-1.1.1/venues/stages/biotech/license.S.HTML
+-rwxr-xr-x   0        0        0     3068 2024-04-16 20:48:34.543389 biotech-1.1.1/venues/stages/biotech/module.s.HTML
+-rwxr-xr-x   0        0        0     1615 2024-04-19 16:31:12.412493 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      640 2024-04-19 16:26:52.595637 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      259 2024-04-19 16:20:24.028904 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
+-rwxr-xr-x   0        0        0     1458 2024-04-19 20:37:55.182742 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.648116 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/paths.py
+-rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.660116 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
+-rwxr-xr-x   0        0        0      562 2024-04-17 21:48:05.111704 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
+-rwxr-xr-x   0        0        0     1163 2024-04-17 21:49:49.362841 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1734 2024-04-19 16:26:14.672115 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
+-rwxr-xr-x   0        0        0     2173 2024-04-19 16:27:13.567375 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      965 2024-04-19 16:27:13.567375 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0     2744 2024-04-19 19:39:17.347586 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1137 2024-04-19 16:27:13.567375 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      643 2024-04-19 16:26:14.684115 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
+-rwxr-xr-x   0        0        0     3672 2024-04-19 19:29:49.876463 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
+-rwxr-xr-x   0        0        0      789 2024-04-19 16:26:14.712115 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
+-rwxr-xr-x   0        0        0     2031 2024-04-19 16:27:13.563375 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1282 2024-04-15 20:31:31.342880 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0     1743 2024-04-19 18:03:45.582807 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      418 2024-04-17 20:03:55.692458 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      687 2024-04-15 22:21:10.822989 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3455 2024-04-17 21:41:59.150872 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
+-rwxr-xr-x   0        0        0      746 2024-04-17 23:09:52.928659 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0      849 2024-04-17 20:12:15.035804 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
+-rwxr-xr-x   0        0        0      933 2024-04-15 23:20:20.086332 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3451 2024-04-19 16:26:14.724115 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
+-rwxr-xr-x   0        0        0     2708 2024-04-19 20:38:18.218488 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
+-rwxr-xr-x   0        0        0      193 2024-04-17 20:02:37.661229 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
+-rwxr-xr-x   0        0        0      566 2024-04-17 23:09:07.804988 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
+-rwxr-xr-x   0        0        0     1834 2024-04-19 18:55:07.129933 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
+-rw-r--r--   0        0        0     1851 2024-04-19 18:55:11.397883 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      799 2024-04-19 16:27:13.563375 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
+-rw-r--r--   0        0        0     3981 2024-04-19 20:36:32.447704 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
+-rw-r--r--   0        0        0     1513 2024-04-19 20:34:02.861444 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc
+-rw-r--r--   0        0        0     1478 2024-04-19 20:33:58.205499 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py
+-rwxr-xr-x   0        0        0      754 2024-04-18 00:33:41.120405 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
+-rw-r--r--   0        0        0     1826 2024-04-19 18:56:22.468973 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-19 18:56:27.160910 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      996 2024-04-19 16:26:14.764114 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
+-rwxr-xr-x   0        0        0     9002 2024-04-19 20:36:06.236009 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
+-rwxr-xr-x   0        0        0     2930 2024-04-19 20:30:14.916104 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
+-rw-r--r--   0        0        0     1699 2024-04-19 20:33:08.038083 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      834 2024-04-16 20:48:34.547389 biotech-1.1.1/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
+-rwxr-xr-x   0        0        0      951 2024-04-16 20:49:56.266040 biotech-1.1.1/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      479 2024-04-16 20:49:28.130498 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1838 2024-04-19 16:27:13.567375 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      347 2024-04-16 20:48:34.555389 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/dynamic_port.py
+-rwxr-xr-x   0        0        0     2105 2024-04-19 16:26:14.612116 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/on.py
+-rwxr-xr-x   0        0        0     2201 2024-04-18 02:31:19.570492 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
+-rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
+-rwxr-xr-x   0        0        0     1441 2024-04-18 02:04:22.961501 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
+-rwxr-xr-x   0        0        0      774 2024-04-16 20:48:34.555389 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
+-rwxr-xr-x   0        0        0     1336 2024-04-15 21:13:32.676638 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      309 2024-04-17 23:41:26.722721 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      562 2024-04-17 23:41:26.734721 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      525 2024-04-17 23:09:55.764639 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      908 2024-04-19 20:05:11.362609 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      636 2024-04-18 01:15:59.039315 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      289 2024-04-17 23:05:28.138584 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
+-rwxr-xr-x   0        0        0      803 2024-04-19 20:05:09.858629 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
+-rwxr-xr-x   0        0        0      378 2024-04-18 01:13:51.928249 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
+-rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
+-rwxr-xr-x   0        0        0     2182 2024-04-18 01:57:52.896535 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
+-rwxr-xr-x   0        0        0     2125 2024-04-18 01:58:34.052216 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1027 2024-04-17 23:41:26.738721 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1368 2024-04-17 23:38:58.631806 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
+-rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
+-rwxr-xr-x   0        0        0      152 2024-04-19 16:48:50.419277 biotech-1.1.1/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3443 2024-04-19 20:02:47.664429 biotech-1.1.1/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.1/venues/stages/biotech/procedures/intro/intro.S.HTML
+-rwxr-xr-x   0        0        0     5074 2024-04-19 20:02:38.772528 biotech-1.1.1/venues/stages/biotech/procedures/intro/on.py
+-rw-r--r--   0        0        0     2887 2024-04-19 19:04:05.278996 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
+-rw-r--r--   0        0        0     3989 2024-04-19 19:03:05.467745 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/adventure.py
+-rwxr-xr-x   0        0        0     1267 2024-04-19 16:26:52.599637 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      905 2024-04-19 16:56:52.013564 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      901 2024-04-19 16:26:14.840113 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      614 2024-04-19 16:56:41.273688 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
+-rwxr-xr-x   0        0        0      138 2024-04-19 17:33:23.717242 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/intro.proc.py
+-rwxr-xr-x   0        0        0     3047 2024-04-19 19:04:01.875038 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/keg/__init__.py
+-rw-r--r--   0        0        0     3044 2024-04-19 19:04:05.278996 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/variables/__init__.py
+-rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321766 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       33 2024-04-17 22:47:27.362384 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/__init__.py
+-rwxr-xr-x   0        0        0      192 2024-04-17 22:47:29.166371 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1930 2024-04-19 16:45:15.609992 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3212 2024-04-19 16:26:52.583637 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/_ops/__pycache__/start.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4487 2024-04-19 16:26:14.828113 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/_ops/start.py
+-rwxr-xr-x   0        0        0     1267 2024-04-19 16:26:52.599637 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      855 2024-04-19 16:26:52.631636 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      901 2024-04-19 16:26:14.840113 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      572 2024-04-19 16:26:14.856113 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/send_paths.py
+-rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/intro.S.HTML
+-rwxr-xr-x   0        0        0     1991 2024-04-18 03:48:25.192521 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/keg/__init__.py
+-rwxr-xr-x   0        0        0     1394 2024-04-18 06:18:52.492292 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/keg/__init__v1.py
+-rwxr-xr-x   0        0        0     2895 2024-04-18 05:23:09.408255 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1447 2024-04-16 20:48:34.559388 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/keg/quart__init__.py
+-rwxr-xr-x   0        0        0     2039 2024-04-19 16:45:13.398021 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/on.py
+-rwxr-xr-x   0        0        0     4069 2024-04-19 16:41:30.225039 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/intro.proc.py
+-rwxr-xr-x   0        0        0     2819 2024-04-19 16:40:32.337866 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/keg/__init__.py
+-rwxr-xr-x   0        0        0     3015 2024-04-19 16:40:36.437807 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3062 2024-04-19 16:26:53.431626 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/moves/__pycache__/adventure.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4716 2024-04-19 16:26:14.896113 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/moves/adventure.py
+-rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/variables/__init__.py
+-rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321765 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      172 2024-04-16 20:48:34.551389 biotech-1.1.1/venues/stages/biotech/procedures/procedures.S.HTML
+-rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 biotech-1.1.1/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 biotech-1.1.1/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
+-rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 biotech-1.1.1/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 biotech-1.1.1/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 biotech-1.1.1/venues/stages/biotech/topics/aggregate/__init__.py
+-rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 biotech-1.1.1/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 biotech-1.1.1/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      708 2024-04-16 20:48:34.591388 biotech-1.1.1/venues/stages/biotech/topics/alarm_parser/__init__.py
+-rwxr-xr-x   0        0        0      673 2024-04-16 20:49:28.126498 biotech-1.1.1/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 biotech-1.1.1/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      405 2024-04-16 20:48:34.579388 biotech-1.1.1/venues/stages/biotech/topics/exceptions.py
+-rwxr-xr-x   0        0        0     1190 2024-01-27 05:31:08.525189 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
+-rwxr-xr-x   0        0        0     2446 2024-04-17 19:24:25.140060 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__init__.py
+-rwxr-xr-x   0        0        0     2491 2024-04-17 19:24:52.839918 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4471 2024-02-01 06:11:56.801715 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1050 2024-04-16 06:10:03.111579 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1920 2024-01-31 18:50:23.812071 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
+-rwxr-xr-x   0        0        0       24 2024-01-26 17:38:56.558087 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
+-rwxr-xr-x   0        0        0       24 2024-01-26 17:38:52.854129 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
+-rwxr-xr-x   0        0        0      751 2024-04-17 19:16:04.226583 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
+-rwxr-xr-x   0        0        0     1981 2024-04-17 19:25:47.591625 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__init__.py
+-rwxr-xr-x   0        0        0     2283 2024-04-17 19:25:53.011595 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4019 2024-01-31 18:51:47.652157 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3843 2024-04-17 19:25:53.099595 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4426 2024-01-27 06:34:32.979965 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3559 2024-04-17 19:25:22.227762 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/treasury.py
+-rwxr-xr-x   0        0        0     1727 2024-04-17 19:15:19.882965 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/shares.s.HTML
+-rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 biotech-1.1.1/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1558 2024-04-18 05:22:02.832642 biotech-1.1.1/venues/stages/biotech/topics/implicit/proc/__init__.py
+-rwxr-xr-x   0        0        0     1155 2024-04-18 05:46:33.436738 biotech-1.1.1/venues/stages/biotech/topics/implicit/thread/__init__.py
+-rwxr-xr-x   0        0        0      855 2024-04-18 06:05:23.346518 biotech-1.1.1/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       90 2024-04-17 22:51:08.968798 biotech-1.1.1/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 22:33:48.860256 biotech-1.1.1/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
+-rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 biotech-1.1.1/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
+-rwxr-xr-x   0        0        0      470 2024-04-17 23:02:14.419990 biotech-1.1.1/venues/stages/biotech/topics/printout/bracket.py
+-rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 biotech-1.1.1/venues/stages/biotech/topics/printout/passes.py
+-rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 biotech-1.1.1/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2163 2024-04-19 18:50:11.157390 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__init__.py
+-rw-r--r--   0        0        0     1997 2024-04-19 18:52:58.595432 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
+-rw-r--r--   0        0        0     1818 2024-04-19 18:54:33.250328 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-18 01:45:27.254200 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1766 2024-04-19 18:53:11.523281 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-18 01:48:34.504806 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-18 01:45:24.082223 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
+-rwxr-xr-x   0        0        0      195 2024-04-16 22:50:54.515336 biotech-1.1.1/venues/stages/biotech/topics/process_on/process_on.S.HTML
+-rwxr-xr-x   0        0        0     1470 2024-04-18 04:12:56.845888 biotech-1.1.1/venues/stages/biotech/topics/quay/garage.py
+-rwxr-xr-x   0        0        0     2546 2024-04-18 04:38:41.478278 biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_1.py
+-rwxr-xr-x   0        0        0     1612 2024-04-18 04:54:58.414971 biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_2.py
+-rwxr-xr-x   0        0        0      551 2024-04-18 05:20:40.701113 biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_3.py
+-rwxr-xr-x   0        0        0     1083 2024-04-18 05:19:11.645613 biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_4.py
+-rwxr-xr-x   0        0        0     1442 2024-04-16 20:48:34.591388 biotech-1.1.1/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
+-rwxr-xr-x   0        0        0     1464 2024-04-16 20:49:28.126498 biotech-1.1.1/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 biotech-1.1.1/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
+-rw-r--r--   0        0        0     1776 2024-04-19 19:50:41.332444 biotech-1.1.1/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0      461 2024-04-17 23:59:06.614967 biotech-1.1.1/venues/stages/biotech/topics/show/show.S.HTML
+-rwxr-xr-x   0        0        0     2305 2024-04-19 19:50:39.412465 biotech-1.1.1/venues/stages/biotech/topics/show/variable.py
+-rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
+-rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
+-rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
+-rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
+-rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
+-rwxr-xr-x   0        0        0      273 2024-04-16 20:48:34.583388 biotech-1.1.1/venues/stages/biotech/topics/start--/one.py
+-rwxr-xr-x   0        0        0      406 2024-04-16 20:48:34.587388 biotech-1.1.1/venues/stages/biotech/topics/start--/sequentially.py
+-rwxr-xr-x   0        0        0      532 2024-04-16 20:48:34.587388 biotech-1.1.1/venues/stages/biotech/topics/start--/simultaneously.py
+-rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 biotech-1.1.1/venues/stages/biotech/topics/topics.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 biotech-1.1.1/venues/stages/biotech/variables/__init__.py
+-rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.1/PKG-INFO
```

### Comparing `biotech-1.1.0/pyproject.toml` & `biotech-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 [tool.poetry]
 name = "biotech"
-version = "1.1.0"
+version = "1.1.1"
 description = "A health monitoring stack"
 authors = []
 readme = "readme.md"
 
 packages = [
     { include = "biotech", from = "venues/stages" }
 ]
```

### Comparing `biotech-1.1.0/readme.md` & `biotech-1.1.1/readme.md`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venue.S.HTML` & `biotech-1.1.1/venue.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg` & `biotech-1.1.1/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML` & `biotech-1.1.1/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/___itinerary/itinerary.S.HTML` & `biotech-1.1.1/venues/stages/biotech/___itinerary/itinerary.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/___itinerary/maybes.s.HTML` & `biotech-1.1.1/venues/stages/biotech/___itinerary/maybes.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout/start.py` & `biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout_v2/start.py` & `biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout_v2/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/__license/options/gpl-3.0-standalone.html` & `biotech-1.1.1/venues/stages/biotech/__license/options/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_book/advanced tutorial.s.HTML` & `biotech-1.1.1/venues/stages/biotech/_book/advanced tutorial.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_book/book.s.HTML` & `biotech-1.1.1/venues/stages/biotech/_book/book.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_book/relevant.s.HTML` & `biotech-1.1.1/venues/stages/biotech/_book/relevant.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_clique/__init__.py` & `biotech-1.1.1/venues/stages/biotech/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/DB/records.json` & `biotech-1.1.1/venues/stages/biotech/_status/DB/records.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996%*

 * *Differences: {"'_default'": "{'373': OrderedDict([('paths', [OrderedDict([('path', "*

 * *               "'_status/monitors/9_aggregation_format_and_exit/status_1.py'), ('empty', False), "*

 * *               "('parsed', True), ('stats', OrderedDict([('passes', 1), ('alarms', 0)])), "*

 * *               "('checks', [OrderedDict([('check', 'aggregation format and exit'), ('passed', "*

 * *               "True), ('elapsed', [5.123598545000277, 'seconds'])])])]), OrderedDict([('path', "*

 * *               "'_status/monitors/0_start/status_1.py') […]*

```diff
@@ -47115,14 +47115,604 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 14
                 },
                 "empty": 0
             }
         },
+        "373": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                5.123598545000277,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py",
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
+                                5.060430509998696,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/0_start/status_1.py",
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
+                                5.084781204997853,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4.1_bad_import/status_1.py",
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
+                                5.087485496998852,
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
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.087504283997987,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_bad_import/status_1.py",
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
+                                5.067970943000546,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/-1_start/status_1.py",
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
+                                5.15712831899873,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5__file__/status_1.py",
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
+                                3.1262471079971874,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_empty_glob/status_1.py",
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
+                                5.0429398640008,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/6_various/status_1.py",
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
+                                5.054823099999339,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2/status_1.py",
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
+                                5.124283929999365,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1/status_1.py",
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
+                                5.114799333001429,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/7/status_1.py",
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
+                                5.186842901999626,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/8_DB/status_1.py",
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
+                                9.071498438999697,
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
+        "374": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                9.121952779001731,
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
+        "375": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                5.118632326000807,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py",
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
+                                5.068774233997829,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/0_start/status_1.py",
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
+                                5.083116093999706,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4.1_bad_import/status_1.py",
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
+                                5.038675677002175,
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
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.087787518998084,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_bad_import/status_1.py",
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
+                                5.073999009000545,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/-1_start/status_1.py",
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
+                                5.181808789999195,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5__file__/status_1.py",
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
+                                3.154342693000217,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_empty_glob/status_1.py",
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
+                                5.044023749000189,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/6_various/status_1.py",
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
+                                5.0860596310012625,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2/status_1.py",
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
+                                5.138421331001155,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1/status_1.py",
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
+                                5.177556522998202,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/7/status_1.py",
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
+                                5.160560323998652,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/8_DB/status_1.py",
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
+                                9.07893609200255,
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
         "38": {
             "alarms": [],
             "paths": [
                 {
                     "empty": true,
                     "parsed": true,
                     "path": "_status/status_py.py"
```

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/establish.py` & `biotech-1.1.1/venues/stages/biotech/_status/establish.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/-1_start/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/-1_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/0_start/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/0_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/1/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/1/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/11/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/11/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/2/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/2/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/3_empty_glob/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/3_empty_glob/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/4.1_bad_import/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/4.1_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/4_bad_import/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/4_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/1_health.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/1_health.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/7/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/7/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/8_DB/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/8_DB/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/8_DB/variable/status_db/records.json` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/8_DB/variable/status_db/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'_default'": "{'223': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [1.2953998520970345e-05, 'seconds']), ('passed', "*

 * *               "True)])]), ('empty', False), ('parsed', True), ('path', 'guarantee_1.py'), "*

 * *               "('records', ['proceeds None\\r\\n', 'checks in module True\\r\\n', 'check "*

 * *               '1\\r\\n\', \'{\\r\\n\', "    \'path\': \\r\\n", '*

 * *               '"\'/biotech/venues/stages/biotech/procedures/health_scan […]*

```diff
@@ -4796,14 +4796,132 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 1
                 },
                 "empty": 0
             }
         },
+        "223": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.2953998520970345e-05,
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
+                        "    'path': \r\n",
+                        "'/biotech/venues/stages/biotech/procedures/health_scan/process/modules/__health_\r\n",
+                        "scan_utilities/show/variable.py',\r\n",
+                        "    'line': 50,\r\n",
+                        "    'variable': {\r\n",
+                        "        'pid': 6712,\r\n",
+                        "        'proceeds': {\r\n",
+                        "            'empty': False,\r\n",
+                        "            'parsed': True,\r\n",
+                        "            'stats': {'passes': 1, 'alarms': 0},\r\n",
+                        "            'checks': [\r\n",
+                        "                {\r\n",
+                        "                    'check': 'check 1',\r\n",
+                        "                    'passed': True,\r\n",
+                        "                    'elapsed': [1.2953998520970345e-05, 'seconds']\r\n",
+                        "                }\r\n",
+                        "            ]\r\n",
+                        "        },\r\n",
+                        "        'harbor': {'host': '0.0.0.0', 'port': 52435}\r\n",
+                        "    }\r\n",
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
+        "224": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.0406998626422137e-05,
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
+                        "    'path': \r\n",
+                        "'/biotech/venues/stages/biotech/procedures/health_scan/process/modules/__health_\r\n",
+                        "scan_utilities/show/variable.py',\r\n",
+                        "    'line': 50,\r\n",
+                        "    'variable': {\r\n",
+                        "        'pid': 7318,\r\n",
+                        "        'proceeds': {\r\n",
+                        "            'empty': False,\r\n",
+                        "            'parsed': True,\r\n",
+                        "            'stats': {'passes': 1, 'alarms': 0},\r\n",
+                        "            'checks': [\r\n",
+                        "                {\r\n",
+                        "                    'check': 'check 1',\r\n",
+                        "                    'passed': True,\r\n",
+                        "                    'elapsed': [1.0406998626422137e-05, 'seconds']\r\n",
+                        "                }\r\n",
+                        "            ]\r\n",
+                        "        },\r\n",
+                        "        'harbor': {'host': '0.0.0.0', 'port': 52435}\r\n",
+                        "    }\r\n",
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
         "23": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
```

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status/status.proc.py` & `biotech-1.1.1/venues/stages/biotech/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py` & `biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json` & `biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/_status_advanced/status.proc.py` & `biotech-1.1.1/venues/stages/biotech/_status_advanced/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/architecture.s.HTML` & `biotech-1.1.1/venues/stages/biotech/architecture.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/module.s.HTML` & `biotech-1.1.1/venues/stages/biotech/module.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/on.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/on.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,19 +43,15 @@
 #
 #----
 
 def aggregator_procedure_on (
 	port,
 	packet
 ):
-	show_variable ("""
-	
-	aggregator_procedure_on
-	
-	""")
+	show_variable ("""aggregator_procedure_on""")
 
 	limit_start = 25000
 		
 	path_of_the_scan_process = find_aggregator_procedure_paths ()
 	process_string = (
 		f'''python3 { path_of_the_scan_process } keg open --port { port }'''
 	)
@@ -72,14 +68,14 @@
 		env = process_environment,
 		name = "aggregator"
 	)
 	
 	time.sleep (1)
 	show_variable ({
 		'the aggregator procedure:': the_venture
-	}, mode = "show")
+	}, mode = "condensed")
 
 	return the_venture
```

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 	the_path = the_packet ["path"]
 	the_result = the_packet ["result"]
 	#the_pid = the_packet ["pid"]
 	
 	
 	show_variable ({
 		"done with scan, stopping:": the_packet
-	}, mode = "show")
+	}, mode = "condensed")
 
 
 	#---
 	#
 	#	Once the status of the scan has been established,
 	# 	then the scan process can be stopped.
 	#
@@ -64,15 +64,14 @@
 	#----
 	
 	show_variable ({
 		"times": aggregator_variables ["internal_statuses"] [ the_path ] ["times"]
 	}, mode = "show")
 	
 	
-	
 	try:
 		aggregator_variables ["internal_statuses"] [ the_path ] ["records"] = parse_p_expect_records (
 			records = aggregator_variables ["internal_statuses"] [ the_path ] ["process"] ["records"] (),
 			format = "UTF8"
 		)
 	except Exception:
 		show_variable ("The records could not be parsed!")
```

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 19:38:19 2024 UTC, .py size: 8610 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,253 +1,249 @@
-00000000: 6f0d 0d0a 0000 0000 2bc8 2266 a221 0000  o.......+."f.!..
+00000000: 6f0d 0d0a 0000 0000 b6d5 2266 2a23 0000  o........."f*#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6404 6405 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6406 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6407 6c08 6d09 5a09 0100 6400 6408 6c0a  d.l.m.Z...d.d.l.
-00000070: 6d0a 5a0a 0100 6400 6409 6c0b 5a0b 6400  m.Z...d.d.l.Z.d.
-00000080: 6409 6c0c 5a0c 6400 6409 6c0d 5a0d 0900  d.l.Z.d.d.l.Z...
-00000090: 640a 640b 8400 5a0e 6409 5300 290c e900  d.d...Z.d.S.)...
+00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6405 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6406 6c08 6d09 5a09 0100 6400 6407 6c0a  d.l.m.Z...d.d.l.
+00000070: 6d0a 5a0a 0100 6400 6408 6c0b 5a0b 6400  m.Z...d.d.l.Z.d.
+00000080: 6408 6c0c 5a0c 6400 6408 6c0d 5a0d 0900  d.l.Z.d.d.l.Z...
+00000090: 6409 640a 8400 5a0e 6408 5300 290b e900  d.d...Z.d.S.)...
 000000a0: 0000 0029 01da 1272 6574 7269 6576 655f  ...)...retrieve_
-000000b0: 7661 7269 6162 6c65 73e9 0200 0000 2901  variables.....).
-000000c0: da13 646f 6e65 5f77 6974 685f 7363 616e  ..done_with_scan
-000000d0: 5f6d 6f76 65e9 0100 0000 2901 da0e 6174  _move.....)...at
-000000e0: 7461 6368 5f72 6563 6f72 6473 2901 da16  tach_records)...
-000000f0: 7061 7273 655f 705f 6578 7065 6374 5f72  parse_p_expect_r
-00000100: 6563 6f72 6473 2901 da0d 7368 6f77 5f76  ecords)...show_v
-00000110: 6172 6961 626c 6529 01da 0670 7072 696e  ariable)...pprin
-00000120: 744e 6300 0000 0000 0000 0000 0000 000e  tNc.............
-00000130: 0000 000b 0000 0043 0000 0073 d005 0000  .......C...s....
-00000140: 7400 8300 7d00 7c00 6401 1900 7d01 7c00  t...}.|.d...}.|.
-00000150: 6402 1900 7d02 0900 7c00 6403 1900 6404  d...}...|.d...d.
-00000160: 1900 7d03 6900 7d04 6700 7d05 7c02 4400  ..}.i.}.g.}.|.D.
-00000170: 9002 5daf 7d06 7c02 7c06 1900 7d07 7c07  ..].}.|.|...}.|.
-00000180: 6405 1900 7d08 0900 7a2d 6406 7c02 7c06  d...}...z-d.|.|.
-00000190: 1900 6406 1900 7600 7250 7401 7c02 7c06  ..d...v.rPt.|.|.
-000001a0: 1900 6406 1900 6406 1900 8301 6400 6b03  ..d...d.....d.k.
-000001b0: 7250 7c02 7c06 1900 6406 1900 6406 1900  rP|.|...d...d...
-000001c0: a002 a100 7d09 7c09 6407 6b02 724c 6408  ....}.|.d.k.rLd.
-000001d0: 7c08 6409 3c00 6e04 640a 7c08 6409 3c00  |.d.<.n.d.|.d.<.
-000001e0: 5700 6e1b 0400 7403 796c 0100 7d0a 0100  W.n...t.yl..}...
-000001f0: 7a0f 7404 640b 7c0a 8302 0100 640c 7c08  z.t.d.|.....d.|.
-00000200: 6409 3c00 5700 5900 6400 7d0a 7e0a 6e05  d.<.W.Y.d.}.~.n.
-00000210: 6400 7d0a 7e0a 7701 7700 7405 7c06 8301  d.}.~.w.w.t.|...
-00000220: 0100 0900 7a50 7c08 640d 1900 6408 6b02  ....zP|.d...d.k.
-00000230: 72c1 7c08 6409 1900 6408 6b02 72c1 7c08  r.|.d...d.k.r.|.
-00000240: 640e 1900 640a 6b02 72c1 7406 7c02 7c06  d...d.k.r.t.|.|.
-00000250: 1900 640f 1900 6410 1900 8301 6411 6b05  ..d...d.....d.k.
-00000260: 72c1 7407 a007 a100 7408 7c02 7c06 1900  r.t.....t.|.|...
-00000270: 640f 1900 6410 1900 8301 1800 7408 7c03  d...d.......t.|.
-00000280: 8301 6b05 72c1 7a08 7c02 7c06 1900 6412  ..k.r.z.|.|...d.
-00000290: 1900 7d0b 5700 6e0b 0400 7403 79b6 0100  ..}.W.n...t.y...
-000002a0: 0100 0100 6413 7d0b 5900 6e01 7700 7409  ....d.}.Y.n.w.t.
-000002b0: 7c06 6414 7c0b 6415 9c02 6416 9c02 8301  |.d.|.d...d.....
-000002c0: 0100 5700 6e19 0400 7403 79db 0100 7d0a  ..W.n...t.y...}.
-000002d0: 0100 7a0d 7404 6417 740a a00b a100 8302  ..z.t.d.t.......
-000002e0: 0100 5700 5900 6400 7d0a 7e0a 6e05 6400  ..W.Y.d.}.~.n.d.
-000002f0: 7d0a 7e0a 7701 7700 0900 7a63 7c08 6418  }.~.w.w...zc|.d.
-00000300: 1900 6408 6b02 9001 723f 7c08 6419 1900  ..d.k...r?|.d...
-00000310: 640a 6b02 9001 723f 7407 a007 a100 7408  d.k...r?t.....t.
-00000320: 7c02 7c06 1900 640f 1900 641a 1900 8301  |.|...d...d.....
-00000330: 1800 7d0c 740c 641b 7c0c 6901 8301 0100  ..}.t.d.|.i.....
-00000340: 7c0c 641c 6b05 9001 723f 740c 641d 7c06  |.d.k...r?t.d.|.
-00000350: 6901 8301 0100 7c06 641e 641f 6701 6407  i.....|.d.d.g.d.
-00000360: 6420 9c04 7c00 6402 1900 7c06 1900 6421  d ..|.d...|...d!
-00000370: 3c00 6422 7c00 6402 1900 7c06 1900 6423  <.d"|.d...|...d#
-00000380: 1900 6406 3c00 6424 7c00 6402 1900 7c06  ..d.<.d$|.d...|.
-00000390: 1900 6405 1900 6425 3c00 7c00 6402 1900  ..d...d%<.|.d...
-000003a0: 7c06 1900 6406 1900 6406 1900 a00d a100  |...d...d.......
-000003b0: 0100 740c 6426 7c06 6901 8301 0100 5700  ..t.d&|.i.....W.
-000003c0: 6e1a 0400 7403 9001 795a 0100 7d0a 0100  n...t...yZ..}...
-000003d0: 7a0d 7404 6427 740a a00b a100 8302 0100  z.t.d't.........
-000003e0: 5700 5900 6400 7d0a 7e0a 6e05 6400 7d0a  W.Y.d.}.~.n.d.}.
-000003f0: 7e0a 7701 7700 0900 7abd 0900 7c08 640d  ~.w.w...z...|.d.
-00000400: 1900 6408 6b02 7c08 6409 1900 6408 6b02  ..d.k.|.d...d.k.
-00000410: 7c08 640e 1900 640a 6b02 7406 7c02 7c06  |.d...d.k.t.|.|.
-00000420: 1900 640f 1900 641a 1900 8301 6411 6b05  ..d...d.....d.k.
-00000430: 7406 7c02 7c06 1900 6412 1900 8301 6428  t.|.|...d.....d(
-00000440: 6b02 7407 a007 a100 7408 7c02 7c06 1900  k.t.....t.|.|...
-00000450: 640f 1900 641a 1900 8301 1800 6429 9c06  d...d.......d)..
-00000460: 7d0d 0900 7c08 640d 1900 6408 6b02 9002  }...|.d...d.k...
-00000470: 7218 7c08 6409 1900 6408 6b02 9002 7218  r.|.d...d.k...r.
-00000480: 7c08 640e 1900 640a 6b02 9002 7218 7406  |.d...d.k...r.t.
-00000490: 7c02 7c06 1900 640f 1900 641a 1900 8301  |.|...d...d.....
-000004a0: 6411 6b05 9002 7218 7406 7c02 7c06 1900  d.k...r.t.|.|...
-000004b0: 6412 1900 8301 6428 6b02 9002 7218 7407  d.....d(k...r.t.
-000004c0: a007 a100 7408 7c02 7c06 1900 640f 1900  ....t.|.|...d...
-000004d0: 641a 1900 8301 1800 7d0c 740c 642a 7c0c  d.......}.t.d*|.
-000004e0: 6901 8301 0100 7c0c 642b 6b05 9002 7218  i.....|.d+k...r.
-000004f0: 740c 642c 7c06 6901 8301 0100 7a08 7c02  t.d,|.i.....z.|.
-00000500: 7c06 1900 642d 1900 7d08 5700 6e0c 0400  |...d-..}.W.n...
-00000510: 7403 9001 79f2 0100 0100 0100 6413 7d08  t...y.......d.}.
-00000520: 5900 6e01 7700 7c06 641e 642e 6701 7c08  Y.n.w.|.d.d.g.|.
-00000530: 6407 642f 9c05 7c00 6402 1900 7c06 1900  d.d/..|.d...|...
-00000540: 6421 3c00 6422 7c00 6402 1900 7c06 1900  d!<.d"|.d...|...
-00000550: 6423 1900 6406 3c00 7c00 6402 1900 7c06  d#..d.<.|.d...|.
-00000560: 1900 6406 1900 6406 1900 a00d a100 0100  ..d...d.........
-00000570: 5700 6e18 0400 7403 9002 7931 0100 7d0a  W.n...t...y1..}.
-00000580: 0100 7a0b 7404 6430 7c0a 8302 0100 5700  ..z.t.d0|.....W.
-00000590: 5900 6400 7d0a 7e0a 6e05 6400 7d0a 7e0a  Y.d.}.~.n.d.}.~.
-000005a0: 7701 7700 0900 7a36 7c08 640d 1900 6408  w.w...z6|.d...d.
-000005b0: 6b02 9002 7268 7c08 6419 1900 6408 6b02  k...rh|.d...d.k.
-000005c0: 9002 7268 7c08 640e 1900 640a 6b02 9002  ..rh|.d...d.k...
-000005d0: 7268 7c08 6409 1900 6408 6b03 9002 7268  rh|.d...d.k...rh
-000005e0: 7c06 6431 6700 7c08 6407 6432 9c05 7c00  |.d1g.|.d.d2..|.
-000005f0: 6402 1900 7c06 1900 6421 3c00 6422 7c00  d...|...d!<.d"|.
-00000600: 6402 1900 7c06 1900 6423 1900 6406 3c00  d...|...d#..d.<.
-00000610: 5700 6e1a 0400 7403 9002 7983 0100 7d0a  W.n...t...y...}.
-00000620: 0100 7a0d 7404 6433 740a a00b a100 8302  ..z.t.d3t.......
-00000630: 0100 5700 5900 6400 7d0a 7e0a 6e05 6400  ..W.Y.d.}.~.n.d.
-00000640: 7d0a 7e0a 7701 7700 0900 0900 7a28 7c08  }.~.w.w.....z(|.
-00000650: 6409 1900 640a 6b02 9002 72ad 7c08 640d  d...d.k...r.|.d.
-00000660: 1900 6408 6b02 9002 72ad 7c08 640e 1900  ..d.k...r.|.d...
-00000670: 6408 6b02 9002 72ad 7c08 6434 1900 6408  d.k...r.|.d4..d.
-00000680: 6b02 9002 72ad 6422 7c00 6402 1900 7c06  k...r.d"|.d...|.
-00000690: 1900 6423 1900 6406 3c00 5700 7118 0400  ..d#..d.<.W.q...
-000006a0: 7403 9002 79c8 0100 7d0a 0100 7a0d 7404  t...y...}...z.t.
-000006b0: 6433 740a a00b a100 8302 0100 5700 5900  d3t.........W.Y.
-000006c0: 6400 7d0a 7e0a 7118 6400 7d0a 7e0a 7701  d.}.~.q.d.}.~.w.
-000006d0: 7700 7c02 4400 5d1a 7d06 7c02 7c06 1900  w.|.D.].}.|.|...
-000006e0: 6423 1900 6406 1900 6422 6b03 9002 72e4  d#..d...d"k...r.
-000006f0: 7c05 a00e 7c06 7c00 6402 1900 7c06 1900  |...|.|.d...|...
-00000700: 6435 9c02 a101 0100 9002 71cb 7c05 5300  d5........q.|.S.
-00000710: 2936 4eda 0d72 6563 6f72 6473 5f6c 6576  )6N..records_lev
-00000720: 656c da11 696e 7465 726e 616c 5f73 7461  el..internal_sta
-00000730: 7475 7365 73da 0f69 6e74 726f 5f76 6172  tuses..intro_var
-00000740: 6961 626c 6573 da0a 7469 6d65 5f6c 696d  iables..time_lim
-00000750: 6974 da0b 6f63 6375 7272 656e 6365 73da  it..occurrences.
-00000760: 0770 726f 6365 7373 54da 0379 6573 7a15  .processT..yesz.
-00000770: 7363 616e 2070 726f 6365 7373 2069 7320  scan process is 
-00000780: 616c 6976 65da 026e 6f7a 1e70 726f 6365  alive..noz.proce
-00000790: 7373 2061 6c69 7665 2063 6865 636b 2065  ss alive check e
-000007a0: 7863 6570 7469 6f6e 3ada 0775 6e6b 6e6f  xception:..unkno
-000007b0: 776e 7a14 7363 616e 2070 726f 6365 7373  wnz.scan process
-000007c0: 2073 7461 7274 6564 7a18 7363 616e 2070   startedz.scan p
-000007d0: 726f 6365 7373 2077 6173 2073 746f 7070  rocess was stopp
-000007e0: 6564 da05 7469 6d65 73da 0773 7461 7274  ed..times..start
-000007f0: 6564 7205 0000 00da 0772 6563 6f72 6473  edr......records
-00000800: 7a09 6e6f 7420 666f 756e 647a 1374 696d  z.not foundz.tim
-00000810: 6520 6c69 6d69 7420 6578 6365 6564 6564  e limit exceeded
-00000820: 2902 da05 616c 6172 6d7a 0b74 6865 2072  )...alarmz.the r
-00000830: 6563 6f72 6473 2902 da04 7061 7468 da06  ecords)...path..
-00000840: 7265 7375 6c74 7a1b 7469 6d65 206c 696d  resultz.time lim
-00000850: 6974 2063 6865 636b 2065 7863 6570 7469  it check excepti
-00000860: 6f6e 3a7a 1c73 6361 6e20 7072 6f63 6573  on:z.scan proces
-00000870: 7320 7665 6e74 7572 6520 7374 6172 7465  s venture starte
-00000880: 647a 2073 6361 6e20 7072 6f63 6573 7320  dz scan process 
-00000890: 6e6f 7469 6669 6564 2061 6767 7265 6761  notified aggrega
-000008a0: 746f 727a 0f76 656e 7475 7265 2073 7461  torz.venture sta
-000008b0: 7274 6564 7a1d 656c 6170 7365 6420 7769  rtedz.elapsed wi
-000008c0: 7468 6f75 7420 6e6f 7469 6669 6361 7469  thout notificati
-000008d0: 6f6e 3ae9 0500 0000 7a1e 6174 7465 6d70  on:.....z.attemp
-000008e0: 7469 6e67 2074 6f20 7374 6f70 2074 6865  ting to stop the
-000008f0: 2070 726f 6365 7373 7a3f 5468 6572 6520   processz?There 
-00000900: 7761 7320 6d6f 7374 206c 696b 656c 7920  was most likely 
-00000910: 616e 2069 6e74 6572 6e61 6c20 7072 6f62  an internal prob
-00000920: 6c65 6d20 7374 6172 7469 6e67 2074 6865  lem starting the
-00000930: 2070 726f 6365 7373 2e7a 4f41 6674 6572   process.zOAfter
-00000940: 2035 2073 6563 6f6e 6473 2c20 7468 6520   5 seconds, the 
-00000950: 7072 6f63 6573 7320 6469 6420 6e6f 7420  process did not 
-00000960: 6e6f 7469 6679 2074 6865 2061 6767 7265  notify the aggre
-00000970: 6761 746f 7220 7468 6174 2069 7420 6861  gator that it ha
-00000980: 6420 7374 6172 7465 642e 2904 7217 0000  d started.).r...
-00000990: 0072 1600 0000 fa0b 616c 6172 6d20 6e6f  .r......alarm no
-000009a0: 7465 73da 0665 7869 7465 64da 0f72 6573  tes..exited..res
-000009b0: 756c 7473 5f6f 665f 7363 616e da04 646f  ults_of_scan..do
-000009c0: 6e65 da06 7374 6174 7573 7a3a 5468 6520  ne..statusz:The 
-000009d0: 7072 6f63 6573 7320 6469 646e 2774 206e  process didn't n
-000009e0: 6f74 6966 7920 7468 6520 6167 6772 6567  otify the aggreg
-000009f0: 6174 6f72 2077 6974 6869 6e20 3520 7365  ator within 5 se
-00000a00: 636f 6e64 732e 7a10 646f 6e65 2072 6561  conds.z.done rea
-00000a10: 736f 6e20 6769 7665 7a18 7072 6f63 6573  son givez.proces
-00000a20: 7320 6d61 7920 6861 7665 2073 746f 7070  s may have stopp
-00000a30: 6564 7a23 7072 6f63 6573 7320 6e6f 6e2d  edz#process non-
-00000a40: 6e6f 7469 6669 6361 7469 6f6e 2065 7863  notification exc
-00000a50: 6570 7469 6f6e 3a72 0100 0000 2906 da01  eption:r....)...
-00000a60: 31da 0132 da01 33da 0134 da01 36da 0137  1..2..3..4..6..7
-00000a70: da07 656c 6170 7365 64e9 0a00 0000 7a2b  ..elapsed.....z+
-00000a80: 7265 636f 7264 7320 7765 7265 206e 6f74  records were not
-00000a90: 2072 6574 7269 6576 6564 2061 6674 6572   retrieved after
-00000aa0: 2031 3020 7365 636f 6e64 73da 0a6f 6363   10 seconds..occ
-00000ab0: 7572 656e 6365 737a 2d41 6674 6572 2031  urencesz-After 1
-00000ac0: 3020 7365 636f 6e64 732c 206e 6f20 7072  0 seconds, no pr
-00000ad0: 6f63 6573 7320 6c6f 6773 2077 6572 6520  ocess logs were 
-00000ae0: 666f 756e 642e 2905 7217 0000 0072 1600  found.).r....r..
-00000af0: 0000 721a 0000 0072 2700 0000 721b 0000  ..r....r'...r...
-00000b00: 007a 2870 726f 6365 7373 206c 6f67 7320  .z(process logs 
-00000b10: 7469 6d65 206c 696d 6974 2063 6865 636b  time limit check
-00000b20: 2065 7863 6570 7469 6f6e 3a7a 3054 6865   exception:z0The
-00000b30: 2070 726f 6365 7373 2065 7869 7465 6420   process exited 
-00000b40: 6265 666f 7265 2072 6573 756c 7473 2063  before results c
-00000b50: 6f75 6c64 2062 6520 7365 6e74 2e29 0572  ould be sent.).r
-00000b60: 1700 0000 7216 0000 0072 1a00 0000 720e  ....r....r....r.
-00000b70: 0000 0072 1b00 0000 7a1a 7061 7273 6520  ...r....z.parse 
-00000b80: 616e 6420 6368 6563 6b20 6578 6365 7074  and check except
-00000b90: 696f 6e3a 7a1b 7363 616e 2072 6563 6f72  ion:z.scan recor
-00000ba0: 6473 2077 6572 6520 7265 7472 6965 7665  ds were retrieve
-00000bb0: 6429 0272 1700 0000 da09 696e 7465 726e  d).r......intern
-00000bc0: 616c 7329 0f72 0200 0000 da04 7479 7065  als).r......type
-00000bd0: da08 6973 5f61 6c69 7665 da09 4578 6365  ..is_alive..Exce
-00000be0: 7074 696f 6eda 0570 7269 6e74 7206 0000  ption..printr...
-00000bf0: 00da 036c 656e da04 7469 6d65 da05 666c  ...len..time..fl
-00000c00: 6f61 7472 0400 0000 da09 7472 6163 6562  oatr......traceb
-00000c10: 6163 6bda 0a66 6f72 6d61 745f 6578 6372  ack..format_excr
-00000c20: 0800 0000 da09 7465 726d 696e 6174 65da  ......terminate.
-00000c30: 0661 7070 656e 6429 0eda 1461 6767 7265  .append)...aggre
-00000c40: 6761 746f 725f 7661 7269 6162 6c65 7372  gator_variablesr
-00000c50: 0a00 0000 720b 0000 0072 0d00 0000 da08  ....r....r......
-00000c60: 7374 6174 7573 6573 da0a 756e 6669 6e69  statuses..unfini
-00000c70: 7368 6564 da0b 7374 6174 7573 5f70 6174  shed..status_pat
-00000c80: 68da 0e73 7461 7475 735f 6f66 5f70 6174  h..status_of_pat
-00000c90: 6872 0e00 0000 da05 616c 6976 65da 0145  hr......alive..E
-00000ca0: da10 7468 655f 7363 616e 5f72 6563 6f72  ..the_scan_recor
-00000cb0: 6473 7225 0000 00da 0564 6f6f 7273 a900  dsr%.....doors..
-00000cc0: 723d 0000 00fa 712f 6269 6f74 6563 682f  r=....q/biotech/
-00000cd0: 7665 6e75 6573 2f73 7461 6765 732f 6269  venues/stages/bi
-00000ce0: 6f74 6563 682f 7072 6f63 6564 7572 6573  otech/procedures
-00000cf0: 2f61 6767 7265 6761 746f 725f 7072 6f63  /aggregator_proc
-00000d00: 6564 7572 652f 7072 6f63 6573 732f 6d6f  edure/process/mo
-00000d10: 7665 732f 7374 6174 7573 5f63 6865 636b  ves/status_check
-00000d20: 5f6d 6f6e 6974 6f72 2f74 6865 5f70 6879  _monitor/the_phy
-00000d30: 7369 6361 6c2e 7079 da24 7061 7273 655f  sical.py.$parse_
-00000d40: 616e 645f 6368 6563 6b5f 6973 5f61 6c69  and_check_is_ali
-00000d50: 7665 5f6f 665f 7374 6174 7573 6573 1f00  ve_of_statuses..
-00000d60: 0000 7348 0100 0006 0108 0208 0202 020c  ..sH............
-00000d70: 0604 0204 010a 0108 0208 0102 0202 0410  ................
-00000d80: 0118 0114 0108 010a 0108 0204 800e 020a  ................
-00000d90: 0114 0308 8002 fc08 0702 0402 040c 020c  ................
-00000da0: 010c 0118 0124 0202 0210 010c 0108 0102  .....$..........
-00000db0: ff02 0302 0102 0202 0104 fe08 fe04 800e  ................
-00000dc0: 080e 010c 0108 8002 fe02 0602 070e 020e  ................
-00000dd0: 011c 0202 0204 0106 ff0a 0402 0104 0106  ................
-00000de0: ff02 0702 0202 0202 ff02 0412 f814 0b14  ................
-00000df0: 0118 0202 0204 0106 ff04 8010 050e 010c  ................
-00000e00: 0108 8002 fe02 0502 1202 010a 070a 010a  ................
-00000e10: 0116 0112 011a 0106 fa02 090e 080e 010e  ................
-00000e20: 011a 0116 021c 0202 0204 0106 ff0a 0402  ................
-00000e30: 0104 0106 ff02 0410 010e 0108 0102 ff02  ................
-00000e40: 0402 0202 0202 ff02 0402 0212 f614 0d18  ................
-00000e50: 0104 8010 040a 010c 0108 8002 fe02 0602  ................
-00000e60: 0c0e 020e 010e 020e 0202 0302 0202 0102  ................
-00000e70: 0102 0212 f914 0a04 8010 020e 010c 0108  ................
-00000e80: 8002 fe02 0502 0902 030e 020e 020e 010e  ................
-00000e90: 0114 0204 8010 020e 010c 0108 8002 fe08  ................
-00000ea0: 0616 0104 0102 010a 0108 fe04 8004 0672  ...............r
-00000eb0: 3f00 0000 290f da39 6269 6f74 6563 682e  ?...)..9biotech.
-00000ec0: 7072 6f63 6564 7572 6573 2e61 6767 7265  procedures.aggre
-00000ed0: 6761 746f 725f 7072 6f63 6564 7572 652e  gator_procedure.
-00000ee0: 7072 6f63 6573 732e 7661 7269 6162 6c65  process.variable
-00000ef0: 7372 0200 0000 da0e 646f 6e65 5f77 6974  sr......done_wit
-00000f00: 685f 7363 616e 7204 0000 0072 1500 0000  h_scanr....r....
-00000f10: 7206 0000 00da 3062 696f 7465 6368 2e74  r.....0biotech.t
-00000f20: 6f70 6963 732e 7072 6f63 6573 735f 6f6e  opics.process_on
-00000f30: 2e70 5f65 7870 6563 742e 7061 7273 655f  .p_expect.parse_
-00000f40: 7265 636f 7264 7372 0700 0000 da1c 6269  recordsr......bi
-00000f50: 6f74 6563 682e 746f 7069 6373 2e73 686f  otech.topics.sho
-00000f60: 772e 7661 7269 6162 6c65 7208 0000 0072  w.variabler....r
-00000f70: 0900 0000 722e 0000 0072 3000 0000 da04  ....r....r0.....
-00000f80: 7269 6368 723f 0000 0072 3d00 0000 723d  richr?...r=...r=
-00000f90: 0000 0072 3d00 0000 723e 0000 00da 083c  ...r=...r>.....<
-00000fa0: 6d6f 6475 6c65 3e01 0000 0073 1600 0000  module>....s....
-00000fb0: 0c07 0c01 0c02 0c02 0c01 0c03 0801 0801  ................
-00000fc0: 0803 0205 0c04                           ......
+000000b0: 7661 7269 6162 6c65 73e9 0100 0000 2901  variables.....).
+000000c0: da0e 6174 7461 6368 5f72 6563 6f72 6473  ..attach_records
+000000d0: 2901 da27 6c65 6172 6e5f 6966 5f67 6c6f  )..'learn_if_glo
+000000e0: 6261 6c5f 7469 6d65 5f6c 696d 6974 5f77  bal_time_limit_w
+000000f0: 6173 5f65 7863 6565 6465 6429 01da 1670  as_exceeded)...p
+00000100: 6172 7365 5f70 5f65 7870 6563 745f 7265  arse_p_expect_re
+00000110: 636f 7264 7329 01da 0d73 686f 775f 7661  cords)...show_va
+00000120: 7269 6162 6c65 2901 da06 7070 7269 6e74  riable)...pprint
+00000130: 4e63 0000 0000 0000 0000 0000 0000 0d00  Nc..............
+00000140: 0000 0b00 0000 4300 0000 7312 0600 0074  ......C...s....t
+00000150: 0083 007d 007c 0064 0119 007d 017c 0064  ...}.|.d...}.|.d
+00000160: 0219 007d 027c 0064 0319 0064 0419 007d  ...}.|.d...d...}
+00000170: 0369 007d 0467 007d 057c 0244 0090 025d  .i.}.g.}.|.D...]
+00000180: d17d 067c 027c 0619 007d 077c 0764 0519  .}.|.|...}.|.d..
+00000190: 007d 0809 007a 2d64 067c 027c 0619 0064  .}...z-d.|.|...d
+000001a0: 0619 0076 0072 4f74 017c 027c 0619 0064  ...v.rOt.|.|...d
+000001b0: 0619 0064 0619 0083 0164 006b 0372 4f7c  ...d.....d.k.rO|
+000001c0: 027c 0619 0064 0619 0064 0619 00a0 02a1  .|...d...d......
+000001d0: 007d 097c 0964 076b 0272 4b64 087c 0864  .}.|.d.k.rKd.|.d
+000001e0: 093c 006e 0464 0a7c 0864 093c 0057 006e  .<.n.d.|.d.<.W.n
+000001f0: 1b04 0074 0379 6b01 007d 0a01 007a 0f74  ...t.yk..}...z.t
+00000200: 0464 0b7c 0a83 0201 0064 0c7c 0864 093c  .d.|.....d.|.d.<
+00000210: 0057 0059 0064 007d 0a7e 0a6e 0564 007d  .W.Y.d.}.~.n.d.}
+00000220: 0a7e 0a77 0177 0074 057c 0683 0101 0074  .~.w.w.t.|.....t
+00000230: 067c 0683 0101 0009 007a 6e7c 0864 0d19  .|.......zn|.d..
+00000240: 0064 086b 0272 e27c 0864 0e19 0064 0a6b  .d.k.r.|.d...d.k
+00000250: 0272 e27c 0864 0f19 0064 0a6b 0272 e274  .r.|.d...d.k.r.t
+00000260: 07a0 07a1 0074 087c 027c 0619 0064 1019  .....t.|.|...d..
+00000270: 0064 1119 0083 0118 007d 0b7c 0b64 126b  .d.......}.|.d.k
+00000280: 0572 e27a 087c 027c 0619 0064 1319 007d  .r.z.|.|...d...}
+00000290: 0857 006e 0b04 0074 0379 ad01 0001 0001  .W.n...t.y......
+000002a0: 0064 147d 0859 006e 0177 007c 0664 1567  .d.}.Y.n.w.|.d.g
+000002b0: 007c 0864 0764 169c 057c 0064 0219 007c  .|.d.d...|.d...|
+000002c0: 0619 0064 173c 0064 187c 0064 0219 007c  ...d.<.d.|.d...|
+000002d0: 0619 0064 1919 0064 063c 0064 1a7c 0064  ...d...d.<.d.|.d
+000002e0: 0219 007c 0619 0064 0519 0064 1b3c 007c  ...|...d...d.<.|
+000002f0: 0064 0219 007c 0619 0064 0619 0064 0619  .d...|...d...d..
+00000300: 00a0 09a1 0001 0074 0a64 1c7c 0669 0183  .......t.d.|.i..
+00000310: 0101 0057 006e 1904 0074 0379 fc01 007d  ...W.n...t.y...}
+00000320: 0a01 007a 0d74 0464 1d74 0ba0 0ca1 0083  ...z.t.d.t......
+00000330: 0201 0057 0059 0064 007d 0a7e 0a6e 0564  ...W.Y.d.}.~.n.d
+00000340: 007d 0a7e 0a77 0177 0009 007a 6c7c 0864  .}.~.w.w...zl|.d
+00000350: 0e19 0064 086b 0290 0172 697c 0864 0f19  ...d.k...ri|.d..
+00000360: 0064 0a6b 0290 0172 6974 07a0 07a1 0074  .d.k...rit.....t
+00000370: 087c 027c 0619 0064 1019 0064 1119 0083  .|.|...d...d....
+00000380: 0118 007d 0b7c 0b64 1e6b 0590 0172 697a  ...}.|.d.k...riz
+00000390: 087c 027c 0619 0064 1319 007d 0857 006e  .|.|...d...}.W.n
+000003a0: 0c04 0074 0390 0179 3401 0001 0001 0064  ...t...y4......d
+000003b0: 147d 0859 006e 0177 007c 0664 1f67 007c  .}.Y.n.w.|.d.g.|
+000003c0: 0864 0764 169c 057c 0064 0219 007c 0619  .d.d...|.d...|..
+000003d0: 0064 173c 0064 187c 0064 0219 007c 0619  .d.<.d.|.d...|..
+000003e0: 0064 1919 0064 063c 0064 1a7c 0064 0219  .d...d.<.d.|.d..
+000003f0: 007c 0619 0064 0519 0064 1b3c 007c 0064  .|...d...d.<.|.d
+00000400: 0219 007c 0619 0064 0619 0064 0619 00a0  ...|...d...d....
+00000410: 09a1 0001 0074 0a64 1c7c 0669 0183 0101  .....t.d.|.i....
+00000420: 0057 006e 1a04 0074 0390 0179 8401 007d  .W.n...t...y...}
+00000430: 0a01 007a 0d74 0464 1d74 0ba0 0ca1 0083  ...z.t.d.t......
+00000440: 0201 0057 0059 0064 007d 0a7e 0a6e 0564  ...W.Y.d.}.~.n.d
+00000450: 007d 0a7e 0a77 0177 0009 007a b47c 0864  .}.~.w.w...z.|.d
+00000460: 0e19 0064 086b 027c 0864 0919 0064 086b  ...d.k.|.d...d.k
+00000470: 027c 0864 2019 0064 0a6b 0274 0d7c 027c  .|.d ..d.k.t.|.|
+00000480: 0619 0064 1019 0064 1119 0083 0164 216b  ...d...d.....d!k
+00000490: 0574 0d7c 027c 0619 0064 2219 0083 0164  .t.|.|...d"....d
+000004a0: 236b 0274 07a0 07a1 0074 087c 027c 0619  #k.t.....t.|.|..
+000004b0: 0064 1019 0064 1119 0083 0118 0064 249c  .d...d.......d$.
+000004c0: 067d 0c7c 0864 0e19 0064 086b 0290 0272  .}.|.d...d.k...r
+000004d0: 397c 0864 0919 0064 086b 0290 0272 397c  9|.d...d.k...r9|
+000004e0: 0864 2019 0064 0a6b 0290 0272 3974 0d7c  .d ..d.k...r9t.|
+000004f0: 027c 0619 0064 1019 0064 1119 0083 0164  .|...d...d.....d
+00000500: 216b 0590 0272 3974 0d7c 027c 0619 0064  !k...r9t.|.|...d
+00000510: 2219 0083 0164 236b 0290 0272 3974 07a0  "....d#k...r9t..
+00000520: 07a1 0074 087c 027c 0619 0064 1019 0064  ...t.|.|...d...d
+00000530: 1119 0083 0118 007d 0b7c 0b64 1e6b 0590  .......}.|.d.k..
+00000540: 0272 3974 0a64 257c 0669 0183 0101 007a  .r9t.d%|.i.....z
+00000550: 087c 027c 0619 0064 1319 007d 0857 006e  .|.|...d...}.W.n
+00000560: 0c04 0074 0390 0279 1401 0001 0001 0064  ...t...y.......d
+00000570: 147d 0859 006e 0177 007c 0664 2667 007c  .}.Y.n.w.|.d&g.|
+00000580: 0864 0764 279c 057c 0064 0219 007c 0619  .d.d'..|.d...|..
+00000590: 0064 173c 0064 187c 0064 0219 007c 0619  .d.<.d.|.d...|..
+000005a0: 0064 1919 0064 063c 007c 0064 0219 007c  .d...d.<.|.d...|
+000005b0: 0619 0064 0619 0064 0619 00a0 09a1 0001  ...d...d........
+000005c0: 0057 006e 1804 0074 0390 0279 5201 007d  .W.n...t...yR..}
+000005d0: 0a01 007a 0b74 0464 287c 0a83 0201 0057  ...z.t.d(|.....W
+000005e0: 0059 0064 007d 0a7e 0a6e 0564 007d 0a7e  .Y.d.}.~.n.d.}.~
+000005f0: 0a77 0177 0009 007a 367c 0864 0e19 0064  .w.w...z6|.d...d
+00000600: 086b 0290 0272 897c 0864 0f19 0064 086b  .k...r.|.d...d.k
+00000610: 0290 0272 897c 0864 2019 0064 0a6b 0290  ...r.|.d ..d.k..
+00000620: 0272 897c 0864 0919 0064 086b 0390 0272  .r.|.d...d.k...r
+00000630: 897c 0664 2967 007c 0864 0764 169c 057c  .|.d)g.|.d.d...|
+00000640: 0064 0219 007c 0619 0064 173c 0064 187c  .d...|...d.<.d.|
+00000650: 0064 0219 007c 0619 0064 1919 0064 063c  .d...|...d...d.<
+00000660: 0057 006e 1a04 0074 0390 0279 a401 007d  .W.n...t...y...}
+00000670: 0a01 007a 0d74 0464 2a74 0ba0 0ca1 0083  ...z.t.d*t......
+00000680: 0201 0057 0059 0064 007d 0a7e 0a6e 0564  ...W.Y.d.}.~.n.d
+00000690: 007d 0a7e 0a77 0177 0009 0009 007a 287c  .}.~.w.w.....z(|
+000006a0: 0864 0919 0064 0a6b 0290 0272 ce7c 0864  .d...d.k...r.|.d
+000006b0: 0e19 0064 086b 0290 0272 ce7c 0864 2019  ...d.k...r.|.d .
+000006c0: 0064 086b 0290 0272 ce7c 0864 2b19 0064  .d.k...r.|.d+..d
+000006d0: 086b 0290 0272 ce64 187c 0064 0219 007c  .k...r.d.|.d...|
+000006e0: 0619 0064 1919 0064 063c 0057 0071 1704  ...d...d.<.W.q..
+000006f0: 0074 0390 0279 e901 007d 0a01 007a 0d74  .t...y...}...z.t
+00000700: 0464 2a74 0ba0 0ca1 0083 0201 0057 0059  .d*t.........W.Y
+00000710: 0064 007d 0a7e 0a71 1764 007d 0a7e 0a77  .d.}.~.q.d.}.~.w
+00000720: 0177 007c 0244 005d 1a7d 067c 027c 0619  .w.|.D.].}.|.|..
+00000730: 0064 1919 0064 0619 0064 186b 0390 0372  .d...d...d.k...r
+00000740: 057c 05a0 0e7c 067c 0064 0219 007c 0619  .|...|.|.d...|..
+00000750: 0064 2c9c 02a1 0101 0090 0271 ec7c 0553  .d,........q.|.S
+00000760: 0029 2d4e da0d 7265 636f 7264 735f 6c65  .)-N..records_le
+00000770: 7665 6cda 1169 6e74 6572 6e61 6c5f 7374  vel..internal_st
+00000780: 6174 7573 6573 da0f 696e 7472 6f5f 7661  atuses..intro_va
+00000790: 7269 6162 6c65 73da 0a74 696d 655f 6c69  riables..time_li
+000007a0: 6d69 74da 0b6f 6363 7572 7265 6e63 6573  mit..occurrences
+000007b0: da07 7072 6f63 6573 7354 da03 7965 737a  ..processT..yesz
+000007c0: 1573 6361 6e20 7072 6f63 6573 7320 6973  .scan process is
+000007d0: 2061 6c69 7665 da02 6e6f 7a1e 7072 6f63   alive..noz.proc
+000007e0: 6573 7320 616c 6976 6520 6368 6563 6b20  ess alive check 
+000007f0: 6578 6365 7074 696f 6e3a da07 756e 6b6e  exception:..unkn
+00000800: 6f77 6e7a 1c73 6361 6e20 7072 6f63 6573  ownz.scan proces
+00000810: 7320 7665 6e74 7572 6520 7374 6172 7465  s venture starte
+00000820: 647a 1473 6361 6e20 7072 6f63 6573 7320  dz.scan process 
+00000830: 7374 6172 7465 647a 2073 6361 6e20 7072  startedz scan pr
+00000840: 6f63 6573 7320 6e6f 7469 6669 6564 2061  ocess notified a
+00000850: 6767 7265 6761 746f 72da 0574 696d 6573  ggregator..times
+00000860: 7a0f 7665 6e74 7572 6520 7374 6172 7465  z.venture starte
+00000870: 64e9 1e00 0000 da0a 6f63 6375 7265 6e63  d.......occurenc
+00000880: 6573 7a09 6e6f 7420 666f 756e 647a 6741  esz.not foundzgA
+00000890: 6674 6572 2033 3020 7365 636f 6e64 732c  fter 30 seconds,
+000008a0: 2074 6865 2061 6674 6572 2070 726f 6365   the after proce
+000008b0: 7373 206c 696e 6520 7761 7320 6e6f 7420  ss line was not 
+000008c0: 7265 6163 6865 6420 616e 6420 7468 6520  reached and the 
+000008d0: 7072 6f63 6573 7320 6469 6420 6e6f 7420  process did not 
+000008e0: 6e6f 7469 6679 2074 6865 2061 6767 7265  notify the aggre
+000008f0: 6761 746f 722e 2905 da04 7061 7468 da05  gator.)...path..
+00000900: 616c 6172 6dfa 0b61 6c61 726d 206e 6f74  alarm..alarm not
+00000910: 6573 720d 0000 00da 0665 7869 7465 64da  esr......exited.
+00000920: 0f72 6573 756c 7473 5f6f 665f 7363 616e  .results_of_scan
+00000930: da04 646f 6e65 da06 7374 6174 7573 7a3a  ..done..statusz:
+00000940: 5468 6520 7072 6f63 6573 7320 6469 646e  The process didn
+00000950: 2774 206e 6f74 6966 7920 7468 6520 6167  't notify the ag
+00000960: 6772 6567 6174 6f72 2077 6974 6869 6e20  gregator within 
+00000970: 3520 7365 636f 6e64 732e 7a10 646f 6e65  5 seconds.z.done
+00000980: 2072 6561 736f 6e20 6769 7665 7a18 7072   reason givez.pr
+00000990: 6f63 6573 7320 6d61 7920 6861 7665 2073  ocess may have s
+000009a0: 746f 7070 6564 7a23 7072 6f63 6573 7320  toppedz#process 
+000009b0: 6e6f 6e2d 6e6f 7469 6669 6361 7469 6f6e  non-notification
+000009c0: 2065 7863 6570 7469 6f6e 3ae9 0a00 0000   exception:.....
+000009d0: 7a50 4166 7465 7220 3130 2073 6563 6f6e  zPAfter 10 secon
+000009e0: 6473 2c20 7468 6520 7072 6f63 6573 7320  ds, the process 
+000009f0: 6469 6420 6e6f 7420 6e6f 7469 6679 2074  did not notify t
+00000a00: 6865 2061 6767 7265 6761 746f 7220 7468  he aggregator th
+00000a10: 6174 2069 7420 6861 6420 7374 6172 7465  at it had starte
+00000a20: 642e 7a18 7363 616e 2070 726f 6365 7373  d.z.scan process
+00000a30: 2077 6173 2073 746f 7070 6564 7203 0000   was stoppedr...
+00000a40: 00da 0772 6563 6f72 6473 7201 0000 0029  ...recordsr....)
+00000a50: 06da 0131 da01 32da 0133 da01 34da 0136  ...1..2..3..4..6
+00000a60: da01 377a 2b72 6563 6f72 6473 2077 6572  ..7z+records wer
+00000a70: 6520 6e6f 7420 7265 7472 6965 7665 6420  e not retrieved 
+00000a80: 6166 7465 7220 3130 2073 6563 6f6e 6473  after 10 seconds
+00000a90: 7a2d 4166 7465 7220 3130 2073 6563 6f6e  z-After 10 secon
+00000aa0: 6473 2c20 6e6f 2070 726f 6365 7373 206c  ds, no process l
+00000ab0: 6f67 7320 7765 7265 2066 6f75 6e64 2e29  ogs were found.)
+00000ac0: 0572 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000ad0: 7214 0000 0072 1800 0000 7a28 7072 6f63  r....r....z(proc
+00000ae0: 6573 7320 6c6f 6773 2074 696d 6520 6c69  ess logs time li
+00000af0: 6d69 7420 6368 6563 6b20 6578 6365 7074  mit check except
+00000b00: 696f 6e3a 7a30 5468 6520 7072 6f63 6573  ion:z0The proces
+00000b10: 7320 6578 6974 6564 2062 6566 6f72 6520  s exited before 
+00000b20: 7265 7375 6c74 7320 636f 756c 6420 6265  results could be
+00000b30: 2073 656e 742e 7a1a 7061 7273 6520 616e   sent.z.parse an
+00000b40: 6420 6368 6563 6b20 6578 6365 7074 696f  d check exceptio
+00000b50: 6e3a 7a1b 7363 616e 2072 6563 6f72 6473  n:z.scan records
+00000b60: 2077 6572 6520 7265 7472 6965 7665 6429   were retrieved)
+00000b70: 0272 1500 0000 da09 696e 7465 726e 616c  .r......internal
+00000b80: 7329 0f72 0200 0000 da04 7479 7065 da08  s).r......type..
+00000b90: 6973 5f61 6c69 7665 da09 4578 6365 7074  is_alive..Except
+00000ba0: 696f 6eda 0570 7269 6e74 7204 0000 0072  ion..printr....r
+00000bb0: 0500 0000 da04 7469 6d65 da05 666c 6f61  ......time..floa
+00000bc0: 74da 0974 6572 6d69 6e61 7465 7207 0000  t..terminater...
+00000bd0: 00da 0974 7261 6365 6261 636b da0a 666f  ...traceback..fo
+00000be0: 726d 6174 5f65 7863 da03 6c65 6eda 0661  rmat_exc..len..a
+00000bf0: 7070 656e 6429 0dda 1461 6767 7265 6761  ppend)...aggrega
+00000c00: 746f 725f 7661 7269 6162 6c65 7372 0900  tor_variablesr..
+00000c10: 0000 720a 0000 0072 0c00 0000 da08 7374  ..r....r......st
+00000c20: 6174 7573 6573 da0a 756e 6669 6e69 7368  atuses..unfinish
+00000c30: 6564 da0b 7374 6174 7573 5f70 6174 68da  ed..status_path.
+00000c40: 0e73 7461 7475 735f 6f66 5f70 6174 6872  .status_of_pathr
+00000c50: 0d00 0000 da05 616c 6976 65da 0145 da07  ......alive..E..
+00000c60: 656c 6170 7365 64da 0564 6f6f 7273 a900  elapsed..doors..
+00000c70: 7239 0000 00fa 712f 6269 6f74 6563 682f  r9....q/biotech/
+00000c80: 7665 6e75 6573 2f73 7461 6765 732f 6269  venues/stages/bi
+00000c90: 6f74 6563 682f 7072 6f63 6564 7572 6573  otech/procedures
+00000ca0: 2f61 6767 7265 6761 746f 725f 7072 6f63  /aggregator_proc
+00000cb0: 6564 7572 652f 7072 6f63 6573 732f 6d6f  edure/process/mo
+00000cc0: 7665 732f 7374 6174 7573 5f63 6865 636b  ves/status_check
+00000cd0: 5f6d 6f6e 6974 6f72 2f74 6865 5f70 6879  _monitor/the_phy
+00000ce0: 7369 6361 6c2e 7079 da24 7061 7273 655f  sical.py.$parse_
+00000cf0: 616e 645f 6368 6563 6b5f 6973 5f61 6c69  and_check_is_ali
+00000d00: 7665 5f6f 665f 7374 6174 7573 6573 2100  ve_of_statuses!.
+00000d10: 0000 7346 0100 0006 0108 0208 010c 0104  ..sF............
+00000d20: 0204 010a 0108 0208 0102 0202 0410 0118  ................
+00000d30: 0114 0108 010a 0108 0204 800e 020a 0114  ................
+00000d40: 0108 8002 fe08 0508 0302 0502 0d0c 020c  ................
+00000d50: 010c 011c 0208 0202 0110 010c 0108 0102  ................
+00000d60: ff02 0402 0202 0102 0202 0212 f814 0b14  ................
+00000d70: 0118 0202 0204 0106 ff04 800e 030e 010c  ................
+00000d80: 0108 8002 fe02 0502 080e 020e 011c 020a  ................
+00000d90: 0202 0110 010e 0108 0102 ff02 0402 0202  ................
+00000da0: 0102 0202 0212 f814 0b14 0118 0102 0204  ................
+00000db0: 0106 ff04 8010 030e 010c 0108 8002 fe02  ................
+00000dc0: 0502 120a 020a 010a 0116 0112 011a 0106  ................
+00000dd0: fa0e 0b0e 010e 011a 0116 021c 020a 0202  ................
+00000de0: 0104 0106 ff02 0410 010e 0108 0102 ff02  ................
+00000df0: 0402 0202 0102 0202 0212 f814 0b18 0104  ................
+00000e00: 8010 040a 010c 0108 8002 fe02 0602 0c0e  ................
+00000e10: 020e 010e 020e 0202 0302 0202 0102 0102  ................
+00000e20: 0212 f914 0a04 8010 020e 010c 0108 8002  ................
+00000e30: fe02 0502 0802 030e 020e 020e 010e 0114  ................
+00000e40: 0204 8010 020e 010c 0108 8002 fe08 0616  ................
+00000e50: 0104 0102 010a 0108 fe04 8004 0672 3b00  .............r;.
+00000e60: 0000 290f da39 6269 6f74 6563 682e 7072  ..)..9biotech.pr
+00000e70: 6f63 6564 7572 6573 2e61 6767 7265 6761  ocedures.aggrega
+00000e80: 746f 725f 7072 6f63 6564 7572 652e 7072  tor_procedure.pr
+00000e90: 6f63 6573 732e 7661 7269 6162 6c65 7372  ocess.variablesr
+00000ea0: 0200 0000 721d 0000 0072 0400 0000 da27  ....r....r.....'
+00000eb0: 616c 6172 6d5f 6368 6563 6b73 2e67 6c6f  alarm_checks.glo
+00000ec0: 6261 6c5f 7469 6d65 5f6c 696d 6974 5f65  bal_time_limit_e
+00000ed0: 7863 6565 6465 6472 0500 0000 da30 6269  xceededr.....0bi
+00000ee0: 6f74 6563 682e 746f 7069 6373 2e70 726f  otech.topics.pro
+00000ef0: 6365 7373 5f6f 6e2e 705f 6578 7065 6374  cess_on.p_expect
+00000f00: 2e70 6172 7365 5f72 6563 6f72 6473 7206  .parse_recordsr.
+00000f10: 0000 00da 1c62 696f 7465 6368 2e74 6f70  .....biotech.top
+00000f20: 6963 732e 7368 6f77 2e76 6172 6961 626c  ics.show.variabl
+00000f30: 6572 0700 0000 7208 0000 0072 2900 0000  er....r....r)...
+00000f40: 722c 0000 00da 0472 6963 6872 3b00 0000  r,.....richr;...
+00000f50: 7239 0000 0072 3900 0000 7239 0000 0072  r9...r9...r9...r
+00000f60: 3a00 0000 da08 3c6d 6f64 756c 653e 0100  :.....<module>..
+00000f70: 0000 7316 0000 000c 070c 030c 020c 020c  ..s.............
+00000f80: 010c 0308 0108 0108 0302 050c 04         .............
```

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 
 
 
 #----
 #
 from biotech.procedures.aggregator_procedure.process.variables import retrieve_variables
-from ..done_with_scan import done_with_scan_move
+
 #
 from .records import attach_records
 #
+from .alarm_checks.global_time_limit_exceeded import learn_if_global_time_limit_was_exceeded
+#
 from biotech.topics.process_on.p_expect.parse_records import parse_p_expect_records
 from biotech.topics.show.variable import show_variable
 #
 #
 from pprint import pprint
 import time
 import traceback
@@ -28,23 +30,15 @@
 	This is run over and over again
 	in a loop.
 '''
 def parse_and_check_is_alive_of_statuses ():
 	aggregator_variables = retrieve_variables ()
 
 	records_level = aggregator_variables ["records_level"]
-
 	internal_statuses = aggregator_variables ["internal_statuses"]
-	
-	'''
-	show_variable ({
-		"intro variables:": aggregator_variables ["intro_variables"]
-	})
-	'''
-	
 	time_limit = aggregator_variables ["intro_variables"] ["time_limit"]
 
 	statuses = {}
 	unfinished = []
 	for status_path in internal_statuses:
 		
 		status_of_path = internal_statuses [ status_path ]
@@ -61,101 +55,115 @@
 					if (alive == True):
 						occurrences ["scan process is alive"] = "yes"
 					else:
 						occurrences ["scan process is alive"] = "no"
 				
 		except Exception as E:
 			print ("process alive check exception:", E)
-			#print ("process alive check exception:", traceback.format_exc ())
-		
 			occurrences ["scan process is alive"] = "unknown"		
 		
 		
 		attach_records (status_path)
 		
 		
+		learn_if_global_time_limit_was_exceeded (status_path)
+		
+
+
 		
 		'''
-			This stops the process if the
-			global time limit was exceeded.
+			This checks if a perhaps non started process didn't 
+			notify the aggregator within 30 seconds.
+		
+			The before process line was reached:
+				scan process venture started == "yes"
+			
+			The after process line was not reached:
+				scan process venture started == "no"
+		
+			
+			30 seconds elapsed
 		'''
 		try:
 			if (
-				occurrences ["scan process started"] == "yes" and
-				occurrences ["scan process is alive"] == "yes" and
-				occurrences ["scan process was stopped"] == "no" and
-				len (internal_statuses [ status_path ] ["times"] ["started"]) >= 1
-			):			
-				if (time.time () - float (internal_statuses [ status_path ] ["times"] ["started"]) >= float (time_limit)):	
+				occurrences ["scan process venture started"] == "yes" and
+				occurrences ["scan process started"] == "no" and
+				occurrences ["scan process notified aggregator"] == "no"
+			):
+				elapsed = time.time () - float (internal_statuses [ status_path ] ["times"] ["venture started"]);
 				
+				if (elapsed >= 30):		
 					try:
-						the_scan_records = internal_statuses [ status_path ] ["records"]
+						occurrences = internal_statuses [ status_path ] ["occurences"];
 					except Exception:
-						the_scan_records = "not found"
+						occurrences = "not found"				
 				
-					done_with_scan_move ({
+					aggregator_variables ["internal_statuses"] [ status_path ] ["results_of_scan"] = {
 						"path": status_path,
-						"result":{
-							"alarm": "time limit exceeded",
-							"the records": the_scan_records
-						}
-					})
 						
+						"alarm": "After 30 seconds, the after process line was not reached and the process did not notify the aggregator.",
+						"alarm notes": [],
+						
+						"occurrences": occurrences,
+						
+						"exited": True
+					}
+				
+					aggregator_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
+					aggregator_variables ["internal_statuses"] [ status_path ] ["occurrences"] ["done reason give"] = "The process didn't notify the aggregator within 5 seconds."
+					
+					aggregator_variables ["internal_statuses"] [ status_path ] ["process"] ["process"].terminate ()
+					
+					show_variable ({
+						"process may have stopped": status_path
+					})
 		except Exception as E:
-			print ("time limit check exception:", traceback.format_exc ())
+			print ("process non-notification exception:", traceback.format_exc ())
 			pass;
-		
-
+			
 		
 		'''
-			This checks if the process didn't notify the aggregator within 5 seconds.
+			This checks if a started process didn't 
+			notify the aggregator within 10 seconds.
 		
-				scan process venture started == "yes"
+				scan process started == "yes"
 				scan process notified aggregator == "no"
-				5 seconds elapsed
+				10 seconds elapsed
 		'''
 		try:
 			if (
-				occurrences ["scan process venture started"] == "yes" and
+				occurrences ["scan process started"] == "yes" and
 				occurrences ["scan process notified aggregator"] == "no"
 			):
 				elapsed = time.time () - float (internal_statuses [ status_path ] ["times"] ["venture started"]);
 				
-				show_variable ({
-					"elapsed without notification:": elapsed
-				})
-				
-				if (elapsed >= 5):			
-					show_variable ({
-						"attempting to stop the process": status_path
-					})
-					
-					
+				if (elapsed >= 10):			
+					try:
+						occurrences = internal_statuses [ status_path ] ["occurences"];
+					except Exception:
+						occurrences = "not found"
 					
 					aggregator_variables ["internal_statuses"] [ status_path ] ["results_of_scan"] = {
 						"path": status_path,
 						
-						"alarm": "There was most likely an internal problem starting the process.",
-						"alarm notes": [
-							"After 5 seconds, the process did not notify the aggregator that it had started."
-						],
+						"alarm": "After 10 seconds, the process did not notify the aggregator that it had started.",
+						"alarm notes": [],
+						
+						"occurrences": occurrences,
 						
 						"exited": True
 					}
 				
 					aggregator_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
 					aggregator_variables ["internal_statuses"] [ status_path ] ["occurrences"] ["done reason give"] = "The process didn't notify the aggregator within 5 seconds."
-					
 					aggregator_variables ["internal_statuses"] [ status_path ] ["process"] ["process"].terminate ()
 					
 					show_variable ({
 						"process may have stopped": status_path
 					})
-				
-		
 		except Exception as E:
 			print ("process non-notification exception:", traceback.format_exc ())
 			pass;
 		
 		
 		'''
 			A live process that is indicating that
@@ -171,68 +179,50 @@
 				'scan process is alive': 'yes',
 
 
 				'scan process was stopped': 'no',
 				'scan returned proceeds': 'no',
 				'scan records were retrieved': 'no'
 		'''
-		try:		
-			'''
-			show_variable ({
-				"doors parsed?": ""
-			})
-			'''
-		
+		try:				
 			doors = {
 				"1": occurrences ["scan process started"] == "yes",
 				"2": occurrences ["scan process is alive"] == "yes",
 				"3": occurrences ["scan process was stopped"] == "no",
 				"4": len (internal_statuses [ status_path ] ["times"] ["venture started"]) >= 1,
 				"6": len (internal_statuses [ status_path ] ["records"]) == 0,
 				"7": time.time () - float (internal_statuses [ status_path ] ["times"] ["venture started"])
 			}
 			
-			'''
-			show_variable ({
-				"doors": doors
-			})
-			'''
-			
 		
 			if (
 				occurrences ["scan process started"] == "yes" and
 				occurrences ["scan process is alive"] == "yes" and
 				occurrences ["scan process was stopped"] == "no" and
 				len (internal_statuses [ status_path ] ["times"] ["venture started"]) >= 1 and
 				
 				len (internal_statuses [ status_path ] ["records"]) == 0
 			):
 				elapsed = time.time () - float (internal_statuses [ status_path ] ["times"] ["venture started"]);
-				
-				show_variable ({
-					"elapsed": elapsed
-				})
 			
 				if (elapsed >= 10):			
 					show_variable ({
 						"records were not retrieved after 10 seconds": status_path
 					})
 					
 					try:
 						occurrences = internal_statuses [ status_path ] ["occurences"];
 					except Exception:
 						occurrences = "not found"
 					
 					aggregator_variables ["internal_statuses"] [ status_path ] ["results_of_scan"] = {
 						"path": status_path,
 						
-						"alarm": "There was most likely an internal problem starting the process.",
-						"alarm notes": [
-							"After 10 seconds, no process logs were found."
-						],
+						"alarm": "After 10 seconds, no process logs were found.",
+						"alarm notes": [],
 						
 						"occurences": occurrences,
 						
 						"exited": True
 					}
 				
 					aggregator_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
@@ -286,15 +276,14 @@
 		
 		'''
 			objective:
 				This stops the process if:
 					the process is alive, but unresponsive?
 		'''
 		
-		
 
 		
 		'''
 			This indicate that the process is done normally
 		'''
 		try:
 			if (
```

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,17 @@
 	
 	"details": 2,
 	
 	#
 	#
 	#
 	"internal_statuses": {},
-	"internal_statuses_built": "no"
+	"internal_statuses_built": "no",
+	
+	"anomalies": []
 }
 
 def setup_internal_statuses (
 	status_check_paths,
 	relative_path
 ):
 	for status_check_path in status_check_paths:
```

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 16:26:14 2024 UTC, .py size: 2910 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,106 +1,107 @@
-00000000: 6f0d 0d0a 0000 0000 269b 2266 5e0b 0000  o.......&."f^...
+00000000: 6f0d 0d0a 0000 0000 56d4 2266 720b 0000  o.......V."fr...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
+00000020: 0008 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 0900  Z.d.d.l.m.Z.....
 00000040: 0900 6403 6404 6405 9c02 6406 6900 6407  ..d.d.d...d.i.d.
-00000050: 6900 6408 6409 9c06 5a03 640a 640b 8400  i.d.d...Z.d.d...
-00000060: 5a04 640c 640d 8400 5a05 640e 640f 8400  Z.d.d...Z.d.d...
-00000070: 5a06 6410 6411 8400 5a07 6412 6413 8400  Z.d.d...Z.d.d...
-00000080: 5a08 6414 5300 2915 7a66 0a09 6672 6f6d  Z.d.S.).zf..from
-00000090: 2062 696f 7465 6368 2e70 726f 6365 6475   biotech.procedu
-000000a0: 7265 732e 6167 6772 6567 6174 6f72 5f70  res.aggregator_p
-000000b0: 726f 6365 6475 7265 2e70 726f 6365 7373  rocedure.process
-000000c0: 2e76 6172 6961 626c 6573 2069 6d70 6f72  .variables impor
-000000d0: 7420 7265 7472 6965 7665 5f61 6767 7265  t retrieve_aggre
-000000e0: 6761 746f 725f 7661 7269 6162 6c65 730a  gator_variables.
-000000f0: e900 0000 0029 01da 0b66 6f72 6d61 745f  .....)...format_
-00000100: 7061 7468 7a07 302e 302e 302e 30da 0029  pathz.0.0.0.0..)
-00000110: 02da 0468 6f73 74da 0470 6f72 74e9 0300  ...host..port...
-00000120: 0000 e902 0000 00da 026e 6f29 06da 0c69  .........no)...i
-00000130: 6e74 726f 5f68 6172 626f 72da 0d72 6563  ntro_harbor..rec
-00000140: 6f72 6473 5f6c 6576 656c da0f 696e 7472  ords_level..intr
-00000150: 6f5f 7661 7269 6162 6c65 73da 0764 6574  o_variables..det
-00000160: 6169 6c73 da11 696e 7465 726e 616c 5f73  ails..internal_s
-00000170: 7461 7475 7365 73da 1769 6e74 6572 6e61  tatuses..interna
-00000180: 6c5f 7374 6174 7573 6573 5f62 7569 6c74  l_statuses_built
-00000190: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-000001a0: 000a 0000 0043 0000 0073 4c00 0000 7c00  .....C...sL...|.
-000001b0: 4400 5d21 7d02 6401 6401 6401 6401 6402  D.]!}.d.d.d.d.d.
-000001c0: 6401 6401 6403 6404 9c08 6405 6406 6901  d.d.d.d...d.d.i.
-000001d0: 6403 6403 6403 6407 9c03 6700 6400 6400  d.d.d.d...g.d.d.
-000001e0: 6408 9c06 7400 6409 1900 7401 7c02 7c01  d...t.d...t.|.|.
-000001f0: 8302 3c00 7102 6400 5300 290a 4e72 0800  ..<.q.d.S.).Nr..
-00000200: 0000 da07 756e 6b6e 6f77 6e72 0300 0000  ....unknownr....
-00000210: 2908 7a1c 7363 616e 2070 726f 6365 7373  ).z.scan process
-00000220: 2076 656e 7475 7265 2073 7461 7274 6564   venture started
-00000230: 7a14 7363 616e 2070 726f 6365 7373 2073  z.scan process s
-00000240: 7461 7274 6564 7a20 7363 616e 2070 726f  tartedz scan pro
-00000250: 6365 7373 206e 6f74 6966 6965 6420 6167  cess notified ag
-00000260: 6772 6567 6174 6f72 7a18 7363 616e 2070  gregatorz.scan p
-00000270: 726f 6365 7373 2077 6173 2073 746f 7070  rocess was stopp
-00000280: 6564 7a15 7363 616e 2070 726f 6365 7373  edz.scan process
-00000290: 2069 7320 616c 6976 657a 1673 6361 6e20   is alivez.scan 
-000002a0: 7265 7475 726e 6564 2070 726f 6365 6564  returned proceed
-000002b0: 737a 1b73 6361 6e20 7265 636f 7264 7320  sz.scan records 
-000002c0: 7765 7265 2072 6574 7269 6576 6564 7a10  were retrievedz.
-000002d0: 646f 6e65 2072 6561 736f 6e20 6769 7665  done reason give
-000002e0: da07 7072 6f63 6573 73da 0770 656e 6469  ..process..pendi
-000002f0: 6e67 2903 da07 7374 6172 7465 64da 0565  ng)...started..e
-00000300: 6e64 6564 da07 656c 6170 7365 6429 06da  nded..elapsed)..
-00000310: 0b6f 6363 7572 7265 6e63 6573 da06 7374  .occurrences..st
-00000320: 6174 7573 da05 7469 6d65 73da 0772 6563  atus..times..rec
-00000330: 6f72 6473 7210 0000 00da 0f72 6573 756c  ordsr......resul
-00000340: 7473 5f6f 665f 7363 616e 720d 0000 0029  ts_of_scanr....)
-00000350: 02da 1461 6767 7265 6761 746f 725f 7661  ...aggregator_va
-00000360: 7269 6162 6c65 7372 0200 0000 2903 da12  riablesr....)...
-00000370: 7374 6174 7573 5f63 6865 636b 5f70 6174  status_check_pat
-00000380: 6873 da0d 7265 6c61 7469 7665 5f70 6174  hs..relative_pat
-00000390: 68da 1173 7461 7475 735f 6368 6563 6b5f  h..status_check_
-000003a0: 7061 7468 a900 721e 0000 00fa 5c2f 6269  path..r.....\/bi
-000003b0: 6f74 6563 682f 7665 6e75 6573 2f73 7461  otech/venues/sta
-000003c0: 6765 732f 6269 6f74 6563 682f 7072 6f63  ges/biotech/proc
-000003d0: 6564 7572 6573 2f61 6767 7265 6761 746f  edures/aggregato
-000003e0: 725f 7072 6f63 6564 7572 652f 7072 6f63  r_procedure/proc
-000003f0: 6573 732f 7661 7269 6162 6c65 732f 5f5f  ess/variables/__
-00000400: 696e 6974 5f5f 2e70 79da 1773 6574 7570  init__.py..setup
-00000410: 5f69 6e74 6572 6e61 6c5f 7374 6174 7573  _internal_status
-00000420: 6573 3c00 0000 7330 0000 0008 0402 0c02  es<...s0........
-00000430: 0702 0802 0702 0702 0802 0702 0704 c504  ................
-00000440: 4102 ff02 0602 0102 0104 fd02 0602 0202  A...............
-00000450: 0104 b106 fe08 0104 ff04 5572 2000 0000  ..........Ur ...
-00000460: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000470: 0001 0000 0043 0000 0073 0400 0000 6400  .....C...s....d.
-00000480: 5300 a901 4e72 1e00 0000 721e 0000 0072  S...Nr....r....r
-00000490: 1e00 0000 721e 0000 0072 1f00 0000 da06  ....r....r......
-000004a0: 6368 616e 6765 9800 0000 f302 0000 0004  change..........
-000004b0: 0172 2200 0000 6300 0000 0000 0000 0000  .r"...c.........
-000004c0: 0000 0000 0000 0001 0000 0043 0000 00f3  ...........C....
-000004d0: 0400 0000 7400 5300 7221 0000 00a9 0172  ....t.S.r!.....r
-000004e0: 1a00 0000 721e 0000 0072 1e00 0000 721e  ....r....r....r.
-000004f0: 0000 0072 1f00 0000 da12 7265 7472 6965  ...r......retrie
-00000500: 7665 5f76 6172 6961 626c 6573 9b00 0000  ve_variables....
-00000510: 7223 0000 0072 2600 0000 6300 0000 0000  r#...r&...c.....
-00000520: 0000 0000 0000 0000 0000 0001 0000 0043  ...............C
-00000530: 0000 0072 2400 0000 7221 0000 0072 2500  ...r$...r!...r%.
-00000540: 0000 721e 0000 0072 1e00 0000 721e 0000  ..r....r....r...
-00000550: 0072 1f00 0000 da1d 7265 7472 6965 7665  .r......retrieve
-00000560: 5f61 6767 7265 6761 746f 725f 7661 7269  _aggregator_vari
-00000570: 6162 6c65 739e 0000 0072 2300 0000 7227  ables....r#...r'
-00000580: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000590: 0000 0000 0100 0000 4300 0000 7224 0000  ........C...r$..
-000005a0: 0072 2100 0000 7225 0000 0072 1e00 0000  .r!...r%...r....
-000005b0: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
-000005c0: 0872 6574 7269 6576 65a1 0000 0072 2300  .retrieve....r#.
-000005d0: 0000 7228 0000 004e 2909 da07 5f5f 646f  ..r(...N)...__do
-000005e0: 635f 5fda 4162 696f 7465 6368 2e70 726f  c__.Abiotech.pro
-000005f0: 6365 6475 7265 732e 6167 6772 6567 6174  cedures.aggregat
-00000600: 6f72 5f70 726f 6365 6475 7265 2e70 726f  or_procedure.pro
-00000610: 6365 7373 2e6d 6f76 6573 2e66 6f72 6d61  cess.moves.forma
-00000620: 745f 7061 7468 7202 0000 0072 1a00 0000  t_pathr....r....
-00000630: 7220 0000 0072 2200 0000 7226 0000 0072  r ...r"...r&...r
-00000640: 2700 0000 7228 0000 0072 1e00 0000 721e  '...r(...r....r.
-00000650: 0000 0072 1e00 0000 721f 0000 00da 083c  ...r....r......<
-00000660: 6d6f 6475 6c65 3e01 0000 0073 2400 0000  module>....s$...
-00000670: 0402 0c04 0203 0207 0215 0201 04fe 0205  ................
-00000680: 0202 0207 0205 0201 06eb 0818 085c 0803  .............\..
-00000690: 0803 0c03                                ....
+00000050: 6900 6408 6700 6409 9c07 5a03 640a 640b  i.d.g.d...Z.d.d.
+00000060: 8400 5a04 640c 640d 8400 5a05 640e 640f  ..Z.d.d...Z.d.d.
+00000070: 8400 5a06 6410 6411 8400 5a07 6412 6413  ..Z.d.d...Z.d.d.
+00000080: 8400 5a08 6414 5300 2915 7a66 0a09 6672  ..Z.d.S.).zf..fr
+00000090: 6f6d 2062 696f 7465 6368 2e70 726f 6365  om biotech.proce
+000000a0: 6475 7265 732e 6167 6772 6567 6174 6f72  dures.aggregator
+000000b0: 5f70 726f 6365 6475 7265 2e70 726f 6365  _procedure.proce
+000000c0: 7373 2e76 6172 6961 626c 6573 2069 6d70  ss.variables imp
+000000d0: 6f72 7420 7265 7472 6965 7665 5f61 6767  ort retrieve_agg
+000000e0: 7265 6761 746f 725f 7661 7269 6162 6c65  regator_variable
+000000f0: 730a e900 0000 0029 01da 0b66 6f72 6d61  s......)...forma
+00000100: 745f 7061 7468 7a07 302e 302e 302e 30da  t_pathz.0.0.0.0.
+00000110: 0029 02da 0468 6f73 74da 0470 6f72 74e9  .)...host..port.
+00000120: 0300 0000 e902 0000 00da 026e 6f29 07da  ...........no)..
+00000130: 0c69 6e74 726f 5f68 6172 626f 72da 0d72  .intro_harbor..r
+00000140: 6563 6f72 6473 5f6c 6576 656c da0f 696e  ecords_level..in
+00000150: 7472 6f5f 7661 7269 6162 6c65 73da 0764  tro_variables..d
+00000160: 6574 6169 6c73 da11 696e 7465 726e 616c  etails..internal
+00000170: 5f73 7461 7475 7365 73da 1769 6e74 6572  _statuses..inter
+00000180: 6e61 6c5f 7374 6174 7573 6573 5f62 7569  nal_statuses_bui
+00000190: 6c74 da09 616e 6f6d 616c 6965 7363 0200  lt..anomaliesc..
+000001a0: 0000 0000 0000 0000 0000 0300 0000 0a00  ................
+000001b0: 0000 4300 0000 734c 0000 007c 0044 005d  ..C...sL...|.D.]
+000001c0: 217d 0264 0164 0164 0164 0164 0264 0164  !}.d.d.d.d.d.d.d
+000001d0: 0164 0364 049c 0864 0564 0669 0164 0364  .d.d...d.d.i.d.d
+000001e0: 0364 0364 079c 0367 0064 0064 0064 089c  .d.d...g.d.d.d..
+000001f0: 0674 0064 0919 0074 017c 027c 0183 023c  .t.d...t.|.|...<
+00000200: 0071 0264 0053 0029 0a4e 7208 0000 00da  .q.d.S.).Nr.....
+00000210: 0775 6e6b 6e6f 776e 7203 0000 0029 087a  .unknownr....).z
+00000220: 1c73 6361 6e20 7072 6f63 6573 7320 7665  .scan process ve
+00000230: 6e74 7572 6520 7374 6172 7465 647a 1473  nture startedz.s
+00000240: 6361 6e20 7072 6f63 6573 7320 7374 6172  can process star
+00000250: 7465 647a 2073 6361 6e20 7072 6f63 6573  tedz scan proces
+00000260: 7320 6e6f 7469 6669 6564 2061 6767 7265  s notified aggre
+00000270: 6761 746f 727a 1873 6361 6e20 7072 6f63  gatorz.scan proc
+00000280: 6573 7320 7761 7320 7374 6f70 7065 647a  ess was stoppedz
+00000290: 1573 6361 6e20 7072 6f63 6573 7320 6973  .scan process is
+000002a0: 2061 6c69 7665 7a16 7363 616e 2072 6574   alivez.scan ret
+000002b0: 7572 6e65 6420 7072 6f63 6565 6473 7a1b  urned proceedsz.
+000002c0: 7363 616e 2072 6563 6f72 6473 2077 6572  scan records wer
+000002d0: 6520 7265 7472 6965 7665 647a 1064 6f6e  e retrievedz.don
+000002e0: 6520 7265 6173 6f6e 2067 6976 65da 0770  e reason give..p
+000002f0: 726f 6365 7373 da07 7065 6e64 696e 6729  rocess..pending)
+00000300: 03da 0773 7461 7274 6564 da05 656e 6465  ...started..ende
+00000310: 64da 0765 6c61 7073 6564 2906 da0b 6f63  d..elapsed)...oc
+00000320: 6375 7272 656e 6365 73da 0673 7461 7475  currences..statu
+00000330: 73da 0574 696d 6573 da07 7265 636f 7264  s..times..record
+00000340: 7372 1100 0000 da0f 7265 7375 6c74 735f  sr......results_
+00000350: 6f66 5f73 6361 6e72 0d00 0000 2902 da14  of_scanr....)...
+00000360: 6167 6772 6567 6174 6f72 5f76 6172 6961  aggregator_varia
+00000370: 626c 6573 7202 0000 0029 03da 1273 7461  blesr....)...sta
+00000380: 7475 735f 6368 6563 6b5f 7061 7468 73da  tus_check_paths.
+00000390: 0d72 656c 6174 6976 655f 7061 7468 da11  .relative_path..
+000003a0: 7374 6174 7573 5f63 6865 636b 5f70 6174  status_check_pat
+000003b0: 68a9 0072 1f00 0000 fa5c 2f62 696f 7465  h..r.....\/biote
+000003c0: 6368 2f76 656e 7565 732f 7374 6167 6573  ch/venues/stages
+000003d0: 2f62 696f 7465 6368 2f70 726f 6365 6475  /biotech/procedu
+000003e0: 7265 732f 6167 6772 6567 6174 6f72 5f70  res/aggregator_p
+000003f0: 726f 6365 6475 7265 2f70 726f 6365 7373  rocedure/process
+00000400: 2f76 6172 6961 626c 6573 2f5f 5f69 6e69  /variables/__ini
+00000410: 745f 5f2e 7079 da17 7365 7475 705f 696e  t__.py..setup_in
+00000420: 7465 726e 616c 5f73 7461 7475 7365 733e  ternal_statuses>
+00000430: 0000 0073 3000 0000 0804 020c 0207 0208  ...s0...........
+00000440: 0207 0207 0208 0207 0207 04c5 0441 02ff  .............A..
+00000450: 0206 0201 0201 04fd 0206 0202 0201 04b1  ................
+00000460: 06fe 0801 04ff 0455 7221 0000 0063 0000  .......Ur!...c..
+00000470: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00000480: 0000 4300 0000 7304 0000 0064 0053 00a9  ..C...s....d.S..
+00000490: 014e 721f 0000 0072 1f00 0000 721f 0000  .Nr....r....r...
+000004a0: 0072 1f00 0000 7220 0000 00da 0663 6861  .r....r .....cha
+000004b0: 6e67 659a 0000 00f3 0200 0000 0401 7223  nge...........r#
+000004c0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000004d0: 0000 0000 0100 0000 4300 0000 f304 0000  ........C.......
+000004e0: 0074 0053 0072 2200 0000 a901 721b 0000  .t.S.r".....r...
+000004f0: 0072 1f00 0000 721f 0000 0072 1f00 0000  .r....r....r....
+00000500: 7220 0000 00da 1272 6574 7269 6576 655f  r .....retrieve_
+00000510: 7661 7269 6162 6c65 739d 0000 0072 2400  variables....r$.
+00000520: 0000 7227 0000 0063 0000 0000 0000 0000  ..r'...c........
+00000530: 0000 0000 0000 0000 0100 0000 4300 0000  ............C...
+00000540: 7225 0000 0072 2200 0000 7226 0000 0072  r%...r"...r&...r
+00000550: 1f00 0000 721f 0000 0072 1f00 0000 7220  ....r....r....r 
+00000560: 0000 00da 1d72 6574 7269 6576 655f 6167  .....retrieve_ag
+00000570: 6772 6567 6174 6f72 5f76 6172 6961 626c  gregator_variabl
+00000580: 6573 a000 0000 7224 0000 0072 2800 0000  es....r$...r(...
+00000590: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000005a0: 0001 0000 0043 0000 0072 2500 0000 7222  .....C...r%...r"
+000005b0: 0000 0072 2600 0000 721f 0000 0072 1f00  ...r&...r....r..
+000005c0: 0000 721f 0000 0072 2000 0000 da08 7265  ..r....r .....re
+000005d0: 7472 6965 7665 a300 0000 7224 0000 0072  trieve....r$...r
+000005e0: 2900 0000 4e29 09da 075f 5f64 6f63 5f5f  )...N)...__doc__
+000005f0: da41 6269 6f74 6563 682e 7072 6f63 6564  .Abiotech.proced
+00000600: 7572 6573 2e61 6767 7265 6761 746f 725f  ures.aggregator_
+00000610: 7072 6f63 6564 7572 652e 7072 6f63 6573  procedure.proces
+00000620: 732e 6d6f 7665 732e 666f 726d 6174 5f70  s.moves.format_p
+00000630: 6174 6872 0200 0000 721b 0000 0072 2100  athr....r....r!.
+00000640: 0000 7223 0000 0072 2700 0000 7228 0000  ..r#...r'...r(..
+00000650: 0072 2900 0000 721f 0000 0072 1f00 0000  .r)...r....r....
+00000660: 721f 0000 0072 2000 0000 da08 3c6d 6f64  r....r .....<mod
+00000670: 756c 653e 0100 0000 7326 0000 0004 020c  ule>....s&......
+00000680: 0402 0302 0702 1502 0104 fe02 0502 0202  ................
+00000690: 0702 0502 0102 0206 e908 1a08 5c08 0308  ............\...
+000006a0: 030c 03                                  ...
```

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/on.py` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py` & `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro/on.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro/process/adventure.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/adventure.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro/process/keg/__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/__pycache__/on.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/_ops/__pycache__/start.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/_ops/__pycache__/start.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/_ops/start.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/_ops/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/on.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/send_paths.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/send_paths.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/__init__v1.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/keg/__init__v1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/quart__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/keg/quart__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/on.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/intro.proc.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/intro.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/keg/__init__.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/moves/__pycache__/adventure.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/moves/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/moves/adventure.py` & `biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/moves/adventure.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/aggregate/__init__.py` & `biotech-1.1.1/venues/stages/biotech/topics/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/alarm_parser/__init__.py` & `biotech-1.1.1/venues/stages/biotech/topics/alarm_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__init__.py` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__init__.py` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/treasury.py` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/treasury.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/help_documentation/shares.s.HTML` & `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/shares.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/implicit/proc/__init__.py` & `biotech-1.1.1/venues/stages/biotech/topics/implicit/proc/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/implicit/thread/__init__.py` & `biotech-1.1.1/venues/stages/biotech/topics/implicit/thread/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/printout/passes.py` & `biotech-1.1.1/venues/stages/biotech/topics/printout/passes.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__init__.py` & `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/implicit.py` & `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/parse_records.py` & `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/quay/garage.py` & `biotech-1.1.1/venues/stages/biotech/topics/quay/garage.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/quay/implicit_process_test_1.py` & `biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/quay/implicit_process_test_2.py` & `biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_2.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/quay/implicit_process_test_3.py` & `biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_3.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/quay/implicit_process_test_4.py` & `biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_4.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py` & `biotech-1.1.1/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/show/variable.py` & `biotech-1.1.1/venues/stages/biotech/topics/show/variable.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc` & `biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/venues/stages/biotech/topics/start--/simultaneously.py` & `biotech-1.1.1/venues/stages/biotech/topics/start--/simultaneously.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.0/PKG-INFO` & `biotech-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotech
-Version: 1.1.0
+Version: 1.1.1
 Summary: A health monitoring stack
 License: GPL-3.0-only
 Keywords: alarms,screening,monitors,cybernetics,neurons,nervous system,bioelectric,homeostasis,reliability,consistency,integrity,guarantees,vows,oaths,assurances,insurances,ensurances,speed,calmness,education,augmentation,enhancement,improvements
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

