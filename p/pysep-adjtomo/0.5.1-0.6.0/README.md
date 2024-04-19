# Comparing `tmp/pysep-adjtomo-0.5.1.tar.gz` & `tmp/pysep_adjtomo-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysep-adjtomo-0.5.1.tar", last modified: Wed Nov 22 03:05:59 2023, max compression
+gzip compressed data, was "pysep_adjtomo-0.6.0.tar", last modified: Fri Apr 19 23:07:55 2024, max compression
```

## Comparing `pysep-adjtomo-0.5.1.tar` & `pysep_adjtomo-0.6.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-11-22 03:05:59.230828 pysep-adjtomo-0.5.1/
--rw-r--r--   0 chow       (501) staff       (20)     1082 2023-02-23 03:25:28.000000 pysep-adjtomo-0.5.1/LICENSE.txt
--rw-r--r--   0 chow       (501) staff       (20)       76 2023-02-23 03:28:29.000000 pysep-adjtomo-0.5.1/MANIFEST.in
--rw-r--r--   0 chow       (501) staff       (20)     3098 2023-11-22 03:05:59.230627 pysep-adjtomo-0.5.1/PKG-INFO
--rw-r--r--   0 chow       (501) staff       (20)     1217 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/README.md
--rw-r--r--   0 chow       (501) staff       (20)      727 2023-11-22 03:01:42.000000 pysep-adjtomo-0.5.1/pyproject.toml
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-11-22 03:05:59.225023 pysep-adjtomo-0.5.1/pysep/
--rw-r--r--   0 chow       (501) staff       (20)      708 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/__init__.py
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-11-22 03:05:59.223677 pysep-adjtomo-0.5.1/pysep/configs/
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-11-22 03:05:59.225324 pysep-adjtomo-0.5.1/pysep/configs/alvizuri_tape_2018/
--rw-r--r--   0 chow       (501) staff       (20)      928 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/configs/alvizuri_tape_2018/2006-10-09T013528_NORTH_KOREA.yaml
--rw-r--r--   0 chow       (501) staff       (20)      576 2023-02-23 03:25:28.000000 pysep-adjtomo-0.5.1/pysep/configs/alvizuri_tape_2018/event_list_alvizuri_tape_2018.txt
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-11-22 03:05:59.225586 pysep-adjtomo-0.5.1/pysep/configs/denali_nodal/
--rw-r--r--   0 chow       (501) staff       (20)      988 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NODAL.yaml
--rw-r--r--   0 chow       (501) staff       (20)     1021 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NONNODAL.yaml
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-11-22 03:05:59.225952 pysep-adjtomo-0.5.1/pysep/configs/misc_events/
--rw-r--r--   0 chow       (501) staff       (20)     1000 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/configs/misc_events/1988-02-15T181000_KERNVILLE_EXPLOSION.yaml
--rw-r--r--   0 chow       (501) staff       (20)      963 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/configs/misc_events/2015-10-18T051831_TAAN_FJORD_LANDSLIDE.yaml
--rw-r--r--   0 chow       (501) staff       (20)      962 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/configs/misc_events/2016-01-24T103037_INISKIN.yaml
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-11-22 03:05:59.226408 pysep-adjtomo-0.5.1/pysep/configs/mtuq_workshop_2022/
--rw-r--r--   0 chow       (501) staff       (20)     1003 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/configs/mtuq_workshop_2022/2009-04-07T201255_ANCHORAGE.yaml
--rw-r--r--   0 chow       (501) staff       (20)     1021 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/configs/mtuq_workshop_2022/2014-08-25T161903_ICELAND.yaml
--rw-r--r--   0 chow       (501) staff       (20)     1017 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/configs/mtuq_workshop_2022/2017-09-03T033001_NORTH_KOREA.yaml
--rw-r--r--   0 chow       (501) staff       (20)     1085 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/configs/mtuq_workshop_2022/2020-04-04T015318_SOUTHERN_CALIFORNIA.yaml
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-11-22 03:05:59.226637 pysep-adjtomo-0.5.1/pysep/configs/scec/
--rw-r--r--   0 chow       (501) staff       (20)      981 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/configs/scec/2002-03-16T213324_SOUTHERN_CALIFORNIA.yaml
--rw-r--r--   0 chow       (501) staff       (20)      792 2023-02-23 03:25:28.000000 pysep-adjtomo-0.5.1/pysep/configs/scec/event_list_scec_simulations.txt
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-11-22 03:05:59.226888 pysep-adjtomo-0.5.1/pysep/configs/tape_etal_2018/
--rw-r--r--   0 chow       (501) staff       (20)      957 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/configs/tape_etal_2018/2012-04-11T092157_TAPE_2018.yaml
--rw-r--r--   0 chow       (501) staff       (20)      311 2023-02-23 03:25:28.000000 pysep-adjtomo-0.5.1/pysep/configs/tape_etal_2018/event_list_tape_etal_2018.txt
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-11-22 03:05:59.227448 pysep-adjtomo-0.5.1/pysep/configs/test/
--rw-r--r--   0 chow       (501) staff       (20)      934 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/configs/test/check_rotate_12Z.yaml
--rw-r--r--   0 chow       (501) staff       (20)      948 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/configs/test/test_config_rotate_bug.yaml
--rw-r--r--   0 chow       (501) staff       (20)     1008 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/configs/test/test_mass_download.yaml
--rw-r--r--   0 chow       (501) staff       (20)      992 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/configs/test/test_remove_data_gaps.yaml
--rw-r--r--   0 chow       (501) staff       (20)     1003 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/configs/test/test_station_ids.yaml
--rw-r--r--   0 chow       (501) staff       (20)    46932 2023-02-23 03:25:28.000000 pysep-adjtomo-0.5.1/pysep/declust.py
--rw-r--r--   0 chow       (501) staff       (20)    98532 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/pysep.py
--rwxr-xr-x   0 chow       (501) staff       (20)   112327 2023-11-22 02:59:13.000000 pysep-adjtomo-0.5.1/pysep/recsec.py
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-11-22 03:05:59.228059 pysep-adjtomo-0.5.1/pysep/tests/
--rw-r--r--   0 chow       (501) staff       (20)     3548 2023-02-23 03:25:28.000000 pysep-adjtomo-0.5.1/pysep/tests/test_declust.py
--rw-r--r--   0 chow       (501) staff       (20)     8441 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/tests/test_process.py
--rw-r--r--   0 chow       (501) staff       (20)     2981 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/tests/test_pysep.py
--rw-r--r--   0 chow       (501) staff       (20)     4596 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/tests/test_recsec.py
--rw-r--r--   0 chow       (501) staff       (20)     8859 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/tests/test_utils.py
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-11-22 03:05:59.229397 pysep-adjtomo-0.5.1/pysep/utils/
--rw-r--r--   0 chow       (501) staff       (20)        0 2023-02-23 03:25:28.000000 pysep-adjtomo-0.5.1/pysep/utils/__init__.py
--rw-r--r--   0 chow       (501) staff       (20)    18260 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/utils/cap_sac.py
--rw-r--r--   0 chow       (501) staff       (20)    13888 2023-11-22 02:59:57.000000 pysep-adjtomo-0.5.1/pysep/utils/curtail.py
--rw-r--r--   0 chow       (501) staff       (20)     7426 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/utils/fetch.py
--rw-r--r--   0 chow       (501) staff       (20)     6522 2023-02-23 03:25:28.000000 pysep-adjtomo-0.5.1/pysep/utils/fmt.py
--rw-r--r--   0 chow       (501) staff       (20)    25447 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/utils/io.py
--rw-r--r--   0 chow       (501) staff       (20)     4447 2023-02-23 03:25:28.000000 pysep-adjtomo-0.5.1/pysep/utils/llnl.py
--rw-r--r--   0 chow       (501) staff       (20)    20325 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/utils/mt.py
--rw-r--r--   0 chow       (501) staff       (20)    16417 2023-09-03 07:07:56.000000 pysep-adjtomo-0.5.1/pysep/utils/plot.py
--rw-r--r--   0 chow       (501) staff       (20)    19848 2023-11-22 02:59:00.000000 pysep-adjtomo-0.5.1/pysep/utils/process.py
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-11-22 03:05:59.230271 pysep-adjtomo-0.5.1/pysep_adjtomo.egg-info/
--rw-r--r--   0 chow       (501) staff       (20)     3098 2023-11-22 03:05:59.000000 pysep-adjtomo-0.5.1/pysep_adjtomo.egg-info/PKG-INFO
--rw-r--r--   0 chow       (501) staff       (20)     1881 2023-11-22 03:05:59.000000 pysep-adjtomo-0.5.1/pysep_adjtomo.egg-info/SOURCES.txt
--rw-r--r--   0 chow       (501) staff       (20)        1 2023-11-22 03:05:59.000000 pysep-adjtomo-0.5.1/pysep_adjtomo.egg-info/dependency_links.txt
--rw-r--r--   0 chow       (501) staff       (20)       70 2023-11-22 03:05:59.000000 pysep-adjtomo-0.5.1/pysep_adjtomo.egg-info/entry_points.txt
--rw-r--r--   0 chow       (501) staff       (20)       48 2023-11-22 03:05:59.000000 pysep-adjtomo-0.5.1/pysep_adjtomo.egg-info/requires.txt
--rw-r--r--   0 chow       (501) staff       (20)        6 2023-11-22 03:05:59.000000 pysep-adjtomo-0.5.1/pysep_adjtomo.egg-info/top_level.txt
--rw-r--r--   0 chow       (501) staff       (20)       38 2023-11-22 03:05:59.230863 pysep-adjtomo-0.5.1/setup.cfg
--rw-r--r--   0 chow       (501) staff       (20)       38 2023-02-23 03:25:28.000000 pysep-adjtomo-0.5.1/setup.py
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-04-19 23:07:55.902778 pysep_adjtomo-0.6.0/
+-rw-r--r--   0 chow       (501) staff       (20)     1082 2023-02-23 03:25:28.000000 pysep_adjtomo-0.6.0/LICENSE.txt
+-rw-r--r--   0 chow       (501) staff       (20)       76 2023-02-23 03:28:29.000000 pysep_adjtomo-0.6.0/MANIFEST.in
+-rw-r--r--   0 chow       (501) staff       (20)     3098 2024-04-19 23:07:55.902578 pysep_adjtomo-0.6.0/PKG-INFO
+-rw-r--r--   0 chow       (501) staff       (20)     1217 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/README.md
+-rw-r--r--   0 chow       (501) staff       (20)      727 2024-04-19 23:03:39.000000 pysep_adjtomo-0.6.0/pyproject.toml
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-04-19 23:07:55.895896 pysep_adjtomo-0.6.0/pysep/
+-rw-r--r--   0 chow       (501) staff       (20)      708 2023-11-22 02:59:00.000000 pysep_adjtomo-0.6.0/pysep/__init__.py
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-04-19 23:07:55.894247 pysep_adjtomo-0.6.0/pysep/configs/
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-04-19 23:07:55.896291 pysep_adjtomo-0.6.0/pysep/configs/alvizuri_tape_2018/
+-rw-r--r--   0 chow       (501) staff       (20)      928 2024-02-29 19:52:29.000000 pysep_adjtomo-0.6.0/pysep/configs/alvizuri_tape_2018/2006-10-09T013528_NORTH_KOREA.yaml
+-rw-r--r--   0 chow       (501) staff       (20)      576 2023-02-23 03:25:28.000000 pysep_adjtomo-0.6.0/pysep/configs/alvizuri_tape_2018/event_list_alvizuri_tape_2018.txt
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-04-19 23:07:55.896775 pysep_adjtomo-0.6.0/pysep/configs/denali_nodal/
+-rw-r--r--   0 chow       (501) staff       (20)      988 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NODAL.yaml
+-rw-r--r--   0 chow       (501) staff       (20)     1021 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NONNODAL.yaml
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-04-19 23:07:55.897192 pysep_adjtomo-0.6.0/pysep/configs/misc_events/
+-rw-r--r--   0 chow       (501) staff       (20)     1000 2024-02-29 19:52:29.000000 pysep_adjtomo-0.6.0/pysep/configs/misc_events/1988-02-15T181000_KERNVILLE_EXPLOSION.yaml
+-rw-r--r--   0 chow       (501) staff       (20)      963 2024-02-29 19:52:29.000000 pysep_adjtomo-0.6.0/pysep/configs/misc_events/2015-10-18T051831_TAAN_FJORD_LANDSLIDE.yaml
+-rw-r--r--   0 chow       (501) staff       (20)      962 2024-02-29 19:52:29.000000 pysep_adjtomo-0.6.0/pysep/configs/misc_events/2016-01-24T103037_INISKIN.yaml
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-04-19 23:07:55.897756 pysep_adjtomo-0.6.0/pysep/configs/mtuq_workshop_2022/
+-rw-r--r--   0 chow       (501) staff       (20)     1003 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/configs/mtuq_workshop_2022/2009-04-07T201255_ANCHORAGE.yaml
+-rw-r--r--   0 chow       (501) staff       (20)     1021 2024-02-29 19:52:29.000000 pysep_adjtomo-0.6.0/pysep/configs/mtuq_workshop_2022/2014-08-25T161903_ICELAND.yaml
+-rw-r--r--   0 chow       (501) staff       (20)     1017 2024-02-29 19:52:29.000000 pysep_adjtomo-0.6.0/pysep/configs/mtuq_workshop_2022/2017-09-03T033001_NORTH_KOREA.yaml
+-rw-r--r--   0 chow       (501) staff       (20)     1085 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/configs/mtuq_workshop_2022/2020-04-04T015318_SOUTHERN_CALIFORNIA.yaml
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-04-19 23:07:55.898320 pysep_adjtomo-0.6.0/pysep/configs/scec/
+-rw-r--r--   0 chow       (501) staff       (20)      981 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/configs/scec/2002-03-16T213324_SOUTHERN_CALIFORNIA.yaml
+-rw-r--r--   0 chow       (501) staff       (20)      792 2023-02-23 03:25:28.000000 pysep_adjtomo-0.6.0/pysep/configs/scec/event_list_scec_simulations.txt
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-04-19 23:07:55.898746 pysep_adjtomo-0.6.0/pysep/configs/tape_etal_2018/
+-rw-r--r--   0 chow       (501) staff       (20)      957 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/configs/tape_etal_2018/2012-04-11T092157_TAPE_2018.yaml
+-rw-r--r--   0 chow       (501) staff       (20)      311 2023-02-23 03:25:28.000000 pysep_adjtomo-0.6.0/pysep/configs/tape_etal_2018/event_list_tape_etal_2018.txt
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-04-19 23:07:55.899443 pysep_adjtomo-0.6.0/pysep/configs/test/
+-rw-r--r--   0 chow       (501) staff       (20)      934 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/configs/test/check_rotate_12Z.yaml
+-rw-r--r--   0 chow       (501) staff       (20)      948 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/configs/test/test_config_rotate_bug.yaml
+-rw-r--r--   0 chow       (501) staff       (20)     1008 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/configs/test/test_mass_download.yaml
+-rw-r--r--   0 chow       (501) staff       (20)      992 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/configs/test/test_remove_data_gaps.yaml
+-rw-r--r--   0 chow       (501) staff       (20)     1003 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/configs/test/test_station_ids.yaml
+-rw-r--r--   0 chow       (501) staff       (20)    46932 2023-02-23 03:25:28.000000 pysep_adjtomo-0.6.0/pysep/declust.py
+-rw-r--r--   0 chow       (501) staff       (20)    98532 2024-02-29 19:52:29.000000 pysep_adjtomo-0.6.0/pysep/pysep.py
+-rwxr-xr-x   0 chow       (501) staff       (20)   117025 2024-04-19 23:03:39.000000 pysep_adjtomo-0.6.0/pysep/recsec.py
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-04-19 23:07:55.900064 pysep_adjtomo-0.6.0/pysep/tests/
+-rw-r--r--   0 chow       (501) staff       (20)     3548 2023-02-23 03:25:28.000000 pysep_adjtomo-0.6.0/pysep/tests/test_declust.py
+-rw-r--r--   0 chow       (501) staff       (20)     8441 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/tests/test_process.py
+-rw-r--r--   0 chow       (501) staff       (20)     2981 2024-02-29 19:52:29.000000 pysep_adjtomo-0.6.0/pysep/tests/test_pysep.py
+-rw-r--r--   0 chow       (501) staff       (20)     5330 2024-04-19 23:03:39.000000 pysep_adjtomo-0.6.0/pysep/tests/test_recsec.py
+-rw-r--r--   0 chow       (501) staff       (20)    10076 2024-04-19 23:03:39.000000 pysep_adjtomo-0.6.0/pysep/tests/test_utils.py
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-04-19 23:07:55.901283 pysep_adjtomo-0.6.0/pysep/utils/
+-rw-r--r--   0 chow       (501) staff       (20)        0 2023-02-23 03:25:28.000000 pysep_adjtomo-0.6.0/pysep/utils/__init__.py
+-rw-r--r--   0 chow       (501) staff       (20)    18996 2024-04-19 23:03:39.000000 pysep_adjtomo-0.6.0/pysep/utils/cap_sac.py
+-rw-r--r--   0 chow       (501) staff       (20)    13888 2024-02-29 19:52:29.000000 pysep_adjtomo-0.6.0/pysep/utils/curtail.py
+-rw-r--r--   0 chow       (501) staff       (20)     7426 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/utils/fetch.py
+-rw-r--r--   0 chow       (501) staff       (20)     6522 2023-02-23 03:25:28.000000 pysep_adjtomo-0.6.0/pysep/utils/fmt.py
+-rw-r--r--   0 chow       (501) staff       (20)    27950 2024-04-19 23:03:39.000000 pysep_adjtomo-0.6.0/pysep/utils/io.py
+-rw-r--r--   0 chow       (501) staff       (20)     4447 2023-02-23 03:25:28.000000 pysep_adjtomo-0.6.0/pysep/utils/llnl.py
+-rw-r--r--   0 chow       (501) staff       (20)    20325 2023-11-22 02:59:00.000000 pysep_adjtomo-0.6.0/pysep/utils/mt.py
+-rw-r--r--   0 chow       (501) staff       (20)    16417 2023-09-03 07:07:56.000000 pysep_adjtomo-0.6.0/pysep/utils/plot.py
+-rw-r--r--   0 chow       (501) staff       (20)    19848 2023-11-22 02:59:00.000000 pysep_adjtomo-0.6.0/pysep/utils/process.py
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-04-19 23:07:55.902229 pysep_adjtomo-0.6.0/pysep_adjtomo.egg-info/
+-rw-r--r--   0 chow       (501) staff       (20)     3098 2024-04-19 23:07:55.000000 pysep_adjtomo-0.6.0/pysep_adjtomo.egg-info/PKG-INFO
+-rw-r--r--   0 chow       (501) staff       (20)     1881 2024-04-19 23:07:55.000000 pysep_adjtomo-0.6.0/pysep_adjtomo.egg-info/SOURCES.txt
+-rw-r--r--   0 chow       (501) staff       (20)        1 2024-04-19 23:07:55.000000 pysep_adjtomo-0.6.0/pysep_adjtomo.egg-info/dependency_links.txt
+-rw-r--r--   0 chow       (501) staff       (20)       70 2024-04-19 23:07:55.000000 pysep_adjtomo-0.6.0/pysep_adjtomo.egg-info/entry_points.txt
+-rw-r--r--   0 chow       (501) staff       (20)       48 2024-04-19 23:07:55.000000 pysep_adjtomo-0.6.0/pysep_adjtomo.egg-info/requires.txt
+-rw-r--r--   0 chow       (501) staff       (20)        6 2024-04-19 23:07:55.000000 pysep_adjtomo-0.6.0/pysep_adjtomo.egg-info/top_level.txt
+-rw-r--r--   0 chow       (501) staff       (20)       38 2024-04-19 23:07:55.902813 pysep_adjtomo-0.6.0/setup.cfg
+-rw-r--r--   0 chow       (501) staff       (20)       38 2023-02-23 03:25:28.000000 pysep_adjtomo-0.6.0/setup.py
```

### Comparing `pysep-adjtomo-0.5.1/LICENSE.txt` & `pysep_adjtomo-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/PKG-INFO` & `pysep_adjtomo-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysep-adjtomo
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python Seismogram Extraction and Processing
 Author: adjTomo Dev Team
 Author-email: adjtomo@gmail.com
 License: MIT License
         
         Copyright (c) University of Alaska Fairbanks
