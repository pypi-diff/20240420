# Comparing `tmp/biotech-1.1.1.tar.gz` & `tmp/biotech-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotech-1.1.1.tar", max compression
+gzip compressed data, was "biotech-1.1.2.tar", max compression
```

## Comparing `biotech-1.1.1.tar` & `biotech-1.1.2.tar`

### file list

```diff
@@ -1,786 +1,766 @@
--rwxr-xr-x   0        0        0      211 2024-04-16 02:07:59.993436 biotech-1.1.1/license.S.HTML
--rwxr-xr-x   0        0        0     1145 2024-04-19 20:38:42.426229 biotech-1.1.1/pyproject.toml
--rwxr-xr-x   0        0        0     3866 2024-04-16 20:53:30.034757 biotech-1.1.1/readme.md
--rwxr-xr-x   0        0        0     2331 2024-04-19 15:34:34.407444 biotech-1.1.1/venue.S.HTML
--rwxr-xr-x   0        0        0   838272 2024-04-16 02:03:26.700967 biotech-1.1.1/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
--rwxr-xr-x   0        0        0     1270 2024-04-17 22:22:59.944800 biotech-1.1.1/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
--rwxr-xr-x   0        0        0     4079 2024-04-16 20:48:34.871383 biotech-1.1.1/venues/stages/biotech/___itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0      645 2024-04-16 20:48:34.875383 biotech-1.1.1/venues/stages/biotech/___itinerary/maybes.s.HTML
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout/script.py
--rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout/start.py
--rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
--rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
--rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
--rwxr-xr-x   0        0        0      385 2024-04-17 18:49:44.656786 biotech-1.1.1/venues/stages/biotech/__glossary/biotech_1
--rwxr-xr-x   0        0        0      114 2024-04-17 18:45:06.744254 biotech-1.1.1/venues/stages/biotech/__glossary/glossary.S.HTML
--rwxr-xr-x   0        0        0      130 2024-04-19 16:49:02.311131 biotech-1.1.1/venues/stages/biotech/__init__.py
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 biotech-1.1.1/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0     1252 2024-04-16 20:48:34.867383 biotech-1.1.1/venues/stages/biotech/_book/advanced tutorial.s.HTML
--rwxr-xr-x   0        0        0     1786 2024-04-16 20:48:34.867383 biotech-1.1.1/venues/stages/biotech/_book/book.s.HTML
--rwxr-xr-x   0        0        0      542 2024-04-16 20:48:34.867383 biotech-1.1.1/venues/stages/biotech/_book/relevant.s.HTML
--rwxr-xr-x   0        0        0     2129 2024-04-17 19:24:51.191926 biotech-1.1.1/venues/stages/biotech/_clique/__init__.py
--rwxr-xr-x   0        0        0     2493 2024-04-17 19:24:52.839918 biotech-1.1.1/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 biotech-1.1.1/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 biotech-1.1.1/venues/stages/biotech/_clique/group/__init__.py
--rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 biotech-1.1.1/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 biotech-1.1.1/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0  1334817 2024-04-19 20:37:52.170777 biotech-1.1.1/venues/stages/biotech/_status/DB/records.json
--rwxr-xr-x   0        0        0     1156 2024-04-19 17:06:33.102985 biotech-1.1.1/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
--rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 biotech-1.1.1/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
--rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 biotech-1.1.1/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
--rwxr-xr-x   0        0        0     1463 2024-04-19 17:05:25.115746 biotech-1.1.1/venues/stages/biotech/_status/establish.py
--rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416142 biotech-1.1.1/venues/stages/biotech/_status/monitors/-1_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 biotech-1.1.1/venues/stages/biotech/_status/monitors/-1_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      720 2024-04-16 20:48:34.887383 biotech-1.1.1/venues/stages/biotech/_status/monitors/-1_start/status_1.py
--rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 biotech-1.1.1/venues/stages/biotech/_status/monitors/0_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 biotech-1.1.1/venues/stages/biotech/_status/monitors/0_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      793 2024-04-16 20:48:34.883383 biotech-1.1.1/venues/stages/biotech/_status/monitors/0_start/status_1.py
--rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708148 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/path_1_health.py
--rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/path_2_health.py
--rwxr-xr-x   0        0        0     1161 2024-04-16 20:48:34.903383 biotech-1.1.1/venues/stages/biotech/_status/monitors/1/status_1.py
--rwxr-xr-x   0        0        0      367 2024-04-16 03:23:58.043895 biotech-1.1.1/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 biotech-1.1.1/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1147 2024-04-19 19:06:56.036882 biotech-1.1.1/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
--rw-r--r--   0        0        0      316 2024-04-19 18:57:32.516036 biotech-1.1.1/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       77 2024-04-19 18:57:24.196146 biotech-1.1.1/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1208 2024-04-19 17:04:46.812176 biotech-1.1.1/venues/stages/biotech/_status/monitors/11/status_1.py
--rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/1_health.py
--rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/2_health.py
--rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/modules/MODULE_1.py
--rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1214 2024-04-16 20:48:34.899383 biotech-1.1.1/venues/stages/biotech/_status/monitors/2/status_1.py
--rwxr-xr-x   0        0        0      794 2024-04-16 20:48:34.891383 biotech-1.1.1/venues/stages/biotech/_status/monitors/3_empty_glob/status_1.py
--rwxr-xr-x   0        0        0      289 2024-04-16 00:28:17.871373 biotech-1.1.1/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      517 2024-04-16 00:32:46.948536 biotech-1.1.1/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      942 2024-04-16 20:48:34.883383 biotech-1.1.1/venues/stages/biotech/_status/monitors/4.1_bad_import/status_1.py
--rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 biotech-1.1.1/venues/stages/biotech/_status/monitors/4_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 biotech-1.1.1/venues/stages/biotech/_status/monitors/4_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      939 2024-04-16 20:48:34.887383 biotech-1.1.1/venues/stages/biotech/_status/monitors/4_bad_import/status_1.py
--rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/1_health.py
--rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      867 2024-04-16 20:48:34.891383 biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/status_1.py
--rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/1_health.py
--rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/2_health.py
--rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/3_health.py
--rw-r--r--   0        0        0     1036 2024-04-19 19:54:47.501752 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc
--rw-r--r--   0        0        0      183 2024-04-19 19:54:47.501752 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/2_health.cpython-310.pyc
--rw-r--r--   0        0        0      169 2024-04-19 19:54:47.505751 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/3_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      926 2024-04-19 19:53:38.302512 biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/status_1.py
--rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 biotech-1.1.1/venues/stages/biotech/_status/monitors/7/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 biotech-1.1.1/venues/stages/biotech/_status/monitors/7/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0      809 2024-04-16 20:48:34.907383 biotech-1.1.1/venues/stages/biotech/_status/monitors/7/status_1.py
--rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 biotech-1.1.1/venues/stages/biotech/_status/monitors/8_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 biotech-1.1.1/venues/stages/biotech/_status/monitors/8_DB/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0     1561 2024-04-19 19:13:07.956368 biotech-1.1.1/venues/stages/biotech/_status/monitors/8_DB/status_1.py
--rwxr-xr-x   0        0        0    84462 2024-04-19 20:37:42.406890 biotech-1.1.1/venues/stages/biotech/_status/monitors/8_DB/variable/status_db/records.json
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_2.py
--rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_3.py
--rwxr-xr-x   0        0        0     1402 2024-04-19 19:21:30.822364 biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/status_1.py
--rwxr-xr-x   0        0        0      984 2024-04-18 03:32:30.971629 biotech-1.1.1/venues/stages/biotech/_status/status.proc.py
--rwxr-xr-x   0        0        0      256 2024-04-16 20:48:34.875383 biotech-1.1.1/venues/stages/biotech/_status/status.s.HTML
--rwxr-xr-x   0        0        0     1483 2024-04-16 20:48:34.851384 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
--rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
--rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
--rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 biotech-1.1.1/venues/stages/biotech/_status_advanced/status.proc.py
--rwxr-xr-x   0        0        0     1779 2024-04-16 20:48:34.575388 biotech-1.1.1/venues/stages/biotech/architecture.s.HTML
--rwxr-xr-x   0        0        0      241 2024-04-16 20:53:18.546926 biotech-1.1.1/venues/stages/biotech/emojis.S.HTML
--rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 biotech-1.1.1/venues/stages/biotech/license.S.HTML
--rwxr-xr-x   0        0        0     3068 2024-04-16 20:48:34.543389 biotech-1.1.1/venues/stages/biotech/module.s.HTML
--rwxr-xr-x   0        0        0     1615 2024-04-19 16:31:12.412493 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      640 2024-04-19 16:26:52.595637 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      259 2024-04-19 16:20:24.028904 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
--rwxr-xr-x   0        0        0     1458 2024-04-19 20:37:55.182742 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.648116 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/paths.py
--rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.660116 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
--rwxr-xr-x   0        0        0      562 2024-04-17 21:48:05.111704 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
--rwxr-xr-x   0        0        0     1163 2024-04-17 21:49:49.362841 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1734 2024-04-19 16:26:14.672115 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
--rwxr-xr-x   0        0        0     2173 2024-04-19 16:27:13.567375 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      965 2024-04-19 16:27:13.567375 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0     2744 2024-04-19 19:39:17.347586 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0     1137 2024-04-19 16:27:13.567375 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      643 2024-04-19 16:26:14.684115 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
--rwxr-xr-x   0        0        0     3672 2024-04-19 19:29:49.876463 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
--rwxr-xr-x   0        0        0      789 2024-04-19 16:26:14.712115 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
--rwxr-xr-x   0        0        0     2031 2024-04-19 16:27:13.563375 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
--rwxr-xr-x   0        0        0     1282 2024-04-15 20:31:31.342880 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0     1743 2024-04-19 18:03:45.582807 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      418 2024-04-17 20:03:55.692458 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      687 2024-04-15 22:21:10.822989 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
--rwxr-xr-x   0        0        0     3455 2024-04-17 21:41:59.150872 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
--rwxr-xr-x   0        0        0      746 2024-04-17 23:09:52.928659 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
--rwxr-xr-x   0        0        0      849 2024-04-17 20:12:15.035804 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
--rwxr-xr-x   0        0        0      933 2024-04-15 23:20:20.086332 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
--rwxr-xr-x   0        0        0     3451 2024-04-19 16:26:14.724115 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
--rwxr-xr-x   0        0        0     2708 2024-04-19 20:38:18.218488 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
--rwxr-xr-x   0        0        0      193 2024-04-17 20:02:37.661229 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
--rwxr-xr-x   0        0        0      566 2024-04-17 23:09:07.804988 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
--rwxr-xr-x   0        0        0     1834 2024-04-19 18:55:07.129933 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
--rw-r--r--   0        0        0     1851 2024-04-19 18:55:11.397883 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      799 2024-04-19 16:27:13.563375 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
--rw-r--r--   0        0        0     3981 2024-04-19 20:36:32.447704 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
--rw-r--r--   0        0        0     1513 2024-04-19 20:34:02.861444 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc
--rw-r--r--   0        0        0     1478 2024-04-19 20:33:58.205499 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py
--rwxr-xr-x   0        0        0      754 2024-04-18 00:33:41.120405 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
--rw-r--r--   0        0        0     1826 2024-04-19 18:56:22.468973 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-19 18:56:27.160910 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      996 2024-04-19 16:26:14.764114 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
--rwxr-xr-x   0        0        0     9002 2024-04-19 20:36:06.236009 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
--rwxr-xr-x   0        0        0     2930 2024-04-19 20:30:14.916104 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
--rw-r--r--   0        0        0     1699 2024-04-19 20:33:08.038083 biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      834 2024-04-16 20:48:34.547389 biotech-1.1.1/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
--rwxr-xr-x   0        0        0      951 2024-04-16 20:49:56.266040 biotech-1.1.1/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      479 2024-04-16 20:49:28.130498 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
--rwxr-xr-x   0        0        0     1838 2024-04-19 16:27:13.567375 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      347 2024-04-16 20:48:34.555389 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/dynamic_port.py
--rwxr-xr-x   0        0        0     2105 2024-04-19 16:26:14.612116 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/on.py
--rwxr-xr-x   0        0        0     2201 2024-04-18 02:31:19.570492 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
--rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
--rwxr-xr-x   0        0        0     1441 2024-04-18 02:04:22.961501 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
--rwxr-xr-x   0        0        0      774 2024-04-16 20:48:34.555389 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
--rwxr-xr-x   0        0        0     1336 2024-04-15 21:13:32.676638 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      309 2024-04-17 23:41:26.722721 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      562 2024-04-17 23:41:26.734721 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      525 2024-04-17 23:09:55.764639 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      908 2024-04-19 20:05:11.362609 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0      636 2024-04-18 01:15:59.039315 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      289 2024-04-17 23:05:28.138584 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
--rwxr-xr-x   0        0        0      803 2024-04-19 20:05:09.858629 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
--rwxr-xr-x   0        0        0      378 2024-04-18 01:13:51.928249 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
--rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
--rwxr-xr-x   0        0        0     2182 2024-04-18 01:57:52.896535 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
--rwxr-xr-x   0        0        0     2125 2024-04-18 01:58:34.052216 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1027 2024-04-17 23:41:26.738721 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0     1368 2024-04-17 23:38:58.631806 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
--rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
--rwxr-xr-x   0        0        0      152 2024-04-19 16:48:50.419277 biotech-1.1.1/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3443 2024-04-19 20:02:47.664429 biotech-1.1.1/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.1/venues/stages/biotech/procedures/intro/intro.S.HTML
--rwxr-xr-x   0        0        0     5074 2024-04-19 20:02:38.772528 biotech-1.1.1/venues/stages/biotech/procedures/intro/on.py
--rw-r--r--   0        0        0     2887 2024-04-19 19:04:05.278996 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
--rw-r--r--   0        0        0     3989 2024-04-19 19:03:05.467745 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/adventure.py
--rwxr-xr-x   0        0        0     1267 2024-04-19 16:26:52.599637 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      905 2024-04-19 16:56:52.013564 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      901 2024-04-19 16:26:14.840113 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      614 2024-04-19 16:56:41.273688 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
--rwxr-xr-x   0        0        0      138 2024-04-19 17:33:23.717242 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/intro.proc.py
--rwxr-xr-x   0        0        0     3047 2024-04-19 19:04:01.875038 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/keg/__init__.py
--rw-r--r--   0        0        0     3044 2024-04-19 19:04:05.278996 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/variables/__init__.py
--rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321766 biotech-1.1.1/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       33 2024-04-17 22:47:27.362384 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/__init__.py
--rwxr-xr-x   0        0        0      192 2024-04-17 22:47:29.166371 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1930 2024-04-19 16:45:15.609992 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     3212 2024-04-19 16:26:52.583637 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/_ops/__pycache__/start.cpython-310.pyc
--rwxr-xr-x   0        0        0     4487 2024-04-19 16:26:14.828113 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/_ops/start.py
--rwxr-xr-x   0        0        0     1267 2024-04-19 16:26:52.599637 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      855 2024-04-19 16:26:52.631636 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      901 2024-04-19 16:26:14.840113 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      572 2024-04-19 16:26:14.856113 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/send_paths.py
--rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/intro.S.HTML
--rwxr-xr-x   0        0        0     1991 2024-04-18 03:48:25.192521 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/keg/__init__.py
--rwxr-xr-x   0        0        0     1394 2024-04-18 06:18:52.492292 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/keg/__init__v1.py
--rwxr-xr-x   0        0        0     2895 2024-04-18 05:23:09.408255 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1447 2024-04-16 20:48:34.559388 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/keg/quart__init__.py
--rwxr-xr-x   0        0        0     2039 2024-04-19 16:45:13.398021 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/on.py
--rwxr-xr-x   0        0        0     4069 2024-04-19 16:41:30.225039 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/intro.proc.py
--rwxr-xr-x   0        0        0     2819 2024-04-19 16:40:32.337866 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/keg/__init__.py
--rwxr-xr-x   0        0        0     3015 2024-04-19 16:40:36.437807 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3062 2024-04-19 16:26:53.431626 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/moves/__pycache__/adventure.cpython-310.pyc
--rwxr-xr-x   0        0        0     4716 2024-04-19 16:26:14.896113 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/moves/adventure.py
--rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/variables/__init__.py
--rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321765 biotech-1.1.1/venues/stages/biotech/procedures/intro_v1/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      172 2024-04-16 20:48:34.551389 biotech-1.1.1/venues/stages/biotech/procedures/procedures.S.HTML
--rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 biotech-1.1.1/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
--rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 biotech-1.1.1/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
--rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 biotech-1.1.1/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 biotech-1.1.1/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 biotech-1.1.1/venues/stages/biotech/topics/aggregate/__init__.py
--rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 biotech-1.1.1/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 biotech-1.1.1/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      708 2024-04-16 20:48:34.591388 biotech-1.1.1/venues/stages/biotech/topics/alarm_parser/__init__.py
--rwxr-xr-x   0        0        0      673 2024-04-16 20:49:28.126498 biotech-1.1.1/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 biotech-1.1.1/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      405 2024-04-16 20:48:34.579388 biotech-1.1.1/venues/stages/biotech/topics/exceptions.py
--rwxr-xr-x   0        0        0     1190 2024-01-27 05:31:08.525189 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
--rwxr-xr-x   0        0        0     2446 2024-04-17 19:24:25.140060 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__init__.py
--rwxr-xr-x   0        0        0     2491 2024-04-17 19:24:52.839918 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4471 2024-02-01 06:11:56.801715 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1050 2024-04-16 06:10:03.111579 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     1920 2024-01-31 18:50:23.812071 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
--rwxr-xr-x   0        0        0       24 2024-01-26 17:38:56.558087 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
--rwxr-xr-x   0        0        0       24 2024-01-26 17:38:52.854129 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
--rwxr-xr-x   0        0        0      751 2024-04-17 19:16:04.226583 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
--rwxr-xr-x   0        0        0     1981 2024-04-17 19:25:47.591625 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__init__.py
--rwxr-xr-x   0        0        0     2283 2024-04-17 19:25:53.011595 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4019 2024-01-31 18:51:47.652157 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     3843 2024-04-17 19:25:53.099595 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
--rwxr-xr-x   0        0        0     4426 2024-01-27 06:34:32.979965 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
--rwxr-xr-x   0        0        0     3559 2024-04-17 19:25:22.227762 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/treasury.py
--rwxr-xr-x   0        0        0     1727 2024-04-17 19:15:19.882965 biotech-1.1.1/venues/stages/biotech/topics/help_documentation/shares.s.HTML
--rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 biotech-1.1.1/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1558 2024-04-18 05:22:02.832642 biotech-1.1.1/venues/stages/biotech/topics/implicit/proc/__init__.py
--rwxr-xr-x   0        0        0     1155 2024-04-18 05:46:33.436738 biotech-1.1.1/venues/stages/biotech/topics/implicit/thread/__init__.py
--rwxr-xr-x   0        0        0      855 2024-04-18 06:05:23.346518 biotech-1.1.1/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       90 2024-04-17 22:51:08.968798 biotech-1.1.1/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 22:33:48.860256 biotech-1.1.1/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
--rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 biotech-1.1.1/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
--rwxr-xr-x   0        0        0      470 2024-04-17 23:02:14.419990 biotech-1.1.1/venues/stages/biotech/topics/printout/bracket.py
--rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 biotech-1.1.1/venues/stages/biotech/topics/printout/passes.py
--rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 biotech-1.1.1/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2163 2024-04-19 18:50:11.157390 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__init__.py
--rw-r--r--   0        0        0     1997 2024-04-19 18:52:58.595432 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
--rw-r--r--   0        0        0     1818 2024-04-19 18:54:33.250328 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-18 01:45:27.254200 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1766 2024-04-19 18:53:11.523281 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-18 01:48:34.504806 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-18 01:45:24.082223 biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
--rwxr-xr-x   0        0        0      195 2024-04-16 22:50:54.515336 biotech-1.1.1/venues/stages/biotech/topics/process_on/process_on.S.HTML
--rwxr-xr-x   0        0        0     1470 2024-04-18 04:12:56.845888 biotech-1.1.1/venues/stages/biotech/topics/quay/garage.py
--rwxr-xr-x   0        0        0     2546 2024-04-18 04:38:41.478278 biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_1.py
--rwxr-xr-x   0        0        0     1612 2024-04-18 04:54:58.414971 biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_2.py
--rwxr-xr-x   0        0        0      551 2024-04-18 05:20:40.701113 biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_3.py
--rwxr-xr-x   0        0        0     1083 2024-04-18 05:19:11.645613 biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_4.py
--rwxr-xr-x   0        0        0     1442 2024-04-16 20:48:34.591388 biotech-1.1.1/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
--rwxr-xr-x   0        0        0     1464 2024-04-16 20:49:28.126498 biotech-1.1.1/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 biotech-1.1.1/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
--rw-r--r--   0        0        0     1776 2024-04-19 19:50:41.332444 biotech-1.1.1/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0      461 2024-04-17 23:59:06.614967 biotech-1.1.1/venues/stages/biotech/topics/show/show.S.HTML
--rwxr-xr-x   0        0        0     2305 2024-04-19 19:50:39.412465 biotech-1.1.1/venues/stages/biotech/topics/show/variable.py
--rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
--rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
--rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
--rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
--rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
--rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
--rwxr-xr-x   0        0        0      273 2024-04-16 20:48:34.583388 biotech-1.1.1/venues/stages/biotech/topics/start--/one.py
--rwxr-xr-x   0        0        0      406 2024-04-16 20:48:34.587388 biotech-1.1.1/venues/stages/biotech/topics/start--/sequentially.py
--rwxr-xr-x   0        0        0      532 2024-04-16 20:48:34.587388 biotech-1.1.1/venues/stages/biotech/topics/start--/simultaneously.py
--rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 biotech-1.1.1/venues/stages/biotech/topics/topics.S.HTML
--rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 biotech-1.1.1/venues/stages/biotech/variables/__init__.py
--rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      211 2024-04-16 02:07:59.993436 biotech-1.1.2/license.S.HTML
+-rwxr-xr-x   0        0        0     1145 2024-04-19 22:47:27.763896 biotech-1.1.2/pyproject.toml
+-rwxr-xr-x   0        0        0     3866 2024-04-16 20:53:30.034757 biotech-1.1.2/readme.md
+-rwxr-xr-x   0        0        0     2331 2024-04-19 15:34:34.407444 biotech-1.1.2/venue.S.HTML
+-rwxr-xr-x   0        0        0   838272 2024-04-16 02:03:26.700967 biotech-1.1.2/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
+-rwxr-xr-x   0        0        0     1270 2024-04-17 22:22:59.944800 biotech-1.1.2/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
+-rwxr-xr-x   0        0        0     4079 2024-04-16 20:48:34.871383 biotech-1.1.2/venues/stages/biotech/___itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      645 2024-04-16 20:48:34.875383 biotech-1.1.2/venues/stages/biotech/___itinerary/maybes.s.HTML
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout/script.py
+-rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout/start.py
+-rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
+-rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
+-rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
+-rwxr-xr-x   0        0        0      385 2024-04-17 18:49:44.656786 biotech-1.1.2/venues/stages/biotech/__glossary/biotech_1
+-rwxr-xr-x   0        0        0      114 2024-04-17 18:45:06.744254 biotech-1.1.2/venues/stages/biotech/__glossary/glossary.S.HTML
+-rwxr-xr-x   0        0        0      130 2024-04-19 16:49:02.311131 biotech-1.1.2/venues/stages/biotech/__init__.py
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 biotech-1.1.2/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0     1252 2024-04-16 20:48:34.867383 biotech-1.1.2/venues/stages/biotech/_book/advanced tutorial.s.HTML
+-rwxr-xr-x   0        0        0     1786 2024-04-16 20:48:34.867383 biotech-1.1.2/venues/stages/biotech/_book/book.s.HTML
+-rwxr-xr-x   0        0        0      542 2024-04-16 20:48:34.867383 biotech-1.1.2/venues/stages/biotech/_book/relevant.s.HTML
+-rwxr-xr-x   0        0        0     2129 2024-04-17 19:24:51.191926 biotech-1.1.2/venues/stages/biotech/_clique/__init__.py
+-rwxr-xr-x   0        0        0     2493 2024-04-17 19:24:52.839918 biotech-1.1.2/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 biotech-1.1.2/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 biotech-1.1.2/venues/stages/biotech/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 biotech-1.1.2/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 biotech-1.1.2/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0  1401783 2024-04-19 22:46:46.716354 biotech-1.1.2/venues/stages/biotech/_status/DB/records.json
+-rw-r--r--   0        0        0     1172 2024-04-19 22:15:38.920875 biotech-1.1.2/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 biotech-1.1.2/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 biotech-1.1.2/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1487 2024-04-19 22:15:36.412903 biotech-1.1.2/venues/stages/biotech/_status/establish.py
+-rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416142 biotech-1.1.2/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 biotech-1.1.2/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      720 2024-04-16 20:48:34.887383 biotech-1.1.2/venues/stages/biotech/_status/monitors/-01_start/status_1.py
+-rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 biotech-1.1.2/venues/stages/biotech/_status/monitors/00_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 biotech-1.1.2/venues/stages/biotech/_status/monitors/00_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      793 2024-04-16 20:48:34.883383 biotech-1.1.2/venues/stages/biotech/_status/monitors/00_start/status_1.py
+-rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708148 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/path_1_health.py
+-rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/path_2_health.py
+-rwxr-xr-x   0        0        0     1161 2024-04-16 20:48:34.903383 biotech-1.1.2/venues/stages/biotech/_status/monitors/01/status_1.py
+-rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/1_health.py
+-rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/2_health.py
+-rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/modules/MODULE_1.py
+-rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1214 2024-04-16 20:48:34.899383 biotech-1.1.2/venues/stages/biotech/_status/monitors/02/status_1.py
+-rwxr-xr-x   0        0        0      794 2024-04-16 20:48:34.891383 biotech-1.1.2/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py
+-rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 biotech-1.1.2/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 biotech-1.1.2/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      939 2024-04-16 20:48:34.887383 biotech-1.1.2/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      289 2024-04-16 00:28:17.871373 biotech-1.1.2/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      517 2024-04-16 00:32:46.948536 biotech-1.1.2/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      942 2024-04-16 20:48:34.883383 biotech-1.1.2/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py
+-rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      867 2024-04-16 20:48:34.891383 biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/status_1.py
+-rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/1_health.py
+-rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/2_health.py
+-rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/3_health.py
+-rw-r--r--   0        0        0     1036 2024-04-19 19:54:47.501752 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/1_health.cpython-310.pyc
+-rw-r--r--   0        0        0      183 2024-04-19 19:54:47.501752 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/2_health.cpython-310.pyc
+-rw-r--r--   0        0        0      169 2024-04-19 19:54:47.505751 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/3_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      955 2024-04-19 22:40:42.880411 biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/status_1.py
+-rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 biotech-1.1.2/venues/stages/biotech/_status/monitors/07/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 biotech-1.1.2/venues/stages/biotech/_status/monitors/07/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0      809 2024-04-16 20:48:34.907383 biotech-1.1.2/venues/stages/biotech/_status/monitors/07/status_1.py
+-rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 biotech-1.1.2/venues/stages/biotech/_status/monitors/08_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 biotech-1.1.2/venues/stages/biotech/_status/monitors/08_DB/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0     1561 2024-04-19 19:13:07.956368 biotech-1.1.2/venues/stages/biotech/_status/monitors/08_DB/status_1.py
+-rwxr-xr-x   0        0        0    93689 2024-04-19 22:46:21.516636 biotech-1.1.2/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_2.py
+-rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_3.py
+-rwxr-xr-x   0        0        0     1442 2024-04-19 22:43:25.306602 biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py
+-rwxr-xr-x   0        0        0      367 2024-04-16 03:23:58.043895 biotech-1.1.2/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 biotech-1.1.2/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1189 2024-04-19 21:55:08.998787 biotech-1.1.2/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
+-rw-r--r--   0        0        0      316 2024-04-19 18:57:32.516036 biotech-1.1.2/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.2/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       77 2024-04-19 18:57:24.196146 biotech-1.1.2/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1250 2024-04-19 21:55:16.358703 biotech-1.1.2/venues/stages/biotech/_status/monitors/11/status_1.py
+-rwxr-xr-x   0        0        0      984 2024-04-18 03:32:30.971629 biotech-1.1.2/venues/stages/biotech/_status/status.proc.py
+-rwxr-xr-x   0        0        0      256 2024-04-16 20:48:34.875383 biotech-1.1.2/venues/stages/biotech/_status/status.s.HTML
+-rwxr-xr-x   0        0        0     1483 2024-04-16 20:48:34.851384 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
+-rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
+-rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 biotech-1.1.2/venues/stages/biotech/_status_advanced/status.proc.py
+-rwxr-xr-x   0        0        0     1779 2024-04-16 20:48:34.575388 biotech-1.1.2/venues/stages/biotech/architecture.s.HTML
+-rwxr-xr-x   0        0        0      241 2024-04-16 20:53:18.546926 biotech-1.1.2/venues/stages/biotech/emojis.S.HTML
+-rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 biotech-1.1.2/venues/stages/biotech/license.S.HTML
+-rwxr-xr-x   0        0        0     3068 2024-04-16 20:48:34.543389 biotech-1.1.2/venues/stages/biotech/module.s.HTML
+-rw-r--r--   0        0        0     1596 2024-04-19 21:12:05.931720 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      640 2024-04-19 16:26:52.595637 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      259 2024-04-19 16:20:24.028904 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
+-rwxr-xr-x   0        0        0     1478 2024-04-19 21:11:18.368263 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.648116 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/paths.py
+-rwxr-xr-x   0        0        0      666 2024-04-19 21:46:15.516790 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
+-rwxr-xr-x   0        0        0      562 2024-04-17 21:48:05.111704 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
+-rwxr-xr-x   0        0        0     1163 2024-04-17 21:49:49.362841 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2023 2024-04-19 20:54:28.011750 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
+-rw-r--r--   0        0        0     2447 2024-04-19 20:54:32.867695 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0      999 2024-04-19 20:57:55.937395 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0     2881 2024-04-19 21:20:39.102102 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
+-rw-r--r--   0        0        0     1152 2024-04-19 21:06:40.923425 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      653 2024-04-19 20:56:23.606442 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
+-rwxr-xr-x   0        0        0     3572 2024-04-19 21:20:33.674162 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
+-rwxr-xr-x   0        0        0      769 2024-04-19 21:06:33.619508 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
+-rwxr-xr-x   0        0        0     2031 2024-04-19 16:27:13.563375 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1282 2024-04-15 20:31:31.342880 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0     1916 2024-04-19 22:44:37.277799 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      418 2024-04-17 20:03:55.692458 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      687 2024-04-15 22:21:10.822989 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3455 2024-04-17 21:41:59.150872 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
+-rw-r--r--   0        0        0      728 2024-04-19 20:59:04.160621 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0      849 2024-04-17 20:12:15.035804 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
+-rwxr-xr-x   0        0        0      933 2024-04-15 23:20:20.086332 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3451 2024-04-19 16:26:14.724115 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
+-rwxr-xr-x   0        0        0     2917 2024-04-19 22:44:35.329821 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
+-rwxr-xr-x   0        0        0      193 2024-04-17 20:02:37.661229 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
+-rwxr-xr-x   0        0        0      514 2024-04-19 20:59:00.568662 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
+-rwxr-xr-x   0        0        0     1834 2024-04-19 18:55:07.129933 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
+-rw-r--r--   0        0        0     1851 2024-04-19 18:55:11.397883 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      799 2024-04-19 16:27:13.563375 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
+-rw-r--r--   0        0        0     3986 2024-04-19 22:42:08.999452 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
+-rw-r--r--   0        0        0     1513 2024-04-19 20:34:02.861444 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc
+-rw-r--r--   0        0        0     1478 2024-04-19 20:33:58.205499 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py
+-rwxr-xr-x   0        0        0      754 2024-04-18 00:33:41.120405 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
+-rw-r--r--   0        0        0     1826 2024-04-19 18:56:22.468973 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-19 18:56:27.160910 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      996 2024-04-19 16:26:14.764114 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
+-rwxr-xr-x   0        0        0     9007 2024-04-19 22:42:04.947497 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
+-rwxr-xr-x   0        0        0     3137 2024-04-19 22:45:07.077467 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
+-rw-r--r--   0        0        0     1985 2024-04-19 22:45:12.801403 biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      834 2024-04-16 20:48:34.547389 biotech-1.1.2/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
+-rwxr-xr-x   0        0        0      951 2024-04-16 20:49:56.266040 biotech-1.1.2/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      609 2024-04-19 22:29:43.435688 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
+-rw-r--r--   0        0        0     1904 2024-04-19 22:33:09.357432 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      500 2024-04-19 22:29:36.979758 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/dynamic_port.py
+-rwxr-xr-x   0        0        0     2161 2024-04-19 22:31:07.314772 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/on.py
+-rwxr-xr-x   0        0        0     2200 2024-04-19 22:24:22.967141 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
+-rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
+-rwxr-xr-x   0        0        0     1441 2024-04-18 02:04:22.961501 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
+-rwxr-xr-x   0        0        0      774 2024-04-16 20:48:34.555389 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
+-rwxr-xr-x   0        0        0     1336 2024-04-15 21:13:32.676638 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      309 2024-04-17 23:41:26.722721 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      562 2024-04-17 23:41:26.734721 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      525 2024-04-17 23:09:55.764639 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      908 2024-04-19 20:05:11.362609 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      636 2024-04-18 01:15:59.039315 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      289 2024-04-17 23:05:28.138584 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
+-rwxr-xr-x   0        0        0      803 2024-04-19 20:05:09.858629 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
+-rwxr-xr-x   0        0        0      378 2024-04-18 01:13:51.928249 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
+-rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
+-rwxr-xr-x   0        0        0     2182 2024-04-18 01:57:52.896535 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
+-rwxr-xr-x   0        0        0     2125 2024-04-18 01:58:34.052216 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1828 2024-04-19 21:04:56.668613 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2295 2024-04-19 21:04:32.800884 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
+-rw-r--r--   0        0        0        2 2024-04-19 22:32:11.666067 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/start.py
+-rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
+-rwxr-xr-x   0        0        0      152 2024-04-19 16:48:50.419277 biotech-1.1.2/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4699 2024-04-19 22:17:01.343942 biotech-1.1.2/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.2/venues/stages/biotech/procedures/intro/intro.S.HTML
+-rwxr-xr-x   0        0        0     6305 2024-04-19 22:16:54.188023 biotech-1.1.2/venues/stages/biotech/procedures/intro/on.py
+-rw-r--r--   0        0        0     2906 2024-04-19 21:43:07.254923 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
+-rw-r--r--   0        0        0     4000 2024-04-19 21:42:57.331035 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/adventure.py
+-rw-r--r--   0        0        0     1330 2024-04-19 21:12:05.939720 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      905 2024-04-19 16:56:52.013564 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      959 2024-04-19 21:11:59.243796 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      614 2024-04-19 16:56:41.273688 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
+-rwxr-xr-x   0        0        0      138 2024-04-19 17:33:23.717242 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/intro.proc.py
+-rwxr-xr-x   0        0        0     3084 2024-04-19 21:01:52.394709 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/keg/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-19 21:01:58.358642 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/variables/__init__.py
+-rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321766 biotech-1.1.2/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      172 2024-04-16 20:48:34.551389 biotech-1.1.2/venues/stages/biotech/procedures/procedures.S.HTML
+-rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 biotech-1.1.2/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 biotech-1.1.2/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
+-rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 biotech-1.1.2/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 biotech-1.1.2/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 biotech-1.1.2/venues/stages/biotech/topics/aggregate/__init__.py
+-rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 biotech-1.1.2/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 biotech-1.1.2/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      708 2024-04-16 20:48:34.591388 biotech-1.1.2/venues/stages/biotech/topics/alarm_parser/__init__.py
+-rwxr-xr-x   0        0        0      673 2024-04-16 20:49:28.126498 biotech-1.1.2/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 biotech-1.1.2/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      405 2024-04-16 20:48:34.579388 biotech-1.1.2/venues/stages/biotech/topics/exceptions.py
+-rwxr-xr-x   0        0        0     1190 2024-01-27 05:31:08.525189 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
+-rwxr-xr-x   0        0        0     2446 2024-04-17 19:24:25.140060 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__init__.py
+-rwxr-xr-x   0        0        0     2491 2024-04-17 19:24:52.839918 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4471 2024-02-01 06:11:56.801715 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1050 2024-04-16 06:10:03.111579 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1920 2024-01-31 18:50:23.812071 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
+-rwxr-xr-x   0        0        0       24 2024-01-26 17:38:56.558087 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
+-rwxr-xr-x   0        0        0       24 2024-01-26 17:38:52.854129 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
+-rwxr-xr-x   0        0        0      751 2024-04-17 19:16:04.226583 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
+-rwxr-xr-x   0        0        0     1981 2024-04-17 19:25:47.591625 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__init__.py
+-rwxr-xr-x   0        0        0     2283 2024-04-17 19:25:53.011595 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4019 2024-01-31 18:51:47.652157 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3843 2024-04-17 19:25:53.099595 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4426 2024-01-27 06:34:32.979965 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3559 2024-04-17 19:25:22.227762 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/treasury.py
+-rwxr-xr-x   0        0        0     1727 2024-04-17 19:15:19.882965 biotech-1.1.2/venues/stages/biotech/topics/help_documentation/shares.s.HTML
+-rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 biotech-1.1.2/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1558 2024-04-18 05:22:02.832642 biotech-1.1.2/venues/stages/biotech/topics/implicit/proc/__init__.py
+-rwxr-xr-x   0        0        0     1158 2024-04-19 21:23:01.800513 biotech-1.1.2/venues/stages/biotech/topics/implicit/thread/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-19 21:23:28.056219 biotech-1.1.2/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       90 2024-04-17 22:51:08.968798 biotech-1.1.2/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 22:33:48.860256 biotech-1.1.2/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
+-rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 biotech-1.1.2/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
+-rwxr-xr-x   0        0        0      470 2024-04-17 23:02:14.419990 biotech-1.1.2/venues/stages/biotech/topics/printout/bracket.py
+-rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 biotech-1.1.2/venues/stages/biotech/topics/printout/passes.py
+-rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 biotech-1.1.2/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2166 2024-04-19 22:38:28.357906 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__init__.py
+-rw-r--r--   0        0        0     1997 2024-04-19 22:38:43.137742 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
+-rw-r--r--   0        0        0     1818 2024-04-19 18:54:33.250328 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-18 01:45:27.254200 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1766 2024-04-19 18:53:11.523281 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-18 01:48:34.504806 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-18 01:45:24.082223 biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
+-rwxr-xr-x   0        0        0      195 2024-04-16 22:50:54.515336 biotech-1.1.2/venues/stages/biotech/topics/process_on/process_on.S.HTML
+-rwxr-xr-x   0        0        0     1470 2024-04-18 04:12:56.845888 biotech-1.1.2/venues/stages/biotech/topics/quay/garage.py
+-rwxr-xr-x   0        0        0     2546 2024-04-18 04:38:41.478278 biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_1.py
+-rwxr-xr-x   0        0        0     1612 2024-04-18 04:54:58.414971 biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_2.py
+-rwxr-xr-x   0        0        0      551 2024-04-18 05:20:40.701113 biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_3.py
+-rwxr-xr-x   0        0        0     1083 2024-04-18 05:19:11.645613 biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_4.py
+-rwxr-xr-x   0        0        0     1448 2024-04-19 22:40:22.232641 biotech-1.1.2/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
+-rw-r--r--   0        0        0     1464 2024-04-19 22:41:14.292061 biotech-1.1.2/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 biotech-1.1.2/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-19 21:18:20.963631 biotech-1.1.2/venues/stages/biotech/topics/report_formats/report_formats.S.HTML
+-rw-r--r--   0        0        0     1772 2024-04-19 20:59:56.440027 biotech-1.1.2/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0      461 2024-04-17 23:59:06.614967 biotech-1.1.2/venues/stages/biotech/topics/show/show.S.HTML
+-rwxr-xr-x   0        0        0     2295 2024-04-19 20:59:53.444061 biotech-1.1.2/venues/stages/biotech/topics/show/variable.py
+-rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
+-rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
+-rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
+-rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
+-rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
+-rwxr-xr-x   0        0        0      273 2024-04-16 20:48:34.583388 biotech-1.1.2/venues/stages/biotech/topics/start--/one.py
+-rwxr-xr-x   0        0        0      406 2024-04-16 20:48:34.587388 biotech-1.1.2/venues/stages/biotech/topics/start--/sequentially.py
+-rwxr-xr-x   0        0        0      532 2024-04-16 20:48:34.587388 biotech-1.1.2/venues/stages/biotech/topics/start--/simultaneously.py
+-rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 biotech-1.1.2/venues/stages/biotech/topics/topics.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 biotech-1.1.2/venues/stages/biotech/variables/__init__.py
+-rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.2/PKG-INFO
```

### Comparing `biotech-1.1.1/pyproject.toml` & `biotech-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 [tool.poetry]
 name = "biotech"
-version = "1.1.1"
+version = "1.1.2"
 description = "A health monitoring stack"
 authors = []
 readme = "readme.md"
 
 packages = [
     { include = "biotech", from = "venues/stages" }
 ]
```

### Comparing `biotech-1.1.1/readme.md` & `biotech-1.1.2/readme.md`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venue.S.HTML` & `biotech-1.1.2/venue.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg` & `biotech-1.1.2/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML` & `biotech-1.1.2/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/___itinerary/itinerary.S.HTML` & `biotech-1.1.2/venues/stages/biotech/___itinerary/itinerary.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/___itinerary/maybes.s.HTML` & `biotech-1.1.2/venues/stages/biotech/___itinerary/maybes.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout/start.py` & `biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/___itinerary/processes/errout_v2/start.py` & `biotech-1.1.2/venues/stages/biotech/___itinerary/processes/errout_v2/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/__license/options/gpl-3.0-standalone.html` & `biotech-1.1.2/venues/stages/biotech/__license/options/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_book/advanced tutorial.s.HTML` & `biotech-1.1.2/venues/stages/biotech/_book/advanced tutorial.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_book/book.s.HTML` & `biotech-1.1.2/venues/stages/biotech/_book/book.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_book/relevant.s.HTML` & `biotech-1.1.2/venues/stages/biotech/_book/relevant.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_clique/__init__.py` & `biotech-1.1.2/venues/stages/biotech/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/DB/records.json` & `biotech-1.1.2/venues/stages/biotech/_status/DB/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.979539641943734%*

 * *Differences: {"'_default'": "{'376': OrderedDict([('paths', [OrderedDict([('path', "*

 * *               "'_status/monitors/9_aggregation_format_and_exit/status_1.py'), ('empty', False), "*

 * *               "('parsed', True), ('stats', OrderedDict([('passes', 0), ('alarms', 1)])), "*

 * *               "('checks', [OrderedDict([('check', 'aggregation format and exit'), ('passed', "*

 * *               'False), (\'exception\', "AssertionError({\'checks\': {\'alarms\': 0, \'passes\': '*

 * *               '0}, \'paths\': {\'alarms\': 3, \'empty […]*

```diff
@@ -47705,14 +47705,1566 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 14
                 },
                 "empty": 0
             }
         },
+        "376": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "AssertionError({'checks': {'alarms': 0, 'passes': 0}, 'paths': {'alarms': 3, 'empty': 0}})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 55, in check_1",
+                                "AssertionError: {'checks': {'alarms': 0, 'passes': 0}, 'paths': {'alarms': 3, 'empty': 0}}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 21, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/0_start/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('results')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 19, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 90, in start",
+                                "    the_report = bio [\"results\"]",
+                                "KeyError: 'results'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/4.1_bad_import/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 24, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/11/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('results')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 18, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 90, in start",
+                                "    the_report = bio [\"results\"]",
+                                "KeyError: 'results'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/4_bad_import/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 19, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/-1_start/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('results')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 16, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 90, in start",
+                                "    the_report = bio [\"results\"]",
+                                "KeyError: 'results'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/5__file__/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 14, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_empty_glob/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('results')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 22, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 90, in start",
+                                "    the_report = bio [\"results\"]",
+                                "KeyError: 'results'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/6_various/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 29, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('results')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 25, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 90, in start",
+                                "    the_report = bio [\"results\"]",
+                                "KeyError: 'results'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 14, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/7/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "tinyDB database can be utilized",
+                            "exception": "KeyError('results')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 24, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 90, in start",
+                                "    the_report = bio [\"results\"]",
+                                "KeyError: 'results'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/8_DB/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 21, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/10_time_limits/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "AssertionError({'checks': {'alarms': 0, 'passes': 0}, 'paths': {'alarms': 3, 'empty': 0}})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 55, in check_1",
+                                "AssertionError: {'checks': {'alarms': 0, 'passes': 0}, 'paths': {'alarms': 3, 'empty': 0}}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 21, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/0_start/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('results')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 19, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 90, in start",
+                                "    the_report = bio [\"results\"]",
+                                "KeyError: 'results'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4.1_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 24, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/11/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('results')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 18, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 90, in start",
+                                "    the_report = bio [\"results\"]",
+                                "KeyError: 'results'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 19, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/-1_start/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('results')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 16, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 90, in start",
+                                "    the_report = bio [\"results\"]",
+                                "KeyError: 'results'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5__file__/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 14, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_empty_glob/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('results')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 22, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 90, in start",
+                                "    the_report = bio [\"results\"]",
+                                "KeyError: 'results'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/6_various/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 29, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('results')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 25, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 90, in start",
+                                "    the_report = bio [\"results\"]",
+                                "KeyError: 'results'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 14, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/7/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "tinyDB database can be utilized",
+                            "exception": "KeyError('results')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 24, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 90, in start",
+                                "    the_report = bio [\"results\"]",
+                                "KeyError: 'results'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/8_DB/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 21, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/10_time_limits/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 14,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "377": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 21, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/0_start/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 24, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/11/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 19, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/-1_start/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 14, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_empty_glob/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/6_various/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 29, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 14, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/7/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 21, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/10_time_limits/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                5.080182421002974,
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
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 21, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/0_start/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.0973227089998545,
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
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 24, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/11/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.076436059000116,
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
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 19, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/-1_start/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.169224829998711,
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
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 14, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_empty_glob/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/6_various/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 29, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.194523497000773,
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
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 14, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 59, in start",
+                                "    bio = on ({",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/7/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "tinyDB database can be utilized",
+                            "elapsed": [
+                                5.216391030997329,
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
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 21, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 162, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 159, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/10_time_limits/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 8,
+                    "passes": 6
+                },
+                "empty": 0
+            }
+        },
+        "378": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "AssertionError({'checks': {'alarms': 0, 'passes': 0}, 'paths': {'alarms': 3, 'empty': 0}})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 55, in check_1",
+                                "AssertionError: {'checks': {'alarms': 0, 'passes': 0}, 'paths': {'alarms': 3, 'empty': 0}}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 2, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 1})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 2, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 1}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/6_various/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "AssertionError({'checks': {'alarms': 0, 'passes': 0}, 'paths': {'alarms': 3, 'empty': 0}})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 55, in check_1",
+                                "AssertionError: {'checks': {'alarms': 0, 'passes': 0}, 'paths': {'alarms': 3, 'empty': 0}}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.079821452000033,
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
+                                6.0657988830025715,
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
+                                6.093763917000615,
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
+                                6.097993917999702,
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
+                                6.087028542999178,
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
+                                6.160786312997516,
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
+                                4.155494137998176,
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
+                            "exception": "AssertionError({'alarms': 2, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 1})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 2, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 1}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/6_various/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.107828712996707,
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
+                                6.122188633002224,
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
+                                6.134315068000433,
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
+                                6.140626191998308,
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
+                                10.10495857999922,
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
+                    "alarms": 2,
+                    "passes": 12
+                },
+                "empty": 0
+            }
+        },
+        "379": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                14.198100232999423,
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
         "38": {
             "alarms": [],
             "paths": [
                 {
                     "empty": true,
                     "parsed": true,
                     "path": "_status/status_py.py"
@@ -47913,14 +49465,1261 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 10
                 },
                 "empty": 1
             }
         },
+        "380": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/06_various/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.08742057299969,
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
+                                6.099539047001599,
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
+                                6.116965051998704,
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
+                                6.079120038997644,
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
+                                4.114934564000578,
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
+                                6.088949018998392,
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
+                                6.081802721000713,
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
+                                6.1880246689979685,
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
+                            "exception": "AssertionError({'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/06_various/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.171720776001166,
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
+                                6.210681663000287,
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
+                                14.157731871997385,
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
+                                10.121654624999792,
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
+                                6.0568245419999585,
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
+                    "alarms": 1,
+                    "passes": 13
+                },
+                "empty": 0
+            }
+        },
+        "381": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/06_various/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.096657998001319,
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
+                                6.0975219380015915,
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
+                                6.1862348549984745,
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
+                                6.107738402002724,
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
+                                4.1629596870006935,
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
+                                6.0987686999978905,
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
+                                6.094808034999005,
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
+                                6.162109001998033,
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
+                            "exception": "AssertionError({'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/06_various/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.160690215998329,
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
+                                6.2388610359994345,
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
+                                14.155379811003513,
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
+                                10.126058747999195,
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
+                                6.085770387999219,
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
+                    "alarms": 1,
+                    "passes": 13
+                },
+                "empty": 0
+            }
+        },
+        "382": {
+            "alarms": [],
+            "paths": [],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "383": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/06_various/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 3, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 0}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/06_various/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "384": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 2, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 1})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 2, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 1}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/06_various/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 2, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 1})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 2, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 1}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/06_various/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "385": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 2, 'checks': {'alarms': 1, 'passes': 7}, 'empty': 0})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 2, 'checks': {'alarms': 1, 'passes': 7}, 'empty': 0}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/06_various/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 2, 'checks': {'alarms': 1, 'passes': 7}, 'empty': 0})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 2, 'checks': {'alarms': 1, 'passes': 7}, 'empty': 0}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/06_various/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "386": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 2, 'checks': {'alarms': 1, 'passes': 7}, 'empty': 0})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 2, 'checks': {'alarms': 1, 'passes': 7}, 'empty': 0}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/06_various/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 2, 'checks': {'alarms': 1, 'passes': 7}, 'empty': 0})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 2, 'checks': {'alarms': 1, 'passes': 7}, 'empty': 0}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/06_various/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "387": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 2, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 1})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 2, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 1}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/06_various/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError({'alarms': 2, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 1})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 37, in check_1",
+                                "AssertionError: {'alarms': 2, 'checks': {'alarms': 0, 'passes': 0}, 'empty': 1}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/06_various/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "388": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "AssertionError({'checks': {'alarms': 0, 'passes': 0}, 'paths': {'alarms': 3, 'empty': 0}})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 55, in check_1",
+                                "AssertionError: {'checks': {'alarms': 0, 'passes': 0}, 'paths': {'alarms': 3, 'empty': 0}}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/09_aggregation_format_and_exit/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.069651454999985,
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
+                                6.09494943000027,
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
+                                6.170636097998795,
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
+                                6.101061380002648,
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
+                                4.107726695998281,
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
+                                6.0449240779998945,
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
+                                6.071065107000322,
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
+                                6.141303543001413,
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
+                                6.10294415899989,
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
+                                6.1861246270018455,
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
+                                6.209484005001286,
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
+                            "exception": "AssertionError({'checks': {'alarms': 0, 'passes': 0}, 'paths': {'alarms': 3, 'empty': 0}})",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 55, in check_1",
+                                "AssertionError: {'checks': {'alarms': 0, 'passes': 0}, 'paths': {'alarms': 3, 'empty': 0}}"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/09_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                10.09784174699962,
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
+                                6.0966614940007275,
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
+                    "alarms": 1,
+                    "passes": 13
+                },
+                "empty": 0
+            }
+        },
+        "389": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 26, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 168, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 165, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/09_aggregation_format_and_exit/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "Exception('The intro harbor is already on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/biotech/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 26, in check_1",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 168, in on",
+                                "    check_that_intro_harbor_is_not_on ()",
+                                "  File \"/biotech/venues/stages/biotech/procedures/intro/on.py\", line 165, in check_that_intro_harbor_is_not_on",
+                                "    raise Exception (\"The intro harbor is already on.\")",
+                                "Exception: The intro harbor is already on."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/09_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
         "39": {
             "alarms": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
                             "exception": "Exception('The loop limit was reached.')",
@@ -48903,14 +51702,572 @@
                 "checks": {
                     "alarms": 9,
                     "passes": 1
                 },
                 "empty": 1
             }
         },
+        "390": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.082588358000066,
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
+                                6.092748705003032,
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
+                                6.165069912000035,
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
+                                6.049438275000284,
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
+                                4.130419017001259,
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
+                                6.0982737409976835,
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
+                                6.053375822000817,
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
+                                6.183761563999724,
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
+                                6.115303464001045,
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
+                                6.156751684000483,
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
+                                6.181615654997586,
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
+                                6.115533954001876,
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
+                                10.127923017000285,
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
+                                6.074411757999769,
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
+        "391": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.049152258001413,
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
+                                6.09418904800259,
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
+                                6.188703200001328,
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
+                                6.091211428996758,
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
+                                4.156239201998687,
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
+                                6.093051097999705,
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
+                                6.078211400999862,
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
+                                6.145647044002544,
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
+                                6.1146279820022755,
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
+                                6.157825153000886,
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
+                                6.188270069000282,
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
+                                6.078861147001589,
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
+                                10.11689706299876,
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
+                                6.060024387999874,
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

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 17:05:25 2024 UTC, .py size: 1463 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,74 @@
-00000000: 6f0d 0d0a 0000 0000 55a4 2266 b705 0000  o.......U."f....
+00000000: 6f0d 0d0a 0000 0000 08ed 2266 cf05 0000  o........."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 5a00 0900 6401 6402 6c01 5a01 6401 6402  Z...d.d.l.Z.d.d.
 00000040: 6c02 5a02 6401 6403 6c03 6d04 5a04 6d05  l.Z.d.d.l.m.Z.m.
 00000050: 5a05 6d06 5a06 0100 6401 6402 6c07 5a07  Z.m.Z...d.d.l.Z.
 00000060: 6401 6402 6c08 5a08 6401 6402 6c09 5a09  d.d.l.Z.d.d.l.Z.
 00000070: 0904 6407 6405 6406 8401 5a0a 6402 5300  ..d.d.d...Z.d.S.
 00000080: 2908 7a3e 0a09 5468 6973 206f 6e65 2069  ).z>..This one i
 00000090: 7320 666f 7220 6361 6c6c 696e 670a 090a  s for calling...
 000000a0: 0909 5b78 6f6e 7368 5d20 6269 6f74 6563  ..[xonsh] biotec
 000000b0: 6820 7374 6174 7573 2d69 6e74 6572 6e61  h status-interna
 000000c0: 6c0a e900 0000 004e 2903 da07 6469 726e  l......N)...dirn
 000000d0: 616d 65da 046a 6f69 6eda 086e 6f72 6d70  ame..join..normp
 000000e0: 6174 68da 0063 0100 0000 0000 0000 0000  ath..c..........
-000000f0: 0000 0700 0000 0800 0000 4300 0000 7300  ..........C...s.
+000000f0: 0000 0700 0000 0800 0000 4300 0000 7308  ..........C...s.
 00000100: 0100 0074 00a0 0174 02a1 016a 03a0 04a1  ...t...t...j....
 00000110: 007d 0174 0574 067c 0164 0183 0283 017d  .}.t.t.|.d.....}
 00000120: 0274 0774 0574 067c 0164 0283 0283 0183  .t.t.t.|.d......
 00000130: 017d 0374 0774 0574 067c 0164 0383 0283  .}.t.t.t.|.d....
 00000140: 0183 017d 0474 086a 087c 0064 0464 058d  ...}.t.j.|.d.d..
-00000150: 027d 0574 096a 0a7c 0564 068d 0101 0074  .}.t.j.|.d.....t
-00000160: 0b6a 0c7c 0564 0774 0574 067c 0264 0883  .j.|.d.t.t.|.d..
-00000170: 0283 0174 0574 067c 0264 0983 0283 0167  ...t.t.|.d.....g
-00000180: 027c 037c 0464 0a8d 057d 0674 096a 0a64  .|.|.d...}.t.j.d
-00000190: 0b7c 0664 0c19 0069 0164 068d 0101 007c  .|.d...i.d.....|
-000001a0: 0664 0c19 0064 0d19 0064 0e6b 0273 5c4a  .d...d...d.k.s\J
-000001b0: 007c 0664 0c19 0083 0182 017c 0664 0c19  .|.d.......|.d..
-000001c0: 0064 0f19 0064 0e6b 0273 6a4a 007c 0664  .d...d.k.sjJ.|.d
-000001d0: 0c19 0083 0182 017c 0664 0c19 0064 1019  .......|.d...d..
-000001e0: 0064 0d19 0064 0e6b 0273 7a4a 007c 0664  .d...d.k.szJ.|.d
-000001f0: 0c19 0083 0182 0174 0d64 1183 0101 007c  .......t.d.....|
-00000200: 0653 0029 124e 7a08 2e2e 2f2e 2e2f 2e2e  .S.).Nz.../../..
-00000210: 7a02 2e2e da02 4442 5429 01da 0972 6563  z.....DBT)...rec
-00000220: 7572 7369 7665 2901 da04 6461 7461 46da  ursive)...dataF.
-00000230: 0673 7461 6765 73da 0a73 7461 6765 735f  .stages..stages_
-00000240: 7069 7029 05da 0570 6174 6873 da0c 7369  pip)...paths..si
-00000250: 6d75 6c74 616e 656f 7573 da0c 6d6f 6475  multaneous..modu
-00000260: 6c65 5f70 6174 6873 da0d 7265 6c61 7469  le_paths..relati
-00000270: 7665 5f70 6174 68da 0c64 625f 6469 7265  ve_path..db_dire
-00000280: 6374 6f72 797a 0e62 6f64 7920 7363 616e  ctoryz.body scan
-00000290: 2064 6f6e 65da 0573 7461 7473 da06 616c   done..stats..al
-000002a0: 6172 6d73 7201 0000 00da 0565 6d70 7479  armsr......empty
-000002b0: da06 6368 6563 6b73 7a0f 626f 6479 2073  ..checksz.body s
-000002c0: 6361 6e20 646f 6e65 3f29 0eda 0770 6174  can done?)...pat
-000002d0: 686c 6962 da04 5061 7468 da08 5f5f 6669  hlib..Path..__fi
-000002e0: 6c65 5f5f da06 7061 7265 6e74 da07 7265  le__..parent..re
-000002f0: 736f 6c76 6572 0400 0000 7203 0000 00da  solver....r.....
-00000300: 0373 7472 da04 676c 6f62 da04 7269 6368  .str..glob..rich
-00000310: da0a 7072 696e 745f 6a73 6f6e da09 626f  ..print_json..bo
-00000320: 6479 5f73 6361 6eda 0573 7461 7274 da05  dy_scan..start..
-00000330: 7072 696e 7429 07da 0b67 6c6f 625f 7374  print)...glob_st
-00000340: 7269 6e67 da0b 7468 6973 5f66 6f6c 6465  ring..this_folde
-00000350: 72da 0a73 7472 7563 7475 7265 73da 0974  r..structures..t
-00000360: 6865 5f73 7461 6765 7206 0000 00da 0c73  he_stager......s
-00000370: 7461 7475 735f 7061 7468 73da 0473 6361  tatus_paths..sca
-00000380: 6ea9 0072 2600 0000 fa33 2f62 696f 7465  n..r&....3/biote
-00000390: 6368 2f76 656e 7565 732f 7374 6167 6573  ch/venues/stages
-000003a0: 2f62 696f 7465 6368 2f5f 7374 6174 7573  /biotech/_status
-000003b0: 2f65 7374 6162 6c69 7368 2e70 7972 1e00  /establish.pyr..
-000003c0: 0000 1b00 0000 7332 0000 0010 040e 0212  ......s2........
-000003d0: 0112 010e 0504 0702 0106 ff04 0402 0102  ................
-000003e0: 020c 030c 0102 fe02 0502 0206 f404 0f08  ................
-000003f0: 0108 ff1c 041c 0120 0108 0204 0372 1e00  ....... .....r..
-00000400: 0000 2901 7205 0000 0029 0bda 075f 5f64  ..).r....)...__d
-00000410: 6f63 5f5f 721a 0000 0072 1400 0000 da07  oc__r....r......
-00000420: 6f73 2e70 6174 6872 0200 0000 7203 0000  os.pathr....r...
-00000430: 0072 0400 0000 da02 6f73 721b 0000 0072  .r......osr....r
-00000440: 1d00 0000 721e 0000 0072 2600 0000 7226  ....r....r&...r&
-00000450: 0000 0072 2600 0000 7227 0000 00da 083c  ...r&...r'.....<
-00000460: 6d6f 6475 6c65 3e01 0000 0073 1400 0000  module>....s....
-00000470: 0402 0206 0807 0801 1401 0801 0802 0802  ................
-00000480: 0205 0eff                                ....
+00000150: 027d 057c 05a0 09a1 0001 0074 0a6a 0b7c  .}.|.......t.j.|
+00000160: 0564 068d 0101 0074 0c6a 0d7c 0564 0774  .d.....t.j.|.d.t
+00000170: 0574 067c 0264 0883 0283 0174 0574 067c  .t.|.d.....t.t.|
+00000180: 0264 0983 0283 0167 027c 037c 0464 0a8d  .d.....g.|.|.d..
+00000190: 057d 0674 0a6a 0b64 0b7c 0664 0c19 0069  .}.t.j.d.|.d...i
+000001a0: 0164 068d 0101 007c 0664 0c19 0064 0d19  .d.....|.d...d..
+000001b0: 0064 0e6b 0273 604a 007c 0664 0c19 0083  .d.k.s`J.|.d....
+000001c0: 0182 017c 0664 0c19 0064 0f19 0064 0e6b  ...|.d...d...d.k
+000001d0: 0273 6e4a 007c 0664 0c19 0083 0182 017c  .snJ.|.d.......|
+000001e0: 0664 0c19 0064 1019 0064 0d19 0064 0e6b  .d...d...d...d.k
+000001f0: 0273 7e4a 007c 0664 0c19 0083 0182 0174  .s~J.|.d.......t
+00000200: 0e64 1183 0101 007c 0653 0029 124e 7a08  .d.....|.S.).Nz.
+00000210: 2e2e 2f2e 2e2f 2e2e 7a02 2e2e da02 4442  ../../..z.....DB
+00000220: 5429 01da 0972 6563 7572 7369 7665 2901  T)...recursive).
+00000230: da04 6461 7461 46da 0673 7461 6765 73da  ..dataF..stages.
+00000240: 0a73 7461 6765 735f 7069 7029 05da 0570  .stages_pip)...p
+00000250: 6174 6873 da0c 7369 6d75 6c74 616e 656f  aths..simultaneo
+00000260: 7573 da0c 6d6f 6475 6c65 5f70 6174 6873  us..module_paths
+00000270: da0d 7265 6c61 7469 7665 5f70 6174 68da  ..relative_path.
+00000280: 0c64 625f 6469 7265 6374 6f72 797a 0e62  .db_directoryz.b
+00000290: 6f64 7920 7363 616e 2064 6f6e 65da 0573  ody scan done..s
+000002a0: 7461 7473 da06 616c 6172 6d73 7201 0000  tats..alarmsr...
+000002b0: 00da 0565 6d70 7479 da06 6368 6563 6b73  ...empty..checks
+000002c0: 7a0f 626f 6479 2073 6361 6e20 646f 6e65  z.body scan done
+000002d0: 3f29 0fda 0770 6174 686c 6962 da04 5061  ?)...pathlib..Pa
+000002e0: 7468 da08 5f5f 6669 6c65 5f5f da06 7061  th..__file__..pa
+000002f0: 7265 6e74 da07 7265 736f 6c76 6572 0400  rent..resolver..
+00000300: 0000 7203 0000 00da 0373 7472 da04 676c  ..r......str..gl
+00000310: 6f62 da04 736f 7274 da04 7269 6368 da0a  ob..sort..rich..
+00000320: 7072 696e 745f 6a73 6f6e da09 626f 6479  print_json..body
+00000330: 5f73 6361 6eda 0573 7461 7274 da05 7072  _scan..start..pr
+00000340: 696e 7429 07da 0b67 6c6f 625f 7374 7269  int)...glob_stri
+00000350: 6e67 da0b 7468 6973 5f66 6f6c 6465 72da  ng..this_folder.
+00000360: 0a73 7472 7563 7475 7265 73da 0974 6865  .structures..the
+00000370: 5f73 7461 6765 7206 0000 00da 0c73 7461  _stager......sta
+00000380: 7475 735f 7061 7468 73da 0473 6361 6ea9  tus_paths..scan.
+00000390: 0072 2700 0000 fa33 2f62 696f 7465 6368  .r'....3/biotech
+000003a0: 2f76 656e 7565 732f 7374 6167 6573 2f62  /venues/stages/b
+000003b0: 696f 7465 6368 2f5f 7374 6174 7573 2f65  iotech/_status/e
+000003c0: 7374 6162 6c69 7368 2e70 7972 1f00 0000  stablish.pyr....
+000003d0: 1b00 0000 7334 0000 0010 040e 0212 0112  ....s4..........
+000003e0: 010e 0508 0604 0102 0106 ff04 0602 0102  ................
+000003f0: 020c 030c 0102 fe02 0502 0206 f404 0f08  ................
+00000400: 0108 ff1c 041c 0120 0108 0204 0372 1f00  ....... .....r..
+00000410: 0000 2901 7205 0000 0029 0bda 075f 5f64  ..).r....)...__d
+00000420: 6f63 5f5f 721a 0000 0072 1400 0000 da07  oc__r....r......
+00000430: 6f73 2e70 6174 6872 0200 0000 7203 0000  os.pathr....r...
+00000440: 0072 0400 0000 da02 6f73 721c 0000 0072  .r......osr....r
+00000450: 1e00 0000 721f 0000 0072 2700 0000 7227  ....r....r'...r'
+00000460: 0000 0072 2700 0000 7228 0000 00da 083c  ...r'...r(.....<
+00000470: 6d6f 6475 6c65 3e01 0000 0073 1400 0000  module>....s....
+00000480: 0402 0206 0807 0801 1401 0801 0802 0802  ................
+00000490: 0205 0eff                                ....
```

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/establish.py` & `biotech-1.1.2/venues/stages/biotech/_status/establish.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,18 +39,20 @@
 	
 	status_paths = glob.glob (glob_string, recursive = True)
 
 	
 	# path = str (normpath (join (the_stage, "procedures/health_scan/process/modules_pip/requests/status_codes.py")))
 	# status_paths.pop (status_paths.index (path))
 	
-
+	status_paths.sort ()
 	rich.print_json (
 		data = status_paths
 	)
+	
+
 
 	scan = body_scan.start (
 		paths = status_paths,
 		
 		simultaneous = False,
 		
 		module_paths = [
```

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/-1_start/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/-01_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/0_start/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/00_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/1/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/01/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	
 	this_directory = pathlib.Path (__file__).parent.resolve ()
 	this_module = str (this_directory)
 	the_guarantees = str (normpath (join (this_directory, f"guarantees")))
 	
 
 	
-	scan = biotech.on ({
+	bio = biotech.on ({
 		"glob_string": this_module + "/**/guarantee_*.py",
 		
 		"time_limit": 5,
 		
 		"simultaneous": True,
 		"simultaneous_capacity": 10,
 
@@ -32,14 +32,17 @@
 		],
 
 		"relative_path": this_module,
 		
 		"aggregation_format": 2
 	})
 	
+	bio ["off"] ()
+	scan = bio ["proceeds"]
+	
 	assert (scan ["paths"] [0] ["alarm"] == "time limit exceeded"), scan ["paths"]
 
 	assert (scan ["stats"] ["paths"] ["alarms"] == 1), scan ["stats"]
 	assert (scan ["stats"] ["paths"] ["empty"] == 0), scan ["stats"]
 
 	assert (scan ["stats"] ["checks"] ["passes"] == 0), scan ["stats"]
 	assert (scan ["stats"] ["checks"] ["alarms"] == 0), scan ["stats"]
```

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/11/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 
 '''
 	python3 /biotech/venues/stages/biotech/_status/status.proc.py "_status/monitors/9_aggregation_format_and_exit/status_1.py"
+	python3 /biotech/venues/stages/biotech/_status/status.proc.py "9_aggregation_format_and_exit/status_1.py"
+	
 '''
 
 '''
 	netstat -tuln | grep 52435
 '''
 
 import pathlib
@@ -17,39 +19,45 @@
 def check_1 ():
 	this_directory = pathlib.Path (__file__).parent.resolve ()
 	this_module = str (this_directory)
 	the_guarantees = str (normpath (join (this_directory, f"guarantees")))
 	
 	relative_path = str (normpath (join (this_directory, f"..")))
 	
-	scan = biotech.on ({
+	bio = biotech.on ({
 		"glob_string": this_module + "/**/guarantee_*.py",
 		
 		"simultaneous": True,
-		"simultaneous_capacity": 10,
+		"simultaneous_capacity": 1,
 
 		"module_paths": [
 			normpath (join (this_module, "modules")),
 			normpath (join (this_module, "modules_pip"))
 		],
 
 		"relative_path": relative_path,
 		
 		"aggregation_format": 2
 	})
 
+	bio ["off"] ()
+	scan = bio ["proceeds"]
 
 	#time.sleep (5)
 
-
+	print ("in check after scan")
+	
+	rich.print_json (data = {
+		"scan results": scan
+	})
 	
 	#time.sleep (5)
 
-	assert (scan ["stats"] ["paths"] ["alarms"] == 0), scan ["stats"]
+	assert (scan ["stats"] ["paths"] ["alarms"] == 2), scan ["stats"]
 	assert (scan ["stats"] ["paths"] ["empty"] == 0), scan ["stats"]
 
 	assert (scan ["stats"] ["checks"] ["passes"] == 1), scan ["stats"]
-	assert (scan ["stats"] ["checks"] ["alarms"] == 0), scan ["stats"]
+	assert (scan ["stats"] ["checks"] ["alarms"] == 1), scan ["stats"]
 	
 checks = {
 	'aggregation format and exit': check_1
 }
```

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/2/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/02/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/3_empty_glob/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/4.1_bad_import/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/4_bad_import/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/1_health.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/5__file__/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/05__file__/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/6_various/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/06_various/status_1.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 	stasis = normpath (join (this_directory, "stasis"))
 
 	
 	scan = biotech.start (
 		glob_string = stasis + '/**/*_health.py',
 		
 		simultaneous = True,
+		simultaneous_capacity = 1,
 		
 		relative_path = stasis,
 		module_paths = []
 	)
 	status = scan ['status']
 	paths = status ["paths"]
```

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/7/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/07/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/8_DB/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/08_DB/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/8_DB/variable/status_db/records.json` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9827586206896552%*

 * *Differences: {"'_default'": "{'225': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [2.07029988814611e-05, 'seconds']), ('passed', True)])]), "*

 * *               "('empty', False), ('parsed', True), ('path', 'guarantee_1.py'), ('records', "*

 * *               "['proceeds None\\r\\n', 'checks in module True\\r\\n', 'check 1\\r\\n', '{\\r\\n', "*

 * *               '\'  "variable": {\\r\\n\', \'    "pid": 9094,\\r\\n\', \'    "proceeds": '*

 * *               '{\\r\\n\', \ […]*

```diff
@@ -4914,14 +4914,344 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 1
                 },
                 "empty": 0
             }
         },
+        "225": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.07029988814611e-05,
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
+                        "    \"pid\": 9094,\r\n",
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
+                        "            2.07029988814611e-05,\r\n",
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
+                        "  \"line\": 80\r\n",
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
+        "226": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.9443999665090814e-05,
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
+                        "    \"pid\": 9337,\r\n",
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
+                        "            2.9443999665090814e-05,\r\n",
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
+                        "  \"line\": 80\r\n",
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
+        "227": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.3190004867501557e-06,
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
+                        "    \"pid\": 9988,\r\n",
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
+                        "            2.3190004867501557e-06,\r\n",
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
+                        "  \"line\": 80\r\n",
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
+        "228": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.9529001039918512e-05,
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
+                        "    \"pid\": 10727,\r\n",
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
+                        "            2.9529001039918512e-05,\r\n",
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
+                        "  \"line\": 80\r\n",
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
+        "229": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.0141000024741516e-05,
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
+                        "    \"pid\": 11148,\r\n",
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
+                        "            3.0141000024741516e-05,\r\n",
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
         "23": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
@@ -4938,14 +5268,207 @@
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
+        "230": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.283899812027812e-05,
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
+                        "    \"pid\": 12072,\r\n",
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
+                        "            2.283899812027812e-05,\r\n",
+                        "            \"seconds\"\r\n",
+                        "          ]\r\n",
+                        "        }\r\n",
+                        "      ]\r\n",
+                        "    },\r\n",
+                        "    \"harbor\": {\r\n",
+                        "      \"host\": \"0.0.0.0\",\r\n",
+                        "      \"port\": 52435\r\n"
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
+        "231": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.310996933374554e-06,
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
+                        "    \"pid\": 12494,\r\n",
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
+                        "            2.310996933374554e-06,\r\n",
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
+        "232": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.5214001905405894e-05,
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
+                        "    \"pid\": 12950,\r\n",
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
+                        "            1.5214001905405894e-05,\r\n",
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
                 "alarms": 0,
                 "checks": {
                     "alarms": 0,
                     "passes": 1
                 },
                 "empty": 0
             }
```

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status/monitors/11/status_1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 
 '''
 	python3 /biotech/venues/stages/biotech/_status/status.proc.py "_status/monitors/9_aggregation_format_and_exit/status_1.py"
-	python3 /biotech/venues/stages/biotech/_status/status.proc.py "9_aggregation_format_and_exit/status_1.py"
-	
 '''
 
 '''
 	netstat -tuln | grep 52435
 '''
 
 import pathlib
@@ -19,42 +17,42 @@
 def check_1 ():
 	this_directory = pathlib.Path (__file__).parent.resolve ()
 	this_module = str (this_directory)
 	the_guarantees = str (normpath (join (this_directory, f"guarantees")))
 	
 	relative_path = str (normpath (join (this_directory, f"..")))
 	
-	scan = biotech.on ({
+	bio = biotech.on ({
 		"glob_string": this_module + "/**/guarantee_*.py",
 		
 		"simultaneous": True,
 		"simultaneous_capacity": 10,
 
 		"module_paths": [
 			normpath (join (this_module, "modules")),
 			normpath (join (this_module, "modules_pip"))
 		],
 
 		"relative_path": relative_path,
 		
 		"aggregation_format": 2
 	})
+	
+	bio ["off"] ()
+	scan = bio ["proceeds"]
+
 
 	#time.sleep (5)
 
-	print ("in check after scan")
-	
-	rich.print_json (data = {
-		"scan results": scan
-	})
+
 	
 	#time.sleep (5)
 
-	assert (scan ["stats"] ["paths"] ["alarms"] == 2), scan ["stats"]
+	assert (scan ["stats"] ["paths"] ["alarms"] == 0), scan ["stats"]
 	assert (scan ["stats"] ["paths"] ["empty"] == 0), scan ["stats"]
 
 	assert (scan ["stats"] ["checks"] ["passes"] == 1), scan ["stats"]
-	assert (scan ["stats"] ["checks"] ["alarms"] == 1), scan ["stats"]
+	assert (scan ["stats"] ["checks"] ["alarms"] == 0), scan ["stats"]
 	
 checks = {
 	'aggregation format and exit': check_1
 }
```

### Comparing `biotech-1.1.1/venues/stages/biotech/_status/status.proc.py` & `biotech-1.1.2/venues/stages/biotech/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py` & `biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json` & `biotech-1.1.2/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/_status_advanced/status.proc.py` & `biotech-1.1.2/venues/stages/biotech/_status_advanced/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/architecture.s.HTML` & `biotech-1.1.2/venues/stages/biotech/architecture.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/module.s.HTML` & `biotech-1.1.2/venues/stages/biotech/module.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/on.py` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/on.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 #
 #----
 
 def aggregator_procedure_on (
 	port,
 	packet
 ):
-	show_variable ("""aggregator_procedure_on""")
+	show_variable ("""aggregator_procedure_on""", mode = "condensed")
 
 	limit_start = 25000
 		
 	path_of_the_scan_process = find_aggregator_procedure_paths ()
 	process_string = (
 		f'''python3 { path_of_the_scan_process } keg open --port { port }'''
 	)
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,21 +50,34 @@
 	paths_patch (app, aggregator_procedure_port = port)
 
 	@app.route ("/", methods = [ 'GET' ])
 	def home_get ():	
 		return jsonify ({
 			'/health_scan/<path:health_scan_path>': [ "get" ],
 			'/health_scans/paths': [ "get" ],
-			'/on': [ "get" ]
+			'/on': [ "get" ],
+			'/anomalies': [ "get" ]
 		})
 
 
 	@app.route ("/on", methods = [ 'GET' ])
 	def on_get ():	
 		return "yes"
+		
+	@app.route ("/anomalies", methods = [ 'GET' ])
+	def on_anomalies ():	
+		try:
+			aggregator_variables = retrieve_aggregator_variables ()
+			
+			return jsonify (aggregator_variables ["anomalies"])
+			
+		except Exception:
+			pass;
+			
+		return "not parseable"
 
 		
 	@app.route ('/health_scans/paths', methods = [ 'GET' ])
 	def on__get__health_scans__paths ():	
 		aggregator_variables = retrieve_aggregator_variables ()
 		
 		the_paths = {}
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 16:26:14 2024 UTC, .py size: 1734 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 269b 2266 c606 0000  o.......&."f....
+00000000: 6f0d 0d0a 0000 0000 04da 2266 e707 0000  o........."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6405 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 6407 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6405 6408 6c0d 5a0d 6405  m.Z...d.d.l.Z.d.
@@ -24,113 +24,130 @@
 00000170: 616c 7468 5f73 6361 6e5f 7374 6172 7465  alth_scan_starte
 00000180: 64e9 0000 0000 2901 da1d 7265 7472 6965  d.....)...retrie
 00000190: 7665 5f61 6767 7265 6761 746f 725f 7661  ve_aggregator_va
 000001a0: 7269 6162 6c65 7329 03da 0546 6c61 736b  riables)...Flask
 000001b0: da07 7265 7175 6573 74da 076a 736f 6e69  ..request..jsoni
 000001c0: 6679 4e29 03da 0764 6972 6e61 6d65 da04  fyN)...dirname..
 000001d0: 6a6f 696e da08 6e6f 726d 7061 7468 6302  join..normpathc.
-000001e0: 0000 0000 0000 0000 0000 0007 0000 0005  ................
-000001f0: 0000 0043 0000 0073 ac00 0000 7c01 6401  ...C...s....|.d.
+000001e0: 0000 0000 0000 0000 0000 0008 0000 0005  ................
+000001f0: 0000 0043 0000 0073 c400 0000 7c01 6401  ...C...s....|.d.
 00000200: 6b05 7209 7400 6402 7c00 8302 0100 7401  k.r.t.d.|.....t.
 00000210: 6403 8301 7d02 0900 7402 7c02 7c00 6404  d...}...t.|.|.d.
 00000220: 8d02 0100 7c02 6a03 6405 6406 6701 6407  ....|.j.d.d.g.d.
 00000230: 8d02 6408 6409 8400 8301 7d03 7c02 6a03  ..d.d.....}.|.j.
 00000240: 640a 6406 6701 6407 8d02 640b 640c 8400  d.d.g.d...d.d...
 00000250: 8301 7d04 7c02 6a03 640d 6406 6701 6407  ..}.|.j.d.d.g.d.
 00000260: 8d02 640e 640f 8400 8301 7d05 7c02 6a03  ..d.d.....}.|.j.
 00000270: 6410 6406 6701 6407 8d02 6411 6412 8400  d.d.g.d...d.d...
-00000280: 8301 7d06 7404 7c02 8301 0100 7405 7c02  ..}.t.|.....t.|.
-00000290: 8301 0100 7c02 6a06 6413 7c00 6414 6415  ....|.j.d.|.d.d.
-000002a0: 8d03 0100 6400 5300 2916 4e72 0100 0000  ....d.S.).Nr....
-000002b0: 7a21 6f70 656e 696e 6720 7363 616e 2070  z!opening scan p
-000002c0: 726f 6365 7373 206b 6567 206f 6e20 706f  rocess keg on po
-000002d0: 7274 3a7a 1161 6767 7265 6761 746f 7220  rt:z.aggregator 
-000002e0: 6861 7262 6f72 2901 da19 6167 6772 6567  harbor)...aggreg
-000002f0: 6174 6f72 5f70 726f 6365 6475 7265 5f70  ator_procedure_p
-00000300: 6f72 74fa 012f da03 4745 5429 01da 076d  ort../..GET)...m
-00000310: 6574 686f 6473 6300 0000 0000 0000 0000  ethodsc.........
-00000320: 0000 0000 0000 0005 0000 0053 0000 0073  ...........S...s
-00000330: 1600 0000 7400 6401 6701 6401 6701 6401  ....t.d.g.d.g.d.
-00000340: 6701 6402 9c03 8301 5300 2903 4eda 0367  g.d.....S.).N..g
-00000350: 6574 2903 fa24 2f68 6561 6c74 685f 7363  et)..$/health_sc
-00000360: 616e 2f3c 7061 7468 3a68 6561 6c74 685f  an/<path:health_
-00000370: 7363 616e 5f70 6174 683e fa13 2f68 6561  scan_path>../hea
-00000380: 6c74 685f 7363 616e 732f 7061 7468 73fa  lth_scans/paths.
-00000390: 032f 6f6e 2901 7209 0000 00a9 0072 1500  ./on).r......r..
-000003a0: 0000 7215 0000 00fa 562f 6269 6f74 6563  ..r.....V/biotec
-000003b0: 682f 7665 6e75 6573 2f73 7461 6765 732f  h/venues/stages/
-000003c0: 6269 6f74 6563 682f 7072 6f63 6564 7572  biotech/procedur
-000003d0: 6573 2f61 6767 7265 6761 746f 725f 7072  es/aggregator_pr
-000003e0: 6f63 6564 7572 652f 7072 6f63 6573 732f  ocedure/process/
-000003f0: 6b65 672f 5f5f 696e 6974 5f5f 2e70 79da  keg/__init__.py.
-00000400: 0868 6f6d 655f 6765 7434 0000 0073 0a00  .home_get4...s..
-00000410: 0000 0202 0401 0401 0401 08fd 7a1d 6f70  ............z.op
-00000420: 656e 5f68 6172 626f 722e 3c6c 6f63 616c  en_harbor.<local
-00000430: 733e 2e68 6f6d 655f 6765 7472 1400 0000  s>.home_getr....
-00000440: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000450: 0001 0000 0053 0000 00f3 0400 0000 6401  .....S........d.
-00000460: 5300 a902 4eda 0379 6573 7215 0000 0072  S...N..yesr....r
-00000470: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-00000480: 0000 00da 066f 6e5f 6765 743d 0000 00f3  .....on_get=....
-00000490: 0200 0000 0402 7a1b 6f70 656e 5f68 6172  ......z.open_har
-000004a0: 626f 722e 3c6c 6f63 616c 733e 2e6f 6e5f  bor.<locals>.on_
-000004b0: 6765 7472 1300 0000 6300 0000 0000 0000  getr....c.......
-000004c0: 0000 0000 0003 0000 0004 0000 0053 0000  .............S..
-000004d0: 0073 2800 0000 7400 8300 7d00 6900 7d01  .s(...t...}.i.}.
-000004e0: 7c00 6401 1900 4400 5d06 7d02 6402 7c01  |.d...D.].}.d.|.
-000004f0: 7c02 3c00 7109 7401 7c01 8301 5300 2903  |.<.q.t.|...S.).
-00000500: 4eda 1169 6e74 6572 6e61 6c5f 7374 6174  N..internal_stat
-00000510: 7573 6573 da00 2902 7206 0000 0072 0900  uses..).r....r..
-00000520: 0000 2903 da14 6167 6772 6567 6174 6f72  ..)...aggregator
-00000530: 5f76 6172 6961 626c 6573 da09 7468 655f  _variables..the_
-00000540: 7061 7468 73da 0470 6174 6872 1500 0000  paths..pathr....
-00000550: 7215 0000 0072 1600 0000 da1c 6f6e 5f5f  r....r......on__
-00000560: 6765 745f 5f68 6561 6c74 685f 7363 616e  get__health_scan
-00000570: 735f 5f70 6174 6873 4200 0000 730a 0000  s__pathsB...s...
-00000580: 0006 0204 020c 020a 0108 027a 316f 7065  ...........z1ope
-00000590: 6e5f 6861 7262 6f72 2e3c 6c6f 6361 6c73  n_harbor.<locals
-000005a0: 3e2e 6f6e 5f5f 6765 745f 5f68 6561 6c74  >.on__get__healt
-000005b0: 685f 7363 616e 735f 5f70 6174 6873 7212  h_scans__pathsr.
-000005c0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000005d0: 0100 0000 0100 0000 5300 0000 7218 0000  ........S...r...
-000005e0: 0072 1900 0000 7215 0000 0029 01da 1068  .r....r....)...h
-000005f0: 6561 6c74 685f 7363 616e 5f70 6174 6872  ealth_scan_pathr
-00000600: 1500 0000 7215 0000 0072 1600 0000 da1a  ....r....r......
-00000610: 6f6e 5f5f 6765 745f 5f68 6561 6c74 685f  on__get__health_
-00000620: 7363 616e 5f5f 7061 7468 4d00 0000 721c  scan__pathM...r.
-00000630: 0000 007a 2f6f 7065 6e5f 6861 7262 6f72  ...z/open_harbor
-00000640: 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f5f 6765  .<locals>.on__ge
-00000650: 745f 5f68 6561 6c74 685f 7363 616e 5f5f  t__health_scan__
-00000660: 7061 7468 7a07 302e 302e 302e 3046 2902  pathz.0.0.0.0F).
-00000670: da04 706f 7274 da05 6465 6275 6729 07da  ..port..debug)..
-00000680: 0570 7269 6e74 7207 0000 0072 0300 0000  .printr....r....
-00000690: da05 726f 7574 6572 0400 0000 7202 0000  ..router....r...
-000006a0: 00da 0372 756e 2907 7225 0000 00da 0772  ...run).r%.....r
-000006b0: 6563 6f72 6473 da03 6170 7072 1700 0000  ecords..appr....
-000006c0: 721b 0000 0072 2200 0000 7224 0000 0072  r....r"...r$...r
-000006d0: 1500 0000 7215 0000 0072 1600 0000 da0b  ....r....r......
-000006e0: 6f70 656e 5f68 6172 626f 7224 0000 0073  open_harbor$...s
-000006f0: 2800 0000 0804 0a01 0804 0202 0c03 0e02  (...............
-00000700: 0a01 0e08 0a01 0e04 0a01 0e0a 0a01 0804  ................
-00000710: 0802 0404 0201 0201 0201 0afd 722c 0000  ............r,..
-00000720: 0029 0272 0500 0000 7205 0000 0029 19da  .).r....r....)..
-00000730: 075f 5f64 6f63 5f5f da15 7370 6163 6573  .__doc__..spaces
-00000740: 2e64 6f6e 655f 7769 7468 5f73 6361 6e72  .done_with_scanr
-00000750: 0200 0000 da12 7370 6163 6573 2e70 6174  ......spaces.pat
-00000760: 6873 5f70 6174 6368 7203 0000 00da 1e73  hs_patchr......s
-00000770: 7061 6365 732e 7468 655f 6865 616c 7468  paces.the_health
-00000780: 5f73 6361 6e5f 7374 6172 7465 6472 0400  _scan_startedr..
-00000790: 0000 da39 6269 6f74 6563 682e 7072 6f63  ...9biotech.proc
-000007a0: 6564 7572 6573 2e61 6767 7265 6761 746f  edures.aggregato
-000007b0: 725f 7072 6f63 6564 7572 652e 7072 6f63  r_procedure.proc
-000007c0: 6573 732e 7661 7269 6162 6c65 7372 0600  ess.variablesr..
-000007d0: 0000 da05 666c 6173 6b72 0700 0000 7208  ....flaskr....r.
-000007e0: 0000 0072 0900 0000 da04 7269 6368 da04  ...r......rich..
-000007f0: 6a73 6f6e da07 7061 7468 6c69 62da 026f  json..pathlib..o
-00000800: 73da 076f 732e 7061 7468 720a 0000 0072  s..os.pathr....r
-00000810: 0b00 0000 720c 0000 00da 0373 7973 da09  ....r......sys..
-00000820: 7468 7265 6164 696e 67da 0474 696d 6572  threading..timer
-00000830: 2c00 0000 7215 0000 0072 1500 0000 7215  ,...r....r....r.
-00000840: 0000 0072 1600 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000850: 653e 0100 0000 7322 0000 0004 020c 0c0c  e>....s"........
-00000860: 010c 010c 0214 0308 0108 0308 0108 0114  ................
-00000870: 0108 0108 0108 0102 0502 010e fe         .............
+00000280: 8301 7d06 7c02 6a03 6413 6406 6701 6407  ..}.|.j.d.d.g.d.
+00000290: 8d02 6414 6415 8400 8301 7d07 7404 7c02  ..d.d.....}.t.|.
+000002a0: 8301 0100 7405 7c02 8301 0100 7c02 6a06  ....t.|.....|.j.
+000002b0: 6416 7c00 6417 6418 8d03 0100 6400 5300  d.|.d.d.....d.S.
+000002c0: 2919 4e72 0100 0000 7a21 6f70 656e 696e  ).Nr....z!openin
+000002d0: 6720 7363 616e 2070 726f 6365 7373 206b  g scan process k
+000002e0: 6567 206f 6e20 706f 7274 3a7a 1161 6767  eg on port:z.agg
+000002f0: 7265 6761 746f 7220 6861 7262 6f72 2901  regator harbor).
+00000300: da19 6167 6772 6567 6174 6f72 5f70 726f  ..aggregator_pro
+00000310: 6365 6475 7265 5f70 6f72 74fa 012f da03  cedure_port../..
+00000320: 4745 5429 01da 076d 6574 686f 6473 6300  GET)...methodsc.
+00000330: 0000 0000 0000 0000 0000 0000 0000 0006  ................
+00000340: 0000 0053 0000 0073 1a00 0000 7400 6401  ...S...s....t.d.
+00000350: 6701 6401 6701 6401 6701 6401 6701 6402  g.d.g.d.g.d.g.d.
+00000360: 9c04 8301 5300 2903 4eda 0367 6574 2904  ....S.).N..get).
+00000370: fa24 2f68 6561 6c74 685f 7363 616e 2f3c  .$/health_scan/<
+00000380: 7061 7468 3a68 6561 6c74 685f 7363 616e  path:health_scan
+00000390: 5f70 6174 683e fa13 2f68 6561 6c74 685f  _path>../health_
+000003a0: 7363 616e 732f 7061 7468 73fa 032f 6f6e  scans/paths../on
+000003b0: fa0a 2f61 6e6f 6d61 6c69 6573 2901 7209  ../anomalies).r.
+000003c0: 0000 00a9 0072 1600 0000 7216 0000 00fa  .....r....r.....
+000003d0: 562f 6269 6f74 6563 682f 7665 6e75 6573  V/biotech/venues
+000003e0: 2f73 7461 6765 732f 6269 6f74 6563 682f  /stages/biotech/
+000003f0: 7072 6f63 6564 7572 6573 2f61 6767 7265  procedures/aggre
+00000400: 6761 746f 725f 7072 6f63 6564 7572 652f  gator_procedure/
+00000410: 7072 6f63 6573 732f 6b65 672f 5f5f 696e  process/keg/__in
+00000420: 6974 5f5f 2e70 79da 0868 6f6d 655f 6765  it__.py..home_ge
+00000430: 7434 0000 0073 0c00 0000 0202 0401 0401  t4...s..........
+00000440: 0401 0401 08fc 7a1d 6f70 656e 5f68 6172  ......z.open_har
+00000450: 626f 722e 3c6c 6f63 616c 733e 2e68 6f6d  bor.<locals>.hom
+00000460: 655f 6765 7472 1400 0000 6300 0000 0000  e_getr....c.....
+00000470: 0000 0000 0000 0000 0000 0001 0000 0053  ...............S
+00000480: 0000 00f3 0400 0000 6401 5300 a902 4eda  ........d.S...N.
+00000490: 0379 6573 7216 0000 0072 1600 0000 7216  .yesr....r....r.
+000004a0: 0000 0072 1600 0000 7217 0000 00da 066f  ...r....r......o
+000004b0: 6e5f 6765 743e 0000 00f3 0200 0000 0402  n_get>..........
+000004c0: 7a1b 6f70 656e 5f68 6172 626f 722e 3c6c  z.open_harbor.<l
+000004d0: 6f63 616c 733e 2e6f 6e5f 6765 7472 1500  ocals>.on_getr..
+000004e0: 0000 6300 0000 0000 0000 0000 0000 0001  ..c.............
+000004f0: 0000 0008 0000 0053 0000 0073 2a00 0000  .......S...s*...
+00000500: 7a0a 7400 8300 7d00 7401 7c00 6401 1900  z.t...}.t.|.d...
+00000510: 8301 5700 5300 0400 7402 7914 0100 0100  ..W.S...t.y.....
+00000520: 0100 5900 6402 5300 7700 2903 4eda 0961  ..Y.d.S.w.).N..a
+00000530: 6e6f 6d61 6c69 6573 7a0d 6e6f 7420 7061  nomaliesz.not pa
+00000540: 7273 6561 626c 6529 0372 0600 0000 7209  rseable).r....r.
+00000550: 0000 00da 0945 7863 6570 7469 6f6e 2901  .....Exception).
+00000560: da14 6167 6772 6567 6174 6f72 5f76 6172  ..aggregator_var
+00000570: 6961 626c 6573 7216 0000 0072 1600 0000  iablesr....r....
+00000580: 7217 0000 00da 0c6f 6e5f 616e 6f6d 616c  r......on_anomal
+00000590: 6965 7342 0000 0073 0e00 0000 0202 0601  iesB...s........
+000005a0: 0e02 0c02 0201 0402 02fd 7a21 6f70 656e  ..........z!open
+000005b0: 5f68 6172 626f 722e 3c6c 6f63 616c 733e  _harbor.<locals>
+000005c0: 2e6f 6e5f 616e 6f6d 616c 6965 7372 1300  .on_anomaliesr..
+000005d0: 0000 6300 0000 0000 0000 0000 0000 0003  ..c.............
+000005e0: 0000 0004 0000 0053 0000 0073 2800 0000  .......S...s(...
+000005f0: 7400 8300 7d00 6900 7d01 7c00 6401 1900  t...}.i.}.|.d...
+00000600: 4400 5d06 7d02 6402 7c01 7c02 3c00 7109  D.].}.d.|.|.<.q.
+00000610: 7401 7c01 8301 5300 2903 4eda 1169 6e74  t.|...S.).N..int
+00000620: 6572 6e61 6c5f 7374 6174 7573 6573 da00  ernal_statuses..
+00000630: 2902 7206 0000 0072 0900 0000 2903 7220  ).r....r....).r 
+00000640: 0000 00da 0974 6865 5f70 6174 6873 da04  .....the_paths..
+00000650: 7061 7468 7216 0000 0072 1600 0000 7217  pathr....r....r.
+00000660: 0000 00da 1c6f 6e5f 5f67 6574 5f5f 6865  .....on__get__he
+00000670: 616c 7468 5f73 6361 6e73 5f5f 7061 7468  alth_scans__path
+00000680: 734f 0000 0073 0a00 0000 0602 0402 0c02  sO...s..........
+00000690: 0a01 0802 7a31 6f70 656e 5f68 6172 626f  ....z1open_harbo
+000006a0: 722e 3c6c 6f63 616c 733e 2e6f 6e5f 5f67  r.<locals>.on__g
+000006b0: 6574 5f5f 6865 616c 7468 5f73 6361 6e73  et__health_scans
+000006c0: 5f5f 7061 7468 7372 1200 0000 6301 0000  __pathsr....c...
+000006d0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+000006e0: 0053 0000 0072 1900 0000 721a 0000 0072  .S...r....r....r
+000006f0: 1600 0000 2901 da10 6865 616c 7468 5f73  ....)...health_s
+00000700: 6361 6e5f 7061 7468 7216 0000 0072 1600  can_pathr....r..
+00000710: 0000 7217 0000 00da 1a6f 6e5f 5f67 6574  ..r......on__get
+00000720: 5f5f 6865 616c 7468 5f73 6361 6e5f 5f70  __health_scan__p
+00000730: 6174 685a 0000 0072 1d00 0000 7a2f 6f70  athZ...r....z/op
+00000740: 656e 5f68 6172 626f 722e 3c6c 6f63 616c  en_harbor.<local
+00000750: 733e 2e6f 6e5f 5f67 6574 5f5f 6865 616c  s>.on__get__heal
+00000760: 7468 5f73 6361 6e5f 5f70 6174 687a 0730  th_scan__pathz.0
+00000770: 2e30 2e30 2e30 4629 02da 0470 6f72 74da  .0.0.0F)...port.
+00000780: 0564 6562 7567 2907 da05 7072 696e 7472  .debug)...printr
+00000790: 0700 0000 7203 0000 00da 0572 6f75 7465  ....r......route
+000007a0: 7204 0000 0072 0200 0000 da03 7275 6e29  r....r......run)
+000007b0: 0872 2900 0000 da07 7265 636f 7264 73da  .r).....records.
+000007c0: 0361 7070 7218 0000 0072 1c00 0000 7221  .appr....r....r!
+000007d0: 0000 0072 2600 0000 7228 0000 0072 1600  ...r&...r(...r..
+000007e0: 0000 7216 0000 0072 1700 0000 da0b 6f70  ..r....r......op
+000007f0: 656e 5f68 6172 626f 7224 0000 0073 2c00  en_harbor$...s,.
+00000800: 0000 0804 0a01 0804 0202 0c03 0e02 0a01  ................
+00000810: 0e09 0a01 0e03 0a01 0e0c 0a01 0e0a 0a01  ................
+00000820: 0804 0802 0404 0201 0201 0201 0afd 7230  ..............r0
+00000830: 0000 0029 0272 0500 0000 7205 0000 0029  ...).r....r....)
+00000840: 19da 075f 5f64 6f63 5f5f da15 7370 6163  ...__doc__..spac
+00000850: 6573 2e64 6f6e 655f 7769 7468 5f73 6361  es.done_with_sca
+00000860: 6e72 0200 0000 da12 7370 6163 6573 2e70  nr......spaces.p
+00000870: 6174 6873 5f70 6174 6368 7203 0000 00da  aths_patchr.....
+00000880: 1e73 7061 6365 732e 7468 655f 6865 616c  .spaces.the_heal
+00000890: 7468 5f73 6361 6e5f 7374 6172 7465 6472  th_scan_startedr
+000008a0: 0400 0000 da39 6269 6f74 6563 682e 7072  .....9biotech.pr
+000008b0: 6f63 6564 7572 6573 2e61 6767 7265 6761  ocedures.aggrega
+000008c0: 746f 725f 7072 6f63 6564 7572 652e 7072  tor_procedure.pr
+000008d0: 6f63 6573 732e 7661 7269 6162 6c65 7372  ocess.variablesr
+000008e0: 0600 0000 da05 666c 6173 6b72 0700 0000  ......flaskr....
+000008f0: 7208 0000 0072 0900 0000 da04 7269 6368  r....r......rich
+00000900: da04 6a73 6f6e da07 7061 7468 6c69 62da  ..json..pathlib.
+00000910: 026f 73da 076f 732e 7061 7468 720a 0000  .os..os.pathr...
+00000920: 0072 0b00 0000 720c 0000 00da 0373 7973  .r....r......sys
+00000930: da09 7468 7265 6164 696e 67da 0474 696d  ..threading..tim
+00000940: 6572 3000 0000 7216 0000 0072 1600 0000  er0...r....r....
+00000950: 7216 0000 0072 1700 0000 da08 3c6d 6f64  r....r......<mod
+00000960: 756c 653e 0100 0000 7322 0000 0004 020c  ule>....s"......
+00000970: 0c0c 010c 010c 0214 0308 0108 0308 0108  ................
+00000980: 0114 0108 0108 0108 0102 0502 010e fe    ...............
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 19:29:49 2024 UTC, .py size: 3672 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2dc6 2266 580e 0000  o.......-."fX...
+00000000: 6f0d 0d0a 0000 0000 21e0 2266 f40d 0000  o.......!."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
@@ -30,143 +30,152 @@
 000001d0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
 000001e0: 0003 0000 0073 2000 0000 7c00 6a00 6401  .....s ...|.j.d.
 000001f0: 6402 6701 6403 8d02 8700 6601 6404 6405  d.g.d.....f.d.d.
 00000200: 8408 8301 7d02 6400 5300 2906 4e7a 062f  ....}.d.S.).Nz./
 00000210: 7061 7468 73da 0550 4154 4348 2901 da07  paths..PATCH)...
 00000220: 6d65 7468 6f64 7363 0000 0000 0000 0000  methodsc........
 00000230: 0000 0000 0700 0000 0500 0000 1300 0000  ................
-00000240: 73d0 0000 0009 0074 00a0 0174 026a 03a0  s......t...t.j..
-00000250: 0464 01a1 01a1 017d 0074 0564 027c 0069  .d.....}.t.d.|.i
-00000260: 0183 0101 007c 0064 0319 007d 017c 0064  .....|.d...}.|.d
-00000270: 0419 0089 007c 0064 0519 0089 017c 0064  .....|.d.....|.d
-00000280: 0619 007d 027c 0064 0719 007d 037c 0074  ...}.|.d...}.|.t
-00000290: 0664 083c 007c 0064 0919 0074 0664 0a3c  .d.<.|.d...t.d.<
-000002a0: 0064 0b7c 0076 0072 387c 0064 0b19 0074  .d.|.v.r8|.d...t
-000002b0: 0664 0b3c 0009 0074 077c 0188 0183 0201  .d.<...t.|......
-000002c0: 0064 0c74 0664 0d3c 0087 0287 0087 0166  .d.t.d.<.......f
-000002d0: 0364 0e64 0f84 087d 047c 0272 5d74 087c  .d.d...}.|.r]t.|
-000002e0: 037c 017c 0464 108d 037d 0574 0564 117c  .|.|.d...}.t.d.|
-000002f0: 0569 0164 1264 138d 0201 0064 1453 007c  .i.d.d.....d.S.|
-00000300: 0144 005d 067d 067c 047c 0683 0101 0071  .D.].}.|.|.....q
-00000310: 5f64 1453 0029 157a 570a 0909 7368 6f77  _d.S.).zW...show
-00000320: 5f76 6172 6961 626c 6520 287b 0a09 0909  _variable ({....
-00000330: 2264 6f63 6b22 3a20 7b0a 0909 0909 2276  "dock": {....."v
-00000340: 6572 6222 3a20 2270 6174 6368 222c 0a09  erb": "patch",..
-00000350: 0909 0922 7061 7468 223a 2022 2f70 6174  ..."path": "/pat
-00000360: 6873 220a 0909 097d 0a09 097d 290a 0909  hs"....}...})...
-00000370: da04 7574 6638 7a11 2f70 6174 6873 2074  ..utf8z./paths t
-00000380: 6865 5f70 6163 6b65 74da 1273 7461 7475  he_packet..statu
-00000390: 735f 6368 6563 6b5f 7061 7468 73da 0c6d  s_check_paths..m
-000003a0: 6f64 756c 655f 7061 7468 73da 0d72 656c  odule_paths..rel
-000003b0: 6174 6976 655f 7061 7468 da0c 7369 6d75  ative_path..simu
-000003c0: 6c74 616e 656f 7573 da15 7369 6d75 6c74  ltaneous..simult
-000003d0: 616e 656f 7573 5f63 6170 6163 6974 79da  aneous_capacity.
-000003e0: 0f69 6e74 726f 5f76 6172 6961 626c 6573  .intro_variables
-000003f0: da10 7468 655f 696e 7472 6f5f 6861 7262  ..the_intro_harb
-00000400: 6f72 da0c 696e 7472 6f5f 6861 7262 6f72  or..intro_harbor
-00000410: da0d 7265 636f 7264 735f 6c65 7665 6cda  ..records_level.
-00000420: 0379 6573 da17 696e 7465 726e 616c 5f73  .yes..internal_s
-00000430: 7461 7475 7365 735f 6275 696c 7463 0100  tatuses_builtc..
-00000440: 0000 0000 0000 0000 0000 0400 0000 0600  ................
-00000450: 0000 1300 0000 73be 0000 0074 007c 0088  ......s....t.|..
-00000460: 0283 027d 0164 0174 0164 0219 007c 0119  ...}.d.t.d...|..
-00000470: 0064 0319 0064 043c 0074 0274 03a0 03a1  .d...d.<.t.t....
-00000480: 0083 0174 0164 0219 007c 0119 0064 0519  ...t.d...|...d..
-00000490: 0064 063c 0074 0274 03a0 03a1 0083 017d  .d.<.t.t.......}
-000004a0: 0274 0464 077c 0088 0188 0264 089c 0369  .t.d.|.....d...i
-000004b0: 0183 0101 0074 057c 0088 0188 0264 0988  .....t.|.....d..
-000004c0: 0069 0164 0a9c 0464 0b8d 017d 0374 0464  .i.d...d...}.t.d
-000004d0: 0c7c 0369 0164 0d64 0e8d 0201 007c 0374  .|.i.d.d.....|.t
-000004e0: 0164 0219 007c 0119 0064 0f3c 007c 0274  .d...|...d.<.|.t
-000004f0: 0164 0219 007c 0119 0064 0519 0064 103c  .d...|...d...d.<
-00000500: 0064 0174 0164 0219 007c 0119 0064 0319  .d.t.d...|...d..
-00000510: 0064 113c 007c 0353 0029 124e 7219 0000  .d.<.|.S.).Nr...
-00000520: 00da 1169 6e74 6572 6e61 6c5f 7374 6174  ...internal_stat
-00000530: 7573 6573 da0b 6f63 6375 7272 656e 6365  uses..occurrence
-00000540: 737a 1c73 6361 6e20 7072 6f63 6573 7320  sz.scan process 
-00000550: 7665 6e74 7572 6520 7374 6172 7465 64da  venture started.
-00000560: 0574 696d 6573 7a0f 7665 6e74 7572 6520  .timesz.venture 
-00000570: 7374 6172 7465 647a 0e73 7461 7274 696e  startedz.startin
-00000580: 6720 7363 616e 3a29 03da 1173 7461 7475  g scan:)...statu
-00000590: 735f 6368 6563 6b5f 7061 7468 7211 0000  s_check_pathr...
-000005a0: 0072 1200 0000 da04 706f 7274 2904 721e  .r......port).r.
-000005b0: 0000 0072 1100 0000 7212 0000 00da 1461  ...r....r......a
-000005c0: 6767 7265 6761 746f 725f 7072 6f63 6564  ggregator_proced
-000005d0: 7572 6529 01da 0670 6163 6b65 747a 0974  ure)...packetz.t
-000005e0: 6865 5f73 6361 6e3a da04 7368 6f77 a901  he_scan:..show..
-000005f0: da04 6d6f 6465 da07 7072 6f63 6573 73da  ..mode..process.
-00000600: 0773 7461 7274 6564 7a14 7363 616e 2070  .startedz.scan p
-00000610: 726f 6365 7373 2073 7461 7274 6564 2906  rocess started).
-00000620: 7204 0000 0072 0200 0000 da03 7374 72da  r....r......str.
-00000630: 0474 696d 6572 0500 0000 7207 0000 0029  .timer....r....)
-00000640: 0472 1e00 0000 da08 7265 6c5f 7061 7468  .r......rel_path
-00000650: da0a 7374 6172 745f 7469 6d65 da08 7468  ..start_time..th
-00000660: 655f 7363 616e 2903 da19 6167 6772 6567  e_scan)...aggreg
-00000670: 6174 6f72 5f70 726f 6365 6475 7265 5f70  ator_procedure_p
-00000680: 6f72 7472 1100 0000 7212 0000 00a9 00fa  ortr....r.......
-00000690: 602f 6269 6f74 6563 682f 7665 6e75 6573  `/biotech/venues
-000006a0: 2f73 7461 6765 732f 6269 6f74 6563 682f  /stages/biotech/
-000006b0: 7072 6f63 6564 7572 6573 2f61 6767 7265  procedures/aggre
-000006c0: 6761 746f 725f 7072 6f63 6564 7572 652f  gator_procedure/
-000006d0: 7072 6f63 6573 732f 6b65 672f 7370 6163  process/keg/spac
-000006e0: 6573 2f70 6174 6873 5f70 6174 6368 2e70  es/paths_patch.p
-000006f0: 79da 0776 656e 7475 7265 6a00 0000 7338  y..venturej...s8
-00000700: 0000 000a 0114 021c 010c 0202 0202 0102  ................
-00000710: 0102 0102 0104 fd06 ff02 0802 0202 0202  ................
-00000720: 0104 0302 ff04 fa06 ff02 0d04 0102 ff02  ................
-00000730: 0206 fe10 0414 0114 0104 027a 3170 6174  ...........z1pat
-00000740: 6873 5f70 6174 6368 2e3c 6c6f 6361 6c73  hs_patch.<locals
-00000750: 3e2e 7061 7468 735f 7061 7463 682e 3c6c  >.paths_patch.<l
-00000760: 6f63 616c 733e 2e76 656e 7475 7265 2903  ocals>.venture).
-00000770: da08 6361 7061 6369 7479 da05 6974 656d  ..capacity..item
-00000780: 73da 046d 6f76 657a 1f71 7565 7565 5f63  s..movez.queue_c
-00000790: 6170 6163 6974 795f 6c69 6d69 7465 7220  apacity_limiter 
-000007a0: 7072 6f63 6565 6473 7222 0000 0072 2300  proceedsr"...r#.
-000007b0: 0000 da08 7265 6365 6976 6564 2909 da04  ....received)...
-000007c0: 6a73 6f6e da05 6c6f 6164 7372 0900 0000  json..loadsr....
-000007d0: da04 6461 7461 da06 6465 636f 6465 7205  ..data..decoder.
-000007e0: 0000 0072 0200 0000 7203 0000 0072 0600  ...r....r....r..
-000007f0: 0000 2907 da0a 7468 655f 7061 636b 6574  ..)...the_packet
-00000800: 7210 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00000810: 2f00 0000 da08 7072 6f63 6565 6473 721e  /.....proceedsr.
-00000820: 0000 00a9 0172 2c00 0000 2902 7211 0000  .....r,...).r...
-00000830: 0072 1200 0000 722e 0000 00da 0b70 6174  .r....r......pat
-00000840: 6873 5f70 6174 6368 2400 0000 7348 0000  hs_patch$...sH..
-00000850: 0002 0b12 1002 0104 0106 ff08 0608 0208  ................
-00000860: 0108 0208 0108 070c 0108 030c 0102 0202  ................
-00000870: 0302 0102 0104 fe08 0710 0604 2902 0102  ............)...
-00000880: 0102 0102 0106 fd02 0604 0102 ff02 0206  ................
-00000890: fe04 0908 fc0a 0104 037a 2070 6174 6873  .........z paths
-000008a0: 5f70 6174 6368 2e3c 6c6f 6361 6c73 3e2e  _patch.<locals>.
-000008b0: 7061 7468 735f 7061 7463 6829 01da 0572  paths_patch)...r
-000008c0: 6f75 7465 2903 da03 6170 7072 2c00 0000  oute)...appr,...
-000008d0: 723b 0000 0072 2d00 0000 723a 0000 0072  r;...r-...r:...r
-000008e0: 2e00 0000 723b 0000 001f 0000 0073 0400  ....r;.......s..
-000008f0: 0000 0e05 1201 723b 0000 0029 014e 291b  ......r;...).N).
-00000900: da07 5f5f 646f 635f 5fda 3962 696f 7465  ..__doc__.9biote
-00000910: 6368 2e70 726f 6365 6475 7265 732e 6167  ch.procedures.ag
-00000920: 6772 6567 6174 6f72 5f70 726f 6365 6475  gregator_procedu
-00000930: 7265 2e70 726f 6365 7373 2e76 6172 6961  re.process.varia
-00000940: 626c 6573 7202 0000 0072 0300 0000 da41  blesr....r.....A
-00000950: 6269 6f74 6563 682e 7072 6f63 6564 7572  biotech.procedur
-00000960: 6573 2e61 6767 7265 6761 746f 725f 7072  es.aggregator_pr
-00000970: 6f63 6564 7572 652e 7072 6f63 6573 732e  ocedure.process.
-00000980: 6d6f 7665 732e 666f 726d 6174 5f70 6174  moves.format_pat
-00000990: 6872 0400 0000 da1c 6269 6f74 6563 682e  hr......biotech.
-000009a0: 746f 7069 6373 2e73 686f 772e 7661 7269  topics.show.vari
-000009b0: 6162 6c65 7205 0000 00da 2c62 696f 7465  abler.....,biote
-000009c0: 6368 2e74 6f70 6963 732e 7175 6575 6573  ch.topics.queues
-000009d0: 2e71 7565 7565 5f63 6170 6163 6974 795f  .queue_capacity_
-000009e0: 6c69 6d69 7465 7272 0600 0000 da21 6269  limiterr.....!bi
-000009f0: 6f74 6563 682e 7072 6f63 6564 7572 6573  otech.procedures
-00000a00: 2e68 6561 6c74 685f 7363 616e 2e6f 6e72  .health_scan.onr
-00000a10: 0700 0000 da05 666c 6173 6b72 0800 0000  ......flaskr....
-00000a20: 7209 0000 00da 0472 6963 6872 3400 0000  r......richr4...
-00000a30: da07 7061 7468 6c69 62da 026f 73da 076f  ..pathlib..os..o
-00000a40: 732e 7061 7468 720a 0000 0072 0b00 0000  s.pathr....r....
-00000a50: 720c 0000 00da 0373 7973 da09 7468 7265  r......sys..thre
-00000a60: 6164 696e 6772 2800 0000 723b 0000 0072  adingr(...r;...r
-00000a70: 2d00 0000 722d 0000 0072 2d00 0000 722e  -...r-...r-...r.
-00000a80: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000a90: 0073 2200 0000 0401 1007 0c01 0c02 0c01  .s".............
-00000aa0: 0c01 1003 0801 0803 0801 0801 1401 0801  ................
-00000ab0: 0801 0801 0207 0efd                      ........
+00000240: 73cc 0000 0074 0064 0164 0264 038d 0201  s....t.d.d.d....
+00000250: 0074 01a0 0274 036a 04a0 0564 04a1 01a1  .t...t.j...d....
+00000260: 017d 0074 0064 0564 0264 038d 0201 007c  .}.t.d.d.d.....|
+00000270: 0064 0619 007d 017c 0064 0719 0089 007c  .d...}.|.d.....|
+00000280: 0064 0819 0089 017c 0064 0919 007d 027c  .d.....|.d...}.|
+00000290: 0064 0a19 007d 037c 0074 0664 0b3c 007c  .d...}.|.t.d.<.|
+000002a0: 0064 0c19 0074 0664 0d3c 0064 0e7c 0076  .d...t.d.<.d.|.v
+000002b0: 0072 3d7c 0064 0e19 0074 0664 0e3c 0009  .r=|.d...t.d.<..
+000002c0: 0074 077c 0188 0183 0201 0064 0f74 0664  .t.|.......d.t.d
+000002d0: 103c 0087 0287 0087 0166 0364 1164 1284  .<.......f.d.d..
+000002e0: 087d 047c 0272 5b74 087c 037c 017c 0464  .}.|.r[t.|.|.|.d
+000002f0: 138d 037d 0509 0064 1453 007c 0144 005d  ...}...d.S.|.D.]
+00000300: 067d 067c 047c 0683 0101 0071 5d64 1453  .}.|.|.....q]d.S
+00000310: 0029 1561 0501 0000 0a09 0909 7b0a 0909  .).a........{...
+00000320: 0909 2270 6174 6873 223a 205b 5d2c 0a0a  .."paths": [],..
+00000330: 0909 0909 2272 656c 6174 6976 655f 7061  ...."relative_pa
+00000340: 7468 223a 2046 616c 7365 2c0a 0909 0909  th": False,.....
+00000350: 2272 656c 6174 6976 655f 7061 7468 223a  "relative_path":
+00000360: 2022 2f62 696f 7465 6368 2f76 656e 7565   "/biotech/venue
+00000370: 732f 7761 7265 686f 7573 652f 305f 6578  s/warehouse/0_ex
+00000380: 616d 706c 652f 6d6f 6475 6c65 7322 2c0a  ample/modules",.
+00000390: 0909 0909 0a09 0909 096d 6f64 756c 655f  .........module_
+000003a0: 7061 7468 7320 3d20 5b5d 2c0a 0909 0909  paths = [],.....
+000003b0: 0a09 0909 0973 696d 756c 7461 6e65 6f75  .....simultaneou
+000003c0: 7320 3d20 4661 6c73 652c 0a09 0909 0973  s = False,.....s
+000003d0: 696d 756c 7461 6e65 6f75 735f 6361 7061  imultaneous_capa
+000003e0: 6369 7479 203d 2031 302c 0a09 0909 090a  city = 10,......
+000003f0: 0909 0909 6265 666f 7265 203d 2046 616c  ....before = Fal
+00000400: 7365 2c0a 0909 0909 6166 7465 7220 3d20  se,.....after = 
+00000410: 4661 6c73 650a 0909 097d 0a09 097a 0f2f  False....}...z./
+00000420: 7061 7468 7320 7265 6365 6976 6564 da09  paths received..
+00000430: 636f 6e64 656e 7365 64a9 01da 046d 6f64  condensed....mod
+00000440: 65da 0475 7466 387a 1c2f 7061 7468 7320  e..utf8z./paths 
+00000450: 7061 7273 6564 2074 6865 2074 6865 5f70  parsed the the_p
+00000460: 6163 6b65 74da 1273 7461 7475 735f 6368  acket..status_ch
+00000470: 6563 6b5f 7061 7468 73da 0c6d 6f64 756c  eck_paths..modul
+00000480: 655f 7061 7468 73da 0d72 656c 6174 6976  e_paths..relativ
+00000490: 655f 7061 7468 da0c 7369 6d75 6c74 616e  e_path..simultan
+000004a0: 656f 7573 da15 7369 6d75 6c74 616e 656f  eous..simultaneo
+000004b0: 7573 5f63 6170 6163 6974 79da 0f69 6e74  us_capacity..int
+000004c0: 726f 5f76 6172 6961 626c 6573 da10 7468  ro_variables..th
+000004d0: 655f 696e 7472 6f5f 6861 7262 6f72 da0c  e_intro_harbor..
+000004e0: 696e 7472 6f5f 6861 7262 6f72 da0d 7265  intro_harbor..re
+000004f0: 636f 7264 735f 6c65 7665 6cda 0379 6573  cords_level..yes
+00000500: da17 696e 7465 726e 616c 5f73 7461 7475  ..internal_statu
+00000510: 7365 735f 6275 696c 7463 0100 0000 0000  ses_builtc......
+00000520: 0000 0000 0000 0400 0000 0600 0000 1300  ................
+00000530: 0000 73c2 0000 0074 007c 0088 0283 027d  ..s....t.|.....}
+00000540: 0164 0174 0164 0219 007c 0119 0064 0319  .d.t.d...|...d..
+00000550: 0064 043c 0074 0274 03a0 03a1 0083 0174  .d.<.t.t.......t
+00000560: 0164 0219 007c 0119 0064 0519 0064 063c  .d...|...d...d.<
+00000570: 0074 0274 03a0 03a1 0083 017d 0274 0464  .t.t.......}.t.d
+00000580: 077c 009b 0064 089d 0364 0964 0a8d 0201  .|...d...d.d....
+00000590: 0074 057c 0088 0188 0264 0b88 0069 0164  .t.|.....d...i.d
+000005a0: 0c9c 0464 0d8d 017d 037c 0374 0164 0219  ...d...}.|.t.d..
+000005b0: 007c 0119 0064 0e3c 007c 0274 0164 0219  .|...d.<.|.t.d..
+000005c0: 007c 0119 0064 0519 0064 0f3c 0064 0174  .|...d...d.<.d.t
+000005d0: 0164 0219 007c 0119 0064 0319 0064 103c  .d...|...d...d.<
+000005e0: 0074 0464 117c 009b 0064 089d 0364 0964  .t.d.|...d...d.d
+000005f0: 0a8d 0201 007c 0353 0029 124e 721c 0000  .....|.S.).Nr...
+00000600: 00da 1169 6e74 6572 6e61 6c5f 7374 6174  ...internal_stat
+00000610: 7573 6573 da0b 6f63 6375 7272 656e 6365  uses..occurrence
+00000620: 737a 1c73 6361 6e20 7072 6f63 6573 7320  sz.scan process 
+00000630: 7665 6e74 7572 6520 7374 6172 7465 64da  venture started.
+00000640: 0574 696d 6573 7a0f 7665 6e74 7572 6520  .timesz.venture 
+00000650: 7374 6172 7465 647a 0f73 7461 7274 696e  startedz.startin
+00000660: 6720 7363 616e 2027 fa01 2772 0f00 0000  g scan '..'r....
+00000670: 7210 0000 00da 0470 6f72 7429 04da 1173  r......port)...s
+00000680: 7461 7475 735f 6368 6563 6b5f 7061 7468  tatus_check_path
+00000690: 7214 0000 0072 1500 0000 da14 6167 6772  r....r......aggr
+000006a0: 6567 6174 6f72 5f70 726f 6365 6475 7265  egator_procedure
+000006b0: 2901 da06 7061 636b 6574 da07 7072 6f63  )...packet..proc
+000006c0: 6573 73da 0773 7461 7274 6564 7a14 7363  ess..startedz.sc
+000006d0: 616e 2070 726f 6365 7373 2073 7461 7274  an process start
+000006e0: 6564 7a0e 7363 616e 2073 7461 7274 6564  edz.scan started
+000006f0: 2027 2906 7204 0000 0072 0200 0000 da03   ').r....r......
+00000700: 7374 72da 0474 696d 6572 0500 0000 7207  str..timer....r.
+00000710: 0000 0029 0472 2300 0000 da08 7265 6c5f  ...).r#.....rel_
+00000720: 7061 7468 da0a 7374 6172 745f 7469 6d65  path..start_time
+00000730: da08 7468 655f 7363 616e 2903 da19 6167  ..the_scan)...ag
+00000740: 6772 6567 6174 6f72 5f70 726f 6365 6475  gregator_procedu
+00000750: 7265 5f70 6f72 7472 1400 0000 7215 0000  re_portr....r...
+00000760: 00a9 00fa 602f 6269 6f74 6563 682f 7665  ....`/biotech/ve
+00000770: 6e75 6573 2f73 7461 6765 732f 6269 6f74  nues/stages/biot
+00000780: 6563 682f 7072 6f63 6564 7572 6573 2f61  ech/procedures/a
+00000790: 6767 7265 6761 746f 725f 7072 6f63 6564  ggregator_proced
+000007a0: 7572 652f 7072 6f63 6573 732f 6b65 672f  ure/process/keg/
+000007b0: 7370 6163 6573 2f70 6174 6873 5f70 6174  spaces/paths_pat
+000007c0: 6368 2e70 79da 0776 656e 7475 7265 6100  ch.py..venturea.
+000007d0: 0000 7324 0000 000a 0114 021c 010c 0214  ..s$............
+000007e0: 0202 0202 0202 0202 0104 0302 ff04 fa06  ................
+000007f0: ff10 0d14 0114 0114 0204 037a 3170 6174  ...........z1pat
+00000800: 6873 5f70 6174 6368 2e3c 6c6f 6361 6c73  hs_patch.<locals
+00000810: 3e2e 7061 7468 735f 7061 7463 682e 3c6c  >.paths_patch.<l
+00000820: 6f63 616c 733e 2e76 656e 7475 7265 2903  ocals>.venture).
+00000830: da08 6361 7061 6369 7479 da05 6974 656d  ..capacity..item
+00000840: 73da 046d 6f76 65da 0872 6563 6569 7665  s..move..receive
+00000850: 6429 0972 0500 0000 da04 6a73 6f6e da05  d).r......json..
+00000860: 6c6f 6164 7372 0900 0000 da04 6461 7461  loadsr......data
+00000870: da06 6465 636f 6465 7202 0000 0072 0300  ..decoder....r..
+00000880: 0000 7206 0000 0029 07da 0a74 6865 5f70  ..r....)...the_p
+00000890: 6163 6b65 7472 1300 0000 7216 0000 0072  acketr....r....r
+000008a0: 1700 0000 7230 0000 00da 0870 726f 6365  ....r0.....proce
+000008b0: 6564 7372 2300 0000 a901 722d 0000 0029  edsr#.....r-...)
+000008c0: 0272 1400 0000 7215 0000 0072 2f00 0000  .r....r....r/...
+000008d0: da0b 7061 7468 735f 7061 7463 6824 0000  ..paths_patch$..
+000008e0: 0073 3c00 0000 0c13 1201 0c01 0804 0802  .s<.............
+000008f0: 0801 0802 0801 0807 0c01 0803 0c01 0202  ................
+00000900: 0203 0201 0201 04fe 0807 1006 0422 0201  ............."..
+00000910: 0201 0201 0201 06fd 0206 040b 08fc 0a01  ................
+00000920: 0403 7a20 7061 7468 735f 7061 7463 682e  ..z paths_patch.
+00000930: 3c6c 6f63 616c 733e 2e70 6174 6873 5f70  <locals>.paths_p
+00000940: 6174 6368 2901 da05 726f 7574 6529 03da  atch)...route)..
+00000950: 0361 7070 722d 0000 0072 3c00 0000 722e  .appr-...r<...r.
+00000960: 0000 0072 3b00 0000 722f 0000 0072 3c00  ...r;...r/...r<.
+00000970: 0000 1f00 0000 7304 0000 000e 0512 0172  ......s........r
+00000980: 3c00 0000 2901 4e29 1bda 075f 5f64 6f63  <...).N)...__doc
+00000990: 5f5f da39 6269 6f74 6563 682e 7072 6f63  __.9biotech.proc
+000009a0: 6564 7572 6573 2e61 6767 7265 6761 746f  edures.aggregato
+000009b0: 725f 7072 6f63 6564 7572 652e 7072 6f63  r_procedure.proc
+000009c0: 6573 732e 7661 7269 6162 6c65 7372 0200  ess.variablesr..
+000009d0: 0000 7203 0000 00da 4162 696f 7465 6368  ..r.....Abiotech
+000009e0: 2e70 726f 6365 6475 7265 732e 6167 6772  .procedures.aggr
+000009f0: 6567 6174 6f72 5f70 726f 6365 6475 7265  egator_procedure
+00000a00: 2e70 726f 6365 7373 2e6d 6f76 6573 2e66  .process.moves.f
+00000a10: 6f72 6d61 745f 7061 7468 7204 0000 00da  ormat_pathr.....
+00000a20: 1c62 696f 7465 6368 2e74 6f70 6963 732e  .biotech.topics.
+00000a30: 7368 6f77 2e76 6172 6961 626c 6572 0500  show.variabler..
+00000a40: 0000 da2c 6269 6f74 6563 682e 746f 7069  ...,biotech.topi
+00000a50: 6373 2e71 7565 7565 732e 7175 6575 655f  cs.queues.queue_
+00000a60: 6361 7061 6369 7479 5f6c 696d 6974 6572  capacity_limiter
+00000a70: 7206 0000 00da 2162 696f 7465 6368 2e70  r.....!biotech.p
+00000a80: 726f 6365 6475 7265 732e 6865 616c 7468  rocedures.health
+00000a90: 5f73 6361 6e2e 6f6e 7207 0000 00da 0566  _scan.onr......f
+00000aa0: 6c61 736b 7208 0000 0072 0900 0000 da04  laskr....r......
+00000ab0: 7269 6368 7235 0000 00da 0770 6174 686c  richr5.....pathl
+00000ac0: 6962 da02 6f73 da07 6f73 2e70 6174 6872  ib..os..os.pathr
+00000ad0: 0a00 0000 720b 0000 0072 0c00 0000 da03  ....r....r......
+00000ae0: 7379 73da 0974 6872 6561 6469 6e67 7229  sys..threadingr)
+00000af0: 0000 0072 3c00 0000 722e 0000 0072 2e00  ...r<...r....r..
+00000b00: 0000 722e 0000 0072 2f00 0000 da08 3c6d  ..r....r/.....<m
+00000b10: 6f64 756c 653e 0100 0000 7322 0000 0004  odule>....s"....
+00000b20: 0110 070c 010c 020c 010c 0110 0308 0108  ................
+00000b30: 0308 0108 0114 0108 0108 0108 0102 070e  ................
+00000b40: fd                                       .
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 16:26:14 2024 UTC, .py size: 789 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-00000000: 6f0d 0d0a 0000 0000 269b 2266 1503 0000  o.......&."f....
+00000000: 6f0d 0d0a 0000 0000 d9dc 2266 0103 0000  o........."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 5a07 6400  m.Z...d.d.l.Z.d.
 00000060: 6404 6c08 5a08 6405 6406 8400 5a09 6404  d.l.Z.d.d...Z.d.
 00000070: 5300 2907 e900 0000 0029 01da 0d73 686f  S.)......)...sho
 00000080: 775f 7661 7269 6162 6c65 2901 da14 6167  w_variable)...ag
 00000090: 6772 6567 6174 6f72 5f76 6172 6961 626c  gregator_variabl
 000000a0: 6573 2902 da05 466c 6173 6bda 0772 6571  es)...Flask..req
 000000b0: 7565 7374 4e63 0100 0000 0000 0000 0000  uestNc..........
 000000c0: 0000 0200 0000 0400 0000 4300 0000 731c  ..........C...s.
 000000d0: 0000 007c 006a 0064 0164 0267 0164 038d  ...|.j.d.d.g.d..
 000000e0: 0264 0464 0584 0083 017d 0164 0053 0029  .d.d.....}.d.S.)
-000000f0: 064e fa18 2f74 6865 5f68 6561 6c74 685f  .N../the_health_
+000000f0: 064e 7a18 2f74 6865 5f68 6561 6c74 685f  .Nz./the_health_
 00000100: 7363 616e 5f73 7461 7274 6564 da05 5041  scan_started..PA
 00000110: 5443 4829 01da 076d 6574 686f 6473 6300  TCH)...methodsc.
 00000120: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-00000130: 0000 0053 0000 0073 5000 0000 7400 6401  ...S...sP...t.d.
-00000140: 6402 6403 6404 9c02 6901 8301 0100 7401  d.d.d...i.....t.
-00000150: a002 7403 6a04 a005 6405 a101 a101 7d00  ..t.j...d.....}.
-00000160: 7c00 6406 1900 7d01 7400 6407 7c00 6901  |.d...}.t.d.|.i.
-00000170: 8301 0100 6408 7406 6409 1900 7c01 1900  ....d.t.d...|...
-00000180: 640a 1900 640b 3c00 640c 5300 290d 4eda  d...d.<.d.S.).N.
-00000190: 0464 6f63 6bda 0570 6174 6368 7206 0000  .dock..patchr...
-000001a0: 0029 02da 0476 6572 62da 0470 6174 68da  .)...verb..path.
-000001b0: 0475 7466 3872 0c00 0000 7a1f 7468 655f  .utf8r....z.the_
-000001c0: 6865 616c 7468 5f73 6361 6e5f 7374 6172  health_scan_star
-000001d0: 7465 643a 2070 6163 6b65 74da 0379 6573  ted: packet..yes
-000001e0: da11 696e 7465 726e 616c 5f73 7461 7475  ..internal_statu
-000001f0: 7365 73da 0b6f 6363 7572 7265 6e63 6573  ses..occurrences
-00000200: 7a20 7363 616e 2070 726f 6365 7373 206e  z scan process n
-00000210: 6f74 6966 6965 6420 6167 6772 6567 6174  otified aggregat
-00000220: 6f72 da08 7265 6365 6976 6564 2907 7202  or..received).r.
-00000230: 0000 00da 046a 736f 6eda 056c 6f61 6473  .....json..loads
-00000240: 7205 0000 00da 0464 6174 61da 0664 6563  r......data..dec
-00000250: 6f64 6572 0300 0000 2902 da0a 7468 655f  oder....)...the_
-00000260: 7061 636b 6574 da08 7468 655f 7061 7468  packet..the_path
-00000270: a900 7218 0000 00fa 6c2f 6269 6f74 6563  ..r.....l/biotec
-00000280: 682f 7665 6e75 6573 2f73 7461 6765 732f  h/venues/stages/
-00000290: 6269 6f74 6563 682f 7072 6f63 6564 7572  biotech/procedur
-000002a0: 6573 2f61 6767 7265 6761 746f 725f 7072  es/aggregator_pr
-000002b0: 6f63 6564 7572 652f 7072 6f63 6573 732f  ocedure/process/
-000002c0: 6b65 672f 7370 6163 6573 2f74 6865 5f68  keg/spaces/the_h
-000002d0: 6561 6c74 685f 7363 616e 5f73 7461 7274  ealth_scan_start
-000002e0: 6564 2e70 79da 1e70 6174 6368 5f5f 7468  ed.py..patch__th
-000002f0: 655f 6865 616c 7468 5f73 6361 6e5f 7374  e_health_scan_st
-00000300: 6172 7465 6413 0000 0073 1a00 0000 0202  arted....s......
-00000310: 0201 0201 0201 04fe 06ff 1207 0802 0202  ................
-00000320: 0401 06ff 1404 0403 7a3f 7468 655f 6865  ........z?the_he
-00000330: 616c 7468 5f73 6361 6e5f 7374 6172 7465  alth_scan_starte
-00000340: 642e 3c6c 6f63 616c 733e 2e70 6174 6368  d.<locals>.patch
-00000350: 5f5f 7468 655f 6865 616c 7468 5f73 6361  __the_health_sca
-00000360: 6e5f 7374 6172 7465 6429 01da 0572 6f75  n_started)...rou
-00000370: 7465 2902 da03 6170 7072 1a00 0000 7218  te)...appr....r.
-00000380: 0000 0072 1800 0000 7219 0000 00da 1774  ...r....r......t
-00000390: 6865 5f68 6561 6c74 685f 7363 616e 5f73  he_health_scan_s
-000003a0: 7461 7274 6564 1200 0000 7304 0000 000e  tarted....s.....
-000003b0: 010e 0172 1d00 0000 290a da1c 6269 6f74  ...r....)...biot
-000003c0: 6563 682e 746f 7069 6373 2e73 686f 772e  ech.topics.show.
-000003d0: 7661 7269 6162 6c65 7202 0000 00da 3962  variabler.....9b
-000003e0: 696f 7465 6368 2e70 726f 6365 6475 7265  iotech.procedure
-000003f0: 732e 6167 6772 6567 6174 6f72 5f70 726f  s.aggregator_pro
-00000400: 6365 6475 7265 2e70 726f 6365 7373 2e76  cedure.process.v
-00000410: 6172 6961 626c 6573 7203 0000 00da 0566  ariablesr......f
-00000420: 6c61 736b 7204 0000 0072 0500 0000 da04  laskr....r......
-00000430: 7269 6368 7212 0000 0072 1d00 0000 7218  richr....r....r.
-00000440: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00000450: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000460: 730c 0000 000c 050c 0110 0308 0108 030c  s...............
-00000470: 04                                       .
+00000130: 0000 0053 0000 0073 4a00 0000 7400 6401  ...S...sJ...t.d.
+00000140: 6402 6403 8d02 0100 7401 a002 7403 6a04  d.d.....t...t.j.
+00000150: a005 6404 a101 a101 7d00 7c00 6405 1900  ..d.....}.|.d...
+00000160: 7d01 7400 6406 6402 6403 8d02 0100 6407  }.t.d.d.d.....d.
+00000170: 7406 6408 1900 7c01 1900 6409 1900 640a  t.d...|...d...d.
+00000180: 3c00 640b 5300 290c 4e7a 2172 6563 6569  <.d.S.).Nz!recei
+00000190: 7665 6420 2f74 6865 5f68 6561 6c74 685f  ved /the_health_
+000001a0: 7363 616e 5f73 7461 7274 6564 da09 636f  scan_started..co
+000001b0: 6e64 656e 7365 6429 01da 046d 6f64 65da  ndensed)...mode.
+000001c0: 0475 7466 38da 0470 6174 687a 2b70 6172  .utf8..pathz+par
+000001d0: 7365 6420 7061 636b 6574 2066 726f 6d20  sed packet from 
+000001e0: 2f74 6865 5f68 6561 6c74 685f 7363 616e  /the_health_scan
+000001f0: 5f73 7461 7274 6564 da03 7965 73da 1169  _started..yes..i
+00000200: 6e74 6572 6e61 6c5f 7374 6174 7573 6573  nternal_statuses
+00000210: da0b 6f63 6375 7272 656e 6365 737a 2073  ..occurrencesz s
+00000220: 6361 6e20 7072 6f63 6573 7320 6e6f 7469  can process noti
+00000230: 6669 6564 2061 6767 7265 6761 746f 72da  fied aggregator.
+00000240: 0872 6563 6569 7665 6429 0772 0200 0000  .received).r....
+00000250: da04 6a73 6f6e da05 6c6f 6164 7372 0500  ..json..loadsr..
+00000260: 0000 da04 6461 7461 da06 6465 636f 6465  ....data..decode
+00000270: 7203 0000 0029 02da 0a74 6865 5f70 6163  r....)...the_pac
+00000280: 6b65 74da 0874 6865 5f70 6174 68a9 0072  ket..the_path..r
+00000290: 1600 0000 fa6c 2f62 696f 7465 6368 2f76  .....l/biotech/v
+000002a0: 656e 7565 732f 7374 6167 6573 2f62 696f  enues/stages/bio
+000002b0: 7465 6368 2f70 726f 6365 6475 7265 732f  tech/procedures/
+000002c0: 6167 6772 6567 6174 6f72 5f70 726f 6365  aggregator_proce
+000002d0: 6475 7265 2f70 726f 6365 7373 2f6b 6567  dure/process/keg
+000002e0: 2f73 7061 6365 732f 7468 655f 6865 616c  /spaces/the_heal
+000002f0: 7468 5f73 6361 6e5f 7374 6172 7465 642e  th_scan_started.
+00000300: 7079 da1e 7061 7463 685f 5f74 6865 5f68  py..patch__the_h
+00000310: 6561 6c74 685f 7363 616e 5f73 7461 7274  ealth_scan_start
+00000320: 6564 1300 0000 730c 0000 000c 0212 0208  ed....s.........
+00000330: 010c 0214 0204 037a 3f74 6865 5f68 6561  .......z?the_hea
+00000340: 6c74 685f 7363 616e 5f73 7461 7274 6564  lth_scan_started
+00000350: 2e3c 6c6f 6361 6c73 3e2e 7061 7463 685f  .<locals>.patch_
+00000360: 5f74 6865 5f68 6561 6c74 685f 7363 616e  _the_health_scan
+00000370: 5f73 7461 7274 6564 2901 da05 726f 7574  _started)...rout
+00000380: 6529 02da 0361 7070 7218 0000 0072 1600  e)...appr....r..
+00000390: 0000 7216 0000 0072 1700 0000 da17 7468  ..r....r......th
+000003a0: 655f 6865 616c 7468 5f73 6361 6e5f 7374  e_health_scan_st
+000003b0: 6172 7465 6412 0000 0073 0400 0000 0e01  arted....s......
+000003c0: 0e01 721b 0000 0029 0ada 1c62 696f 7465  ..r....)...biote
+000003d0: 6368 2e74 6f70 6963 732e 7368 6f77 2e76  ch.topics.show.v
+000003e0: 6172 6961 626c 6572 0200 0000 da39 6269  ariabler.....9bi
+000003f0: 6f74 6563 682e 7072 6f63 6564 7572 6573  otech.procedures
+00000400: 2e61 6767 7265 6761 746f 725f 7072 6f63  .aggregator_proc
+00000410: 6564 7572 652e 7072 6f63 6573 732e 7661  edure.process.va
+00000420: 7269 6162 6c65 7372 0300 0000 da05 666c  riablesr......fl
+00000430: 6173 6b72 0400 0000 7205 0000 00da 0472  askr....r......r
+00000440: 6963 6872 1000 0000 721b 0000 0072 1600  ichr....r....r..
+00000450: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000460: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000470: 0c00 0000 0c05 0c01 1003 0801 0803 0c04  ................
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,22 +31,14 @@
 def paths_patch (
 	app,
 	
 	aggregator_procedure_port = None
 ):
 	@app.route ("/paths", methods = [ 'PATCH' ])
 	def paths_patch ():	
-		'''
-		show_variable ({
-			"dock": {
-				"verb": "patch",
-				"path": "/paths"
-			}
-		})
-		'''
 		
 		'''
 			{
 				"paths": [],
 
 				"relative_path": False,
 				"relative_path": "/biotech/venues/warehouse/0_example/modules",
@@ -56,18 +48,17 @@
 				simultaneous = False,
 				simultaneous_capacity = 10,
 				
 				before = False,
 				after = False
 			}
 		'''	
+		show_variable ("/paths received", mode = "condensed")
 		the_packet = json.loads (request.data.decode ('utf8'))
-		show_variable ({
-			"/paths the_packet": the_packet
-		})
+		show_variable ("/paths parsed the the_packet", mode = "condensed")
 
 		#----
 		#
 		status_check_paths = the_packet ["status_check_paths"]
 
 		module_paths = the_packet ["module_paths"]
 		relative_path = the_packet ["relative_path"]
@@ -106,58 +97,53 @@
 		def venture (status_check_path):
 			rel_path = format_path (status_check_path, relative_path);
 		
 			aggregator_variables ["internal_statuses"] [ rel_path ] ["occurrences"] ["scan process venture started"] = "yes"
 			aggregator_variables ["internal_statuses"] [ rel_path ] ["times"] ["venture started"] = str (time.time ())
 		
 			start_time = str (time.time ())
-		
-			show_variable ({
-				"starting scan:": {
-					"status_check_path": status_check_path,
-					"module_paths": module_paths,
-					"relative_path": relative_path
-				}
-			})
+
+			show_variable (f"starting scan '{ status_check_path }'", mode = "condensed")
 		
 			the_scan = turn_on_health_check (
 				packet = {
 					"status_check_path": status_check_path,
 					
 					"module_paths": module_paths,
 					"relative_path": relative_path,
 					
 					"aggregator_procedure": {
 						"port": aggregator_procedure_port
 					}
 				}
 			)
 			
-			show_variable ({
-				"the_scan:": the_scan
-			}, mode = "show")
-			
 			aggregator_variables ["internal_statuses"] [ rel_path ] ["process" ] = the_scan
 			aggregator_variables ["internal_statuses"] [ rel_path ] ["times"] ["started"] = start_time
 			aggregator_variables ["internal_statuses"] [ rel_path ] ["occurrences"] ["scan process started"] = "yes"
 
+			show_variable (f"scan started '{ status_check_path }'", mode = "condensed")
+
+
 			return the_scan;
 		
 		
 		
 		if (simultaneous):
 			proceeds = queue_capacity_limiter (
 				capacity = simultaneous_capacity,
 				items = status_check_paths,
 				move = venture
 			)		
 			
+			'''
 			show_variable ({
 				"queue_capacity_limiter proceeds": proceeds
 			}, mode = "show")
+			'''
 			
 		else:
 			for status_check_path in status_check_paths:
 				venture (status_check_path)
 		
 	
 		return "received"
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,27 +14,19 @@
 import json
 #
 #----
 
 def the_health_scan_started (app):
 	@app.route ("/the_health_scan_started", methods = [ 'PATCH' ])
 	def patch__the_health_scan_started ():
-		show_variable ({
-			"dock": {
-				"verb": "patch",
-				"path": "/the_health_scan_started"
-			}
-		})
+		show_variable ("received /the_health_scan_started", mode = "condensed")
 	
 		the_packet = json.loads (request.data.decode ('utf8'))
-		
 		the_path = the_packet ["path"]
 		
-		show_variable ({
-			"the_health_scan_started: packet": the_packet
-		})
+		show_variable ("parsed packet from /the_health_scan_started", mode = "condensed")
 		
 		aggregator_variables ["internal_statuses"] [ the_path ] ["occurrences"] ["scan process notified aggregator"] = "yes"
 
 	
 		return "received"
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 18:03:38 2024 UTC, .py size: 2705 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 fab1 2266 910a 0000  o........."f....
+00000000: 6f0d 0d0a 0000 0000 d3f3 2266 650b 0000  o........."fe...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 0900 0900 6401 6402 6c01 6d02 5a02  Z.....d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d03 5a03 0100 6405  ..d.d.l.m.Z...d.
 00000050: 6406 6c04 6d05 5a05 0100 6405 6407 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6405 6408 6c08 5a08 6405  m.Z...d.d.l.Z.d.
 00000070: 6408 6c09 5a09 6409 640a 8400 5a0a 6408  d.l.Z.d.d...Z.d.
@@ -13,97 +13,108 @@
 000000c0: 01da 1461 6767 7265 6761 746f 725f 7661  ...aggregator_va
 000000d0: 7269 6162 6c65 73e9 0100 0000 2901 da0f  riables.....)...
 000000e0: 6167 6772 6567 6174 655f 7374 6174 73e9  aggregate_stats.
 000000f0: 0000 0000 2901 da16 7061 7273 655f 705f  ....)...parse_p_
 00000100: 6578 7065 6374 5f72 6563 6f72 6473 2901  expect_records).
 00000110: da0d 7368 6f77 5f76 6172 6961 626c 654e  ..show_variableN
 00000120: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
-00000130: 0008 0000 0043 0000 0073 d001 0000 7c00  .....C...s....|.
+00000130: 0008 0000 0043 0000 0073 0e02 0000 7c00  .....C...s....|.
 00000140: 6401 1900 7d01 7c00 6402 1900 7d02 7400  d...}.|.d...}.t.
-00000150: 6403 7c00 6901 6404 6405 8d02 0100 7401  d.|.i.d.d.....t.
-00000160: 6406 1900 7c01 1900 6407 1900 6407 1900  d...|...d...d...
-00000170: a002 a100 0100 7403 7404 a004 a100 8301  ......t.t.......
-00000180: 7401 6406 1900 7c01 1900 6408 1900 6409  t.d...|...d...d.
-00000190: 3c00 7405 7401 6406 1900 7c01 1900 6408  <.t.t.d...|...d.
-000001a0: 1900 6409 1900 8301 7405 7401 6406 1900  ..d.....t.t.d...
-000001b0: 7c01 1900 6408 1900 640a 1900 8301 1800  |...d...d.......
-000001c0: 7401 6406 1900 7c01 1900 6408 1900 640b  t.d...|...d...d.
-000001d0: 3c00 640c 7401 6406 1900 7c01 1900 640d  <.d.t.d...|...d.
-000001e0: 1900 640e 3c00 7400 6408 7401 6406 1900  ..d.<.t.d.t.d...
-000001f0: 7c01 1900 6408 1900 6901 6404 6405 8d02  |...d...i.d.d...
-00000200: 0100 7a17 7406 7401 6406 1900 7c01 1900  ..z.t.t.d...|...
-00000210: 6407 1900 640f 1900 8300 6410 6411 8d02  d...d.....d.d...
-00000220: 7401 6406 1900 7c01 1900 640f 3c00 5700  t.d...|...d.<.W.
-00000230: 6e0d 0400 7407 7986 0100 0100 0100 7400  n...t.y.......t.
-00000240: 6412 8301 0100 5900 6e01 7700 6401 7c01  d.....Y.n.w.d.|.
-00000250: 6901 7d03 7a0c 7401 6406 1900 7c01 1900  i.}.z.t.d...|...
-00000260: 640f 1900 7c03 640f 3c00 5700 6e0d 0400  d...|.d.<.W.n...
-00000270: 7407 79a4 0100 0100 0100 7400 6413 8301  t.y.......t.d...
-00000280: 0100 5900 6e01 7700 7a0d 7c02 4400 5d08  ..Y.n.w.z.|.D.].
-00000290: 7d04 7c02 7c04 1900 7c03 7c04 3c00 71a8  }.|.|...|.|.<.q.
-000002a0: 5700 6e0d 0400 7407 79bf 0100 0100 0100  W.n...t.y.......
-000002b0: 7400 6414 8301 0100 5900 6e01 7700 7c03  t.d.....Y.n.w.|.
-000002c0: 7401 6406 1900 7c01 1900 6415 3c00 640c  t.d...|...d.<.d.
-000002d0: 7401 6406 1900 7c01 1900 640d 1900 6416  t.d...|...d...d.
-000002e0: 3c00 7400 6417 8301 0100 7404 a008 6418  <.t.d.....t...d.
-000002f0: a101 0100 0900 6419 7401 6406 1900 7c01  ......d.t.d...|.
-00000300: 1900 641a 1900 6407 3c00 6400 5300 291b  ..d...d.<.d.S.).
-00000310: 4eda 0470 6174 68da 0672 6573 756c 747a  N..path..resultz
-00000320: 1964 6f6e 6520 7769 7468 2073 6361 6e2c  .done with scan,
-00000330: 2073 746f 7070 696e 673a da04 7368 6f77   stopping:..show
-00000340: 2901 da04 6d6f 6465 da11 696e 7465 726e  )...mode..intern
-00000350: 616c 5f73 7461 7475 7365 73da 0770 726f  al_statuses..pro
-00000360: 6365 7373 da05 7469 6d65 73da 0565 6e64  cess..times..end
-00000370: 6564 da07 7374 6172 7465 64da 0765 6c61  ed..started..ela
-00000380: 7073 6564 da03 7965 73da 0b6f 6363 7572  psed..yes..occur
-00000390: 7265 6e63 6573 7a18 7363 616e 2070 726f  rencesz.scan pro
-000003a0: 6365 7373 2077 6173 2073 746f 7070 6564  cess was stopped
-000003b0: da07 7265 636f 7264 73da 0455 5446 3829  ..records..UTF8)
-000003c0: 0272 1400 0000 da06 666f 726d 6174 7a20  .r......formatz 
-000003d0: 5468 6520 7265 636f 7264 7320 636f 756c  The records coul
-000003e0: 6420 6e6f 7420 6265 2070 6172 7365 6421  d not be parsed!
-000003f0: 7a35 5468 6520 7265 636f 7264 7320 636f  z5The records co
-00000400: 756c 6420 6e6f 7420 6265 2061 6464 6564  uld not be added
-00000410: 2074 6f20 7468 6520 7265 7375 6c74 7320   to the results 
-00000420: 7061 636b 6574 217a 2b41 2072 6573 756c  packet!z+A resul
-00000430: 7420 696e 2074 6865 2072 6573 756c 7473  t in the results
-00000440: 2063 6f75 6c64 206e 6f74 2062 6520 6164   could not be ad
-00000450: 6465 6421 da0f 7265 7375 6c74 735f 6f66  ded!..results_of
-00000460: 5f73 6361 6e7a 1b73 6361 6e20 7265 636f  _scanz.scan reco
-00000470: 7264 7320 7765 7265 2072 6574 7269 6576  rds were retriev
-00000480: 6564 7a0e 646f 6e65 2077 6974 6820 7363  edz.done with sc
-00000490: 616e 7203 0000 00da 0464 6f6e 65da 0673  anr......done..s
-000004a0: 7461 7475 7329 0972 0700 0000 7202 0000  tatus).r....r...
-000004b0: 00da 0974 6572 6d69 6e61 7465 da03 7374  ...terminate..st
-000004c0: 72da 0474 696d 65da 0566 6c6f 6174 7206  r..time..floatr.
-000004d0: 0000 00da 0945 7863 6570 7469 6f6e da05  .....Exception..
-000004e0: 736c 6565 7029 05da 0a74 6865 5f70 6163  sleep)...the_pac
-000004f0: 6b65 74da 0874 6865 5f70 6174 68da 0a74  ket..the_path..t
-00000500: 6865 5f72 6573 756c 74da 1274 6865 5f72  he_result..the_r
-00000510: 6573 756c 7473 5f70 6163 6b65 7472 0900  esults_packetr..
-00000520: 0000 a900 7224 0000 00fa 5e2f 6269 6f74  ....r$....^/biot
-00000530: 6563 682f 7665 6e75 6573 2f73 7461 6765  ech/venues/stage
-00000540: 732f 6269 6f74 6563 682f 7072 6f63 6564  s/biotech/proced
-00000550: 7572 6573 2f61 6767 7265 6761 746f 725f  ures/aggregator_
-00000560: 7072 6f63 6564 7572 652f 7072 6f63 6573  procedure/proces
-00000570: 732f 6d6f 7665 732f 646f 6e65 5f77 6974  s/moves/done_wit
-00000580: 685f 7363 616e 2e70 79da 1364 6f6e 655f  h_scan.py..done_
-00000590: 7769 7468 5f73 6361 6e5f 6d6f 7665 2500  with_scan_move%.
-000005a0: 0000 735e 0000 0008 0108 0102 0404 0102  ..s^............
-000005b0: ff02 0206 fe18 0a1c 0116 0216 0102 ff12  ................
-000005c0: ff14 0402 0710 0102 ff02 0206 fe02 0602  ................
-000005d0: 0114 0102 0116 fe0c 040c 0102 ff04 0404  ................
-000005e0: ff02 0418 010c 010c 0102 ff02 0308 010e  ................
-000005f0: 0104 ff0c 020c 0102 ff10 0314 0208 030a  ................
-00000600: 0402 0218 0372 2600 0000 290b da07 5f5f  .....r&...)...__
-00000610: 646f 635f 5fda 0976 6172 6961 626c 6573  doc__..variables
-00000620: 7202 0000 0072 0400 0000 da30 6269 6f74  r....r.....0biot
-00000630: 6563 682e 746f 7069 6373 2e70 726f 6365  ech.topics.proce
-00000640: 7373 5f6f 6e2e 705f 6578 7065 6374 2e70  ss_on.p_expect.p
-00000650: 6172 7365 5f72 6563 6f72 6473 7206 0000  arse_recordsr...
-00000660: 00da 1c62 696f 7465 6368 2e74 6f70 6963  ...biotech.topic
-00000670: 732e 7368 6f77 2e76 6172 6961 626c 6572  s.show.variabler
-00000680: 0700 0000 da04 7269 6368 721c 0000 0072  ......richr....r
-00000690: 2600 0000 7224 0000 0072 2400 0000 7224  &...r$...r$...r$
-000006a0: 0000 0072 2500 0000 da08 3c6d 6f64 756c  ...r%.....<modul
-000006b0: 653e 0100 0000 7314 0000 0004 0202 0702  e>....s.........
-000006c0: 050c 080c 010c 020c 0108 0308 030c 04    ...............
+00000150: 6403 7c01 9b00 6404 9d03 6405 6406 8d02  d.|...d...d.d...
+00000160: 0100 7401 6407 1900 7c01 1900 6408 1900  ..t.d...|...d...
+00000170: 6408 1900 a002 a100 0100 7403 7404 a004  d.........t.t...
+00000180: a100 8301 7401 6407 1900 7c01 1900 6409  ....t.d...|...d.
+00000190: 1900 640a 3c00 7405 7401 6407 1900 7c01  ..d.<.t.t.d...|.
+000001a0: 1900 6409 1900 640a 1900 8301 7405 7401  ..d...d.....t.t.
+000001b0: 6407 1900 7c01 1900 6409 1900 640b 1900  d...|...d...d...
+000001c0: 8301 1800 7401 6407 1900 7c01 1900 6409  ....t.d...|...d.
+000001d0: 1900 640c 3c00 640d 7401 6407 1900 7c01  ..d.<.d.t.d...|.
+000001e0: 1900 640e 1900 640f 3c00 7a17 7406 7401  ..d...d.<.z.t.t.
+000001f0: 6407 1900 7c01 1900 6408 1900 6410 1900  d...|...d...d...
+00000200: 8300 6411 6412 8d02 7401 6407 1900 7c01  ..d.d...t.d...|.
+00000210: 1900 6410 3c00 5700 6e0d 0400 7407 797a  ..d.<.W.n...t.yz
+00000220: 0100 0100 0100 7400 6413 8301 0100 5900  ......t.d.....Y.
+00000230: 6e01 7700 0900 7a53 6401 7c01 6901 7d03  n.w...zSd.|.i.}.
+00000240: 7a0c 7401 6407 1900 7c01 1900 6410 1900  z.t.d...|...d...
+00000250: 7c03 6410 3c00 5700 6e0d 0400 7407 799a  |.d.<.W.n...t.y.
+00000260: 0100 0100 0100 7400 6414 8301 0100 5900  ......t.d.....Y.
+00000270: 6e01 7700 7a0d 7c02 4400 5d08 7d04 7c02  n.w.z.|.D.].}.|.
+00000280: 7c04 1900 7c03 7c04 3c00 719e 5700 6e0d  |...|.|.<.q.W.n.
+00000290: 0400 7407 79b5 0100 0100 0100 7400 6415  ..t.y.......t.d.
+000002a0: 8301 0100 5900 6e01 7700 7a0a 7c03 7401  ....Y.n.w.z.|.t.
+000002b0: 6407 1900 7c01 1900 6416 3c00 5700 6e0d  d...|...d.<.W.n.
+000002c0: 0400 7407 79cd 0100 0100 0100 7400 6417  ..t.y.......t.d.
+000002d0: 8301 0100 5900 6e01 7700 5700 6e0d 0400  ....Y.n.w.W.n...
+000002e0: 7407 79dc 0100 0100 0100 7400 6418 8301  t.y.......t.d...
+000002f0: 0100 5900 6e01 7700 640d 7401 6407 1900  ..Y.n.w.d.t.d...
+00000300: 7c01 1900 640e 1900 6419 3c00 7403 7404  |...d...d.<.t.t.
+00000310: a004 a100 8301 7401 6407 1900 7c01 1900  ......t.d...|...
+00000320: 6409 1900 641a 3c00 7404 a008 641b a101  d...d.<.t...d...
+00000330: 0100 0900 641c 7401 6407 1900 7c01 1900  ....d.t.d...|...
+00000340: 641d 1900 6408 3c00 6400 5300 291e 4eda  d...d.<.d.S.).N.
+00000350: 0470 6174 68da 0672 6573 756c 747a 0a54  .path..resultz.T
+00000360: 6865 2073 6361 6e20 227a 1722 2073 656e  he scan "z." sen
+00000370: 7420 2f64 6f6e 655f 7769 7468 5f73 6361  t /done_with_sca
+00000380: 6e2e da09 636f 6e64 656e 7365 6429 01da  n...condensed)..
+00000390: 046d 6f64 65da 1169 6e74 6572 6e61 6c5f  .mode..internal_
+000003a0: 7374 6174 7573 6573 da07 7072 6f63 6573  statuses..proces
+000003b0: 73da 0574 696d 6573 da05 656e 6465 64da  s..times..ended.
+000003c0: 0773 7461 7274 6564 da07 656c 6170 7365  .started..elapse
+000003d0: 64da 0379 6573 da0b 6f63 6375 7272 656e  d..yes..occurren
+000003e0: 6365 737a 1873 6361 6e20 7072 6f63 6573  cesz.scan proces
+000003f0: 7320 7761 7320 7374 6f70 7065 64da 0772  s was stopped..r
+00000400: 6563 6f72 6473 da04 5554 4638 2902 7214  ecords..UTF8).r.
+00000410: 0000 00da 0666 6f72 6d61 747a 2054 6865  .....formatz The
+00000420: 2072 6563 6f72 6473 2063 6f75 6c64 206e   records could n
+00000430: 6f74 2062 6520 7061 7273 6564 217a 3554  ot be parsed!z5T
+00000440: 6865 2072 6563 6f72 6473 2063 6f75 6c64  he records could
+00000450: 206e 6f74 2062 6520 6164 6465 6420 746f   not be added to
+00000460: 2074 6865 2072 6573 756c 7473 2070 6163   the results pac
+00000470: 6b65 7421 7a2b 4120 7265 7375 6c74 2069  ket!z+A result i
+00000480: 6e20 7468 6520 7265 7375 6c74 7320 636f  n the results co
+00000490: 756c 6420 6e6f 7420 6265 2061 6464 6564  uld not be added
+000004a0: 21da 0f72 6573 756c 7473 5f6f 665f 7363  !..results_of_sc
+000004b0: 616e 7a26 5468 6520 7265 7375 6c74 7320  anz&The results 
+000004c0: 7061 636b 6574 2063 6f75 6c64 206e 6f74  packet could not
+000004d0: 2062 6520 6164 6465 642e 7a31 416e 2065   be added.z1An e
+000004e0: 7863 6570 7469 6f6e 206f 6363 7572 7265  xception occurre
+000004f0: 6420 7768 696c 6520 6275 696c 6469 6e67  d while building
+00000500: 2074 6865 2072 6573 756c 7473 2e7a 1b73   the results.z.s
+00000510: 6361 6e20 7265 636f 7264 7320 7765 7265  can records were
+00000520: 2072 6574 7269 6576 6564 7a11 7265 636f   retrievedz.reco
+00000530: 7264 7320 7265 7472 6965 7661 6c72 0300  rds retrievalr..
+00000540: 0000 da04 646f 6e65 da06 7374 6174 7573  ....done..status
+00000550: 2909 7207 0000 0072 0200 0000 da09 7465  ).r....r......te
+00000560: 726d 696e 6174 65da 0373 7472 da04 7469  rminate..str..ti
+00000570: 6d65 da05 666c 6f61 7472 0600 0000 da09  me..floatr......
+00000580: 4578 6365 7074 696f 6eda 0573 6c65 6570  Exception..sleep
+00000590: 2905 da0a 7468 655f 7061 636b 6574 da08  )...the_packet..
+000005a0: 7468 655f 7061 7468 da0a 7468 655f 7265  the_path..the_re
+000005b0: 7375 6c74 da12 7468 655f 7265 7375 6c74  sult..the_result
+000005c0: 735f 7061 636b 6574 7209 0000 00a9 0072  s_packetr......r
+000005d0: 2400 0000 fa5e 2f62 696f 7465 6368 2f76  $....^/biotech/v
+000005e0: 656e 7565 732f 7374 6167 6573 2f62 696f  enues/stages/bio
+000005f0: 7465 6368 2f70 726f 6365 6475 7265 732f  tech/procedures/
+00000600: 6167 6772 6567 6174 6f72 5f70 726f 6365  aggregator_proce
+00000610: 6475 7265 2f70 726f 6365 7373 2f6d 6f76  dure/process/mov
+00000620: 6573 2f64 6f6e 655f 7769 7468 5f73 6361  es/done_with_sca
+00000630: 6e2e 7079 da13 646f 6e65 5f77 6974 685f  n.py..done_with_
+00000640: 7363 616e 5f6d 6f76 6525 0000 0073 6000  scan_move%...s`.
+00000650: 0000 0801 0801 1404 1808 1c01 1602 1601  ................
+00000660: 02ff 12ff 1404 0209 0201 1401 0201 16fe  ................
+00000670: 0c04 0c01 02ff 0205 0203 0402 04ff 0204  ................
+00000680: 1801 0c01 0c01 02ff 0203 0801 0e01 04ff  ................
+00000690: 0c02 0c01 02ff 0203 1401 0c01 0c01 02ff  ................
+000006a0: 0480 0c03 0c01 02ff 1405 1c01 0a02 0202  ................
+000006b0: 1803 7226 0000 0029 0bda 075f 5f64 6f63  ..r&...)...__doc
+000006c0: 5f5f da09 7661 7269 6162 6c65 7372 0200  __..variablesr..
+000006d0: 0000 7204 0000 00da 3062 696f 7465 6368  ..r.....0biotech
+000006e0: 2e74 6f70 6963 732e 7072 6f63 6573 735f  .topics.process_
+000006f0: 6f6e 2e70 5f65 7870 6563 742e 7061 7273  on.p_expect.pars
+00000700: 655f 7265 636f 7264 7372 0600 0000 da1c  e_recordsr......
+00000710: 6269 6f74 6563 682e 746f 7069 6373 2e73  biotech.topics.s
+00000720: 686f 772e 7661 7269 6162 6c65 7207 0000  how.variabler...
+00000730: 00da 0472 6963 6872 1c00 0000 7226 0000  ...richr....r&..
+00000740: 0072 2400 0000 7224 0000 0072 2400 0000  .r$...r$...r$...
+00000750: 7225 0000 00da 083c 6d6f 6475 6c65 3e01  r%.....<module>.
+00000760: 0000 0073 1400 0000 0402 0207 0205 0c08  ...s............
+00000770: 0c01 0c02 0c01 0803 0803 0c04            ............
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 17 23:09:07 2024 UTC, .py size: 566 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,46 @@
-00000000: 6f0d 0d0a 0000 0000 9356 2066 3602 0000  o........V f6...
+00000000: 6f0d 0d0a 0000 0000 14db 2266 0202 0000  o........."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 5a00 0900 6401 6402 6c01 6d02 5a02 0100  Z...d.d.l.m.Z...
 00000040: 6401 6403 6c03 5a03 6401 6403 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6404 6405 6406 6900 6604 6407 6408 8401  d.d.d.i.f.d.d...
 00000060: 5a05 6403 5300 2909 7a34 0a09 6672 6f6d  Z.d.S.).z4..from
 00000070: 206b 6567 2e73 656e 642e 646f 6e65 2069   keg.send.done i
 00000080: 6d70 6f72 7420 7365 6e64 5f64 6f6e 650a  mport send_done.
 00000090: 0973 656e 645f 646f 6e65 2028 290a e900  .send_done ()...
 000000a0: 0000 0029 01da 0d73 686f 775f 7661 7269  ...)...show_vari
 000000b0: 6162 6c65 4e7a 0730 2e30 2e30 2e30 7a05  ableNz.0.0.0.0z.
 000000c0: 2f64 6f6e 65da 0063 0400 0000 0000 0000  /done..c........
 000000d0: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
-000000e0: 734e 0000 0064 017c 009b 0064 027c 029b  sN...d.|...d.|..
-000000f0: 007c 019b 009d 057d 0474 0064 037c 047c  .|.....}.t.d.|.|
-00000100: 0364 049c 0269 0183 0101 0074 016a 027c  .d...i.....t.j.|
-00000110: 047c 0364 058d 027d 0574 0064 067c 056a  .|.d...}.t.d.|.j
-00000120: 037c 056a 0464 079c 0269 0183 0101 0064  .|.j.d...i.....d
-00000130: 0053 0029 084e 7a07 6874 7470 3a2f 2ffa  .S.).Nz.http://.
-00000140: 013a 7a0c 7365 6e64 696e 6720 646f 6e65  .:z.sending done
-00000150: 2902 da03 5552 4cda 0870 726f 6365 6564  )...URL..proceed
-00000160: 7329 01da 046a 736f 6e7a 0e2f 646f 6e65  s)...jsonz./done
-00000170: 2072 6573 706f 6e73 6529 02da 0b73 7461   response)...sta
-00000180: 7475 735f 636f 6465 da04 7465 7874 2905  tus_code..text).
-00000190: 7202 0000 00da 0872 6571 7565 7374 73da  r......requests.
-000001a0: 0570 6174 6368 7208 0000 0072 0900 0000  .patchr....r....
-000001b0: 2906 da04 686f 7374 da08 5552 4c5f 7061  )...host..URL_pa
-000001c0: 7468 da04 706f 7274 7206 0000 0072 0500  th..portr....r..
-000001d0: 0000 da08 7265 7370 6f6e 7365 a900 7210  ....response..r.
-000001e0: 0000 00fa 572f 6269 6f74 6563 682f 7665  ....W/biotech/ve
+000000e0: 7348 0000 0064 017c 009b 0064 027c 029b  sH...d.|...d.|..
+000000f0: 007c 019b 009d 057d 0474 0064 0364 0464  .|.....}.t.d.d.d
+00000100: 058d 0201 0074 016a 027c 047c 0364 068d  .....t.j.|.|.d..
+00000110: 027d 0574 0064 077c 056a 039b 0064 089d  .}.t.d.|.j...d..
+00000120: 0364 0464 058d 0201 0064 0053 0029 094e  .d.d.....d.S.).N
+00000130: 7a07 6874 7470 3a2f 2ffa 013a 7a0d 7365  z.http://..:z.se
+00000140: 6e64 696e 6720 2f64 6f6e 65da 0963 6f6e  nding /done..con
+00000150: 6465 6e73 6564 2901 da04 6d6f 6465 2901  densed)...mode).
+00000160: da04 6a73 6f6e 7a22 7365 6e64 696e 6720  ..jsonz"sending 
+00000170: 2f64 6f6e 6520 7265 6365 6976 6564 2072  /done received r
+00000180: 6573 706f 6e73 653a 2027 fa01 2729 0472  esponse: '..').r
+00000190: 0200 0000 da08 7265 7175 6573 7473 da05  ......requests..
+000001a0: 7061 7463 68da 0474 6578 7429 06da 0468  patch..text)...h
+000001b0: 6f73 74da 0855 524c 5f70 6174 68da 0470  ost..URL_path..p
+000001c0: 6f72 74da 0870 726f 6365 6564 73da 0355  ort..proceeds..U
+000001d0: 524c da08 7265 7370 6f6e 7365 a900 7212  RL..response..r.
+000001e0: 0000 00fa 592f 6269 6f74 6563 682f 7665  ....Y/biotech/ve
 000001f0: 6e75 6573 2f73 7461 6765 732f 6269 6f74  nues/stages/biot
-00000200: 6563 682f 7072 6f63 6564 7572 6573 2f69  ech/procedures/i
-00000210: 6d70 6c69 6369 745f 7072 6f63 6564 7572  mplicit_procedur
-00000220: 652f 7072 6f63 6573 732f 6d6f 7665 732f  e/process/moves/
-00000230: 7365 6e64 5f64 6f6e 652e 7079 da09 7365  send_done.py..se
-00000240: 6e64 5f64 6f6e 6515 0000 0073 1c00 0000  nd_done....s....
-00000250: 1407 0202 0201 0201 0201 04fe 06ff 0e07  ................
-00000260: 0202 0201 0401 0401 04fe 0aff 7212 0000  ............r...
-00000270: 0029 06da 075f 5f64 6f63 5f5f da1c 6269  .)...__doc__..bi
-00000280: 6f74 6563 682e 746f 7069 6373 2e73 686f  otech.topics.sho
-00000290: 772e 7661 7269 6162 6c65 7202 0000 00da  w.variabler.....
-000002a0: 0472 6963 6872 0a00 0000 7212 0000 0072  .richr....r....r
-000002b0: 1000 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
-000002c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000002d0: 0073 1400 0000 0400 0205 0c06 0803 0803  .s..............
-000002e0: 0204 0201 0201 0202 0efb                 ..........
+00000200: 6563 682f 7072 6f63 6564 7572 6573 2f61  ech/procedures/a
+00000210: 6767 7265 6761 746f 725f 7072 6f63 6564  ggregator_proced
+00000220: 7572 652f 7072 6f63 6573 732f 6d6f 7665  ure/process/move
+00000230: 732f 7365 6e64 5f64 6f6e 652e 7079 da09  s/send_done.py..
+00000240: 7365 6e64 5f64 6f6e 6515 0000 0073 0800  send_done....s..
+00000250: 0000 1407 0c02 0e02 1a02 7214 0000 0029  ..........r....)
+00000260: 06da 075f 5f64 6f63 5f5f da1c 6269 6f74  ...__doc__..biot
+00000270: 6563 682e 746f 7069 6373 2e73 686f 772e  ech.topics.show.
+00000280: 7661 7269 6162 6c65 7202 0000 00da 0472  variabler......r
+00000290: 6963 6872 0900 0000 7214 0000 0072 1200  ichr....r....r..
+000002a0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+000002b0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000002c0: 1400 0000 0400 0205 0c06 0803 0803 0204  ................
+000002d0: 0201 0201 0202 0efb                      ........
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,17 +36,15 @@
 
 def done_with_scan_move (the_packet):
 	the_path = the_packet ["path"]
 	the_result = the_packet ["result"]
 	#the_pid = the_packet ["pid"]
 	
 	
-	show_variable ({
-		"done with scan, stopping:": the_packet
-	}, mode = "condensed")
+	show_variable (f'The scan "{ the_path }" sent /done_with_scan.', mode = "condensed")
 
 
 	#---
 	#
 	#	Once the status of the scan has been established,
 	# 	then the scan process can be stopped.
 	#
@@ -59,50 +57,57 @@
 	aggregator_variables ["internal_statuses"] [ the_path ] ["occurrences"] ["scan process was stopped"] = "yes"
 	
 	#print ('turning off scan process with pid:', the_pid)
 	#os.kill (the_pid, 9)
 	#
 	#----
 	
-	show_variable ({
-		"times": aggregator_variables ["internal_statuses"] [ the_path ] ["times"]
-	}, mode = "show")
-	
+
 	
 	try:
 		aggregator_variables ["internal_statuses"] [ the_path ] ["records"] = parse_p_expect_records (
 			records = aggregator_variables ["internal_statuses"] [ the_path ] ["process"] ["records"] (),
 			format = "UTF8"
 		)
 	except Exception:
 		show_variable ("The records could not be parsed!")
 	
-	the_results_packet = {
-		"path": the_path
-	}
 	
-	try:
-		the_results_packet ["records"] = aggregator_variables ["internal_statuses"] [ the_path ] ["records"]
-	except Exception:
-		show_variable ("The records could not be added to the results packet!")
 	
+	'''
+		This sets the results packet
+	'''
 	try:
-		for result in the_result:
-			the_results_packet [ result ] = the_result [ result ]
+		the_results_packet = {
+			"path": the_path
+		}
+	
+		try:
+			the_results_packet ["records"] = aggregator_variables ["internal_statuses"] [ the_path ] ["records"]
+		except Exception:
+			show_variable ("The records could not be added to the results packet!")
+		
+		try:
+			for result in the_result:
+				the_results_packet [ result ] = the_result [ result ]
+		except Exception:
+			show_variable ("A result in the results could not be added!")
+			
+		try:
+			aggregator_variables ["internal_statuses"] [ the_path ] ["results_of_scan"] = the_results_packet	
+		except Exception:
+			show_variable ("The results packet could not be added.")
+			
 	except Exception:
-		show_variable ("A result in the results could not be added!")
+		show_variable ("An exception occurred while building the results.")
 	
-	aggregator_variables ["internal_statuses"] [ the_path ] ["results_of_scan"] = the_results_packet
-	
-	aggregator_variables ["internal_statuses"] [ the_path ] ["occurrences"] ["scan records were retrieved"] = "yes"
-	
-	
-	show_variable ("done with scan")
 	
 	
+	aggregator_variables ["internal_statuses"] [ the_path ] ["occurrences"] ["scan records were retrieved"] = "yes"
+	aggregator_variables ["internal_statuses"] [ the_path ] ["times"] ["records retrieval"] = str (time.time ());
 	
 	time.sleep (1)
 	
 	'''
 		This is only variable that is waited on.
 	'''
 	aggregator_variables ["internal_statuses"] [ the_path ] ["status"] ["process"] = "done"
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 20:36:06 2024 UTC, .py size: 9002 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b6d5 2266 2a23 0000  o........."f*#..
+00000000: 6f0d 0d0a 0000 0000 3cf3 2266 2f23 0000  o.......<."f/#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6405 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6400 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6408 6c0b 5a0b 6400  m.Z...d.d.l.Z.d.
@@ -77,50 +77,50 @@
 000004c0: 067d 0c7c 0864 0e19 0064 086b 0290 0272  .}.|.d...d.k...r
 000004d0: 397c 0864 0919 0064 086b 0290 0272 397c  9|.d...d.k...r9|
 000004e0: 0864 2019 0064 0a6b 0290 0272 3974 0d7c  .d ..d.k...r9t.|
 000004f0: 027c 0619 0064 1019 0064 1119 0083 0164  .|...d...d.....d
 00000500: 216b 0590 0272 3974 0d7c 027c 0619 0064  !k...r9t.|.|...d
 00000510: 2219 0083 0164 236b 0290 0272 3974 07a0  "....d#k...r9t..
 00000520: 07a1 0074 087c 027c 0619 0064 1019 0064  ...t.|.|...d...d
-00000530: 1119 0083 0118 007d 0b7c 0b64 1e6b 0590  .......}.|.d.k..
-00000540: 0272 3974 0a64 257c 0669 0183 0101 007a  .r9t.d%|.i.....z
+00000530: 1119 0083 0118 007d 0b7c 0b64 256b 0590  .......}.|.d%k..
+00000540: 0272 3974 0a64 267c 0669 0183 0101 007a  .r9t.d&|.i.....z
 00000550: 087c 027c 0619 0064 1319 007d 0857 006e  .|.|...d...}.W.n
 00000560: 0c04 0074 0390 0279 1401 0001 0001 0064  ...t...y.......d
-00000570: 147d 0859 006e 0177 007c 0664 2667 007c  .}.Y.n.w.|.d&g.|
-00000580: 0864 0764 279c 057c 0064 0219 007c 0619  .d.d'..|.d...|..
+00000570: 147d 0859 006e 0177 007c 0664 2767 007c  .}.Y.n.w.|.d'g.|
+00000580: 0864 0764 289c 057c 0064 0219 007c 0619  .d.d(..|.d...|..
 00000590: 0064 173c 0064 187c 0064 0219 007c 0619  .d.<.d.|.d...|..
 000005a0: 0064 1919 0064 063c 007c 0064 0219 007c  .d...d.<.|.d...|
 000005b0: 0619 0064 0619 0064 0619 00a0 09a1 0001  ...d...d........
 000005c0: 0057 006e 1804 0074 0390 0279 5201 007d  .W.n...t...yR..}
-000005d0: 0a01 007a 0b74 0464 287c 0a83 0201 0057  ...z.t.d(|.....W
+000005d0: 0a01 007a 0b74 0464 297c 0a83 0201 0057  ...z.t.d)|.....W
 000005e0: 0059 0064 007d 0a7e 0a6e 0564 007d 0a7e  .Y.d.}.~.n.d.}.~
 000005f0: 0a77 0177 0009 007a 367c 0864 0e19 0064  .w.w...z6|.d...d
 00000600: 086b 0290 0272 897c 0864 0f19 0064 086b  .k...r.|.d...d.k
 00000610: 0290 0272 897c 0864 2019 0064 0a6b 0290  ...r.|.d ..d.k..
 00000620: 0272 897c 0864 0919 0064 086b 0390 0272  .r.|.d...d.k...r
-00000630: 897c 0664 2967 007c 0864 0764 169c 057c  .|.d)g.|.d.d...|
+00000630: 897c 0664 2a67 007c 0864 0764 169c 057c  .|.d*g.|.d.d...|
 00000640: 0064 0219 007c 0619 0064 173c 0064 187c  .d...|...d.<.d.|
 00000650: 0064 0219 007c 0619 0064 1919 0064 063c  .d...|...d...d.<
 00000660: 0057 006e 1a04 0074 0390 0279 a401 007d  .W.n...t...y...}
-00000670: 0a01 007a 0d74 0464 2a74 0ba0 0ca1 0083  ...z.t.d*t......
+00000670: 0a01 007a 0d74 0464 2b74 0ba0 0ca1 0083  ...z.t.d+t......
 00000680: 0201 0057 0059 0064 007d 0a7e 0a6e 0564  ...W.Y.d.}.~.n.d
 00000690: 007d 0a7e 0a77 0177 0009 0009 007a 287c  .}.~.w.w.....z(|
 000006a0: 0864 0919 0064 0a6b 0290 0272 ce7c 0864  .d...d.k...r.|.d
 000006b0: 0e19 0064 086b 0290 0272 ce7c 0864 2019  ...d.k...r.|.d .
-000006c0: 0064 086b 0290 0272 ce7c 0864 2b19 0064  .d.k...r.|.d+..d
+000006c0: 0064 086b 0290 0272 ce7c 0864 2c19 0064  .d.k...r.|.d,..d
 000006d0: 086b 0290 0272 ce64 187c 0064 0219 007c  .k...r.d.|.d...|
 000006e0: 0619 0064 1919 0064 063c 0057 0071 1704  ...d...d.<.W.q..
 000006f0: 0074 0390 0279 e901 007d 0a01 007a 0d74  .t...y...}...z.t
-00000700: 0464 2a74 0ba0 0ca1 0083 0201 0057 0059  .d*t.........W.Y
+00000700: 0464 2b74 0ba0 0ca1 0083 0201 0057 0059  .d+t.........W.Y
 00000710: 0064 007d 0a7e 0a71 1764 007d 0a7e 0a77  .d.}.~.q.d.}.~.w
 00000720: 0177 007c 0244 005d 1a7d 067c 027c 0619  .w.|.D.].}.|.|..
 00000730: 0064 1919 0064 0619 0064 186b 0390 0372  .d...d...d.k...r
 00000740: 057c 05a0 0e7c 067c 0064 0219 007c 0619  .|...|.|.d...|..
-00000750: 0064 2c9c 02a1 0101 0090 0271 ec7c 0553  .d,........q.|.S
-00000760: 0029 2d4e da0d 7265 636f 7264 735f 6c65  .)-N..records_le
+00000750: 0064 2d9c 02a1 0101 0090 0271 ec7c 0553  .d-........q.|.S
+00000760: 0029 2e4e da0d 7265 636f 7264 735f 6c65  .).N..records_le
 00000770: 7665 6cda 1169 6e74 6572 6e61 6c5f 7374  vel..internal_st
 00000780: 6174 7573 6573 da0f 696e 7472 6f5f 7661  atuses..intro_va
 00000790: 7269 6162 6c65 73da 0a74 696d 655f 6c69  riables..time_li
 000007a0: 6d69 74da 0b6f 6363 7572 7265 6e63 6573  mit..occurrences
 000007b0: da07 7072 6f63 6573 7354 da03 7965 737a  ..processT..yesz
 000007c0: 1573 6361 6e20 7072 6f63 6573 7320 6973  .scan process is
 000007d0: 2061 6c69 7665 da02 6e6f 7a1e 7072 6f63   alive..noz.proc
@@ -150,100 +150,101 @@
 00000950: 2774 206e 6f74 6966 7920 7468 6520 6167  't notify the ag
 00000960: 6772 6567 6174 6f72 2077 6974 6869 6e20  gregator within 
 00000970: 3520 7365 636f 6e64 732e 7a10 646f 6e65  5 seconds.z.done
 00000980: 2072 6561 736f 6e20 6769 7665 7a18 7072   reason givez.pr
 00000990: 6f63 6573 7320 6d61 7920 6861 7665 2073  ocess may have s
 000009a0: 746f 7070 6564 7a23 7072 6f63 6573 7320  toppedz#process 
 000009b0: 6e6f 6e2d 6e6f 7469 6669 6361 7469 6f6e  non-notification
-000009c0: 2065 7863 6570 7469 6f6e 3ae9 0a00 0000   exception:.....
-000009d0: 7a50 4166 7465 7220 3130 2073 6563 6f6e  zPAfter 10 secon
+000009c0: 2065 7863 6570 7469 6f6e 3ae9 1400 0000   exception:.....
+000009d0: 7a50 4166 7465 7220 3230 2073 6563 6f6e  zPAfter 20 secon
 000009e0: 6473 2c20 7468 6520 7072 6f63 6573 7320  ds, the process 
 000009f0: 6469 6420 6e6f 7420 6e6f 7469 6679 2074  did not notify t
 00000a00: 6865 2061 6767 7265 6761 746f 7220 7468  he aggregator th
 00000a10: 6174 2069 7420 6861 6420 7374 6172 7465  at it had starte
 00000a20: 642e 7a18 7363 616e 2070 726f 6365 7373  d.z.scan process
 00000a30: 2077 6173 2073 746f 7070 6564 7203 0000   was stoppedr...
 00000a40: 00da 0772 6563 6f72 6473 7201 0000 0029  ...recordsr....)
 00000a50: 06da 0131 da01 32da 0133 da01 34da 0136  ...1..2..3..4..6
-00000a60: da01 377a 2b72 6563 6f72 6473 2077 6572  ..7z+records wer
-00000a70: 6520 6e6f 7420 7265 7472 6965 7665 6420  e not retrieved 
-00000a80: 6166 7465 7220 3130 2073 6563 6f6e 6473  after 10 seconds
-00000a90: 7a2d 4166 7465 7220 3130 2073 6563 6f6e  z-After 10 secon
-00000aa0: 6473 2c20 6e6f 2070 726f 6365 7373 206c  ds, no process l
-00000ab0: 6f67 7320 7765 7265 2066 6f75 6e64 2e29  ogs were found.)
-00000ac0: 0572 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000ad0: 7214 0000 0072 1800 0000 7a28 7072 6f63  r....r....z(proc
-00000ae0: 6573 7320 6c6f 6773 2074 696d 6520 6c69  ess logs time li
-00000af0: 6d69 7420 6368 6563 6b20 6578 6365 7074  mit check except
-00000b00: 696f 6e3a 7a30 5468 6520 7072 6f63 6573  ion:z0The proces
-00000b10: 7320 6578 6974 6564 2062 6566 6f72 6520  s exited before 
-00000b20: 7265 7375 6c74 7320 636f 756c 6420 6265  results could be
-00000b30: 2073 656e 742e 7a1a 7061 7273 6520 616e   sent.z.parse an
-00000b40: 6420 6368 6563 6b20 6578 6365 7074 696f  d check exceptio
-00000b50: 6e3a 7a1b 7363 616e 2072 6563 6f72 6473  n:z.scan records
-00000b60: 2077 6572 6520 7265 7472 6965 7665 6429   were retrieved)
-00000b70: 0272 1500 0000 da09 696e 7465 726e 616c  .r......internal
-00000b80: 7329 0f72 0200 0000 da04 7479 7065 da08  s).r......type..
-00000b90: 6973 5f61 6c69 7665 da09 4578 6365 7074  is_alive..Except
-00000ba0: 696f 6eda 0570 7269 6e74 7204 0000 0072  ion..printr....r
-00000bb0: 0500 0000 da04 7469 6d65 da05 666c 6f61  ......time..floa
-00000bc0: 74da 0974 6572 6d69 6e61 7465 7207 0000  t..terminater...
-00000bd0: 00da 0974 7261 6365 6261 636b da0a 666f  ...traceback..fo
-00000be0: 726d 6174 5f65 7863 da03 6c65 6eda 0661  rmat_exc..len..a
-00000bf0: 7070 656e 6429 0dda 1461 6767 7265 6761  ppend)...aggrega
-00000c00: 746f 725f 7661 7269 6162 6c65 7372 0900  tor_variablesr..
-00000c10: 0000 720a 0000 0072 0c00 0000 da08 7374  ..r....r......st
-00000c20: 6174 7573 6573 da0a 756e 6669 6e69 7368  atuses..unfinish
-00000c30: 6564 da0b 7374 6174 7573 5f70 6174 68da  ed..status_path.
-00000c40: 0e73 7461 7475 735f 6f66 5f70 6174 6872  .status_of_pathr
-00000c50: 0d00 0000 da05 616c 6976 65da 0145 da07  ......alive..E..
-00000c60: 656c 6170 7365 64da 0564 6f6f 7273 a900  elapsed..doors..
-00000c70: 7239 0000 00fa 712f 6269 6f74 6563 682f  r9....q/biotech/
-00000c80: 7665 6e75 6573 2f73 7461 6765 732f 6269  venues/stages/bi
-00000c90: 6f74 6563 682f 7072 6f63 6564 7572 6573  otech/procedures
-00000ca0: 2f61 6767 7265 6761 746f 725f 7072 6f63  /aggregator_proc
-00000cb0: 6564 7572 652f 7072 6f63 6573 732f 6d6f  edure/process/mo
-00000cc0: 7665 732f 7374 6174 7573 5f63 6865 636b  ves/status_check
-00000cd0: 5f6d 6f6e 6974 6f72 2f74 6865 5f70 6879  _monitor/the_phy
-00000ce0: 7369 6361 6c2e 7079 da24 7061 7273 655f  sical.py.$parse_
-00000cf0: 616e 645f 6368 6563 6b5f 6973 5f61 6c69  and_check_is_ali
-00000d00: 7665 5f6f 665f 7374 6174 7573 6573 2100  ve_of_statuses!.
-00000d10: 0000 7346 0100 0006 0108 0208 010c 0104  ..sF............
-00000d20: 0204 010a 0108 0208 0102 0202 0410 0118  ................
-00000d30: 0114 0108 010a 0108 0204 800e 020a 0114  ................
-00000d40: 0108 8002 fe08 0508 0302 0502 0d0c 020c  ................
-00000d50: 010c 011c 0208 0202 0110 010c 0108 0102  ................
-00000d60: ff02 0402 0202 0102 0202 0212 f814 0b14  ................
-00000d70: 0118 0202 0204 0106 ff04 800e 030e 010c  ................
-00000d80: 0108 8002 fe02 0502 080e 020e 011c 020a  ................
-00000d90: 0202 0110 010e 0108 0102 ff02 0402 0202  ................
-00000da0: 0102 0202 0212 f814 0b14 0118 0102 0204  ................
-00000db0: 0106 ff04 8010 030e 010c 0108 8002 fe02  ................
-00000dc0: 0502 120a 020a 010a 0116 0112 011a 0106  ................
-00000dd0: fa0e 0b0e 010e 011a 0116 021c 020a 0202  ................
-00000de0: 0104 0106 ff02 0410 010e 0108 0102 ff02  ................
-00000df0: 0402 0202 0102 0202 0212 f814 0b18 0104  ................
-00000e00: 8010 040a 010c 0108 8002 fe02 0602 0c0e  ................
-00000e10: 020e 010e 020e 0202 0302 0202 0102 0102  ................
-00000e20: 0212 f914 0a04 8010 020e 010c 0108 8002  ................
-00000e30: fe02 0502 0802 030e 020e 020e 010e 0114  ................
-00000e40: 0204 8010 020e 010c 0108 8002 fe08 0616  ................
-00000e50: 0104 0102 010a 0108 fe04 8004 0672 3b00  .............r;.
-00000e60: 0000 290f da39 6269 6f74 6563 682e 7072  ..)..9biotech.pr
-00000e70: 6f63 6564 7572 6573 2e61 6767 7265 6761  ocedures.aggrega
-00000e80: 746f 725f 7072 6f63 6564 7572 652e 7072  tor_procedure.pr
-00000e90: 6f63 6573 732e 7661 7269 6162 6c65 7372  ocess.variablesr
-00000ea0: 0200 0000 721d 0000 0072 0400 0000 da27  ....r....r.....'
-00000eb0: 616c 6172 6d5f 6368 6563 6b73 2e67 6c6f  alarm_checks.glo
-00000ec0: 6261 6c5f 7469 6d65 5f6c 696d 6974 5f65  bal_time_limit_e
-00000ed0: 7863 6565 6465 6472 0500 0000 da30 6269  xceededr.....0bi
-00000ee0: 6f74 6563 682e 746f 7069 6373 2e70 726f  otech.topics.pro
-00000ef0: 6365 7373 5f6f 6e2e 705f 6578 7065 6374  cess_on.p_expect
-00000f00: 2e70 6172 7365 5f72 6563 6f72 6473 7206  .parse_recordsr.
-00000f10: 0000 00da 1c62 696f 7465 6368 2e74 6f70  .....biotech.top
-00000f20: 6963 732e 7368 6f77 2e76 6172 6961 626c  ics.show.variabl
-00000f30: 6572 0700 0000 7208 0000 0072 2900 0000  er....r....r)...
-00000f40: 722c 0000 00da 0472 6963 6872 3b00 0000  r,.....richr;...
-00000f50: 7239 0000 0072 3900 0000 7239 0000 0072  r9...r9...r9...r
-00000f60: 3a00 0000 da08 3c6d 6f64 756c 653e 0100  :.....<module>..
-00000f70: 0000 7316 0000 000c 070c 030c 020c 020c  ..s.............
-00000f80: 010c 0308 0108 0108 0302 050c 04         .............
+00000a60: da01 37e9 0a00 0000 7a2b 7265 636f 7264  ..7.....z+record
+00000a70: 7320 7765 7265 206e 6f74 2072 6574 7269  s were not retri
+00000a80: 6576 6564 2061 6674 6572 2031 3020 7365  eved after 10 se
+00000a90: 636f 6e64 737a 2d41 6674 6572 2031 3020  condsz-After 10 
+00000aa0: 7365 636f 6e64 732c 206e 6f20 7072 6f63  seconds, no proc
+00000ab0: 6573 7320 6c6f 6773 2077 6572 6520 666f  ess logs were fo
+00000ac0: 756e 642e 2905 7215 0000 0072 1600 0000  und.).r....r....
+00000ad0: 7217 0000 0072 1400 0000 7218 0000 007a  r....r....r....z
+00000ae0: 2870 726f 6365 7373 206c 6f67 7320 7469  (process logs ti
+00000af0: 6d65 206c 696d 6974 2063 6865 636b 2065  me limit check e
+00000b00: 7863 6570 7469 6f6e 3a7a 3054 6865 2070  xception:z0The p
+00000b10: 726f 6365 7373 2065 7869 7465 6420 6265  rocess exited be
+00000b20: 666f 7265 2072 6573 756c 7473 2063 6f75  fore results cou
+00000b30: 6c64 2062 6520 7365 6e74 2e7a 1a70 6172  ld be sent.z.par
+00000b40: 7365 2061 6e64 2063 6865 636b 2065 7863  se and check exc
+00000b50: 6570 7469 6f6e 3a7a 1b73 6361 6e20 7265  eption:z.scan re
+00000b60: 636f 7264 7320 7765 7265 2072 6574 7269  cords were retri
+00000b70: 6576 6564 2902 7215 0000 00da 0969 6e74  eved).r......int
+00000b80: 6572 6e61 6c73 290f 7202 0000 00da 0474  ernals).r......t
+00000b90: 7970 65da 0869 735f 616c 6976 65da 0945  ype..is_alive..E
+00000ba0: 7863 6570 7469 6f6e da05 7072 696e 7472  xception..printr
+00000bb0: 0400 0000 7205 0000 00da 0474 696d 65da  ....r......time.
+00000bc0: 0566 6c6f 6174 da09 7465 726d 696e 6174  .float..terminat
+00000bd0: 6572 0700 0000 da09 7472 6163 6562 6163  er......tracebac
+00000be0: 6bda 0a66 6f72 6d61 745f 6578 63da 036c  k..format_exc..l
+00000bf0: 656e da06 6170 7065 6e64 290d da14 6167  en..append)...ag
+00000c00: 6772 6567 6174 6f72 5f76 6172 6961 626c  gregator_variabl
+00000c10: 6573 7209 0000 0072 0a00 0000 720c 0000  esr....r....r...
+00000c20: 00da 0873 7461 7475 7365 73da 0a75 6e66  ...statuses..unf
+00000c30: 696e 6973 6865 64da 0b73 7461 7475 735f  inished..status_
+00000c40: 7061 7468 da0e 7374 6174 7573 5f6f 665f  path..status_of_
+00000c50: 7061 7468 720d 0000 00da 0561 6c69 7665  pathr......alive
+00000c60: da01 45da 0765 6c61 7073 6564 da05 646f  ..E..elapsed..do
+00000c70: 6f72 73a9 0072 3a00 0000 fa71 2f62 696f  ors..r:....q/bio
+00000c80: 7465 6368 2f76 656e 7565 732f 7374 6167  tech/venues/stag
+00000c90: 6573 2f62 696f 7465 6368 2f70 726f 6365  es/biotech/proce
+00000ca0: 6475 7265 732f 6167 6772 6567 6174 6f72  dures/aggregator
+00000cb0: 5f70 726f 6365 6475 7265 2f70 726f 6365  _procedure/proce
+00000cc0: 7373 2f6d 6f76 6573 2f73 7461 7475 735f  ss/moves/status_
+00000cd0: 6368 6563 6b5f 6d6f 6e69 746f 722f 7468  check_monitor/th
+00000ce0: 655f 7068 7973 6963 616c 2e70 79da 2470  e_physical.py.$p
+00000cf0: 6172 7365 5f61 6e64 5f63 6865 636b 5f69  arse_and_check_i
+00000d00: 735f 616c 6976 655f 6f66 5f73 7461 7475  s_alive_of_statu
+00000d10: 7365 7321 0000 0073 4601 0000 0601 0802  ses!...sF.......
+00000d20: 0801 0c01 0402 0401 0a01 0802 0801 0202  ................
+00000d30: 0204 1001 1801 1401 0801 0a01 0802 0480  ................
+00000d40: 0e02 0a01 1401 0880 02fe 0805 0803 0205  ................
+00000d50: 020d 0c02 0c01 0c01 1c02 0802 0201 1001  ................
+00000d60: 0c01 0801 02ff 0204 0202 0201 0202 0202  ................
+00000d70: 12f8 140b 1401 1802 0202 0401 06ff 0480  ................
+00000d80: 0e03 0e01 0c01 0880 02fe 0205 0208 0e02  ................
+00000d90: 0e01 1c02 0a02 0201 1001 0e01 0801 02ff  ................
+00000da0: 0204 0202 0201 0202 0202 12f8 140b 1401  ................
+00000db0: 1801 0202 0401 06ff 0480 1003 0e01 0c01  ................
+00000dc0: 0880 02fe 0205 0212 0a02 0a01 0a01 1601  ................
+00000dd0: 1201 1a01 06fa 0e0b 0e01 0e01 1a01 1602  ................
+00000de0: 1c02 0a02 0201 0401 06ff 0204 1001 0e01  ................
+00000df0: 0801 02ff 0204 0202 0201 0202 0202 12f8  ................
+00000e00: 140b 1801 0480 1004 0a01 0c01 0880 02fe  ................
+00000e10: 0206 020c 0e02 0e01 0e02 0e02 0203 0202  ................
+00000e20: 0201 0201 0202 12f9 140a 0480 1002 0e01  ................
+00000e30: 0c01 0880 02fe 0205 0208 0203 0e02 0e02  ................
+00000e40: 0e01 0e02 1402 0480 1002 0e01 0c01 0880  ................
+00000e50: 02fe 0806 1601 0401 0201 0a01 08fe 0480  ................
+00000e60: 0406 723c 0000 0029 0fda 3962 696f 7465  ..r<...)..9biote
+00000e70: 6368 2e70 726f 6365 6475 7265 732e 6167  ch.procedures.ag
+00000e80: 6772 6567 6174 6f72 5f70 726f 6365 6475  gregator_procedu
+00000e90: 7265 2e70 726f 6365 7373 2e76 6172 6961  re.process.varia
+00000ea0: 626c 6573 7202 0000 0072 1d00 0000 7204  blesr....r....r.
+00000eb0: 0000 00da 2761 6c61 726d 5f63 6865 636b  ....'alarm_check
+00000ec0: 732e 676c 6f62 616c 5f74 696d 655f 6c69  s.global_time_li
+00000ed0: 6d69 745f 6578 6365 6564 6564 7205 0000  mit_exceededr...
+00000ee0: 00da 3062 696f 7465 6368 2e74 6f70 6963  ..0biotech.topic
+00000ef0: 732e 7072 6f63 6573 735f 6f6e 2e70 5f65  s.process_on.p_e
+00000f00: 7870 6563 742e 7061 7273 655f 7265 636f  xpect.parse_reco
+00000f10: 7264 7372 0600 0000 da1c 6269 6f74 6563  rdsr......biotec
+00000f20: 682e 746f 7069 6373 2e73 686f 772e 7661  h.topics.show.va
+00000f30: 7269 6162 6c65 7207 0000 0072 0800 0000  riabler....r....
+00000f40: 722a 0000 0072 2d00 0000 da04 7269 6368  r*...r-.....rich
+00000f50: 723c 0000 0072 3a00 0000 723a 0000 0072  r<...r:...r:...r
+00000f60: 3a00 0000 723b 0000 00da 083c 6d6f 6475  :...r;.....<modu
+00000f70: 6c65 3e01 0000 0073 1600 0000 0c07 0c03  le>....s........
+00000f80: 0c02 0c02 0c01 0c03 0801 0801 0803 0205  ................
+00000f90: 0c04                                     ..
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,24 +132,24 @@
 		try:
 			if (
 				occurrences ["scan process started"] == "yes" and
 				occurrences ["scan process notified aggregator"] == "no"
 			):
 				elapsed = time.time () - float (internal_statuses [ status_path ] ["times"] ["venture started"]);
 				
-				if (elapsed >= 10):			
+				if (elapsed >= 20):			
 					try:
 						occurrences = internal_statuses [ status_path ] ["occurences"];
 					except Exception:
 						occurrences = "not found"
 					
 					aggregator_variables ["internal_statuses"] [ status_path ] ["results_of_scan"] = {
 						"path": status_path,
 						
-						"alarm": "After 10 seconds, the process did not notify the aggregator that it had started.",
+						"alarm": "After 20 seconds, the process did not notify the aggregator that it had started.",
 						"alarm notes": [],
 						
 						"occurrences": occurrences,
 						
 						"exited": True
 					}
 				
@@ -287,14 +287,15 @@
 		'''
 		try:
 			if (
 				occurrences ["scan process is alive"] == "no" and
 
 				occurrences ["scan process started"] == "yes" and
 				occurrences ["scan process was stopped"] == "yes" and
+				
 				occurrences ["scan records were retrieved"] == "yes"
 			):				
 				aggregator_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
 
 		except Exception as E:
 			print ("parse and check exception:", traceback.format_exc ())
 			pass;
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,14 +55,22 @@
 	#
 	"internal_statuses": {},
 	"internal_statuses_built": "no",
 	
 	"anomalies": []
 }
 
+def add_anomaly (anomaly):
+	try:
+		is_JSON = json.dumps (anomaly)
+	
+		aggregator_variables.append (anomaly)
+	except Exception:
+		show_variable ("An anomaly couldn't be added.")
+
 def setup_internal_statuses (
 	status_check_paths,
 	relative_path
 ):
 	for status_check_path in status_check_paths:		
 		aggregator_variables ["internal_statuses"] [ 
 			format_path (status_check_path, relative_path) 
@@ -135,15 +143,16 @@
 				"process": "pending",
 				
 			},
 			
 			"times": {
 				"started": "",
 				"ended": "",
-				"elapsed": ""
+				"elapsed": "",
+				"records retrieval": ""
 			},
 			
 			"records": [],
 			
 			"process": None,
 			"results_of_scan": None
 		}
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 20:30:14 2024 UTC, .py size: 2930 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,125 @@
-00000000: 6f0d 0d0a 0000 0000 56d4 2266 720b 0000  o.......V."fr...
+00000000: 6f0d 0d0a 0000 0000 f3f3 2266 410c 0000  o........."fA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
+00000020: 0008 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 0900  Z.d.d.l.m.Z.....
 00000040: 0900 6403 6404 6405 9c02 6406 6900 6407  ..d.d.d...d.i.d.
 00000050: 6900 6408 6700 6409 9c07 5a03 640a 640b  i.d.g.d...Z.d.d.
 00000060: 8400 5a04 640c 640d 8400 5a05 640e 640f  ..Z.d.d...Z.d.d.
 00000070: 8400 5a06 6410 6411 8400 5a07 6412 6413  ..Z.d.d...Z.d.d.
-00000080: 8400 5a08 6414 5300 2915 7a66 0a09 6672  ..Z.d.S.).zf..fr
-00000090: 6f6d 2062 696f 7465 6368 2e70 726f 6365  om biotech.proce
-000000a0: 6475 7265 732e 6167 6772 6567 6174 6f72  dures.aggregator
-000000b0: 5f70 726f 6365 6475 7265 2e70 726f 6365  _procedure.proce
-000000c0: 7373 2e76 6172 6961 626c 6573 2069 6d70  ss.variables imp
-000000d0: 6f72 7420 7265 7472 6965 7665 5f61 6767  ort retrieve_agg
-000000e0: 7265 6761 746f 725f 7661 7269 6162 6c65  regator_variable
-000000f0: 730a e900 0000 0029 01da 0b66 6f72 6d61  s......)...forma
-00000100: 745f 7061 7468 7a07 302e 302e 302e 30da  t_pathz.0.0.0.0.
-00000110: 0029 02da 0468 6f73 74da 0470 6f72 74e9  .)...host..port.
-00000120: 0300 0000 e902 0000 00da 026e 6f29 07da  ...........no)..
-00000130: 0c69 6e74 726f 5f68 6172 626f 72da 0d72  .intro_harbor..r
-00000140: 6563 6f72 6473 5f6c 6576 656c da0f 696e  ecords_level..in
-00000150: 7472 6f5f 7661 7269 6162 6c65 73da 0764  tro_variables..d
-00000160: 6574 6169 6c73 da11 696e 7465 726e 616c  etails..internal
-00000170: 5f73 7461 7475 7365 73da 1769 6e74 6572  _statuses..inter
-00000180: 6e61 6c5f 7374 6174 7573 6573 5f62 7569  nal_statuses_bui
-00000190: 6c74 da09 616e 6f6d 616c 6965 7363 0200  lt..anomaliesc..
-000001a0: 0000 0000 0000 0000 0000 0300 0000 0a00  ................
-000001b0: 0000 4300 0000 734c 0000 007c 0044 005d  ..C...sL...|.D.]
-000001c0: 217d 0264 0164 0164 0164 0164 0264 0164  !}.d.d.d.d.d.d.d
-000001d0: 0164 0364 049c 0864 0564 0669 0164 0364  .d.d...d.d.i.d.d
-000001e0: 0364 0364 079c 0367 0064 0064 0064 089c  .d.d...g.d.d.d..
-000001f0: 0674 0064 0919 0074 017c 027c 0183 023c  .t.d...t.|.|...<
-00000200: 0071 0264 0053 0029 0a4e 7208 0000 00da  .q.d.S.).Nr.....
-00000210: 0775 6e6b 6e6f 776e 7203 0000 0029 087a  .unknownr....).z
-00000220: 1c73 6361 6e20 7072 6f63 6573 7320 7665  .scan process ve
-00000230: 6e74 7572 6520 7374 6172 7465 647a 1473  nture startedz.s
-00000240: 6361 6e20 7072 6f63 6573 7320 7374 6172  can process star
-00000250: 7465 647a 2073 6361 6e20 7072 6f63 6573  tedz scan proces
-00000260: 7320 6e6f 7469 6669 6564 2061 6767 7265  s notified aggre
-00000270: 6761 746f 727a 1873 6361 6e20 7072 6f63  gatorz.scan proc
-00000280: 6573 7320 7761 7320 7374 6f70 7065 647a  ess was stoppedz
-00000290: 1573 6361 6e20 7072 6f63 6573 7320 6973  .scan process is
-000002a0: 2061 6c69 7665 7a16 7363 616e 2072 6574   alivez.scan ret
-000002b0: 7572 6e65 6420 7072 6f63 6565 6473 7a1b  urned proceedsz.
-000002c0: 7363 616e 2072 6563 6f72 6473 2077 6572  scan records wer
-000002d0: 6520 7265 7472 6965 7665 647a 1064 6f6e  e retrievedz.don
-000002e0: 6520 7265 6173 6f6e 2067 6976 65da 0770  e reason give..p
-000002f0: 726f 6365 7373 da07 7065 6e64 696e 6729  rocess..pending)
-00000300: 03da 0773 7461 7274 6564 da05 656e 6465  ...started..ende
-00000310: 64da 0765 6c61 7073 6564 2906 da0b 6f63  d..elapsed)...oc
-00000320: 6375 7272 656e 6365 73da 0673 7461 7475  currences..statu
-00000330: 73da 0574 696d 6573 da07 7265 636f 7264  s..times..record
-00000340: 7372 1100 0000 da0f 7265 7375 6c74 735f  sr......results_
-00000350: 6f66 5f73 6361 6e72 0d00 0000 2902 da14  of_scanr....)...
-00000360: 6167 6772 6567 6174 6f72 5f76 6172 6961  aggregator_varia
-00000370: 626c 6573 7202 0000 0029 03da 1273 7461  blesr....)...sta
-00000380: 7475 735f 6368 6563 6b5f 7061 7468 73da  tus_check_paths.
-00000390: 0d72 656c 6174 6976 655f 7061 7468 da11  .relative_path..
-000003a0: 7374 6174 7573 5f63 6865 636b 5f70 6174  status_check_pat
-000003b0: 68a9 0072 1f00 0000 fa5c 2f62 696f 7465  h..r.....\/biote
-000003c0: 6368 2f76 656e 7565 732f 7374 6167 6573  ch/venues/stages
-000003d0: 2f62 696f 7465 6368 2f70 726f 6365 6475  /biotech/procedu
-000003e0: 7265 732f 6167 6772 6567 6174 6f72 5f70  res/aggregator_p
-000003f0: 726f 6365 6475 7265 2f70 726f 6365 7373  rocedure/process
-00000400: 2f76 6172 6961 626c 6573 2f5f 5f69 6e69  /variables/__ini
-00000410: 745f 5f2e 7079 da17 7365 7475 705f 696e  t__.py..setup_in
-00000420: 7465 726e 616c 5f73 7461 7475 7365 733e  ternal_statuses>
-00000430: 0000 0073 3000 0000 0804 020c 0207 0208  ...s0...........
-00000440: 0207 0207 0208 0207 0207 04c5 0441 02ff  .............A..
-00000450: 0206 0201 0201 04fd 0206 0202 0201 04b1  ................
-00000460: 06fe 0801 04ff 0455 7221 0000 0063 0000  .......Ur!...c..
-00000470: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-00000480: 0000 4300 0000 7304 0000 0064 0053 00a9  ..C...s....d.S..
-00000490: 014e 721f 0000 0072 1f00 0000 721f 0000  .Nr....r....r...
-000004a0: 0072 1f00 0000 7220 0000 00da 0663 6861  .r....r .....cha
-000004b0: 6e67 659a 0000 00f3 0200 0000 0401 7223  nge...........r#
-000004c0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000004d0: 0000 0000 0100 0000 4300 0000 f304 0000  ........C.......
-000004e0: 0074 0053 0072 2200 0000 a901 721b 0000  .t.S.r".....r...
-000004f0: 0072 1f00 0000 721f 0000 0072 1f00 0000  .r....r....r....
-00000500: 7220 0000 00da 1272 6574 7269 6576 655f  r .....retrieve_
-00000510: 7661 7269 6162 6c65 739d 0000 0072 2400  variables....r$.
-00000520: 0000 7227 0000 0063 0000 0000 0000 0000  ..r'...c........
-00000530: 0000 0000 0000 0000 0100 0000 4300 0000  ............C...
-00000540: 7225 0000 0072 2200 0000 7226 0000 0072  r%...r"...r&...r
-00000550: 1f00 0000 721f 0000 0072 1f00 0000 7220  ....r....r....r 
-00000560: 0000 00da 1d72 6574 7269 6576 655f 6167  .....retrieve_ag
-00000570: 6772 6567 6174 6f72 5f76 6172 6961 626c  gregator_variabl
-00000580: 6573 a000 0000 7224 0000 0072 2800 0000  es....r$...r(...
-00000590: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000005a0: 0001 0000 0043 0000 0072 2500 0000 7222  .....C...r%...r"
-000005b0: 0000 0072 2600 0000 721f 0000 0072 1f00  ...r&...r....r..
-000005c0: 0000 721f 0000 0072 2000 0000 da08 7265  ..r....r .....re
-000005d0: 7472 6965 7665 a300 0000 7224 0000 0072  trieve....r$...r
-000005e0: 2900 0000 4e29 09da 075f 5f64 6f63 5f5f  )...N)...__doc__
-000005f0: da41 6269 6f74 6563 682e 7072 6f63 6564  .Abiotech.proced
-00000600: 7572 6573 2e61 6767 7265 6761 746f 725f  ures.aggregator_
-00000610: 7072 6f63 6564 7572 652e 7072 6f63 6573  procedure.proces
-00000620: 732e 6d6f 7665 732e 666f 726d 6174 5f70  s.moves.format_p
-00000630: 6174 6872 0200 0000 721b 0000 0072 2100  athr....r....r!.
-00000640: 0000 7223 0000 0072 2700 0000 7228 0000  ..r#...r'...r(..
-00000650: 0072 2900 0000 721f 0000 0072 1f00 0000  .r)...r....r....
-00000660: 721f 0000 0072 2000 0000 da08 3c6d 6f64  r....r .....<mod
-00000670: 756c 653e 0100 0000 7326 0000 0004 020c  ule>....s&......
-00000680: 0402 0302 0702 1502 0104 fe02 0502 0202  ................
-00000690: 0702 0502 0102 0206 e908 1a08 5c08 0308  ............\...
-000006a0: 030c 03                                  ...
+00000080: 8400 5a08 6414 6415 8400 5a09 6416 5300  ..Z.d.d...Z.d.S.
+00000090: 2917 7a66 0a09 6672 6f6d 2062 696f 7465  ).zf..from biote
+000000a0: 6368 2e70 726f 6365 6475 7265 732e 6167  ch.procedures.ag
+000000b0: 6772 6567 6174 6f72 5f70 726f 6365 6475  gregator_procedu
+000000c0: 7265 2e70 726f 6365 7373 2e76 6172 6961  re.process.varia
+000000d0: 626c 6573 2069 6d70 6f72 7420 7265 7472  bles import retr
+000000e0: 6965 7665 5f61 6767 7265 6761 746f 725f  ieve_aggregator_
+000000f0: 7661 7269 6162 6c65 730a e900 0000 0029  variables......)
+00000100: 01da 0b66 6f72 6d61 745f 7061 7468 7a07  ...format_pathz.
+00000110: 302e 302e 302e 30da 0029 02da 0468 6f73  0.0.0.0..)...hos
+00000120: 74da 0470 6f72 74e9 0300 0000 e902 0000  t..port.........
+00000130: 00da 026e 6f29 07da 0c69 6e74 726f 5f68  ...no)...intro_h
+00000140: 6172 626f 72da 0d72 6563 6f72 6473 5f6c  arbor..records_l
+00000150: 6576 656c da0f 696e 7472 6f5f 7661 7269  evel..intro_vari
+00000160: 6162 6c65 73da 0764 6574 6169 6c73 da11  ables..details..
+00000170: 696e 7465 726e 616c 5f73 7461 7475 7365  internal_statuse
+00000180: 73da 1769 6e74 6572 6e61 6c5f 7374 6174  s..internal_stat
+00000190: 7573 6573 5f62 7569 6c74 da09 616e 6f6d  uses_built..anom
+000001a0: 616c 6965 7363 0100 0000 0000 0000 0000  aliesc..........
+000001b0: 0000 0200 0000 0800 0000 4300 0000 7338  ..........C...s8
+000001c0: 0000 007a 0d74 00a0 017c 00a1 017d 0174  ...z.t...|...}.t
+000001d0: 02a0 037c 00a1 0101 0057 0064 0053 0004  ...|.....W.d.S..
+000001e0: 0074 0479 1b01 0001 0001 0074 0564 0183  .t.y.......t.d..
+000001f0: 0101 0059 0064 0053 0077 0029 024e 7a1d  ...Y.d.S.w.).Nz.
+00000200: 416e 2061 6e6f 6d61 6c79 2063 6f75 6c64  An anomaly could
+00000210: 6e27 7420 6265 2061 6464 6564 2e29 06da  n't be added.)..
+00000220: 046a 736f 6eda 0564 756d 7073 da14 6167  .json..dumps..ag
+00000230: 6772 6567 6174 6f72 5f76 6172 6961 626c  gregator_variabl
+00000240: 6573 da06 6170 7065 6e64 da09 4578 6365  es..append..Exce
+00000250: 7074 696f 6eda 0d73 686f 775f 7661 7269  ption..show_vari
+00000260: 6162 6c65 2902 da07 616e 6f6d 616c 79da  able)...anomaly.
+00000270: 0769 735f 4a53 4f4e a900 7218 0000 00fa  .is_JSON..r.....
+00000280: 5c2f 6269 6f74 6563 682f 7665 6e75 6573  \/biotech/venues
+00000290: 2f73 7461 6765 732f 6269 6f74 6563 682f  /stages/biotech/
+000002a0: 7072 6f63 6564 7572 6573 2f61 6767 7265  procedures/aggre
+000002b0: 6761 746f 725f 7072 6f63 6564 7572 652f  gator_procedure/
+000002c0: 7072 6f63 6573 732f 7661 7269 6162 6c65  process/variable
+000002d0: 732f 5f5f 696e 6974 5f5f 2e70 79da 0b61  s/__init__.py..a
+000002e0: 6464 5f61 6e6f 6d61 6c79 3e00 0000 730c  dd_anomaly>...s.
+000002f0: 0000 0002 010a 0110 020c 010e 0102 ff72  ...............r
+00000300: 1a00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00000310: 0003 0000 000a 0000 0043 0000 0073 4e00  .........C...sN.
+00000320: 0000 7c00 4400 5d22 7d02 6401 6401 6401  ..|.D.]"}.d.d.d.
+00000330: 6401 6402 6401 6401 6403 6404 9c08 6405  d.d.d.d.d.d...d.
+00000340: 6406 6901 6403 6403 6403 6403 6407 9c04  d.i.d.d.d.d.d...
+00000350: 6700 6400 6400 6408 9c06 7400 6409 1900  g.d.d.d...t.d...
+00000360: 7401 7c02 7c01 8302 3c00 7102 6400 5300  t.|.|...<.q.d.S.
+00000370: 290a 4e72 0800 0000 da07 756e 6b6e 6f77  ).Nr......unknow
+00000380: 6e72 0300 0000 2908 7a1c 7363 616e 2070  nr....).z.scan p
+00000390: 726f 6365 7373 2076 656e 7475 7265 2073  rocess venture s
+000003a0: 7461 7274 6564 7a14 7363 616e 2070 726f  tartedz.scan pro
+000003b0: 6365 7373 2073 7461 7274 6564 7a20 7363  cess startedz sc
+000003c0: 616e 2070 726f 6365 7373 206e 6f74 6966  an process notif
+000003d0: 6965 6420 6167 6772 6567 6174 6f72 7a18  ied aggregatorz.
+000003e0: 7363 616e 2070 726f 6365 7373 2077 6173  scan process was
+000003f0: 2073 746f 7070 6564 7a15 7363 616e 2070   stoppedz.scan p
+00000400: 726f 6365 7373 2069 7320 616c 6976 657a  rocess is alivez
+00000410: 1673 6361 6e20 7265 7475 726e 6564 2070  .scan returned p
+00000420: 726f 6365 6564 737a 1b73 6361 6e20 7265  roceedsz.scan re
+00000430: 636f 7264 7320 7765 7265 2072 6574 7269  cords were retri
+00000440: 6576 6564 7a10 646f 6e65 2072 6561 736f  evedz.done reaso
+00000450: 6e20 6769 7665 da07 7072 6f63 6573 73da  n give..process.
+00000460: 0770 656e 6469 6e67 2904 da07 7374 6172  .pending)...star
+00000470: 7465 64da 0565 6e64 6564 da07 656c 6170  ted..ended..elap
+00000480: 7365 647a 1172 6563 6f72 6473 2072 6574  sedz.records ret
+00000490: 7269 6576 616c 2906 da0b 6f63 6375 7272  rieval)...occurr
+000004a0: 656e 6365 73da 0673 7461 7475 73da 0574  ences..status..t
+000004b0: 696d 6573 da07 7265 636f 7264 7372 1c00  imes..recordsr..
+000004c0: 0000 da0f 7265 7375 6c74 735f 6f66 5f73  ....results_of_s
+000004d0: 6361 6e72 0d00 0000 2902 7212 0000 0072  canr....).r....r
+000004e0: 0200 0000 2903 da12 7374 6174 7573 5f63  ....)...status_c
+000004f0: 6865 636b 5f70 6174 6873 da0d 7265 6c61  heck_paths..rela
+00000500: 7469 7665 5f70 6174 68da 1173 7461 7475  tive_path..statu
+00000510: 735f 6368 6563 6b5f 7061 7468 7218 0000  s_check_pathr...
+00000520: 0072 1800 0000 7219 0000 00da 1773 6574  .r....r......set
+00000530: 7570 5f69 6e74 6572 6e61 6c5f 7374 6174  up_internal_stat
+00000540: 7573 6573 4600 0000 7332 0000 0008 0402  usesF...s2......
+00000550: 0c02 0702 0802 0702 0702 0802 0702 0704  ................
+00000560: c504 4102 ff02 0602 0102 0102 0104 fc02  ..A.............
+00000570: 0702 0202 0104 b006 fe08 0104 ff04 5672  ..............Vr
+00000580: 2900 0000 6300 0000 0000 0000 0000 0000  )...c...........
+00000590: 0000 0000 0001 0000 0043 0000 0073 0400  .........C...s..
+000005a0: 0000 6400 5300 a901 4e72 1800 0000 7218  ..d.S...Nr....r.
+000005b0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+000005c0: 0000 da06 6368 616e 6765 a300 0000 f302  ....change......
+000005d0: 0000 0004 0172 2b00 0000 6300 0000 0000  .....r+...c.....
+000005e0: 0000 0000 0000 0000 0000 0001 0000 0043  ...............C
+000005f0: 0000 00f3 0400 0000 7400 5300 722a 0000  ........t.S.r*..
+00000600: 00a9 0172 1200 0000 7218 0000 0072 1800  ...r....r....r..
+00000610: 0000 7218 0000 0072 1900 0000 da12 7265  ..r....r......re
+00000620: 7472 6965 7665 5f76 6172 6961 626c 6573  trieve_variables
+00000630: a600 0000 722c 0000 0072 2f00 0000 6300  ....r,...r/...c.
+00000640: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00000650: 0000 0043 0000 0072 2d00 0000 722a 0000  ...C...r-...r*..
+00000660: 0072 2e00 0000 7218 0000 0072 1800 0000  .r....r....r....
+00000670: 7218 0000 0072 1900 0000 da1d 7265 7472  r....r......retr
+00000680: 6965 7665 5f61 6767 7265 6761 746f 725f  ieve_aggregator_
+00000690: 7661 7269 6162 6c65 73a9 0000 0072 2c00  variables....r,.
+000006a0: 0000 7230 0000 0063 0000 0000 0000 0000  ..r0...c........
+000006b0: 0000 0000 0000 0000 0100 0000 4300 0000  ............C...
+000006c0: 722d 0000 0072 2a00 0000 722e 0000 0072  r-...r*...r....r
+000006d0: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
+000006e0: 0000 00da 0872 6574 7269 6576 65ac 0000  .....retrieve...
+000006f0: 0072 2c00 0000 7231 0000 004e 290a da07  .r,...r1...N)...
+00000700: 5f5f 646f 635f 5fda 4162 696f 7465 6368  __doc__.Abiotech
+00000710: 2e70 726f 6365 6475 7265 732e 6167 6772  .procedures.aggr
+00000720: 6567 6174 6f72 5f70 726f 6365 6475 7265  egator_procedure
+00000730: 2e70 726f 6365 7373 2e6d 6f76 6573 2e66  .process.moves.f
+00000740: 6f72 6d61 745f 7061 7468 7202 0000 0072  ormat_pathr....r
+00000750: 1200 0000 721a 0000 0072 2900 0000 722b  ....r....r)...r+
+00000760: 0000 0072 2f00 0000 7230 0000 0072 3100  ...r/...r0...r1.
+00000770: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
+00000780: 0072 1900 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000790: 0100 0000 7328 0000 0004 020c 0402 0302  ....s(..........
+000007a0: 0702 1502 0104 fe02 0502 0202 0702 0502  ................
+000007b0: 0102 0206 e908 1a08 0808 5d08 0308 030c  ..........].....
+000007c0: 03                                       .
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py` & `biotech-1.1.2/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/on.py` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/on.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 	
 	the_report = the_health_check ["report"]	
 '''
 
 #----
 #
 from .dynamic_port import dynamic_port
+from biotech.topics.show.variable import show_variable
+
 #
 #
 import flask
 #
 #
 import os
 import pathlib
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 
 
 '''
 	steps:
 		process is started
-		
-		
 '''
-
-
+print ('health scan')
 
 #
 #
 from __health_scan_utilities.coms.done_with_scan import done_with_scan
 from __health_scan_utilities.coms.the_health_scan_started import the_health_scan_started
 from __health_scan_utilities.format_rel_path import format_rel_path
 from __health_scan_utilities.import_from_path import import_from_path
@@ -80,15 +77,15 @@
 		show_variable ({
 			"pid": os.getpid (),
 			"proceeds": proceeds,
 			"harbor": {
 				"host": host,
 				"port": port
 			}
-		}, mode = "show")
+		})
 	except Exception as E:
 		proceeds = {
 			"parsed": False,
 			"alarm": "An exception occurred while running the scan.",
 			"exception": repr (E),
 			"exception trace": find_trace (E)
 		}
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/intro/on.py` & `biotech-1.1.2/venues/stages/biotech/procedures/intro/on.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 
 
 
 from biotech.topics.process_on.p_expect.implicit import process_on_implicit
 from biotech.topics.show.variable import show_variable
+from biotech.topics.implicit.thread import implicit_thread
+	
 #
 #
 import rich	
 from tinydb import TinyDB, Query
 import requests
 #
 #
+import atexit
 import glob
 import json
 import pathlib
 from os.path import dirname, join, normpath
 import os
 import sys
 import threading
@@ -50,15 +53,15 @@
 	module_paths = [],
 	
 	simultaneous = False,
 	simultaneous_capacity = 10,
 	
 	time_limit = "99999999999999999999999"
 ):
-	the_report = on ({
+	bio = on ({
 		"glob_string": glob_string,
 	
 		#
 		#	itinerary: optionally dynamic
 		#
 		"intro_port": intro_port,
 		"aggregator_procedure_port": aggregator_procedure_port,
@@ -80,25 +83,33 @@
 		
 		"simultaneous": simultaneous,
 		"simultaneous_capacity": simultaneous_capacity,
 		
 		"time_limit": time_limit
 	})
 	
+	bio ["off"] ()
+	the_report = bio ["proceeds"]
+	
 	return {
 		"status": the_report,
 		
 		"paths": the_report ["paths"],
 		"alarms": the_report ["alarms"],
 		"stats": the_report ["stats"]
 	}
 
 def on (packet):
 	show_variable ({ "intro": "The intro." }, mode = "condensed")
 
+	show_variable ({ 
+		"glob_string": packet ["glob_string"] 
+	})
+
+
 	'''
 		The other presets are in the
 		intro process.
 	'''
 	if ("intro_port" not in packet):
 		packet ["intro_port"] = 52434
 	if ("records" not in packet):
@@ -164,14 +175,24 @@
 		"python3 " + the_intro_process_path (),
 		
 		#CWD = CWD,
 		env = process_environment,
 		name = "intro"
 	)
 	
+	def at_exit_term ():
+		nonlocal the_intro;
+		
+		try:
+			the_intro ["process"].terminate ()
+		except Exception as E:
+			print ('exit exception:', E)
+	
+	atexit.register (at_exit_term)
+	
 	'''
 		check that the process is on
 	'''
 	'''
 	while True:
 		try:
 			print ("checking if is the intro is on on")
@@ -203,17 +224,15 @@
 		except Exception as E:
 			print (E)
 			pass;
 			
 		time.sleep (1)
 	
 
-	show_variable ({
-		"sending the packet": packet
-	}, mode = "condensed")
+	show_variable ("sending the variables packet", mode = "condensed")
 	
 	'''
 		objective: send the packet to the intro quay
 	'''
 	response = requests.patch (
 		intro_quay_URL + "/start", 
 		json = packet
@@ -244,27 +263,77 @@
 	response = requests.get (
 		intro_quay_URL + "/the_report"
 	)
 	the_report = json.loads (response.text);
 	
 	
 	show_variable ("The intro process starter received the_report.", mode = "condensed")
+	show_variable ({
+		"report": the_report
+	})
 
 	#time.sleep (6000000)
 	
-	the_intro ["process"].terminate ()
-	
-
 	if (type (db_directory) == str):
 		os.makedirs (db_directory, exist_ok = True)
 		db_file = normpath (join (db_directory, f"records.json"))
 		db = TinyDB (db_file)
 		
 		db.insert ({
 			'paths': the_report ["paths"], 
 			'alarms': the_report ["alarms"],
 			'stats': the_report ["stats"]
 		})
 		
 		db.close ()
+	
+	
+	#
+	#
+	#
+	
+	barricaded = True;
+	the_stop = False;
+	def background_task ():
+		nonlocal the_stop;
+		nonlocal barricaded;
+
+		print ("waiting for off to be called")	
+
+		while the_stop == False:
+			time.sleep (.25)
+			
+		the_intro ["process"].terminate ()
+		while barricaded == True:
+			print ('waiting for process to exit')
+		
+			try:
+				print ("is_alive:", the_intro ["process"].is_alive ())
+			
+				if (the_intro ["process"].is_alive () == False):
+					barricaded = False
+			except Exception as E:
+				print ("exception:", E)
+				
+			time.sleep (.25)
+		
+	
+	background_thread = threading.Thread (target=background_task)
+	background_thread.start ()
+
+		
+	def turn_off ():
+		nonlocal the_stop;
+		nonlocal barricaded;
+		
+		the_stop = True
+		
+		while barricaded == True:
+			print ("barricaded")	
+			time.sleep (1)
+		
+		return;
 
-	return the_report
+	return {
+		"off": turn_off,
+		"proceeds": the_report
+	}
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 19:03:05 2024 UTC, .py size: 3989 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e9bf 2266 950f 0000  o........."f....
+00000000: 6f0d 0d0a 0000 0000 61e5 2266 a00f 0000  o.......a."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 ae00 0000 6500  .....@...s....e.
 00000030: 6400 8301 0100 6401 6402 6c01 6d02 5a02  d.....d.d.l.m.Z.
 00000040: 0100 6401 6403 6c03 6d04 5a04 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0b 6d0c 5a0c 0100 6401  ..d.d.l.m.Z...d.
@@ -24,158 +24,159 @@
 00000170: 655f 6973 5f6f 6e29 01da 1873 656e 645f  e_is_on)...send_
 00000180: 7061 7468 735f 746f 5f61 6767 7265 6761  paths_to_aggrega
 00000190: 746f 724e 2903 da07 6469 726e 616d 65da  torN)...dirname.
 000001a0: 046a 6f69 6eda 086e 6f72 6d70 6174 6863  .join..normpathc
 000001b0: 0000 0000 0000 0000 0000 0000 1100 0000  ................
 000001c0: 0d00 0000 0300 0000 73e6 0100 0074 00a0  ........s....t..
 000001d0: 01a1 0089 0169 0089 0087 0087 0166 0264  .....i.......f.d
-000001e0: 0164 0284 087d 0074 0264 0383 0101 0074  .d...}.t.d.....t
-000001f0: 036a 04a0 0564 04a1 017d 0174 067c 017c  .j...d...}.t.|.|
-00000200: 0064 058d 027d 0274 0264 0683 0101 0074  .d...}.t.d.....t
-00000210: 0774 0864 0719 0083 0174 096b 0372 3a74  .t.d.....t.k.r:t
-00000220: 0a64 0883 0101 0074 0ba0 0c64 09a1 0101  .d.....t...d....
-00000230: 0074 0774 0864 0719 0083 0174 096b 0373  .t.t.d.....t.k.s
-00000240: 2974 0864 0719 00a0 0564 0aa1 017d 0374  )t.d.....d...}.t
-00000250: 0864 0719 00a0 0564 0b64 0ca1 027d 0474  .d.....d.d...}.t
-00000260: 0864 0719 00a0 0564 0d64 0ea1 027d 0574  .d.....d.d...}.t
-00000270: 0864 0719 00a0 0564 0f64 10a1 027d 0674  .d.....d.d...}.t
-00000280: 0864 0719 00a0 0564 1164 12a1 027d 0774  .d.....d.d...}.t
-00000290: 0864 0719 00a0 0564 1364 12a1 027d 0874  .d.....d.d...}.t
-000002a0: 0864 0719 00a0 0564 1467 00a1 027d 0974  .d.....d.g...}.t
-000002b0: 0864 0719 00a0 0564 1564 16a1 027d 0a74  .d.....d.d...}.t
-000002c0: 0864 0719 00a0 0564 1764 12a1 027d 0b74  .d.....d.d...}.t
-000002d0: 0864 0719 00a0 0564 1864 19a1 027d 0c74  .d.....d.d...}.t
-000002e0: 0864 0719 00a0 0564 1a64 1ba1 027d 0d74  .d.....d.d...}.t
-000002f0: 0d6a 0d7c 0364 1c64 1d8d 027d 0e74 0e7c  .j.|.d.d...}.t.|
-00000300: 0883 017d 087c 067d 0f74 0274 0864 0719  ...}.|.}.t.t.d..
-00000310: 007c 0e64 1e9c 0283 0101 0074 0f7c 0569  .|.d.......t.|.i
-00000320: 0064 1f8d 027d 1009 0074 107c 0564 208d  .d...}...t.|.d .
-00000330: 0101 007c 0f64 106b 0572 bb74 0264 2183  ...|.d.k.r.t.d!.
-00000340: 0101 0074 117c 057c 0e7c 087c 097c 0b7c  ...t.|.|.|.|.|.|
-00000350: 0c7c 0a7c 0d7c 0f7c 0464 2264 239c 0264  .|.|.|.|.d"d#..d
-00000360: 249c 0964 1f8d 0201 007c 0f64 106b 0572  $..d.....|.d.k.r
-00000370: d674 0264 2583 0101 0088 01a0 12a1 0001  .t.d%...........
-00000380: 007c 0f64 106b 0572 e274 0264 2683 0101  .|.d.k.r.t.d&...
-00000390: 007c 0f64 106b 0572 f174 027c 1088 0064  .|.d.k.r.t.|...d
-000003a0: 279c 0264 2864 298d 0201 0064 0053 0064  '..d(d)....d.S.d
-000003b0: 0053 0029 2a4e 6301 0000 0000 0000 0000  .S.)*Nc.........
-000003c0: 0000 0001 0000 0002 0000 0013 0000 0073  ...............s
-000003d0: 1800 0000 7c00 8900 7400 6401 8301 0100  ....|...t.d.....
-000003e0: 8801 a001 a100 0100 6400 5300 2902 4e7a  ........d.S.).Nz
-000003f0: 2468 6561 6c74 685f 7363 616e 735f 646f  $health_scans_do
-00000400: 6e65 2c20 6f70 656e 696e 6720 7468 6520  ne, opening the 
-00000410: 646f 6f72 2e29 0272 0500 0000 da03 7365  door.).r......se
-00000420: 7429 01da 0a74 6865 5f70 6163 6b65 74a9  t)...the_packet.
-00000430: 02da 1074 6865 5f73 6361 6e5f 7265 7375  ...the_scan_resu
-00000440: 6c74 73da 1c77 6169 745f 756e 7469 6c5f  lts..wait_until_
-00000450: 6865 616c 7468 5f73 6361 6e73 5f64 6f6e  health_scans_don
-00000460: 65a9 00fa 442f 6269 6f74 6563 682f 7665  e...D/biotech/ve
-00000470: 6e75 6573 2f73 7461 6765 732f 6269 6f74  nues/stages/biot
-00000480: 6563 682f 7072 6f63 6564 7572 6573 2f69  ech/procedures/i
-00000490: 6e74 726f 2f70 726f 6365 7373 2f61 6476  ntro/process/adv
-000004a0: 656e 7475 7265 2e70 79da 1168 6561 6c74  enture.py..healt
-000004b0: 685f 7363 616e 735f 646f 6e65 2600 0000  h_scans_done&...
-000004c0: 7306 0000 0004 0308 020c 017a 2461 6476  s..........z$adv
-000004d0: 656e 7475 7265 2e3c 6c6f 6361 6c73 3e2e  enture.<locals>.
-000004e0: 6865 616c 7468 5f73 6361 6e73 5f64 6f6e  health_scans_don
-000004f0: 657a 1b61 626f 7574 2074 6f20 7374 6172  ez.about to star
-00000500: 7420 696e 7472 6f20 6861 7262 6f72 da0f  t intro harbor..
-00000510: 696e 7472 6f5f 7175 6179 5f70 6f72 7429  intro_quay_port)
-00000520: 02da 0470 6f72 7472 1300 0000 7a14 696e  ...portr....z.in
-00000530: 7472 6f20 6861 7262 6f72 2073 7461 7274  tro harbor start
-00000540: 6564 da06 7061 636b 6574 7a15 7761 6974  ed..packetz.wait
-00000550: 696e 6720 666f 7220 7661 7269 6162 6c65  ing for variable
-00000560: 7367 3333 3333 3333 d33f da0b 676c 6f62  sg333333.?..glob
-00000570: 5f73 7472 696e 67da 0a69 6e74 726f 5f70  _string..intro_p
-00000580: 6f72 7469 d2cc 0000 da19 6167 6772 6567  orti......aggreg
-00000590: 6174 6f72 5f70 726f 6365 6475 7265 5f70  ator_procedure_p
-000005a0: 6f72 7469 d3cc 0000 da07 7265 636f 7264  orti......record
-000005b0: 73e9 0300 0000 da0c 6462 5f64 6972 6563  s.......db_direc
-000005c0: 746f 7279 46da 0d72 656c 6174 6976 655f  toryF..relative_
-000005d0: 7061 7468 da0c 6d6f 6475 6c65 5f70 6174  path..module_pat
-000005e0: 6873 da12 6167 6772 6567 6174 696f 6e5f  hs..aggregation_
-000005f0: 666f 726d 6174 e901 0000 00da 0c73 696d  format.......sim
-00000600: 756c 7461 6e65 6f75 73da 1573 696d 756c  ultaneous..simul
-00000610: 7461 6e65 6f75 735f 6361 7061 6369 7479  taneous_capacity
-00000620: e90a 0000 00da 0a74 696d 655f 6c69 6d69  .......time_limi
-00000630: 74da 1739 3939 3939 3939 3939 3939 3939  t..9999999999999
-00000640: 3939 3939 3939 3939 3939 5429 01da 0972  9999999999T)...r
-00000650: 6563 7572 7369 7665 2902 7a12 676f 7420  ecursive).z.got 
-00000660: 7468 6520 7661 7269 6162 6c65 733a da05  the variables:..
-00000670: 6669 6e64 7329 0272 1500 0000 7216 0000  finds).r....r...
-00000680: 0029 0172 1500 0000 7a24 7468 6520 6167  .).r....z$the ag
-00000690: 6772 6567 6174 6f72 2070 726f 6365 6475  gregator procedu
-000006a0: 7265 2068 6173 2073 7461 7274 6564 7a07  re has startedz.
-000006b0: 302e 302e 302e 3029 0272 1500 0000 da04  0.0.0.0).r......
-000006c0: 686f 7374 2909 da12 7374 6174 7573 5f63  host)...status_c
-000006d0: 6865 636b 5f70 6174 6873 721d 0000 0072  heck_pathsr....r
-000006e0: 1e00 0000 7221 0000 0072 2200 0000 721f  ....r!...r"...r.
-000006f0: 0000 0072 2400 0000 da0d 7265 636f 7264  ...r$.....record
-00000700: 735f 6c65 7665 6cda 1074 6865 5f69 6e74  s_level..the_int
-00000710: 726f 5f68 6172 626f 727a 2d70 6174 6873  ro_harborz-paths
-00000720: 2073 656e 742c 2077 6169 7469 6e67 2075   sent, waiting u
-00000730: 6e74 696c 2074 6865 2073 6361 6e73 2061  ntil the scans a
-00000740: 7265 2064 6f6e 652e 7a1e 646f 6e65 2061  re done.z.done a
-00000750: 7761 6974 696e 6720 7468 6520 6865 616c  waiting the heal
-00000760: 7468 2073 6361 6e73 2902 7a27 7468 655f  th scans).z'the_
-00000770: 6167 6772 6567 6174 6f72 5f70 726f 6365  aggregator_proce
-00000780: 6475 7265 2061 6674 6572 2073 746f 7070  dure after stopp
-00000790: 6564 3a7a 1769 6e74 726f 3a20 7468 655f  ed:z.intro: the_
-000007a0: 7363 616e 5f72 6573 756c 7473 da04 7368  scan_results..sh
-000007b0: 6f77 2901 da04 6d6f 6465 2913 da09 7468  ow)...mode)...th
-000007c0: 7265 6164 696e 67da 0545 7665 6e74 7205  reading..Eventr.
-000007d0: 0000 00da 026f 73da 0765 6e76 6972 6f6e  .....os..environ
-000007e0: da03 6765 7472 0200 0000 da04 7479 7065  ..getr......type
-000007f0: 7203 0000 00da 0464 6963 74da 0570 7269  r......dict..pri
-00000800: 6e74 da04 7469 6d65 da05 736c 6565 70da  nt..time..sleep.
-00000810: 0467 6c6f 62da 0373 7472 7206 0000 0072  .glob..strr....r
-00000820: 0700 0000 7208 0000 00da 0477 6169 7429  ....r......wait)
-00000830: 1172 1300 0000 7215 0000 00da 0668 6172  .r....r......har
-00000840: 626f 7272 1700 0000 7218 0000 0072 1900  borr....r....r..
-00000850: 0000 721a 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00000860: 0072 1e00 0000 721f 0000 0072 2100 0000  .r....r....r!...
-00000870: 7222 0000 0072 2400 0000 7227 0000 0072  r"...r$...r'...r
-00000880: 2a00 0000 da18 7468 655f 6167 6772 6567  *.....the_aggreg
-00000890: 6174 6f72 5f70 726f 6365 6475 7265 7211  ator_procedurer.
-000008a0: 0000 0072 0e00 0000 7212 0000 00da 0961  ...r....r......a
-000008b0: 6476 656e 7475 7265 2300 0000 738c 0000  dventure#...s...
-000008c0: 0008 0104 010e 0108 090c 0402 0102 0102  ................
-000008d0: 0106 fe08 0510 0208 010a 0110 fe0e 0910  ................
-000008e0: 0510 0110 0810 0210 0210 0110 0210 0110  ................
-000008f0: 0110 020e 0608 0104 0102 0206 0102 0108  ................
-00000900: fe02 0502 0102 0106 fe02 0602 0302 0106  ................
-00000910: ff08 0408 0102 0302 0102 0202 0202 0102  ................
-00000920: 0202 0102 0502 0202 0202 0302 0104 fe04  ................
-00000930: ee06 fe08 1b08 0108 0208 0208 0108 0202  ................
-00000940: 0102 0102 0104 fe02 030a fd04 ff72 3d00  .............r=.
-00000950: 0000 291a 7235 0000 00da 2462 696f 7465  ..).r5....$biote
-00000960: 6368 2e70 726f 6365 6475 7265 732e 696e  ch.procedures.in
-00000970: 7472 6f2e 7072 6f63 6573 732e 6b65 6772  tro.process.kegr
-00000980: 0200 0000 da2a 6269 6f74 6563 682e 7072  .....*biotech.pr
-00000990: 6f63 6564 7572 6573 2e69 6e74 726f 2e70  ocedures.intro.p
-000009a0: 726f 6365 7373 2e76 6172 6961 626c 6573  rocess.variables
-000009b0: 7203 0000 00da 1e62 696f 7465 6368 2e74  r......biotech.t
-000009c0: 6f70 6963 732e 7072 696e 746f 7574 2e70  opics.printout.p
-000009d0: 6173 7365 7372 0400 0000 da1c 6269 6f74  assesr......biot
-000009e0: 6563 682e 746f 7069 6373 2e73 686f 772e  ech.topics.show.
-000009f0: 7661 7269 6162 6c65 7205 0000 00da 2a62  variabler.....*b
-00000a00: 696f 7465 6368 2e70 726f 6365 6475 7265  iotech.procedure
-00000a10: 732e 6167 6772 6567 6174 6f72 5f70 726f  s.aggregator_pro
-00000a20: 6365 6475 7265 2e6f 6e72 0600 0000 da3d  cedure.onr.....=
-00000a30: 6269 6f74 6563 682e 7072 6f63 6564 7572  biotech.procedur
-00000a40: 6573 2e69 6e74 726f 2e70 726f 6365 7373  es.intro.process
-00000a50: 2e63 6f6d 732e 6167 6772 6567 6174 6f72  .coms.aggregator
-00000a60: 5f70 726f 6365 6475 7265 2e6f 6e72 0700  _procedure.onr..
-00000a70: 0000 da45 6269 6f74 6563 682e 7072 6f63  ...Ebiotech.proc
-00000a80: 6564 7572 6573 2e69 6e74 726f 2e70 726f  edures.intro.pro
-00000a90: 6365 7373 2e63 6f6d 732e 6167 6772 6567  cess.coms.aggreg
-00000aa0: 6174 6f72 5f70 726f 6365 6475 7265 2e73  ator_procedure.s
-00000ab0: 656e 645f 7061 7468 7372 0800 0000 7238  end_pathsr....r8
-00000ac0: 0000 00da 046a 736f 6eda 0770 6174 686c  .....json..pathl
-00000ad0: 6962 da07 6f73 2e70 6174 6872 0900 0000  ib..os.pathr....
-00000ae0: 720a 0000 0072 0b00 0000 7230 0000 0072  r....r....r0...r
-00000af0: 2e00 0000 7236 0000 0072 3d00 0000 7211  ....r6...r=...r.
-00000b00: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-00000b10: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000b20: 7322 0000 0008 010c 050c 010c 030c 010c  s"..............
-00000b30: 020c 020c 0108 0308 0108 0114 0108 0108  ................
-00000b40: 0108 0102 040c 05                        .......
+000001e0: 0164 0284 087d 0074 0264 0364 0464 058d  .d...}.t.d.d.d..
+000001f0: 0201 0074 036a 04a0 0564 06a1 017d 0174  ...t.j...d...}.t
+00000200: 067c 017c 0064 078d 027d 0274 0264 0864  .|.|.d...}.t.d.d
+00000210: 0464 058d 0201 0074 0774 0864 0919 0083  .d.....t.t.d....
+00000220: 0174 096b 0372 3e74 0a64 0a83 0101 0074  .t.k.r>t.d.....t
+00000230: 0ba0 0c64 0ba1 0101 0074 0774 0864 0919  ...d.....t.t.d..
+00000240: 0083 0174 096b 0373 2d74 0864 0919 00a0  ...t.k.s-t.d....
+00000250: 0564 0ca1 017d 0374 0864 0919 00a0 0564  .d...}.t.d.....d
+00000260: 0d64 0ea1 027d 0474 0864 0919 00a0 0564  .d...}.t.d.....d
+00000270: 0f64 10a1 027d 0574 0864 0919 00a0 0564  .d...}.t.d.....d
+00000280: 1164 12a1 027d 0674 0864 0919 00a0 0564  .d...}.t.d.....d
+00000290: 1364 14a1 027d 0774 0864 0919 00a0 0564  .d...}.t.d.....d
+000002a0: 1564 14a1 027d 0874 0864 0919 00a0 0564  .d...}.t.d.....d
+000002b0: 1667 00a1 027d 0974 0864 0919 00a0 0564  .g...}.t.d.....d
+000002c0: 1764 18a1 027d 0a74 0864 0919 00a0 0564  .d...}.t.d.....d
+000002d0: 1964 14a1 027d 0b74 0864 0919 00a0 0564  .d...}.t.d.....d
+000002e0: 1a64 1ba1 027d 0c74 0864 0919 00a0 0564  .d...}.t.d.....d
+000002f0: 1c64 1da1 027d 0d74 0d6a 0d7c 0364 1e64  .d...}.t.j.|.d.d
+00000300: 1f8d 027d 0e74 0e7c 0883 017d 087c 067d  ...}.t.|...}.|.}
+00000310: 0f74 0274 0864 0919 007c 0e64 209c 0283  .t.t.d...|.d ...
+00000320: 0101 0074 0f7c 0569 0064 218d 027d 1009  ...t.|.i.d!..}..
+00000330: 0074 107c 0564 228d 0101 007c 0f64 126b  .t.|.d"....|.d.k
+00000340: 0572 c174 0264 2364 0464 058d 0201 0074  .r.t.d#d.d.....t
+00000350: 117c 057c 0e7c 087c 097c 0b7c 0c7c 0a7c  .|.|.|.|.|.|.|.|
+00000360: 0d7c 0f7c 0464 2464 259c 0264 269c 0964  .|.|.d$d%..d&..d
+00000370: 218d 0201 007c 0f64 126b 0572 de74 0264  !....|.d.k.r.t.d
+00000380: 2764 0464 058d 0201 0088 01a0 12a1 0001  'd.d............
+00000390: 0074 0264 2864 0464 058d 0201 0074 027c  .t.d(d.d.....t.|
+000003a0: 1088 0064 299c 0264 2a64 058d 0201 0064  ...d)..d*d.....d
+000003b0: 0053 0029 2b4e 6301 0000 0000 0000 0000  .S.)+Nc.........
+000003c0: 0000 0001 0000 0004 0000 0013 0000 0073  ...............s
+000003d0: 1c00 0000 7c00 8900 7400 6401 6402 6403  ....|...t.d.d.d.
+000003e0: 8d02 0100 8801 a001 a100 0100 6400 5300  ............d.S.
+000003f0: 2904 4e7a 2468 6561 6c74 685f 7363 616e  ).Nz$health_scan
+00000400: 735f 646f 6e65 2c20 6f70 656e 696e 6720  s_done, opening 
+00000410: 7468 6520 646f 6f72 2eda 0963 6f6e 6465  the door...conde
+00000420: 6e73 6564 a901 da04 6d6f 6465 2902 7205  nsed....mode).r.
+00000430: 0000 00da 0373 6574 2901 da0a 7468 655f  .....set)...the_
+00000440: 7061 636b 6574 a902 da10 7468 655f 7363  packet....the_sc
+00000450: 616e 5f72 6573 756c 7473 da1c 7761 6974  an_results..wait
+00000460: 5f75 6e74 696c 5f68 6561 6c74 685f 7363  _until_health_sc
+00000470: 616e 735f 646f 6e65 a900 fa44 2f62 696f  ans_done...D/bio
+00000480: 7465 6368 2f76 656e 7565 732f 7374 6167  tech/venues/stag
+00000490: 6573 2f62 696f 7465 6368 2f70 726f 6365  es/biotech/proce
+000004a0: 6475 7265 732f 696e 7472 6f2f 7072 6f63  dures/intro/proc
+000004b0: 6573 732f 6164 7665 6e74 7572 652e 7079  ess/adventure.py
+000004c0: da11 6865 616c 7468 5f73 6361 6e73 5f64  ..health_scans_d
+000004d0: 6f6e 6526 0000 0073 0600 0000 0403 0c02  one&...s........
+000004e0: 0c01 7a24 6164 7665 6e74 7572 652e 3c6c  ..z$adventure.<l
+000004f0: 6f63 616c 733e 2e68 6561 6c74 685f 7363  ocals>.health_sc
+00000500: 616e 735f 646f 6e65 7a1b 6162 6f75 7420  ans_donez.about 
+00000510: 746f 2073 7461 7274 2069 6e74 726f 2068  to start intro h
+00000520: 6172 626f 7272 0c00 0000 720d 0000 00da  arborr....r.....
+00000530: 0f69 6e74 726f 5f71 7561 795f 706f 7274  .intro_quay_port
+00000540: 2902 da04 706f 7274 7216 0000 007a 1469  )...portr....z.i
+00000550: 6e74 726f 2068 6172 626f 7220 7374 6172  ntro harbor star
+00000560: 7465 64da 0670 6163 6b65 747a 1577 6169  ted..packetz.wai
+00000570: 7469 6e67 2066 6f72 2076 6172 6961 626c  ting for variabl
+00000580: 6573 6733 3333 3333 33d3 3fda 0b67 6c6f  esg333333.?..glo
+00000590: 625f 7374 7269 6e67 da0a 696e 7472 6f5f  b_string..intro_
+000005a0: 706f 7274 69d2 cc00 00da 1961 6767 7265  porti......aggre
+000005b0: 6761 746f 725f 7072 6f63 6564 7572 655f  gator_procedure_
+000005c0: 706f 7274 69d3 cc00 00da 0772 6563 6f72  porti......recor
+000005d0: 6473 e903 0000 00da 0c64 625f 6469 7265  ds.......db_dire
+000005e0: 6374 6f72 7946 da0d 7265 6c61 7469 7665  ctoryF..relative
+000005f0: 5f70 6174 68da 0c6d 6f64 756c 655f 7061  _path..module_pa
+00000600: 7468 73da 1261 6767 7265 6761 7469 6f6e  ths..aggregation
+00000610: 5f66 6f72 6d61 74e9 0100 0000 da0c 7369  _format.......si
+00000620: 6d75 6c74 616e 656f 7573 da15 7369 6d75  multaneous..simu
+00000630: 6c74 616e 656f 7573 5f63 6170 6163 6974  ltaneous_capacit
+00000640: 79e9 0a00 0000 da0a 7469 6d65 5f6c 696d  y.......time_lim
+00000650: 6974 da17 3939 3939 3939 3939 3939 3939  it..999999999999
+00000660: 3939 3939 3939 3939 3939 3954 2901 da09  99999999999T)...
+00000670: 7265 6375 7273 6976 6529 027a 1267 6f74  recursive).z.got
+00000680: 2074 6865 2076 6172 6961 626c 6573 3ada   the variables:.
+00000690: 0566 696e 6473 2902 7218 0000 0072 1900  .finds).r....r..
+000006a0: 0000 2901 7218 0000 007a 2474 6865 2061  ..).r....z$the a
+000006b0: 6767 7265 6761 746f 7220 7072 6f63 6564  ggregator proced
+000006c0: 7572 6520 6861 7320 7374 6172 7465 647a  ure has startedz
+000006d0: 0730 2e30 2e30 2e30 2902 7218 0000 00da  .0.0.0.0).r.....
+000006e0: 0468 6f73 7429 09da 1273 7461 7475 735f  .host)...status_
+000006f0: 6368 6563 6b5f 7061 7468 7372 2000 0000  check_pathsr ...
+00000700: 7221 0000 0072 2400 0000 7225 0000 0072  r!...r$...r%...r
+00000710: 2200 0000 7227 0000 00da 0d72 6563 6f72  "...r'.....recor
+00000720: 6473 5f6c 6576 656c da10 7468 655f 696e  ds_level..the_in
+00000730: 7472 6f5f 6861 7262 6f72 7a2d 7061 7468  tro_harborz-path
+00000740: 7320 7365 6e74 2c20 7761 6974 696e 6720  s sent, waiting 
+00000750: 756e 7469 6c20 7468 6520 7363 616e 7320  until the scans 
+00000760: 6172 6520 646f 6e65 2e7a 1e64 6f6e 6520  are done.z.done 
+00000770: 6177 6169 7469 6e67 2074 6865 2068 6561  awaiting the hea
+00000780: 6c74 6820 7363 616e 7329 027a 2774 6865  lth scans).z'the
+00000790: 5f61 6767 7265 6761 746f 725f 7072 6f63  _aggregator_proc
+000007a0: 6564 7572 6520 6166 7465 7220 7374 6f70  edure after stop
+000007b0: 7065 643a 7a17 696e 7472 6f3a 2074 6865  ped:z.intro: the
+000007c0: 5f73 6361 6e5f 7265 7375 6c74 73da 0473  _scan_results..s
+000007d0: 686f 7729 13da 0974 6872 6561 6469 6e67  how)...threading
+000007e0: da05 4576 656e 7472 0500 0000 da02 6f73  ..Eventr......os
+000007f0: da07 656e 7669 726f 6eda 0367 6574 7202  ..environ..getr.
+00000800: 0000 00da 0474 7970 6572 0300 0000 da04  .....typer......
+00000810: 6469 6374 da05 7072 696e 74da 0474 696d  dict..print..tim
+00000820: 65da 0573 6c65 6570 da04 676c 6f62 da03  e..sleep..glob..
+00000830: 7374 7272 0600 0000 7207 0000 0072 0800  strr....r....r..
+00000840: 0000 da04 7761 6974 2911 7216 0000 0072  ....wait).r....r
+00000850: 1800 0000 da06 6861 7262 6f72 721a 0000  ......harborr...
+00000860: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
+00000870: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
+00000880: 2200 0000 7224 0000 0072 2500 0000 7227  "...r$...r%...r'
+00000890: 0000 0072 2a00 0000 722d 0000 00da 1874  ...r*...r-.....t
+000008a0: 6865 5f61 6767 7265 6761 746f 725f 7072  he_aggregator_pr
+000008b0: 6f63 6564 7572 6572 1400 0000 7211 0000  ocedurer....r...
+000008c0: 0072 1500 0000 da09 6164 7665 6e74 7572  .r......adventur
+000008d0: 6523 0000 0073 8600 0000 0801 0401 0e01  e#...s..........
+000008e0: 0c09 0c02 0201 0201 0201 06fe 0c05 1002  ................
+000008f0: 0801 0a01 10fe 0e09 1005 1001 1008 1002  ................
+00000900: 1002 1001 1002 1001 1001 1002 0e06 0801  ................
+00000910: 0401 0202 0601 0201 08fe 0205 0201 0201  ................
+00000920: 06fe 0206 0203 0201 06ff 0804 0c01 0203  ................
+00000930: 0201 0202 0202 0201 0202 0201 0205 0202  ................
+00000940: 0202 0203 0201 04fe 04ee 06fe 081b 0c01  ................
+00000950: 0802 0c02 0202 0201 0201 04fe 0203 0afd  ................
+00000960: 723f 0000 0029 1a72 3700 0000 da24 6269  r?...).r7....$bi
+00000970: 6f74 6563 682e 7072 6f63 6564 7572 6573  otech.procedures
+00000980: 2e69 6e74 726f 2e70 726f 6365 7373 2e6b  .intro.process.k
+00000990: 6567 7202 0000 00da 2a62 696f 7465 6368  egr.....*biotech
+000009a0: 2e70 726f 6365 6475 7265 732e 696e 7472  .procedures.intr
+000009b0: 6f2e 7072 6f63 6573 732e 7661 7269 6162  o.process.variab
+000009c0: 6c65 7372 0300 0000 da1e 6269 6f74 6563  lesr......biotec
+000009d0: 682e 746f 7069 6373 2e70 7269 6e74 6f75  h.topics.printou
+000009e0: 742e 7061 7373 6573 7204 0000 00da 1c62  t.passesr......b
+000009f0: 696f 7465 6368 2e74 6f70 6963 732e 7368  iotech.topics.sh
+00000a00: 6f77 2e76 6172 6961 626c 6572 0500 0000  ow.variabler....
+00000a10: da2a 6269 6f74 6563 682e 7072 6f63 6564  .*biotech.proced
+00000a20: 7572 6573 2e61 6767 7265 6761 746f 725f  ures.aggregator_
+00000a30: 7072 6f63 6564 7572 652e 6f6e 7206 0000  procedure.onr...
+00000a40: 00da 3d62 696f 7465 6368 2e70 726f 6365  ..=biotech.proce
+00000a50: 6475 7265 732e 696e 7472 6f2e 7072 6f63  dures.intro.proc
+00000a60: 6573 732e 636f 6d73 2e61 6767 7265 6761  ess.coms.aggrega
+00000a70: 746f 725f 7072 6f63 6564 7572 652e 6f6e  tor_procedure.on
+00000a80: 7207 0000 00da 4562 696f 7465 6368 2e70  r.....Ebiotech.p
+00000a90: 726f 6365 6475 7265 732e 696e 7472 6f2e  rocedures.intro.
+00000aa0: 7072 6f63 6573 732e 636f 6d73 2e61 6767  process.coms.agg
+00000ab0: 7265 6761 746f 725f 7072 6f63 6564 7572  regator_procedur
+00000ac0: 652e 7365 6e64 5f70 6174 6873 7208 0000  e.send_pathsr...
+00000ad0: 0072 3a00 0000 da04 6a73 6f6e da07 7061  .r:.....json..pa
+00000ae0: 7468 6c69 62da 076f 732e 7061 7468 7209  thlib..os.pathr.
+00000af0: 0000 0072 0a00 0000 720b 0000 0072 3200  ...r....r....r2.
+00000b00: 0000 7230 0000 0072 3800 0000 723f 0000  ..r0...r8...r?..
+00000b10: 0072 1400 0000 7214 0000 0072 1400 0000  .r....r....r....
+00000b20: 7215 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000b30: 0000 0073 2200 0000 0801 0c05 0c01 0c03  ...s"...........
+00000b40: 0c01 0c02 0c02 0c01 0803 0801 0801 1401  ................
+00000b50: 0801 0801 0801 0204 0c05                 ..........
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/adventure.py` & `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/adventure.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,29 +36,27 @@
 	wait_until_health_scans_done = threading.Event ()
 	the_scan_results = {}
 	def health_scans_done (the_packet):
 		nonlocal the_scan_results;
 		
 		the_scan_results = the_packet
 	
-		show_variable ("health_scans_done, opening the door.")
+		show_variable ("health_scans_done, opening the door.", mode = "condensed")
 		wait_until_health_scans_done.set ()
 
 
-	show_variable ("""about to start intro harbor""")
-
-	#raise Exception ("!!!!!!!!!!!!!!!!!!!!!!!")
+	show_variable ("""about to start intro harbor""", mode = "condensed")
 
 	port = os.environ.get ('intro_quay_port')
 	harbor = open_harbor (
 		port = port,
 		health_scans_done = health_scans_done
 	)
 
-	show_variable ("""intro harbor started""")
+	show_variable ("""intro harbor started""", mode = "condensed")
 	
 	while type (intro_variables ["packet"]) != dict:
 		print ("waiting for variables")
 		time.sleep (.3)
 		
 		
 	#----
@@ -108,22 +106,22 @@
 	the_aggregator_procedure = aggregator_procedure_on (	
 		port = aggregator_procedure_port,
 		packet = {}
 	)
 	
 	
 	'''
-		check if the implicit procedure is on
+		check if the aggregator is on
 	'''
 	await_aggregator_procedure_is_on (
 		port = aggregator_procedure_port
 	)
 	
 	if (records_level >= 3):
-		show_variable ("the aggregator procedure has started")
+		show_variable ("the aggregator procedure has started", mode = "condensed")
 
 	
 	send_paths_to_aggregator (
 		port = aggregator_procedure_port,
 		packet = {
 			"status_check_paths": finds,
 			
@@ -146,26 +144,26 @@
 				"port": intro_port,
 				"host": "0.0.0.0"
 			}
 		}
 	)	
 
 	if (records_level >= 3):
-		show_variable ("paths sent, waiting until the scans are done.")
+		show_variable ("paths sent, waiting until the scans are done.", mode = "condensed")
 	
 	wait_until_health_scans_done.wait ()
 
-	if (records_level >= 3):
-		show_variable ("done awaiting the health scans")
+	show_variable ("done awaiting the health scans", mode = "condensed")
 	
-	if (records_level >= 3):
-		show_variable ({
-			"the_aggregator_procedure after stopped:": the_aggregator_procedure,
-			"intro: the_scan_results": the_scan_results 
-		}, mode = "show")
+	show_variable ({
+		"the_aggregator_procedure after stopped:": the_aggregator_procedure,
+		"intro: the_scan_results": the_scan_results 
+	}, mode = "show")
+
 
 	
+
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 16:26:14 2024 UTC, .py size: 901 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 269b 2266 8503 0000  o.......&."f....
+00000000: 6f0d 0d0a 0000 0000 1fde 2266 bf03 0000  o........."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 5a00 6401 6402 6c01 6d02 0200 0100 6d03  Z.d.d.l.m.....m.
 00000040: 5a04 0100 6401 6403 6c05 6d06 5a07 0100  Z...d.d.l.m.Z...
 00000050: 6401 6404 6c08 6d09 5a09 0100 6401 6402  d.d.l.m.Z...d.d.
 00000060: 6c0a 5a0a 0905 6408 6406 6407 8401 5a0b  l.Z...d.d.d...Z.
 00000070: 6402 5300 2909 7a98 0a09 6672 6f6d 2062  d.S.).z...from b
@@ -14,67 +14,71 @@
 000000d0: 6365 6475 7265 5f69 735f 6f6e 0a09 6177  cedure_is_on..aw
 000000e0: 6169 745f 6167 6772 6567 6174 6f72 5f70  ait_aggregator_p
 000000f0: 726f 6365 6475 7265 5f69 735f 6f6e 2028  rocedure_is_on (
 00000100: 706f 7274 203d 2030 290a 090a 090a 090a  port = 0).......
 00000110: e900 0000 004e 2901 da08 7072 6573 656e  .....N)...presen
 00000120: 7473 2901 da0d 7368 6f77 5f76 6172 6961  ts)...show_varia
 00000130: 626c 65da 0063 0100 0000 0000 0000 0000  ble..c..........
-00000140: 0000 0300 0000 0700 0000 0300 0000 7332  ..............s2
-00000150: 0000 0074 0064 0183 0101 0087 0066 0164  ...t.d.......f.d
-00000160: 0264 0384 087d 0174 016a 027c 0174 0364  .d...}.t.j.|.t.d
-00000170: 0467 0183 0164 0564 0464 0664 078d 057d  .g...d.d.d.d...}
-00000180: 027c 0253 0029 084e 7a2a 6177 6169 7469  .|.S.).Nz*awaiti
-00000190: 6e67 2074 6865 206f 7065 6e20 6f66 2074  ng the open of t
-000001a0: 6865 2061 6767 7265 6761 746f 7220 6861  he aggregator ha
-000001b0: 7262 6f72 6301 0000 0000 0000 0000 0000  rborc...........
-000001c0: 0003 0000 0008 0000 0013 0000 0073 6600  .............sf.
-000001d0: 0000 7400 6401 8301 0100 7a22 6402 8800  ..t.d.....z"d...
-000001e0: 9b00 6403 9d03 7d01 7401 a002 7c01 a101  ..d...}.t...|...
-000001f0: 7d02 7c02 6a03 6404 6b02 721d 7c02 6a04  }.|.j.d.k.r.|.j.
-00000200: 6405 6b02 7222 5700 6406 5300 5700 7405  d.k.r"W.d.S.W.t.
-00000210: 6407 8301 8201 5700 7405 6407 8301 8201  d.....W.t.d.....
-00000220: 0400 7405 7932 0100 0100 0100 5900 7405  ..t.y2......Y.t.
-00000230: 6407 8301 8201 7700 2908 4e7a 0f09 6368  d.....w.).Nz..ch
-00000240: 6563 6b69 6e67 2069 7320 6f6e 7a0f 6874  ecking is onz.ht
-00000250: 7470 3a2f 2f30 2e30 2e30 2e30 3a7a 032f  tp://0.0.0.0:z./
-00000260: 6f6e e9c8 0000 00da 0379 6573 547a 066e  on.......yesTz.n
-00000270: 6f74 206f 6e29 0672 0300 0000 da08 7265  ot on).r......re
-00000280: 7175 6573 7473 da03 6765 74da 0b73 7461  quests..get..sta
-00000290: 7475 735f 636f 6465 da04 7465 7874 da09  tus_code..text..
-000002a0: 4578 6365 7074 696f 6e29 03da 0361 7267  Exception)...arg
-000002b0: da03 5552 4cda 0872 6573 706f 6e73 65a9  ..URL..response.
-000002c0: 01da 0470 6f72 74a9 00fa 4f2f 6269 6f74  ...port...O/biot
-000002d0: 6563 682f 7665 6e75 6573 2f73 7461 6765  ech/venues/stage
-000002e0: 732f 6269 6f74 6563 682f 7072 6f63 6564  s/biotech/proced
-000002f0: 7572 6573 2f69 6e74 726f 2f63 6f6d 732f  ures/intro/coms/
-00000300: 6167 6772 6567 6174 6f72 5f70 726f 6365  aggregator_proce
-00000310: 6475 7265 2f6f 6e2e 7079 da04 7365 6e64  dure/on.py..send
-00000320: 1500 0000 731c 0000 0008 0102 020c 010a  ....s...........
-00000330: 0114 0106 0102 ff08 0502 fb08 050c fd02  ................
-00000340: 0108 0202 fd7a 2e61 7761 6974 5f61 6767  .....z.await_agg
-00000350: 7265 6761 746f 725f 7072 6f63 6564 7572  regator_procedur
-00000360: 655f 6973 5f6f 6e2e 3c6c 6f63 616c 733e  e_is_on.<locals>
-00000370: 2e73 656e 64e9 0100 0000 e914 0000 0072  .send..........r
-00000380: 0100 0000 2903 da05 6c6f 6f70 73da 0564  ....)...loops..d
-00000390: 656c 6179 da07 7265 636f 7264 7329 0472  elay..records).r
-000003a0: 0300 0000 da0b 6379 636c 655f 6c6f 6f70  ......cycle_loop
-000003b0: 73da 0573 7461 7274 da0e 6379 636c 655f  s..start..cycle_
-000003c0: 7072 6573 656e 7473 2903 7210 0000 0072  presents).r....r
-000003d0: 1300 0000 da0c 7468 655f 7072 6f63 6565  ......the_procee
-000003e0: 6473 7211 0000 0072 0f00 0000 7212 0000  dsr....r....r...
-000003f0: 00da 2061 7761 6974 5f61 6767 7265 6761  .. await_aggrega
-00000400: 746f 725f 7072 6f63 6564 7572 655f 6973  tor_procedure_is
-00000410: 5f6f 6e10 0000 0073 1400 0000 0803 0c02  _on....s........
-00000420: 040e 0201 0801 0203 0201 0202 06f8 040b  ................
-00000430: 721d 0000 0029 0172 0400 0000 290c da07  r....).r....)...
-00000440: 5f5f 646f 635f 5fda 1462 6f74 616e 6973  __doc__..botanis
-00000450: 742e 6379 636c 652e 6c6f 6f70 73da 0563  t.cycle.loops..c
-00000460: 7963 6c65 7216 0000 0072 1900 0000 da17  ycler....r......
-00000470: 626f 7461 6e69 7374 2e63 7963 6c65 2e70  botanist.cycle.p
-00000480: 7265 7365 6e74 7372 0200 0000 721b 0000  resentsr....r...
-00000490: 00da 1c62 696f 7465 6368 2e74 6f70 6963  ...biotech.topic
-000004a0: 732e 7368 6f77 2e76 6172 6961 626c 6572  s.show.variabler
-000004b0: 0300 0000 7207 0000 0072 1d00 0000 7211  ....r....r....r.
-000004c0: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-000004d0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000004e0: 730e 0000 0004 0112 080c 010c 0108 0202  s...............
-000004f0: 030e ff                                  ...
+00000140: 0000 0300 0000 0700 0000 0300 0000 7336  ..............s6
+00000150: 0000 0074 0064 0164 0264 038d 0201 0087  ...t.d.d.d......
+00000160: 0066 0164 0464 0584 087d 0174 016a 027c  .f.d.d...}.t.j.|
+00000170: 0174 0364 0667 0183 0164 0764 0664 0864  .t.d.g...d.d.d.d
+00000180: 098d 057d 027c 0253 0029 0a4e 7a2a 6177  ...}.|.S.).Nz*aw
+00000190: 6169 7469 6e67 2074 6865 206f 7065 6e20  aiting the open 
+000001a0: 6f66 2074 6865 2061 6767 7265 6761 746f  of the aggregato
+000001b0: 7220 6861 7262 6f72 da09 636f 6e64 656e  r harbor..conden
+000001c0: 7365 64a9 01da 046d 6f64 6563 0100 0000  sed....modec....
+000001d0: 0000 0000 0000 0000 0300 0000 0800 0000  ................
+000001e0: 1300 0000 736a 0000 0074 0064 0164 0264  ....sj...t.d.d.d
+000001f0: 038d 0201 007a 2264 0488 009b 0064 059d  .....z"d.....d..
+00000200: 037d 0174 01a0 027c 01a1 017d 027c 026a  .}.t...|...}.|.j
+00000210: 0364 066b 0272 1f7c 026a 0464 076b 0272  .d.k.r.|.j.d.k.r
+00000220: 2457 0064 0853 0057 0074 0564 0983 0182  $W.d.S.W.t.d....
+00000230: 0157 0074 0564 0983 0182 0104 0074 0579  .W.t.d.......t.y
+00000240: 3401 0001 0001 0059 0074 0564 0983 0182  4......Y.t.d....
+00000250: 0177 0029 0a4e 7a21 0963 6865 636b 696e  .w.).Nz!.checkin
+00000260: 6720 6966 2074 6865 2061 6767 7265 6761  g if the aggrega
+00000270: 746f 7220 6973 206f 6e72 0500 0000 7206  tor is onr....r.
+00000280: 0000 007a 0f68 7474 703a 2f2f 302e 302e  ...z.http://0.0.
+00000290: 302e 303a 7a03 2f6f 6ee9 c800 0000 da03  0.0:z./on.......
+000002a0: 7965 7354 7a06 6e6f 7420 6f6e 2906 7203  yesTz.not on).r.
+000002b0: 0000 00da 0872 6571 7565 7374 73da 0367  .....requests..g
+000002c0: 6574 da0b 7374 6174 7573 5f63 6f64 65da  et..status_code.
+000002d0: 0474 6578 74da 0945 7863 6570 7469 6f6e  .text..Exception
+000002e0: 2903 da03 6172 67da 0355 524c da08 7265  )...arg..URL..re
+000002f0: 7370 6f6e 7365 a901 da04 706f 7274 a900  sponse....port..
+00000300: fa57 2f62 696f 7465 6368 2f76 656e 7565  .W/biotech/venue
+00000310: 732f 7374 6167 6573 2f62 696f 7465 6368  s/stages/biotech
+00000320: 2f70 726f 6365 6475 7265 732f 696e 7472  /procedures/intr
+00000330: 6f2f 7072 6f63 6573 732f 636f 6d73 2f61  o/process/coms/a
+00000340: 6767 7265 6761 746f 725f 7072 6f63 6564  ggregator_proced
+00000350: 7572 652f 6f6e 2e70 79da 0473 656e 6415  ure/on.py..send.
+00000360: 0000 0073 1c00 0000 0c01 0202 0c01 0a01  ...s............
+00000370: 1401 0601 02ff 0805 02fb 0805 0cfd 0201  ................
+00000380: 0802 02fd 7a2e 6177 6169 745f 6167 6772  ....z.await_aggr
+00000390: 6567 6174 6f72 5f70 726f 6365 6475 7265  egator_procedure
+000003a0: 5f69 735f 6f6e 2e3c 6c6f 6361 6c73 3e2e  _is_on.<locals>.
+000003b0: 7365 6e64 e901 0000 00e9 1400 0000 7201  send..........r.
+000003c0: 0000 0029 03da 056c 6f6f 7073 da05 6465  ...)...loops..de
+000003d0: 6c61 79da 0772 6563 6f72 6473 2904 7203  lay..records).r.
+000003e0: 0000 00da 0b63 7963 6c65 5f6c 6f6f 7073  .....cycle_loops
+000003f0: da05 7374 6172 74da 0e63 7963 6c65 5f70  ..start..cycle_p
+00000400: 7265 7365 6e74 7329 0372 1300 0000 7216  resents).r....r.
+00000410: 0000 00da 0c74 6865 5f70 726f 6365 6564  .....the_proceed
+00000420: 7372 1400 0000 7212 0000 0072 1500 0000  sr....r....r....
+00000430: da20 6177 6169 745f 6167 6772 6567 6174  . await_aggregat
+00000440: 6f72 5f70 726f 6365 6475 7265 5f69 735f  or_procedure_is_
+00000450: 6f6e 1000 0000 7314 0000 000c 030c 0204  on....s.........
+00000460: 0e02 0108 0102 0302 0102 0206 f804 0b72  ...............r
+00000470: 2000 0000 2901 7204 0000 0029 0cda 075f   ...).r....)..._
+00000480: 5f64 6f63 5f5f da14 626f 7461 6e69 7374  _doc__..botanist
+00000490: 2e63 7963 6c65 2e6c 6f6f 7073 da05 6379  .cycle.loops..cy
+000004a0: 636c 6572 1900 0000 721c 0000 00da 1762  cler....r......b
+000004b0: 6f74 616e 6973 742e 6379 636c 652e 7072  otanist.cycle.pr
+000004c0: 6573 656e 7473 7202 0000 0072 1e00 0000  esentsr....r....
+000004d0: da1c 6269 6f74 6563 682e 746f 7069 6373  ..biotech.topics
+000004e0: 2e73 686f 772e 7661 7269 6162 6c65 7203  .show.variabler.
+000004f0: 0000 0072 0a00 0000 7220 0000 0072 1400  ...r....r ...r..
+00000500: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00000510: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000520: 0e00 0000 0401 1208 0c01 0c01 0802 0203  ................
+00000530: 0eff                                     ..
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py` & `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from biotech.topics.show.variable import show_variable
 
 import requests
 
 def await_aggregator_procedure_is_on (
 	port = ""
 ):
-	show_variable ("awaiting the open of the aggregator harbor")
+	show_variable ("awaiting the open of the aggregator harbor", mode = "condensed")
 
 	def send (arg):
-		show_variable ('	checking is on')
+		show_variable ('	checking if the aggregator is on', mode = "condensed")
 	
 		try:
 			URL = f"http://0.0.0.0:{ port }/on"
 			response = requests.get (URL)
 			if (response.status_code == 200 and response.text == "yes"):
 				return True;
 		except Exception:
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py` & `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/keg/__init__.py` & `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/keg/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,21 +116,19 @@
 		coms with aggregator
 	'''	
 	#
 	#	for the aggregator to send the report
 	#
 	@app.route ("/done", methods = [ 'PATCH' ])
 	def done_patch ():
-		print ("@ [patch] /done")
+		show_variable ("intro_harbor got /done", mode = "condensed")
 	
 		the_packet = json.loads (request.data.decode ('utf8'))
 			
-		show_variable ({
-			"intro harbor /done: the_packet": the_packet
-		})
+		show_variable ("intro_harbor /done, packet parsed", mode = "condensed")
 	
 		intro_variables ["the_report"] = the_packet
 		intro_variables ["the_report_is_ready"] = "yes"
 	
 	
 		'''
 			This might stop the intro process or something....
```

### Comparing `biotech-1.1.1/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 19:04:01 2024 UTC, .py size: 3047 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 21c0 2266 e70b 0000  o.......!."f....
+00000000: 6f0d 0d0a 0000 0000 c0db 2266 0c0c 0000  o........."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
 00000030: 5a00 0900 6401 6402 6c01 6d02 5a02 0100  Z...d.d.l.m.Z...
 00000040: 6401 6403 6c03 6d04 5a04 0100 6401 6404  d.d.l.m.Z...d.d.
 00000050: 6c05 5a05 6401 6404 6c06 5a06 6401 6404  l.Z.d.d.l.Z.d.d.
 00000060: 6c07 5a07 6401 6405 6c08 6d09 5a09 6d0a  l.Z.d.d.l.m.Z.m.
 00000070: 5a0a 6d0b 5a0b 0100 6401 6404 6c0c 5a0c  Z.m.Z...d.d.l.Z.
@@ -119,73 +119,74 @@
 00000760: 6f72 7429 0272 0b00 0000 7203 0000 0072  ort).r....r....r
 00000770: 0c00 0000 720c 0000 0072 0c00 0000 720f  ....r....r....r.
 00000780: 0000 0072 2b00 0000 6e00 0000 7302 0000  ...r+...n...s...
 00000790: 000c 027a 1f6f 7065 6e5f 6861 7262 6f72  ...z.open_harbor
 000007a0: 2e3c 6c6f 6361 6c73 3e2e 7468 655f 7265  .<locals>.the_re
 000007b0: 706f 7274 7a05 2f64 6f6e 6563 0000 0000  portz./donec....
 000007c0: 0000 0000 0000 0000 0100 0000 0500 0000  ................
-000007d0: 5300 0000 733c 0000 0074 0064 0183 0101  S...s<...t.d....
-000007e0: 0074 01a0 0274 036a 04a0 0564 02a1 01a1  .t...t.j...d....
-000007f0: 017d 0074 0664 037c 0069 0183 0101 007c  .}.t.d.|.i.....|
-00000800: 0074 0764 043c 0064 0574 0764 063c 0009  .t.d.<.d.t.d.<..
-00000810: 0064 0753 0029 084e 7a0f 4020 5b70 6174  .d.S.).Nz.@ [pat
-00000820: 6368 5d20 2f64 6f6e 6572 1b00 0000 7a1e  ch] /doner....z.
-00000830: 696e 7472 6f20 6861 7262 6f72 202f 646f  intro harbor /do
-00000840: 6e65 3a20 7468 655f 7061 636b 6574 722b  ne: the_packetr+
-00000850: 0000 0072 1900 0000 7229 0000 0072 1f00  ...r....r)...r..
-00000860: 0000 2908 da05 7072 696e 7472 2000 0000  ..)...printr ...
-00000870: 7221 0000 0072 0a00 0000 7222 0000 0072  r!...r....r"...r
-00000880: 2300 0000 7204 0000 0072 0300 0000 7224  #...r....r....r$
-00000890: 0000 0072 0c00 0000 720c 0000 0072 0f00  ...r....r....r..
-000008a0: 0000 da0a 646f 6e65 5f70 6174 6368 7900  ....done_patchy.
-000008b0: 0000 7312 0000 0008 0212 0202 0204 0106  ..s.............
-000008c0: ff08 0408 0102 0304 097a 1f6f 7065 6e5f  .........z.open_
-000008d0: 6861 7262 6f72 2e3c 6c6f 6361 6c73 3e2e  harbor.<locals>.
-000008e0: 646f 6e65 5f70 6174 6368 6301 0000 0000  done_patchc.....
-000008f0: 0000 0000 0000 0001 0000 0005 0000 0013  ................
-00000900: 0000 0073 1c00 0000 7400 6401 8301 0100  ...s....t.d.....
-00000910: 8800 6a01 6402 8801 6403 6404 8d03 0100  ..j.d...d.d.....
-00000920: 6400 5300 2905 4e7a 0c73 7461 7274 696e  d.S.).Nz.startin
-00000930: 6720 6170 707a 0730 2e30 2e30 2e30 4629  g appz.0.0.0.0F)
-00000940: 02da 0470 6f72 74da 0564 6562 7567 2902  ...port..debug).
-00000950: 722c 0000 00da 0372 756e 2901 da0a 7374  r,.....run)...st
-00000960: 6f70 5f65 7665 6e74 2902 da03 6170 7072  op_event)...appr
-00000970: 2e00 0000 720c 0000 0072 0f00 0000 7227  ....r....r....r'
-00000980: 0000 009e 0000 0073 0c00 0000 0801 0402  .......s........
-00000990: 0201 0201 0201 0afd 2902 da06 7461 7267  ........)...targ
-000009a0: 6574 720d 0000 0054 290b 722c 0000 00da  etr....T).r,....
-000009b0: 0474 7970 65da 0369 6e74 7209 0000 00da  .type..intr.....
-000009c0: 085f 5f6e 616d 655f 5fda 0572 6f75 7465  .__name__..route
-000009d0: da09 7468 7265 6164 696e 67da 0545 7665  ..threading..Eve
-000009e0: 6e74 da06 5468 7265 6164 da06 6461 656d  nt..Thread..daem
-000009f0: 6f6e 7227 0000 0029 0d72 2e00 0000 7226  onr'...).r....r&
-00000a00: 0000 00da 1168 6561 6c74 685f 7363 616e  .....health_scan
-00000a10: 735f 646f 6e65 722b 0000 00da 0f72 6570  s_doner+.....rep
-00000a20: 6f72 745f 6973 5f72 6561 6479 7217 0000  ort_is_readyr...
-00000a30: 0072 1a00 0000 7227 0000 0072 2800 0000  .r....r'...r(...
-00000a40: 722a 0000 0072 2d00 0000 7231 0000 00da  r*...r-...r1....
-00000a50: 0668 6172 626f 7272 0c00 0000 2903 7232  .harborr....).r2
-00000a60: 0000 0072 2e00 0000 7226 0000 0072 0f00  ...r....r&...r..
-00000a70: 0000 da0b 6f70 656e 5f68 6172 626f 7227  ....open_harbor'
-00000a80: 0000 0073 3c00 0000 0a05 0c02 0401 0802  ...s<...........
-00000a90: 0402 0401 1002 0a01 1004 0a01 0203 0e06  ................
-00000aa0: 0e01 0e18 0a01 0e07 0a01 0e07 0a01 0204  ................
-00000ab0: 0e06 0a01 0219 0208 0e03 080b 1001 0601  ................
-00000ac0: 0802 0402 723f 0000 0029 17da 075f 5f64  ....r?...)...__d
-00000ad0: 6f63 5f5f da2a 6269 6f74 6563 682e 7072  oc__.*biotech.pr
-00000ae0: 6f63 6564 7572 6573 2e69 6e74 726f 2e70  ocedures.intro.p
-00000af0: 726f 6365 7373 2e76 6172 6961 626c 6573  rocess.variables
-00000b00: 7203 0000 00da 1c62 696f 7465 6368 2e74  r......biotech.t
-00000b10: 6f70 6963 732e 7368 6f77 2e76 6172 6961  opics.show.varia
-00000b20: 626c 6572 0400 0000 7220 0000 00da 0770  bler....r .....p
-00000b30: 6174 686c 6962 da02 6f73 da07 6f73 2e70  athlib..os..os.p
-00000b40: 6174 6872 0500 0000 7206 0000 0072 0700  athr....r....r..
-00000b50: 0000 da03 7379 73da 0f6d 756c 7469 7072  ....sys..multipr
-00000b60: 6f63 6573 7369 6e67 7208 0000 0072 3800  ocessingr....r8.
-00000b70: 0000 da04 7469 6d65 da05 666c 6173 6b72  ....time..flaskr
-00000b80: 0900 0000 720a 0000 0072 0b00 0000 da04  ....r....r......
-00000b90: 7269 6368 723f 0000 0072 0c00 0000 720c  richr?...r....r.
-00000ba0: 0000 0072 0c00 0000 720f 0000 00da 083c  ...r....r......<
-00000bb0: 6d6f 6475 6c65 3e01 0000 0073 2400 0000  module>....s$...
-00000bc0: 0403 020a 0c06 0c01 0803 0801 0801 1401  ................
-00000bd0: 0801 0c01 0801 0801 1403 0801 0205 0201  ................
-00000be0: 0601 0efd                                ....
+000007d0: 5300 0000 7340 0000 0074 0064 0164 0264  S...s@...t.d.d.d
+000007e0: 038d 0201 0074 01a0 0274 036a 04a0 0564  .....t...t.j...d
+000007f0: 04a1 01a1 017d 0074 0064 0564 0264 038d  .....}.t.d.d.d..
+00000800: 0201 007c 0074 0664 063c 0064 0774 0664  ...|.t.d.<.d.t.d
+00000810: 083c 0009 0064 0953 0029 0a4e 7a16 696e  .<...d.S.).Nz.in
+00000820: 7472 6f5f 6861 7262 6f72 2067 6f74 202f  tro_harbor got /
+00000830: 646f 6e65 da09 636f 6e64 656e 7365 6429  done..condensed)
+00000840: 01da 046d 6f64 6572 1b00 0000 7a21 696e  ...moder....z!in
+00000850: 7472 6f5f 6861 7262 6f72 202f 646f 6e65  tro_harbor /done
+00000860: 2c20 7061 636b 6574 2070 6172 7365 6472  , packet parsedr
+00000870: 2b00 0000 7219 0000 0072 2900 0000 721f  +...r....r)...r.
+00000880: 0000 0029 0772 0400 0000 7220 0000 0072  ...).r....r ...r
+00000890: 2100 0000 720a 0000 0072 2200 0000 7223  !...r....r"...r#
+000008a0: 0000 0072 0300 0000 7224 0000 0072 0c00  ...r....r$...r..
+000008b0: 0000 720c 0000 0072 0f00 0000 da0a 646f  ..r....r......do
+000008c0: 6e65 5f70 6174 6368 7900 0000 730e 0000  ne_patchy...s...
+000008d0: 000c 0212 020c 0208 0208 0102 0304 097a  ...............z
+000008e0: 1f6f 7065 6e5f 6861 7262 6f72 2e3c 6c6f  .open_harbor.<lo
+000008f0: 6361 6c73 3e2e 646f 6e65 5f70 6174 6368  cals>.done_patch
+00000900: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000910: 0005 0000 0013 0000 0073 1c00 0000 7400  .........s....t.
+00000920: 6401 8301 0100 8800 6a01 6402 8801 6403  d.......j.d...d.
+00000930: 6404 8d03 0100 6400 5300 2905 4e7a 0c73  d.....d.S.).Nz.s
+00000940: 7461 7274 696e 6720 6170 707a 0730 2e30  tarting appz.0.0
+00000950: 2e30 2e30 4629 02da 0470 6f72 74da 0564  .0.0F)...port..d
+00000960: 6562 7567 2902 da05 7072 696e 74da 0372  ebug)...print..r
+00000970: 756e 2901 da0a 7374 6f70 5f65 7665 6e74  un)...stop_event
+00000980: 2902 da03 6170 7072 2f00 0000 720c 0000  )...appr/...r...
+00000990: 0072 0f00 0000 7227 0000 009c 0000 0073  .r....r'.......s
+000009a0: 0c00 0000 0801 0402 0201 0201 0201 0afd  ................
+000009b0: 2902 da06 7461 7267 6574 720d 0000 0054  )...targetr....T
+000009c0: 290b 7231 0000 00da 0474 7970 65da 0369  ).r1.....type..i
+000009d0: 6e74 7209 0000 00da 085f 5f6e 616d 655f  ntr......__name_
+000009e0: 5fda 0572 6f75 7465 da09 7468 7265 6164  _..route..thread
+000009f0: 696e 67da 0545 7665 6e74 da06 5468 7265  ing..Event..Thre
+00000a00: 6164 da06 6461 656d 6f6e 7227 0000 0029  ad..daemonr'...)
+00000a10: 0d72 2f00 0000 7226 0000 00da 1168 6561  .r/...r&.....hea
+00000a20: 6c74 685f 7363 616e 735f 646f 6e65 722b  lth_scans_doner+
+00000a30: 0000 00da 0f72 6570 6f72 745f 6973 5f72  .....report_is_r
+00000a40: 6561 6479 7217 0000 0072 1a00 0000 7227  eadyr....r....r'
+00000a50: 0000 0072 2800 0000 722a 0000 0072 2e00  ...r(...r*...r..
+00000a60: 0000 7233 0000 00da 0668 6172 626f 7272  ..r3.....harborr
+00000a70: 0c00 0000 2903 7234 0000 0072 2f00 0000  ....).r4...r/...
+00000a80: 7226 0000 0072 0f00 0000 da0b 6f70 656e  r&...r......open
+00000a90: 5f68 6172 626f 7227 0000 0073 3c00 0000  _harbor'...s<...
+00000aa0: 0a05 0c02 0401 0802 0402 0401 1002 0a01  ................
+00000ab0: 1004 0a01 0203 0e06 0e01 0e18 0a01 0e07  ................
+00000ac0: 0a01 0e07 0a01 0204 0e06 0a01 0217 0208  ................
+00000ad0: 0e03 080b 1001 0601 0802 0402 7241 0000  ............rA..
+00000ae0: 0029 17da 075f 5f64 6f63 5f5f da2a 6269  .)...__doc__.*bi
+00000af0: 6f74 6563 682e 7072 6f63 6564 7572 6573  otech.procedures
+00000b00: 2e69 6e74 726f 2e70 726f 6365 7373 2e76  .intro.process.v
+00000b10: 6172 6961 626c 6573 7203 0000 00da 1c62  ariablesr......b
+00000b20: 696f 7465 6368 2e74 6f70 6963 732e 7368  iotech.topics.sh
+00000b30: 6f77 2e76 6172 6961 626c 6572 0400 0000  ow.variabler....
+00000b40: 7220 0000 00da 0770 6174 686c 6962 da02  r .....pathlib..
+00000b50: 6f73 da07 6f73 2e70 6174 6872 0500 0000  os..os.pathr....
+00000b60: 7206 0000 0072 0700 0000 da03 7379 73da  r....r......sys.
+00000b70: 0f6d 756c 7469 7072 6f63 6573 7369 6e67  .multiprocessing
+00000b80: 7208 0000 0072 3a00 0000 da04 7469 6d65  r....r:.....time
+00000b90: da05 666c 6173 6b72 0900 0000 720a 0000  ..flaskr....r...
+00000ba0: 0072 0b00 0000 da04 7269 6368 7241 0000  .r......richrA..
+00000bb0: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00000bc0: 720f 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000bd0: 0000 0073 2400 0000 0403 020a 0c06 0c01  ...s$...........
+00000be0: 0803 0801 0801 1401 0801 0c01 0801 0801  ................
+00000bf0: 1403 0801 0205 0201 0601 0efd            ............
```

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/aggregate/__init__.py` & `biotech-1.1.2/venues/stages/biotech/topics/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/alarm_parser/__init__.py` & `biotech-1.1.2/venues/stages/biotech/topics/alarm_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__init__.py` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__init__.py` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/basin/treasury.py` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/basin/treasury.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/help_documentation/shares.s.HTML` & `biotech-1.1.2/venues/stages/biotech/topics/help_documentation/shares.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/implicit/proc/__init__.py` & `biotech-1.1.2/venues/stages/biotech/topics/implicit/proc/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/implicit/thread/__init__.py` & `biotech-1.1.2/venues/stages/biotech/topics/implicit/thread/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 '''
 	description:
 		it is inadvisable to stop threads..?
 			https://stackoverflow.com/questions/323972/is-there-any-way-to-kill-a-thread
 '''
 
 '''
+
+	from biotech.topics.implicit.thread import implicit_thread
 	def task (
 		stop_event = None
 	):		
 		while not stop_event.is_set ():
 			time.sleep(1)
 
-	from biotech.topics.implicit.thread import implicit_thread
+	
 	the_task = implicit_thread (
 		task = task
 	)
 	the_task ['on'] ()
 	the_task ['off'] ()
 '''
```

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 18 05:46:33 2024 UTC, .py size: 1155 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b9b3 2066 8304 0000  o......... f....
+00000000: 6f0d 0d0a 0000 0000 b5e0 2266 8604 0000  o........."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 5a00 0900 0900 0900 6401 6402 6c01 5a01  Z.......d.d.l.Z.
 00000040: 6401 6402 6c02 5a02 0902 6405 6403 6404  d.d.l.Z...d.d.d.
 00000050: 8401 5a03 6402 5300 2906 7a14 0a09 6974  ..Z.d.S.).z...it
 00000060: 696e 6572 6172 793a 0a09 095b 205d 200a  inerary:...[ ] .
 00000070: e900 0000 004e 6301 0000 0000 0000 0000  .....Nc.........
@@ -21,34 +21,34 @@
 00000140: 7265 6164 da06 6461 656d 6f6e da05 7374  read..daemon..st
 00000150: 6172 74a9 00a9 03da 0f69 6d70 6c69 6369  art......implici
 00000160: 745f 7468 7265 6164 7202 0000 00da 0474  t_threadr......t
 00000170: 6173 6b72 0900 0000 fa41 2f62 696f 7465  askr.....A/biote
 00000180: 6368 2f76 656e 7565 732f 7374 6167 6573  ch/venues/stages
 00000190: 2f62 696f 7465 6368 2f74 6f70 6963 732f  /biotech/topics/
 000001a0: 696d 706c 6963 6974 2f74 6872 6561 642f  implicit/thread/
-000001b0: 5f5f 696e 6974 5f5f 2e70 79da 026f 6e31  __init__.py..on1
+000001b0: 5f5f 696e 6974 5f5f 2e70 79da 026f 6e33  __init__.py..on3
 000001c0: 0000 0073 0e00 0000 0403 0201 0402 02ff  ...s............
 000001d0: 06fe 0606 0c01 7a1b 696d 706c 6963 6974  ......z.implicit
 000001e0: 5f74 6872 6561 642e 3c6c 6f63 616c 733e  _thread.<locals>
 000001f0: 2e6f 6e63 0000 0000 0000 0000 0000 0000  .onc............
 00000200: 0000 0000 0200 0000 1300 0000 731c 0000  ............s...
 00000210: 0074 0064 0183 0101 0088 01a0 01a1 0001  .t.d............
 00000220: 0088 00a0 02a1 0001 0064 0053 0029 024e  .........d.S.).N
 00000230: 7a14 7374 6f70 7069 6e67 2074 6865 2070  z.stopping the p
 00000240: 726f 6365 7373 2903 da05 7072 696e 74da  rocess)...print.
 00000250: 0373 6574 da04 6a6f 696e 7209 0000 0029  .set..joinr....)
 00000260: 0272 0b00 0000 7202 0000 0072 0900 0000  .r....r....r....
-00000270: 720d 0000 00da 036f 6666 3d00 0000 7306  r......off=...s.
+00000270: 720d 0000 00da 036f 6666 3f00 0000 7306  r......off?...s.
 00000280: 0000 0008 0408 020c 017a 1c69 6d70 6c69  .........z.impli
 00000290: 6369 745f 7468 7265 6164 2e3c 6c6f 6361  cit_thread.<loca
 000002a0: 6c73 3e2e 6f66 6629 0272 0e00 0000 7212  ls>.off).r....r.
 000002b0: 0000 0029 0272 0500 0000 da05 4576 656e  ...).r......Even
 000002c0: 7429 0372 0c00 0000 720e 0000 0072 1200  t).r....r....r..
 000002d0: 0000 7209 0000 0072 0a00 0000 720d 0000  ..r....r....r...
-000002e0: 0072 0b00 0000 2b00 0000 730e 0000 0004  .r....+...s.....
+000002e0: 0072 0b00 0000 2d00 0000 730e 0000 0004  .r....-...s.....
 000002f0: 0308 0110 020e 0c02 0a02 0106 fe72 0b00  .............r..
 00000300: 0000 2901 4e29 04da 075f 5f64 6f63 5f5f  ..).N)...__doc__
 00000310: 7205 0000 00da 0474 696d 6572 0b00 0000  r......timer....
 00000320: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
 00000330: 0d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000340: 0000 7310 0000 0004 0202 0502 0602 0f08  ..s.............
+00000340: 0000 7310 0000 0004 0202 0502 0602 1108  ..s.............
 00000350: 0b08 0102 030e ff                        .......
```

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/printout/passes.py` & `biotech-1.1.2/venues/stages/biotech/topics/printout/passes.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__init__.py` & `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 		the_queue = Queue ()
 		
 	report = {
 		"journal": []
 	}
 	p = pexpect.spawn (
 		process_string,
+		
 		cwd = CWD,
 		env = env,
 		timeout = None,
 		
 		# encoding='utf-8'
 	)
 	def awareness_EOF (p):
```

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 18:50:11 2024 UTC, .py size: 2163 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e3bc 2266 7308 0000  o........."fs...
+00000000: 6f0d 0d0a 0000 0000 64f2 2266 7608 0000  o.......d."fv...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 0100 6404 6405 8400 5a08 6402 6402 6900  ..d.d...Z.d.d.i.
 00000070: 6406 6402 6605 6407 6408 8401 5a09 6402  d.d.f.d.d...Z.d.
@@ -89,15 +89,15 @@
 00000580: 5446 385f 7061 7273 6564 da10 6865 7861  TF8_parsed..hexa
 00000590: 6465 6369 6d61 6c5f 6c69 6e65 da12 6865  decimal_line..he
 000005a0: 7861 6465 6369 6d61 6c5f 7061 7273 6564  xadecimal_parsed
 000005b0: da0b 6c69 6e65 5f70 6172 7365 64a9 03da  ..line_parsed...
 000005c0: 046e 616d 65da 0672 6570 6f72 74da 0974  .name..report..t
 000005d0: 6865 5f71 7565 7565 7209 0000 0072 0a00  he_queuer....r..
 000005e0: 0000 da0d 6177 6172 656e 6573 735f 454f  ....awareness_EO
-000005f0: 4649 0000 0073 3a00 0000 0801 0802 0202  FI...s:.........
+000005f0: 464a 0000 0073 3a00 0000 0801 0802 0202  FJ...s:.........
 00000600: 0a01 0804 0c01 0401 0801 02fe 0204 0801  ................
 00000610: 0801 0c01 0401 0801 02fe 0207 0201 04fe  ................
 00000620: 0205 0201 04fe 06fb 0a0b 0e02 0802 1802  ................
 00000630: 0803 10d6 7a21 7072 6f63 6573 735f 6f6e  ....z!process_on
 00000640: 2e3c 6c6f 6361 6c73 3e2e 6177 6172 656e  .<locals>.awaren
 00000650: 6573 735f 454f 467a 1670 6578 7065 6374  ess_EOFz.pexpect
 00000660: 2073 7061 776e 2073 7461 7274 6564 3f29   spawn started?)
@@ -108,16 +108,16 @@
 000006b0: 6973 7465 7272 0b00 0000 2908 da0e 7072  isterr....)...pr
 000006c0: 6f63 6573 735f 7374 7269 6e67 722a 0000  ocess_stringr*..
 000006d0: 00da 0343 5744 720f 0000 0072 2800 0000  ...CWDr....r(...
 000006e0: da0a 7374 6f70 5f65 7665 6e74 7221 0000  ..stop_eventr!..
 000006f0: 0072 2b00 0000 7209 0000 0072 2700 0000  .r+...r....r'...
 00000700: 720a 0000 00da 0a70 726f 6365 7373 5f6f  r......process_o
 00000710: 6e28 0000 0073 2800 0000 0a0b 0805 0801  n(...s(.........
-00000720: 0802 0601 0403 04ff 0403 0201 0201 0201  ................
-00000730: 0201 06fc 1008 082f 0c02 0802 0203 0202  ......./........
+00000720: 0802 0601 0403 04ff 0403 0201 0202 0201  ................
+00000730: 0201 06fb 1009 082f 0c02 0802 0203 0202  ......./........
 00000740: 06fd 7235 0000 0029 0ada 075f 5f64 6f63  ..r5...)...__doc
 00000750: 5f5f 722e 0000 00da 0472 6963 6872 3000  __r......richr0.
 00000760: 0000 722c 0000 00da 0f6d 756c 7469 7072  ..r,.....multipr
 00000770: 6f63 6573 7369 6e67 7202 0000 0072 0300  ocessingr....r..
 00000780: 0000 720b 0000 0072 3500 0000 7209 0000  ..r....r5...r...
 00000790: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
 000007a0: da08 3c6d 6f64 756c 653e 0100 0000 731a  ..<module>....s.
```

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/implicit.py` & `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/process_on/p_expect/parse_records.py` & `biotech-1.1.2/venues/stages/biotech/topics/process_on/p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/quay/garage.py` & `biotech-1.1.2/venues/stages/biotech/topics/quay/garage.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_1.py` & `biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_2.py` & `biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_2.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_3.py` & `biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_3.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/quay/implicit_process_test_4.py` & `biotech-1.1.2/venues/stages/biotech/topics/quay/implicit_process_test_4.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py` & `biotech-1.1.2/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,21 +49,21 @@
 	# Create a queue to collect the results
 	results_queue = Queue ()
 
 	# Create threads to process items
 	threads = []
 	for index, item in enumerate (items):
 		thread = threading.Thread (target=process_with_semaphore, args=(item, index, results_queue))
-		thread.start()
-		threads.append(thread)
+		thread.start ()
+		threads.append (thread)
 
 	# Wait for all threads to complete
 	for thread in threads:
 		thread.join ()
 
 	# Collect results from the queue and reorder them based on the original item order
-	results = [None] * len(items)
-	while not results_queue.empty():
-		index, result = results_queue.get()
-		results[index] = result
+	results = [None] * len (items)
+	while not results_queue.empty ():
+		index, result = results_queue.get ()
+		results [index] = result
 	
 	return results;
```

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 20:48:34 2024 UTC, .py size: 1442 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 22e4 1e66 a205 0000  o......."..f....
+00000000: 6f0d 0d0a 0000 0000 d6f2 2266 a805 0000  o........."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6700  m.Z...d.d.l.Z.g.
 00000050: 6404 6405 6406 8400 6603 6407 6408 8401  d.d.d...f.d.d...
 00000060: 5a05 6402 5300 2909 6161 0100 000a 0966  Z.d.S.).aa.....f
 00000070: 726f 6d20 6269 6f74 6563 682e 6d69 7865  rom biotech.mixe
```

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 19 19:50:39 2024 UTC, .py size: 2305 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0fcb 2266 0109 0000  o........."f....
+00000000: 6f0d 0d0a 0000 0000 60dc 2266 f708 0000  o.......`."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 0900 6401 6402 6c01 5a01 6401 6403  Z...d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 0100 6401 6402 6c04 5a04  l.m.Z...d.d.l.Z.
 00000050: 6401 6404 6c05 6d05 5a05 0100 6401 6402  d.d.l.m.Z...d.d.
 00000060: 6c06 5a06 6401 6402 6c07 5a07 6405 6406  l.Z.d.d.l.Z.d.d.
 00000070: 8400 5a08 640a 6408 6409 8401 5a09 6402  ..Z.d.d.d...Z.d.
@@ -38,74 +38,78 @@
 00000250: 6e61 6d65 da08 665f 6c69 6e65 6e6f da09  name..f_lineno..
 00000260: 7472 6163 6562 6163 6bda 0a65 7874 7261  traceback..extra
 00000270: 6374 5f74 62da 0974 625f 6c69 6e65 6e6f  ct_tb..tb_lineno
 00000280: 2906 da08 6669 6c65 6e61 6d65 da06 6c69  )...filename..li
 00000290: 6e65 6e6f 7208 0000 00da 0865 7863 5f74  nenor......exc_t
 000002a0: 7970 65da 0965 7863 5f76 616c 7565 da0d  ype..exc_value..
 000002b0: 6578 635f 7472 6163 6562 6163 6ba9 0072  exc_traceback..r
-000002c0: 1700 0000 fa36 2f62 696f 7465 6368 2f76  .....6/biotech/v
+000002c0: 1700 0000 fa6e 2f62 696f 7465 6368 2f76  .....n/biotech/v
 000002d0: 656e 7565 732f 7374 6167 6573 2f62 696f  enues/stages/bio
-000002e0: 7465 6368 2f74 6f70 6963 732f 7368 6f77  tech/topics/show
-000002f0: 2f76 6172 6961 626c 652e 7079 da11 6765  /variable.py..ge
-00000300: 745f 6669 6c65 5f61 6e64 5f6c 696e 651b  t_file_and_line.
-00000310: 0000 0073 3200 0000 0401 0401 0202 0601  ...s2...........
-00000320: 0601 0801 0e02 1205 1001 0e03 1401 0204  ................
-00000330: 1201 0c01 0401 02ff 0203 0e01 0c01 0401  ................
-00000340: 02ff 02ff 0804 02fe 0802 7219 0000 00da  ..........r.....
-00000350: 0472 6963 6863 0200 0000 0000 0000 0000  .richc..........
-00000360: 0000 0b00 0000 0b00 0000 4300 0000 7364  ..........C...sd
-00000370: 0100 007a 9964 017d 0264 017d 037a 0374  ...z.d.}.d.}.z.t
-00000380: 0083 0082 0101 0001 0001 0074 01a0 02a1  ...........t....
-00000390: 005c 037d 047d 057d 067a 087c 066a 036a  .\.}.}.}.z.|.j.j
-000003a0: 046a 056a 067d 0257 006e 0904 0074 0079  .j.j.}.W.n...t.y
-000003b0: 2401 0001 0001 0059 006e 0177 007a 077c  $......Y.n.w.z.|
-000003c0: 066a 036a 046a 077d 0357 006e 0904 0074  .j.j.j.}.W.n...t
-000003d0: 0079 3501 0001 0001 0059 006e 0177 0059  .y5......Y.n.w.Y
-000003e0: 007c 0164 026b 0272 4674 087c 007c 027c  .|.d.k.rFt.|.|.|
-000003f0: 0364 039c 0383 0101 0057 0064 0053 007c  .d.......W.d.S.|
-00000400: 0164 046b 0272 7d74 0983 007d 077c 07a0  .d.k.r}t...}.|..
-00000410: 0aa1 008f 0f7d 087c 076a 0b7c 0064 0564  .....}.|.j.|.d.d
-00000420: 068d 0201 0057 0064 0004 0004 0083 0301  .....W.d........
-00000430: 006e 0831 0073 6377 0101 0001 0001 0059  .n.1.scw.......Y
-00000440: 0001 007c 08a0 0ca1 007d 0974 0b7c 029b  ...|.....}.t.|..
-00000450: 0064 077c 039b 0064 089d 047c 0917 0064  .d.|...d...|...d
-00000460: 0564 068d 0201 0057 0064 0053 007c 0164  .d.....W.d.S.|.d
-00000470: 096b 0272 8d74 0da0 0b7c 007c 027c 0364  .k.r.t...|.|.|.d
-00000480: 039c 03a1 0101 0057 0064 0053 0074 0d6a  .......W.d.S.t.j
-00000490: 0e7c 007c 027c 0364 039c 0364 0a8d 0101  .|.|.|.d...d....
-000004a0: 0057 0064 0053 0004 0074 0079 b101 007d  .W.d.S...t.y...}
-000004b0: 0a01 007a 0c74 0b64 0b7c 0a83 0201 0057  ...z.t.d.|.....W
-000004c0: 0059 0064 007d 0a7e 0a64 0053 0064 007d  .Y.d.}.~.d.S.d.}
-000004d0: 0a7e 0a77 0177 0029 0c4e 7204 0000 0072  .~.w.w.).Nr....r
-000004e0: 0300 0000 2903 da08 7661 7269 6162 6c65  ....)...variable
-000004f0: da04 7061 7468 da04 6c69 6e65 da09 636f  ..path..line..co
-00000500: 6e64 656e 7365 64da 0029 01da 0365 6e64  ndensed..)...end
-00000510: fa01 3a7a 023a 20da 0473 686f 7729 01da  ..:z.: ..show)..
-00000520: 0464 6174 617a 1c76 6172 6961 626c 6520  .dataz.variable 
-00000530: 7072 696e 7469 6e67 2065 7863 6570 7469  printing excepti
-00000540: 6f6e 3a29 0f72 0600 0000 7207 0000 0072  on:).r....r....r
-00000550: 0800 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
-00000560: 0000 0072 0d00 0000 720e 0000 0072 0300  ...r....r....r..
-00000570: 0000 7202 0000 00da 0763 6170 7475 7265  ..r......capture
-00000580: 7209 0000 00da 0367 6574 721a 0000 00da  r......getr.....
-00000590: 0a70 7269 6e74 5f6a 736f 6e29 0b72 1b00  .print_json).r..
-000005a0: 0000 da04 6d6f 6465 7212 0000 0072 1300  ....moder....r..
-000005b0: 0000 7214 0000 0072 1500 0000 7216 0000  ..r....r....r...
-000005c0: 00da 0763 6f6e 736f 6c65 7224 0000 00da  ...consoler$....
-000005d0: 0d6f 7574 7075 745f 7374 7269 6e67 da01  .output_string..
-000005e0: 4572 1700 0000 7217 0000 0072 1800 0000  Er....r....r....
-000005f0: da0d 7368 6f77 5f76 6172 6961 626c 653e  ..show_variable>
-00000600: 0000 0073 5c00 0000 0203 0401 0401 0201  ...s\...........
-00000610: 0601 0601 0e01 0202 1001 0c01 0401 02ff  ................
-00000620: 0203 0e01 0c01 0401 02ff 0280 0803 0201  ................
-00000630: 0201 0201 0201 0efd 0806 0601 0a02 1001  ................
-00000640: 1cff 0804 2207 0802 0401 0201 0201 0201  ...."...........
-00000650: 0efd 0407 0201 0201 0201 10fd 0e06 1801  ................
-00000660: 0880 02ff 722b 0000 0029 0172 1a00 0000  ....r+...).r....
-00000670: 290a da07 5f5f 646f 635f 5f72 1a00 0000  )...__doc__r....
-00000680: da0c 7269 6368 2e63 6f6e 736f 6c65 7202  ..rich.consoler.
-00000690: 0000 00da 0769 6e73 7065 6374 7203 0000  .....inspectr...
-000006a0: 0072 0700 0000 720f 0000 0072 1900 0000  .r....r....r....
-000006b0: 722b 0000 0072 1700 0000 7217 0000 0072  r+...r....r....r
-000006c0: 1700 0000 7218 0000 00da 083c 6d6f 6475  ....r......<modu
-000006d0: 6c65 3e01 0000 0073 1400 0000 0401 0205  le>....s........
-000006e0: 0809 0c01 0803 0c01 0801 0801 0804 0e23  ...............#
+000002e0: 7465 6368 2f70 726f 6365 6475 7265 732f  tech/procedures/
+000002f0: 6865 616c 7468 5f73 6361 6e2f 7072 6f63  health_scan/proc
+00000300: 6573 732f 6d6f 6475 6c65 732f 5f5f 6865  ess/modules/__he
+00000310: 616c 7468 5f73 6361 6e5f 7574 696c 6974  alth_scan_utilit
+00000320: 6965 732f 7368 6f77 2f76 6172 6961 626c  ies/show/variabl
+00000330: 652e 7079 da11 6765 745f 6669 6c65 5f61  e.py..get_file_a
+00000340: 6e64 5f6c 696e 651b 0000 0073 3200 0000  nd_line....s2...
+00000350: 0401 0401 0202 0601 0601 0801 0e02 1205  ................
+00000360: 1001 0e03 1401 0204 1201 0c01 0401 02ff  ................
+00000370: 0203 0e01 0c01 0401 02ff 02ff 0804 02fe  ................
+00000380: 0802 7219 0000 00da 0472 6963 6863 0200  ..r......richc..
+00000390: 0000 0000 0000 0000 0000 0b00 0000 0b00  ................
+000003a0: 0000 4300 0000 7360 0100 007a 9764 017d  ..C...s`...z.d.}
+000003b0: 0264 017d 037a 0374 0083 0082 0101 0001  .d.}.z.t........
+000003c0: 0001 0074 01a0 02a1 005c 037d 047d 057d  ...t.....\.}.}.}
+000003d0: 067a 087c 066a 036a 046a 056a 067d 0257  .z.|.j.j.j.j.}.W
+000003e0: 006e 0904 0074 0079 2401 0001 0001 0059  .n...t.y$......Y
+000003f0: 006e 0177 007a 077c 066a 036a 046a 077d  .n.w.z.|.j.j.j.}
+00000400: 0357 006e 0904 0074 0079 3501 0001 0001  .W.n...t.y5.....
+00000410: 0059 006e 0177 0059 007c 0164 026b 0272  .Y.n.w.Y.|.d.k.r
+00000420: 4674 087c 007c 027c 0364 039c 0383 0101  Ft.|.|.|.d......
+00000430: 0057 0064 0053 007c 0164 046b 0272 7b74  .W.d.S.|.d.k.r{t
+00000440: 0983 007d 077c 07a0 0aa1 008f 0f7d 087c  ...}.|.......}.|
+00000450: 076a 0b7c 0064 0564 068d 0201 0057 0064  .j.|.d.d.....W.d
+00000460: 0004 0004 0083 0301 006e 0831 0073 6377  .........n.1.scw
+00000470: 0101 0001 0001 0059 0001 007c 08a0 0ca1  .......Y...|....
+00000480: 007d 0974 0b7c 029b 0064 077c 039b 0064  .}.t.|...d.|...d
+00000490: 089d 047c 0917 0083 0101 0057 0064 0053  ...|.......W.d.S
+000004a0: 007c 0164 096b 0272 8b74 0da0 0b7c 007c  .|.d.k.r.t...|.|
+000004b0: 027c 0364 039c 03a1 0101 0057 0064 0053  .|.d.......W.d.S
+000004c0: 0074 0d6a 0e7c 007c 027c 0364 039c 0364  .t.j.|.|.|.d...d
+000004d0: 0a8d 0101 0057 0064 0053 0004 0074 0079  .....W.d.S...t.y
+000004e0: af01 007d 0a01 007a 0c74 0b64 0b7c 0a83  ...}...z.t.d.|..
+000004f0: 0201 0057 0059 0064 007d 0a7e 0a64 0053  ...W.Y.d.}.~.d.S
+00000500: 0064 007d 0a7e 0a77 0177 0029 0c4e 7204  .d.}.~.w.w.).Nr.
+00000510: 0000 0072 0300 0000 2903 da08 7661 7269  ...r....)...vari
+00000520: 6162 6c65 da04 7061 7468 da04 6c69 6e65  able..path..line
+00000530: da09 636f 6e64 656e 7365 64da 0029 01da  ..condensed..)..
+00000540: 0365 6e64 fa01 3a7a 023a 20da 0473 686f  .end..:z.: ..sho
+00000550: 7729 01da 0464 6174 617a 1c76 6172 6961  w)...dataz.varia
+00000560: 626c 6520 7072 696e 7469 6e67 2065 7863  ble printing exc
+00000570: 6570 7469 6f6e 3a29 0f72 0600 0000 7207  eption:).r....r.
+00000580: 0000 0072 0800 0000 720a 0000 0072 0b00  ...r....r....r..
+00000590: 0000 720c 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+000005a0: 0072 0300 0000 7202 0000 00da 0763 6170  .r....r......cap
+000005b0: 7475 7265 7209 0000 00da 0367 6574 721a  turer......getr.
+000005c0: 0000 00da 0a70 7269 6e74 5f6a 736f 6e29  .....print_json)
+000005d0: 0b72 1b00 0000 da04 6d6f 6465 7212 0000  .r......moder...
+000005e0: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
+000005f0: 7216 0000 00da 0763 6f6e 736f 6c65 7224  r......consoler$
+00000600: 0000 00da 0d6f 7574 7075 745f 7374 7269  .....output_stri
+00000610: 6e67 da01 4572 1700 0000 7217 0000 0072  ng..Er....r....r
+00000620: 1800 0000 da0d 7368 6f77 5f76 6172 6961  ......show_varia
+00000630: 626c 653e 0000 0073 5c00 0000 0203 0401  ble>...s\.......
+00000640: 0401 0201 0601 0601 0e01 0202 1001 0c01  ................
+00000650: 0401 02ff 0203 0e01 0c01 0401 02ff 0280  ................
+00000660: 0803 0201 0201 0201 0201 0efd 0806 0601  ................
+00000670: 0a02 1001 1cff 0804 1e07 0802 0401 0201  ................
+00000680: 0201 0201 0efd 0407 0201 0201 0201 10fd  ................
+00000690: 0e06 1801 0880 02ff 722b 0000 0029 0172  ........r+...).r
+000006a0: 1a00 0000 290a da07 5f5f 646f 635f 5f72  ....)...__doc__r
+000006b0: 1a00 0000 da0c 7269 6368 2e63 6f6e 736f  ......rich.conso
+000006c0: 6c65 7202 0000 00da 0769 6e73 7065 6374  ler......inspect
+000006d0: 7203 0000 0072 0700 0000 720f 0000 0072  r....r....r....r
+000006e0: 1900 0000 722b 0000 0072 1700 0000 7217  ....r+...r....r.
+000006f0: 0000 0072 1700 0000 7218 0000 00da 083c  ...r....r......<
+00000700: 6d6f 6475 6c65 3e01 0000 0073 1400 0000  module>....s....
+00000710: 0401 0205 0809 0c01 0803 0c01 0801 0801  ................
+00000720: 0804 0e23                                ...#
```

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/show/variable.py` & `biotech-1.1.2/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 			output_string = capture.get()
 						
 			#output_string = str (console.render (console.print (variable)))
 			
 			#line = str (lineno)
 			#file = str (filename)
 			
-			print (f"{ filename }:{ lineno }: " + output_string, end = "")
+			print (f"{ filename }:{ lineno }: " + output_string)
 		
 		elif (mode == "show"):
 			rich.print ({
 				"variable": variable,
 				"path": filename,
 				"line": lineno
 			})
```

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc` & `biotech-1.1.2/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/venues/stages/biotech/topics/start--/simultaneously.py` & `biotech-1.1.2/venues/stages/biotech/topics/start--/simultaneously.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.1/PKG-INFO` & `biotech-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotech
-Version: 1.1.1
+Version: 1.1.2
 Summary: A health monitoring stack
 License: GPL-3.0-only
 Keywords: alarms,screening,monitors,cybernetics,neurons,nervous system,bioelectric,homeostasis,reliability,consistency,integrity,guarantees,vows,oaths,assurances,insurances,ensurances,speed,calmness,education,augmentation,enhancement,improvements
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