```

### Comparing `pysep-adjtomo-0.5.1/README.md` & `pysep_adjtomo-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pyproject.toml` & `pysep_adjtomo-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysep-adjtomo"
-version = "0.5.1"
+version = "0.6.0"
 description = "Python Seismogram Extraction and Processing"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "adjTomo Dev Team"},
     {email = "adjtomo@gmail.com"}
```

### Comparing `pysep-adjtomo-0.5.1/pysep/__init__.py` & `pysep_adjtomo-0.6.0/pysep/__init__.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/alvizuri_tape_2018/2006-10-09T013528_NORTH_KOREA.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/alvizuri_tape_2018/2006-10-09T013528_NORTH_KOREA.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/alvizuri_tape_2018/event_list_alvizuri_tape_2018.txt` & `pysep_adjtomo-0.6.0/pysep/configs/alvizuri_tape_2018/event_list_alvizuri_tape_2018.txt`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NODAL.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NODAL.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NONNODAL.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/denali_nodal/2019-02-25T182230_CANTWELL_NONNODAL.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/misc_events/1988-02-15T181000_KERNVILLE_EXPLOSION.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/misc_events/1988-02-15T181000_KERNVILLE_EXPLOSION.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/misc_events/2015-10-18T051831_TAAN_FJORD_LANDSLIDE.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/misc_events/2015-10-18T051831_TAAN_FJORD_LANDSLIDE.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/misc_events/2016-01-24T103037_INISKIN.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/misc_events/2016-01-24T103037_INISKIN.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/mtuq_workshop_2022/2009-04-07T201255_ANCHORAGE.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/mtuq_workshop_2022/2009-04-07T201255_ANCHORAGE.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/mtuq_workshop_2022/2014-08-25T161903_ICELAND.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/mtuq_workshop_2022/2014-08-25T161903_ICELAND.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/mtuq_workshop_2022/2017-09-03T033001_NORTH_KOREA.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/mtuq_workshop_2022/2017-09-03T033001_NORTH_KOREA.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/mtuq_workshop_2022/2020-04-04T015318_SOUTHERN_CALIFORNIA.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/mtuq_workshop_2022/2020-04-04T015318_SOUTHERN_CALIFORNIA.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/scec/2002-03-16T213324_SOUTHERN_CALIFORNIA.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/scec/2002-03-16T213324_SOUTHERN_CALIFORNIA.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/scec/event_list_scec_simulations.txt` & `pysep_adjtomo-0.6.0/pysep/configs/scec/event_list_scec_simulations.txt`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/tape_etal_2018/2012-04-11T092157_TAPE_2018.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/tape_etal_2018/2012-04-11T092157_TAPE_2018.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/test/check_rotate_12Z.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/test/check_rotate_12Z.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/test/test_config_rotate_bug.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/test/test_config_rotate_bug.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/test/test_mass_download.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/test/test_mass_download.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/test/test_remove_data_gaps.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/test/test_remove_data_gaps.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/configs/test/test_station_ids.yaml` & `pysep_adjtomo-0.6.0/pysep/configs/test/test_station_ids.yaml`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/declust.py` & `pysep_adjtomo-0.6.0/pysep/declust.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/pysep.py` & `pysep_adjtomo-0.6.0/pysep/pysep.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/recsec.py` & `pysep_adjtomo-0.6.0/pysep/recsec.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,14 +91,15 @@
 import textwrap
 import numpy as np
 import matplotlib.pyplot as plt
 
 from glob import glob
 from datetime import datetime
 from matplotlib.ticker import MultipleLocator
+from matplotlib.patches import Rectangle
 from obspy import read, Stream
 from obspy.geodetics import (kilometers2degrees, gps2dist_azimuth)
 
 from pysep import logger
 from pysep.utils.cap_sac import origin_time_from_sac_header, SACDICT
 from pysep.utils.io import read_sem
 from pysep.utils.curtail import subset_streams
@@ -121,29 +122,37 @@
     """
     Record section plotting tool which takes ObsPy streams and:
 
     1) preprocesses and filters waveforms,
     2) sorts source-receiver pairs based on User input,
     3) produces record section waveform figures.
     """
-    def __init__(self, pysep_path=None, syn_path=None, 
-                 stations=None, source=None, st=None, st_syn=None, 
-                 sort_by="default", scale_by=None, time_shift_s=None, 
-                 zero_pad_s=None, move_out=None, 
-                 min_period_s=None, max_period_s=None,
-                 preprocess=None, max_traces_per_rs=None, integrate=0,
-                 xlim_s=None, components="ZRTNE12", y_label_loc="default",
-                 y_axis_spacing=1, amplitude_scale_factor=1,
-                 azimuth_start_deg=0., distance_units="km", tmarks=None,
-                 geometric_spreading_factor=0.5, geometric_spreading_k_val=None,
-                 geometric_spreading_exclude=None,
-                 geometric_spreading_ymax=None, geometric_spreading_save=None,
-                 figsize=(9, 11), show=True, save="./record_section.png",
-                 overwrite=False, log_level="DEBUG", synsyn=False, srcfmt=None, 
-                 wildcard="*", syn_wildcard=None, **kwargs):
+    def __init__(
+            # Data input parameters
+            self, pysep_path=None, syn_path=None, stations=None, source=None, 
+            st=None, st_syn=None, windows=None, synsyn=False, srcfmt=None, 
+            wildcard="*", syn_wildcard=None, 
+            # Data organization parameters
+            sort_by="default", scale_by=None, time_shift_s=None, 
+            zero_pad_s=None, move_out=None, 
+            # Data processing parameters
+            preprocess=True, min_period_s=None, max_period_s=None, integrate=0, 
+            trim=True, taper=True,
+            # Plotting aesthetic 
+            xlim_s=None, components="ZRTNE12", y_label_loc="default",
+            y_axis_spacing=1, amplitude_scale_factor=1, azimuth_start_deg=0., 
+            distance_units="km", tmarks=None,
+            # Geometric Spreading
+            geometric_spreading_factor=0.5, geometric_spreading_k_val=None,
+            geometric_spreading_exclude=None,
+            geometric_spreading_ymax=None, geometric_spreading_save=None,
+            # Figure generation control parameters
+            figsize=(9, 11), show=True, save="./record_section.png",
+            overwrite=True, max_traces_per_rs=None, log_level="DEBUG", 
+            **kwargs):
         """
         .. note::
             Used for reading in Pysep-generated waveforms
 
         :type pysep_path: str
         :param pysep_path: path to Pysep output, which is expected to contain
             trace-wise SAC waveform files which will be read in. See 
@@ -193,14 +202,23 @@
 
         :type st: obspy.core.stream.Stream
         :param st: Stream objects containing observed time series to be plotted
             on the record section. Can contain any number of traces
         :type st_syn: obspy.core.stream.Stream
         :param st_syn: Stream objects containing synthetic time series to be
             plotted on the record section. Must be same length as `st`
+        :type windows: dict of lists of tuples
+        :param windows: EXPERIMENTAL FEATURE -- plot misfit windows collected
+            by windowing algorithm like Pyflex. Essentially these are provided
+            as start and end times for each trace in the Stream. The dictionary
+            should be formated where keys are the Trace IDs of observed
+            waveforms, and values are lists of tuples, where each tuple 
+            represents a window start and end time in seconds. See 
+            `pysep.utils.io.read_asdfdataset` for code on how windows are 
+            structured
 
         .. note::
             Waveform plotting organization parameters
 
         :type sort_by: str
         :param sort_by: How to sort the Y-axis of the record section, available:
 
@@ -291,35 +309,41 @@
             azimuthal angle for the waveform at the top of the figure.
             Set to 0 for default behavior
         :type distance_units: str
         :param distance_units: Y-axis units when sorting by epicentral distance
             'km': kilometers on the sphere
             'deg': degrees on the sphere
             'km_utm': kilometers on flat plane, UTM coordinate system
+        :type components: str
+        :param components: a sequence of strings representing acceptable
+            components from the data. Also determines the order these are shown
+            EVEN when sorted by other variables. For example, components=='ZR'
+            would only display Z and R components, and Z components would be
+            should BEFORE R components for the SAME station.
 
         .. note::
             Data processing parameters
 
         :type preprocess: str
-        :param preprocess: choose which data to preprocess, options are:
+        :param preprocess: choose whether preprocessing steps listed below are 
+            applied to waveform data, and if so, which data are procesed:
 
-            - None: do not run preprocessing step, including filter (Default)
-            - 'st': process waveforms in `st`
-            - 'st_syn': process waveforms in `st_syn`. st still must be given
-            - 'both': process waveforms in both `st` and `st_syn`
+            - True: process waveforms in both `st` and `st_syn` (Default)
+            - False: do not run any processing on waveforms
+            - 'st': only process waveforms in `st`
+            - 'st_syn': only process waveforms in `st_syn`. st still required
         :type min_period_s: float
-        :param min_period_s: minimum filter period in seconds
+        :param min_period_s: minimum filter period in seconds, if not given 
+            and `max_period_s` also not given, then no filtering is applied
         :type max_period_s: float
-        :param max_period_s: maximum filter period in seconds
-        :type components: str
-        :param components: a sequence of strings representing acceptable
-            components from the data. Also determines the order these are shown
-            EVEN when sorted by other variables. For example, components=='ZR'
-            would only display Z and R components, and Z components would be
-            should BEFORE R components for the SAME station.
+        :param max_period_s: maximum filter period in seconds, if not given
+            and `min_period_s` also not given, then no filtering is applied
+        :type trim: bool
+        :param trim: trim waveforms to the same length, and if any data gaps
+            are present, fill with mean values by default
         :type integrate: int
         :param integrate: apply integration `integrate` times on all traces.
             acceptable values [-inf, inf], where positive values are integration
             and negative values are differentiation
 
             e.g., if integrate == 2,  will integrate each trace twice.
             or    if integrate == -1, will differentiate once
@@ -475,20 +499,22 @@
         # to ensure int -> float
         try:
             self.time_shift_s = float(time_shift_s)
         except (TypeError, ValueError):
             self.time_shift_s = time_shift_s
         self.zero_pad_s = zero_pad_s
 
-        # Filtering parameters
+        # Processing parameters
+        self.preprocess = preprocess
         self.min_period_s = min_period_s
         self.max_period_s = max_period_s
-        self.preprocess = preprocess
         self.max_traces_per_rs = max_traces_per_rs
         self.integrate = int(integrate)
+        self.trim = bool(trim)
+        self.taper = bool(taper)
 
         # Plotting parameters
         self.xlim_s = xlim_s
         self.distance_units = distance_units.lower()
         self.y_label_loc = y_label_loc
         self.tmarks = tmarks
         self.figsize = figsize
@@ -515,14 +541,17 @@
         self.amplitude_scaling = []
         self.amplitude_scaling_syn = []
         self.y_axis = []
         self.xlim = []  # unit: samples
         self.xlim_syn = []
         self.sorted_idx = []
 
+        # Experimental Feature
+        self.windows = windows
+
     def read_data(self, path, data_type, wildcard="*", source=None,
                   stations=None, srcfmt=None):
         """
         General function that attempts to read in observed and synthetic data
         in User-provided format that can either be SAC files or SPECFEM format
         two-column ASCII files.
 
@@ -607,15 +636,15 @@
                                        stations=stations, source_format=srcfmt)
                         logger.debug(fid)
                     except Exception as e:
                         logger.warning(f"unexpected read error {fid}: {e}")
         else:
             raise NotImplementedError("`data_type` must be 'data' or 'syn'")
 
-        return st
+        return st                
 
     def check_parameters(self):
         """
         Check that parameters are set properly and in line with how they
         are expected by the program
 
         .. note::
@@ -709,31 +738,38 @@
         acceptable_scale_factor = [int, float, list]
         if type(self.amplitude_scale_factor) not in acceptable_scale_factor:
             err.amplitude_scale_factor = f"must be in {acceptable_scale_factor}"
         if isinstance(self.amplitude_scale_factor, list) and \
                 len(self.amplitude_scale_factor) != len(self.st):
             err.amplitude_scale_factor = f"must be list length {len(self.st)}"
 
+        acceptable_preprocess = [True, False, "st", "st_syn"]
+        if self.preprocess not in acceptable_preprocess:
+            err.preprocess = f"must be in {acceptable_preprocess}"
+
+        if self.preprocess == "st_syn":
+            assert(self.st is not None and self.st_syn is not None), (
+                f"`preprocess` choice requires both `st` & `st_syn` to exist."
+                f"If you only have one or the other, set: `preprocess`=='st'"
+            )
+
         if self.min_period_s is not None and self.max_period_s is not None:
             if self.min_period_s >= self.max_period_s:
                 err.min_period_s = "must be less than `max_period_s`"
 
         if self.min_period_s is not None or self.max_period_s is not None:
-            assert(self.preprocess is not None), \
+            assert(self.preprocess is not False), \
                 f"Setting filter bounds requires `preprocess` flag to be set"
-
-        if self.preprocess is not None:
-            acceptable_preprocess = ["both", "st", "st_syn"]
-            if self.preprocess not in acceptable_preprocess:
-                err.preprocess = f"must be in {acceptable_preprocess}"
-        if self.preprocess in ["st_syn", "both"]:
-            assert(self.st is not None and self.st_syn is not None), (
-                f"`preprocess` choice requires both `st` & `st_syn` to exist."
-                f"If you only have one or the other, set: `preprocess`=='st'"
-            )
+            
+        # Do not allow for 0 period filter because that's wrong and will also
+        # trip up later logic checks
+        if self.min_period_s:
+            assert(self.min_period_s != 0) 
+        if self.max_period_s:
+            assert(self.max_period_s != 0) 
 
         # Overwrite the max traces per record section, enforce type int
         if self.max_traces_per_rs is None:
             self.max_traces_per_rs = int(len(self.st))
         else:
             self.max_traces_per_rs = int(self.max_traces_per_rs)
 
@@ -1461,87 +1497,134 @@
         # Find order of magnitude of the length to give a rough estimate
         oom = np.floor(np.log10(rs_len))
         xtick_major = 10 ** oom
         xtick_minor = xtick_major / 2
 
         return xtick_minor, xtick_major
 
-    def process_st(self):
+    def process_st(self, **kwargs):
         """
         Preprocess the Stream with optional filtering in place.
 
         .. note::
+
             Data in memory will be irretrievably altered by running preprocess.
 
+        .. warning::
+
+            if `trim` is False but `zero_pad_s` is True we may run into the
+            issue of filling data gaps with zeros
+
         TODO Add feature to allow list-like periods to individually filter
             seismograms. At the moment we just apply a blanket filter.
-        """
-        if self.preprocess is None:
-            logger.info("no preprocessing (including filtering) applied")
+
+        KWARGS
+        :type max_percentage: float
+        :param max_percentage: percentage of the trace to taper at both ends
+        :type zerophase: bool
+        :param zerophase: whether to apply zero-phase filtering or not,
+            defaults to True
+        :type taper_type: str
+        :param taper_type: type of taper to apply to the waveforms
+        :type fill_value: str or float
+        :param fill_value: value to fill gaps in the data after trimming, 
+            defaults to mean of the trace
+        """
+        max_percentage = float(self.kwargs.get("max_percentage", 0.05))
+        zerophase = bool(self.kwargs.get("zerophase", True))
+        taper_type = self.kwargs.get("taper_type", "cosine")
+        fill_value = self.kwargs.get("fill_value", "mean")
+
+        # Determine which traces we are running through preprocessing
+        if self.preprocess == False:
+            logger.info("no preprocessing will be applied to waveforms")
             return
+        elif self.preprocess == True:
+            preprocess_list = [self.st]
+            if self.st_syn is not None:
+                preprocess_list.append(self.st_syn)
+            n = sum([len(_) for _ in preprocess_list])
+            logger.info(f"preprocessing {n} waveforms")
         elif self.preprocess == "st":
             logger.info(f"preprocessing {len(self.st)} `st` waveforms")
             preprocess_list = [self.st]
         elif self.preprocess == "st_syn":
             logger.info(f"preprocessing {len(self.st_syn)} `st_syn` waveforms")
             preprocess_list = [self.st_syn]
-        elif self.preprocess == "both":
-            logger.info(f"preprocessing {len(self.st) + len(self.st_syn)} "
-                        f"`st` and `st_syn` waveforms")
-            preprocess_list = [self.st, self.st_syn]
 
         for st in preprocess_list:
-            # Fill any data gaps with mean of the data, do it on a trace by 
-            # trace basis to get individual mean values
-            for tr in st:
-                tr.trim(starttime=tr.stats.starttime, endtime=tr.stats.endtime,
-                        pad=True, fill_value=tr.data.mean())
-            st.detrend("demean")
-            st.taper(max_percentage=0.05, type="cosine")
+            if self.trim:
+                logger.debug("trimming start and end times and filling any "
+                             f"gaps with {fill_value}")
+                for tr in st:
+                    if fill_value == "mean":
+                        fill_value = tr.data.mean()
+                    tr.trim(starttime=tr.stats.starttime, 
+                            endtime=tr.stats.endtime, pad=True, 
+                            fill_value=fill_value)
+            
+            # Taper prior to zero pad so that the taper actually hits signal
+            if self.taper:
+                # If we don't demean, then tapering may hit a static offset
+                logger.debug("demean waveform in preparation for tapering")
+                st.detrend("demean")
+
+                logger.debug(f"tapering waveforms with {max_percentage} taper")
+                st.taper(max_percentage=max_percentage, type=taper_type)
 
             # Zero pad start and end of data if requested by user
             if self.zero_pad_s:
+                if not self.taper:
+                    # If we don't demean, zero pad may introduce static offset
+                    logger.debug("demean waveform in preparation for zero pad")
+                    st.detrend("demean")
+
                 _start, _end = self.zero_pad_s
-                logger.info(f"padding zeros to traces with {_start}s before "
+                logger.debug(f"padding zeros to traces with {_start}s before "
                             f"and {_end}s after")
-                for idx, tr in enumerate(st):
+                for tr in st:
                     tr.trim(starttime=tr.stats.starttime - _start,
                             endtime=tr.stats.endtime + _end,
                             pad=True, fill_value=0)
 
-            # Allow multiple filter options based on user input
-            # Max period only == high-pass
-            if self.max_period_s is not None and self.min_period_s is None:
-                logger.info(f"apply highpass filter w/ cutoff "
-                            f"{1/self.max_period_s}")
-                st.filter("highpass", freq=1/self.max_period_s, zerophase=True)
-            # Min period only == low-pass
-            elif self.min_period_s is not None and self.max_period_s is None:
-                logger.info(f"apply lowpass filter w/ cutoff "
-                            f"{1/self.min_period_s}")
-                st.filter("lowpass", freq=1/self.min_period_s, zerophase=True)
-            # Both min and max period == band-pass
-            elif self.min_period_s is not None and \
-                    self.max_period_s is not None:
-                logger.info(f"applying bandpass filter w/ "
-                            f"[{1/self.max_period_s}, {self.min_period_s}]")
-                st.filter("bandpass", freqmin=1/self.max_period_s,
-                          freqmax=1/self.min_period_s, zerophase=True)
-            else:
-                logger.info("no filtering applied")
+            # Apply filtering 
+            if self.min_period_s or self.max_period_s:
+                # Max period only == high-pass filter
+                if self.max_period_s and self.min_period_s is None:
+                    logger.debug(f"apply highpass filter w/ cutoff "
+                                f"{1/self.max_period_s}")
+                    st.filter("highpass", freq=1/self.max_period_s, 
+                              zerophase=zerophase)
+                    
+                # Min period only == low-pass filter
+                elif self.min_period_s and self.max_period_s is None:
+                    logger.debug(f"apply lowpass filter w/ cutoff "
+                                f"{1/self.min_period_s}")
+                    st.filter("lowpass", freq=1/self.min_period_s, 
+                              zerophase=zerophase)
+                    
+                # Both min and max period == band-pass filter
+                elif self.min_period_s and self.max_period_s:
+                    logger.debug(
+                        f"applying bandpass filter w/ "
+                        f"[{1/self.max_period_s}, {self.min_period_s}]"
+                        )
+                    st.filter("bandpass", freqmin=1/self.max_period_s,
+                            freqmax=1/self.min_period_s, zerophase=zerophase)
 
-            # Integrate and differentiate N number of times specified by user
-            st.detrend("simple")
+            # Integrate or differentiate N number of times specified by user
             if self.integrate != 0:
+                st.detrend("simple")
                 if self.integrate < 0:
                     func = "differentiate"
                 elif self.integrate > 0:
                     func = "integrate"
-            for i in range(np.abs(self.integrate)):
-                logger.info(f"{func} all waveform data x{abs(self.integrate)}")
+                for _ in range(np.abs(self.integrate)):
+                    logger.info(f"{func} all waveform data "
+                                f"x{abs(self.integrate)}")
                 getattr(st, func)()
 
     def plot(self, subset=None, page_num=None, **kwargs):
         """
         Plot record sections based on all the available information
 
         :type subset: list of int
@@ -1679,14 +1762,18 @@
             trace is plotted on top of the previous one. y_index should be
             iterated linearly in the loop that calls this function.
         :type choice: str
         :param choice: choice of 'st' or 'st_syn' depending on whether you want
             to plot the observed or synthetic waveforms
         """
         linewidth = self.kwargs.get("linewidth", .25)
+        window_alpha = self.kwargs.get("window_alpha", .1)
+        window_color = self.kwargs.get("window_color", "orange")
+        obs_color = self.kwargs.get("obs_color", "k")
+        syn_color = self.kwargs.get("syn_color", "r")
 
         # Used to differentiate the two types of streams for plotting diffs
         choices = ["st", "st_syn"]
         assert (choice in choices)
         c = choices.index(choice)
         tr = getattr(self, choice)[idx]  # i.e., tr = self.st[idx]
 
@@ -1711,37 +1798,54 @@
         # Flip the sign of the y-axis if we are doing normal absolute
         # sorting because we are flipping the y-axis in _plot_axes()
         if "abs_" in self.sort_by and "_r" not in self.sort_by:
             sign = -1
         else:
             sign = 1
 
-        # Ampplitude scaling may change between observed and synthetic if e.g.,
+        # Amplitude scaling may change between observed and synthetic if e.g.,
         # we are doing trace-wise normalization
         if choice == "st":
             amplitude_scaling = self.amplitude_scaling
             max_amplitudes = self.max_amplitudes
         elif choice == "st_syn":
             amplitude_scaling = self.amplitude_scaling_syn
             max_amplitudes = self.max_amplitudes_syn
 
-        y = sign * tr.data / amplitude_scaling[idx] + self.y_axis[y_index]
-
+        # Avoid ZeroDivisionError if the amplitude scaling value is 0 (#131)
+        scale = amplitude_scaling[idx]
+        if scale == 0:
+            logger.warning("amplitude scaling value is 0, setting to 1, "
+                           "amplitude scaling may not behave as expected")
+            scale = 1
+
+        y = sign * tr.data / scale + self.y_axis[y_index]
+
+        # Experimental: Plot windows over the record section if provided by User
+        if self.windows and tr.id in self.windows:
+            for window in self.windows[tr.id]:
+                rc = Rectangle(xy=(window[0] + tshift, y.min()), 
+                               width=window[1] - window[0], 
+                               height=y.max() - y.min(), alpha=window_alpha, 
+                               color=window_color, zorder=2)
+                self.ax.add_patch(rc)
+                
         # Truncate waveforms to get figure scaling correct. Make the distinction
         # between data and synthetics which may have different start and end 
         # times natively
         if choice == "st":
             start, stop = self.xlim[idx]
         elif choice == "st_syn":
             start, stop = self.xlim_syn[idx]
 
         x = x[start:stop]
         y = y[start:stop]
-        self.ax.plot(x, y, c=["k", "r"][c], linewidth=linewidth, zorder=10)
-
+        self.ax.plot(x, y, c=[obs_color, syn_color][c], linewidth=linewidth, 
+                     zorder=10)
+        
         # Sanity check print station information to check against plot
         log_str = (f"{idx}"
                    f"\t{int(self.y_axis[y_index])}"
                    f"\t{tr.get_id():<6}"
                    f"\t{self.distances[idx]:6.2f}"
                    f"\t{self.azimuths[idx]:6.2f}"
                    f"\t{self.backazimuths[idx]:6.2f}"
@@ -2330,15 +2434,15 @@
     parser.add_argument("--tmarks", default=None, type=float,
                         nargs="+", help="Plot vertical lines at given reference"
                                         "times [s]. Input as a list of values, "
                                         "e.g., --tmarks 0 100 200")
     parser.add_argument("--save", default="./record_section.png", type=str,
                         nargs="?",
                         help="Path to save the resulting record section fig")
-    parser.add_argument("-o", "--overwrite", default=False, action="store_true",
+    parser.add_argument("-o", "--overwrite", default=True, action="store_true",
                         help="overwrite existing figure if path exists")
     parser.add_argument("--synsyn", default=False, action="store_true",
                         help="Let RecSec know that both `pysep_path` and "
                              "`syn_path` should be read in as SPECFEM-"
                              "generated synthetics.")
     parser.add_argument("--srcfmt", default=None, type=str,
                         help="Optional source format for reading the `source` "
```

### Comparing `pysep-adjtomo-0.5.1/pysep/tests/test_declust.py` & `pysep_adjtomo-0.6.0/pysep/tests/test_declust.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/tests/test_process.py` & `pysep_adjtomo-0.6.0/pysep/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/tests/test_pysep.py` & `pysep_adjtomo-0.6.0/pysep/tests/test_pysep.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/tests/test_recsec.py` & `pysep_adjtomo-0.6.0/pysep/tests/test_recsec.py`

 * *Files 13% similar despite different names*

```diff
@@ -133,7 +133,28 @@
                             tr.data)
         tr.stats.starttime -= 100
 
     recsec_w_synthetics.process_st()
     recsec_w_synthetics.get_parameters()
     for tr in recsec_w_synthetics.st:
         assert(tr.stats.time_offset == -100)
+
+def test_recsec_zero_amplitude(recsec):
+    """
+    waveforms that have zero amplitude and are normalized should be able 
+    to bypass normalizations which lead to weird plotting (see #131).
+
+    .. note::
+
+        This does not really test that the method is working correctly because
+        dividing a NumPy array by zero leads to NaNs in the array which just
+        won't plot. This is more of a visual test to make sure that the 
+        zero amplitude is plotting correctly, look for green lines
+    """
+    recsec.kwargs.scale_by = "normalize"
+    recsec.kwargs.obs_color = "green"
+    recsec.linewidth = 30
+    for tr in recsec.st:
+        tr.data *= 0
+    recsec.process_st()
+    recsec.get_parameters()
+    recsec.plot()
```

### Comparing `pysep-adjtomo-0.5.1/pysep/tests/test_utils.py` & `pysep_adjtomo-0.6.0/pysep/tests/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,14 +55,24 @@
     """
     st = append_sac_headers(st=test_st, inv=test_inv, event=test_event)
     assert(not hasattr(test_st[0].stats, "sac"))
     assert(hasattr(st[0].stats, "sac"))
     assert(st[0].stats.sac["evla"] == test_event.preferred_origin().latitude)
 
 
+def test_append_sac_headers_cartesian(test_st, test_inv, test_event):
+    """
+    Make sure we can write SAC headers correctly
+    """
+    st = append_sac_headers(st=test_st, inv=test_inv, event=test_event)
+    assert(not hasattr(test_st[0].stats, "sac"))
+    assert(hasattr(st[0].stats, "sac"))
+    assert(st[0].stats.sac["evla"] == test_event.preferred_origin().latitude)
+
+
 def test_event_tag_and_event_tag_legacy(test_event):
     """
     Check that event tagging works as expected
     """
     # while were here, make sure event tagging works
     tag = format_event_tag(test_event)
     assert(tag == "2009-04-07T201255_SOUTHERN_ALASKA")
@@ -162,14 +172,22 @@
     test_cmtsolution = "./test_data/test_CMTSOLUTION_2014p715167"
 
     st = Stream()
     for test_synthetic in test_synthetics:
         st += read_sem(fid=test_synthetic, source=test_cmtsolution,
                        stations=test_stations)
     assert(st)
+
+    expected_headers = ["iztype", "b", "e", "evla", "evlo", "stla", "stlo", 
+                        "stel", "kevnm", "nzyear", "nzjday", "nzhour", "nzmin", 
+                        "nzsec", "nzmsec", "dist", "az", "baz", "gcarc", 
+                        "lpspol", "lcalda", "evdp", "mag"]
+    for expected_header in expected_headers:
+        assert(expected_header in st[0].stats.sac)
+
     assert(st[0].stats.sac.evla == -40.5405)
 
 
 def test_read_sem_cartesian():
     """
     Test reading SPECFEM-generated synthetics in Cartesian coordinates
     """
@@ -178,15 +196,25 @@
     test_cmtsolution = "./test_data/test_CMTSOLUTION_cartesian"
 
     st = Stream()
     for test_synthetic in test_synthetics:
         st += read_sem(fid=test_synthetic, source=test_cmtsolution,
                        stations=test_stations)
     assert(st)
+
+    expected_headers = ["iztype", "b", "e", "evla", "evlo", "stla", "stlo", 
+                        "kevnm", "nzyear", "nzjday", "nzhour", "nzmin", 
+                        "nzsec", "nzmsec", "dist", "az", "baz", "gcarc", 
+                        "lpspol", "lcalda", "evdp"]
+    for expected_header in expected_headers:
+        assert(expected_header in st[0].stats.sac)
+
     assert(st[0].stats.sac.stla == 67000.0)
+    assert(st[0].stats.sac.evdp == 30.)
+    assert(st[0].stats.sac.b == -10.)
 
 def test_estimate_prefilter_corners(test_st):
     """
     Test prefilter corner estimation based on trace starts time and samp rate
     """
     for tr in test_st:
         f0, f1, f2, f3 = estimate_prefilter_corners(tr)
```

### Comparing `pysep-adjtomo-0.5.1/pysep/utils/cap_sac.py` & `pysep_adjtomo-0.6.0/pysep/utils/cap_sac.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     TODO Add back in information removed from original function
         * Add sensor type somewhere, previously stored in KT? (used for picks)
 
     .. note::
 
         We explicitely set 'iztype, 'b' and 'e' in the SAC header to tell ObsPy
         that the trace start is NOT the origin time. Otherwise all the relative
-        timing (e.g., picks) will be wrong.
+        timing (e.g., picks) in SAC will be wrong.
 
     :type tr: obspy.core.trace.Trace
     :param tr: Trace to append SAC header to
     :type event: obspy.core.event.Event
     :param event: Event with metadata for SAC header
     :type inv: obspy.core.inventory.Inventory
     :param inv: StationXML with metadata for SAC header
@@ -202,14 +202,15 @@
         "dist": dist_km,
         "az": az,  # degrees
         "baz": baz,  # degrees
         "gcarc": dist_deg,  # degrees
         "lpspol": 0,  # 1 if left-hand polarity (usually no in passive seis)
         "lcalda": 1,  # 1 if DIST, AZ, BAZ, GCARC to be calc'd from metadata
     }
+
     # Some Inventory objects will not go all the way to channel, only to station
     try:
         cha = sta[0]
         sac_header["cmpinc"] = cha.dip  # channel dip/inclination in degrees
         sac_header["cmpaz"] = cha.azimuth  # channel azimuth in degrees
     except IndexError:
         pass
@@ -223,14 +224,21 @@
 
     try:
         mag = event.preferred_magnitude().mag
         sac_header["mag"] = mag
     except Exception:  # NOQA
         pass
 
+    # Warn User that the following SAC headers could not be found
+    _warn_about = []
+    for key in ["cmpinc", "cmpaz", "evdp", "mag"]:
+        if key not in sac_header:
+            _warn_about.append(key)
+    logger.warning(f"no SAC header values found for: {_warn_about}")
+    
     # Append SAC header and include back azimuth for rotation
     tr.stats.sac = sac_header
     tr.stats.back_azimuth = baz
 
     return tr
 
 def append_sac_headers_cartesian(st, event, stations):
@@ -293,42 +301,49 @@
     :type rcv_x: float
     :param rcv_x: X coordinate of the receiver in units meters
     :type rcv_y: float
     :param rcv_y: Y coordinate of the receiver in units meters
     :rtype: obspy.core.trace.Trace
     :return: Trace with appended SAC header
     """
-    net_sta = f"{tr.stats.network}.{tr.stats.station}"
-
     src_y = event.preferred_origin().latitude
     src_x = event.preferred_origin().longitude
+    otime = event.preferred_origin().time
+    evdepth_km = event.preferred_origin().depth / 1E3  # units: m -> km
 
     # Calculate Cartesian distance and azimuth/backazimuth
     dist_m = np.sqrt(((rcv_x - src_x) ** 2) + ((rcv_y - src_y) ** 2))
+    dist_km = dist_m * 1E-3  # units: m -> km
+    dist_deg = kilometer2degrees(dist_km)  # spherical earth approximation
     azimuth = np.degrees(np.arctan2((rcv_x - src_x), (rcv_y - src_y))) % 360
     backazimuth = (azimuth - 180) % 360
-    otime = event.preferred_origin().time
-
-    # Barebones SAC header, we only append values required by RecSec
+    
     sac_header = {
+        "iztype": 9,  # Ref time equivalence, IB (9): Begin time
+        "b": tr.stats.starttime - otime,  # begin time
+        "e": tr.stats.npts * tr.stats.delta,  # end time
         "stla": rcv_y,
         "stlo": rcv_x,
         "evla": src_y,
         "evlo": src_x,
-        "dist": dist_m * 1E-3,  # units: km
+        "evdp": evdepth_km,
+        "dist": dist_km,
+        "gcarc": dist_deg,  # degrees
         "az": azimuth,
         "baz": backazimuth,
         "kevnm": format_event_tag_legacy(event),  # only take date code
         "nzyear": otime.year,
         "nzjday": otime.julday,
         "nzhour": otime.hour,
         "nzmin": otime.minute,
         "nzsec": otime.second,
         "nzmsec": otime.microsecond,
-        }
+        "lpspol": 0,  # 1 if left-hand polarity (usually no in passive seis)
+        "lcalda": 1,  # 1 if DIST, AZ, BAZ, GCARC to be calc'd from metadata
+    }
 
     tr.stats.sac = sac_header
 
     return tr
 
 
 def format_sac_header_w_taup_traveltimes(st, model="ak135",
```

### Comparing `pysep-adjtomo-0.5.1/pysep/utils/curtail.py` & `pysep_adjtomo-0.6.0/pysep/utils/curtail.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/utils/fetch.py` & `pysep_adjtomo-0.6.0/pysep/utils/fetch.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/utils/fmt.py` & `pysep_adjtomo-0.6.0/pysep/utils/fmt.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/utils/io.py` & `pysep_adjtomo-0.6.0/pysep/utils/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from obspy.core.inventory.network import Network
 from obspy.core.inventory.station import Station
 from obspy.geodetics import gps2dist_azimuth
 from obspy.core.event import Event, Origin, Magnitude
 
 from pysep import logger
 from pysep.utils.mt import moment_magnitude, seismic_moment
-from pysep.utils.fmt import format_event_tag_legacy, channel_code
+from pysep.utils.fmt import channel_code
 from pysep.utils.cap_sac import append_sac_headers, append_sac_headers_cartesian
 
 
 def read_yaml(fid):
     """
     Read a YAML file and return a dictionary
 
@@ -494,14 +494,75 @@
                     "event_magnitude": float(mag)
                     }
         list_out.append(dict_out)
 
     return list_out
 
 
+def read_asdfdataset(path, evaluation):
+    """
+    Read an ASDFDataSet created by a SeisFlows Pyaflowa inversion run. 
+    The dataset should contain observed and synthetic waveforms, and 
+    optionally contains misfit windows. Will return Streams with SAC headers
+
+    .. note::
+
+        This function makes assumptions about the PyASDF data structure which
+        is defined by the external package Pyatoa. If Pyatoa changes that
+        structure, this function will break.
+
+    :type path: str
+    :param path: Path to the ASDF dataset to be read
+    :type evaluation: str
+    :param evaluation: evaluation to take synthetics from. These are saved
+        following a format specified by Pyatoa, but usually follow the form
+        iteration/step_count, e.g., i01s00 gives iteration 1, step count 0.
+        Take a look at the waveform tags in `ASDFDataSet.waveforms[<station>]`
+        for tags following the 'synthetic_' prefix
+    """
+    # PySEP, by default will not require PyASDF to be installed
+    try:
+        from pyasdf import ASDFDataSet  # NOQA
+    except ImportError:
+        logger.critical("pyasdf is not installed. Please install pyasdf "
+                        "to read ASDF datasets")
+        return None, None
+
+    with ASDFDataSet(path) as ds:
+        event = ds.events[0]
+        st_out = Stream()
+        st_syn_out = Stream()
+        for station in ds.waveforms.list():
+            inv = ds.waveforms[station].StationXML
+            st = ds.waveforms[station].observed
+            st_syn = ds.waveforms[station][f"synthetic_{evaluation}"]
+
+            st_out += append_sac_headers(st, event, inv)
+            st_syn_out += append_sac_headers(st_syn, event, inv)
+
+        # Read windows from the dataset
+        windows = {}
+        if hasattr(ds.auxiliary_data, "MisfitWindows"):
+            iter_ = evaluation[:3]  # 'i01s00' -> 'i01'
+            step = evaluation[3:]
+            for station in ds.auxiliary_data.MisfitWindows[iter_][step].list():
+                parameters = ds.auxiliary_data.MisfitWindows[iter_][step][
+                    station].parameters
+                trace_id = parameters["channel_id"]
+                starttime = parameters["relative_starttime"]
+                endtime = parameters["relative_endtime"]    
+                # initialize empty window array
+                if trace_id not in windows:
+                    windows[trace_id] = []
+                
+                windows[trace_id].append((starttime, endtime))
+
+    return st_out, st_syn_out, windows
+
+
 def write_sem(st, unit, path="./", time_offset=0):
     """
     Write an ObsPy Stream in the two-column ASCII format that Specfem uses
 
     :type st: obspy.core.stream.Stream
     :param st: stream containing synthetic data to be written
     :type unit: str
```

### Comparing `pysep-adjtomo-0.5.1/pysep/utils/llnl.py` & `pysep_adjtomo-0.6.0/pysep/utils/llnl.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/utils/mt.py` & `pysep_adjtomo-0.6.0/pysep/utils/mt.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/utils/plot.py` & `pysep_adjtomo-0.6.0/pysep/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep/utils/process.py` & `pysep_adjtomo-0.6.0/pysep/utils/process.py`

 * *Files identical despite different names*

### Comparing `pysep-adjtomo-0.5.1/pysep_adjtomo.egg-info/PKG-INFO` & `pysep_adjtomo-0.6.0/pysep_adjtomo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysep-adjtomo
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python Seismogram Extraction and Processing
 Author: adjTomo Dev Team
 Author-email: adjtomo@gmail.com
 License: MIT License
         
         Copyright (c) University of Alaska Fairbanks
```

### Comparing `pysep-adjtomo-0.5.1/pysep_adjtomo.egg-info/SOURCES.txt` & `pysep_adjtomo-0.6.0/pysep_adjtomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

