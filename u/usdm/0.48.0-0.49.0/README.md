# Comparing `tmp/usdm-0.48.0.tar.gz` & `tmp/usdm-0.49.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usdm-0.48.0.tar", last modified: Fri Mar 29 08:05:34 2024, max compression
+gzip compressed data, was "usdm-0.49.0.tar", last modified: Sat Apr 20 07:15:44 2024, max compression
```

## Comparing `usdm-0.48.0.tar` & `usdm-0.49.0.tar`

### file list

```diff
@@ -1,228 +1,247 @@
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.288848 usdm-0.48.0/
--rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.48.0/LICENSE
--rw-r--r--   0 daveih     (501) staff       (20)    37067 2024-03-29 08:05:34.288475 usdm-0.48.0/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)    36409 2024-03-23 12:59:10.000000 usdm-0.48.0/README.md
--rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.48.0/pyproject.toml
--rw-r--r--   0 daveih     (501) staff       (20)       38 2024-03-29 08:05:34.288905 usdm-0.48.0/setup.cfg
--rw-r--r--   0 daveih     (501) staff       (20)      972 2023-10-12 07:52:37.000000 usdm-0.48.0/setup.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.173724 usdm-0.48.0/src/
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.287950 usdm-0.48.0/src/usdm.egg-info/
--rw-r--r--   0 daveih     (501) staff       (20)    37067 2024-03-29 08:05:34.000000 usdm-0.48.0/src/usdm.egg-info/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)     7787 2024-03-29 08:05:34.000000 usdm-0.48.0/src/usdm.egg-info/SOURCES.txt
--rw-r--r--   0 daveih     (501) staff       (20)        1 2024-03-29 08:05:34.000000 usdm-0.48.0/src/usdm.egg-info/dependency_links.txt
--rw-r--r--   0 daveih     (501) staff       (20)       73 2024-03-29 08:05:34.000000 usdm-0.48.0/src/usdm.egg-info/requires.txt
--rw-r--r--   0 daveih     (501) staff       (20)       32 2024-03-29 08:05:34.000000 usdm-0.48.0/src/usdm.egg-info/top_level.txt
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.192613 usdm-0.48.0/src/usdm_excel/
--rw-r--r--   0 daveih     (501) staff       (20)     2766 2024-02-22 05:10:08.000000 usdm-0.48.0/src/usdm_excel/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      302 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/alias.py
--rw-r--r--   0 daveih     (501) staff       (20)    17980 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)    15878 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      900 2023-11-27 15:49:16.000000 usdm-0.48.0/src/usdm_excel/cdisc_ct.py
--rw-r--r--   0 daveih     (501) staff       (20)     7198 2024-03-22 09:59:36.000000 usdm-0.48.0/src/usdm_excel/cdisc_ct_library.py
--rw-r--r--   0 daveih     (501) staff       (20)      402 2023-11-27 15:49:16.000000 usdm-0.48.0/src/usdm_excel/code_base.py
--rw-r--r--   0 daveih     (501) staff       (20)     1999 2024-01-02 13:11:00.000000 usdm-0.48.0/src/usdm_excel/configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     2825 2024-02-22 05:10:08.000000 usdm-0.48.0/src/usdm_excel/cross_ref.py
--rw-r--r--   0 daveih     (501) staff       (20)      345 2023-10-12 07:51:31.000000 usdm-0.48.0/src/usdm_excel/ct_version_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.201458 usdm-0.48.0/src/usdm_excel/data/
--rw-r--r--   0 daveih     (501) staff       (20)   833791 2024-03-29 05:59:21.000000 usdm-0.48.0/src/usdm_excel/data/cdisc_bcs.yaml
--rw-r--r--   0 daveih     (501) staff       (20)   994684 2024-03-29 08:02:31.000000 usdm-0.48.0/src/usdm_excel/data/cdisc_ct_2023-12-15.yaml
--rw-r--r--   0 daveih     (501) staff       (20)     1771 2024-03-29 08:02:31.000000 usdm-0.48.0/src/usdm_excel/data/cdisc_ct_config.yaml
--rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.48.0/src/usdm_excel/data/iso_3166.json
--rw-r--r--   0 daveih     (501) staff       (20)    17741 2024-03-29 08:02:31.000000 usdm-0.48.0/src/usdm_excel/data/missing_ct.yaml
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.215374 usdm-0.48.0/src/usdm_excel/document/
--rw-r--r--   0 daveih     (501) staff       (20)      115 2024-02-22 05:10:08.000000 usdm-0.48.0/src/usdm_excel/document/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)    14054 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/document/document.py
--rw-r--r--   0 daveih     (501) staff       (20)     4775 2024-02-22 05:10:08.000000 usdm-0.48.0/src/usdm_excel/document/elements.py
--rw-r--r--   0 daveih     (501) staff       (20)     4330 2024-02-22 05:10:08.000000 usdm-0.48.0/src/usdm_excel/document/macros.py
--rw-r--r--   0 daveih     (501) staff       (20)     5010 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/document/soa.py
--rw-r--r--   0 daveih     (501) staff       (20)     1065 2024-02-22 05:10:08.000000 usdm-0.48.0/src/usdm_excel/document/template_base.py
--rw-r--r--   0 daveih     (501) staff       (20)     4754 2024-02-22 05:10:08.000000 usdm-0.48.0/src/usdm_excel/document/template_m11.py
--rw-r--r--   0 daveih     (501) staff       (20)     5892 2024-02-22 05:10:08.000000 usdm-0.48.0/src/usdm_excel/document/template_plain.py
--rw-r--r--   0 daveih     (501) staff       (20)      772 2024-02-22 05:10:08.000000 usdm-0.48.0/src/usdm_excel/document/utility.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.217621 usdm-0.48.0/src/usdm_excel/errors/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-06 07:20:00.000000 usdm-0.48.0/src/usdm_excel/errors/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      933 2023-10-12 07:51:31.000000 usdm-0.48.0/src/usdm_excel/errors/error.py
--rw-r--r--   0 daveih     (501) staff       (20)      732 2023-10-12 07:51:31.000000 usdm-0.48.0/src/usdm_excel/errors/errors.py
--rw-r--r--   0 daveih     (501) staff       (20)     3338 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/export_as_neo4j_dict.py
--rw-r--r--   0 daveih     (501) staff       (20)     3596 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/export_as_timeline.py
--rw-r--r--   0 daveih     (501) staff       (20)     5215 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/export_as_yworks_dict.py
--rw-r--r--   0 daveih     (501) staff       (20)     1873 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/id_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)     1208 2024-02-22 05:10:08.000000 usdm-0.48.0/src/usdm_excel/iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      883 2023-10-12 07:51:31.000000 usdm-0.48.0/src/usdm_excel/iso_8601_duration.py
--rw-r--r--   0 daveih     (501) staff       (20)      111 2024-03-16 07:07:57.000000 usdm-0.48.0/src/usdm_excel/logger.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)      875 2024-01-02 13:11:00.000000 usdm-0.48.0/src/usdm_excel/option_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)      257 2023-10-12 07:51:31.000000 usdm-0.48.0/src/usdm_excel/other_ct.py
--rw-r--r--   0 daveih     (501) staff       (20)     1401 2024-01-02 13:11:00.000000 usdm-0.48.0/src/usdm_excel/quantity_type.py
--rw-r--r--   0 daveih     (501) staff       (20)     1523 2023-11-27 15:49:16.000000 usdm-0.48.0/src/usdm_excel/range_type.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.219207 usdm-0.48.0/src/usdm_excel/study_design_activity_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-05-03 10:02:41.000000 usdm-0.48.0/src/usdm_excel/study_design_activity_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1436 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.221307 usdm-0.48.0/src/usdm_excel/study_design_amendment_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-01 11:43:59.000000 usdm-0.48.0/src/usdm_excel/study_design_amendment_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     8026 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/study_design_amendment_sheet/study_design_amendment_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.222209 usdm-0.48.0/src/usdm_excel/study_design_arm_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.48.0/src/usdm_excel/study_design_arm_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1809 2023-11-27 15:49:16.000000 usdm-0.48.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.223143 usdm-0.48.0/src/usdm_excel/study_design_conditions_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2024-01-17 06:39:55.000000 usdm-0.48.0/src/usdm_excel/study_design_conditions_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2641 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_excel/study_design_conditions_sheet/study_design_conditions_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.224018 usdm-0.48.0/src/usdm_excel/study_design_content_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-10-12 07:51:31.000000 usdm-0.48.0/src/usdm_excel/study_design_content_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3336 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/study_design_content_sheet/study_design_content_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.226157 usdm-0.48.0/src/usdm_excel/study_design_dictionary_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-01 11:43:59.000000 usdm-0.48.0/src/usdm_excel/study_design_dictionary_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3070 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/study_design_dictionary_sheet/study_design_dictionary_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.230049 usdm-0.48.0/src/usdm_excel/study_design_element_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.48.0/src/usdm_excel/study_design_element_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2134 2023-11-27 15:49:16.000000 usdm-0.48.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.231630 usdm-0.48.0/src/usdm_excel/study_design_eligibility_criteria_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-01 11:43:59.000000 usdm-0.48.0/src/usdm_excel/study_design_eligibility_criteria_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3205 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/study_design_eligibility_criteria_sheet/study_design_eligibility_criteria_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.234478 usdm-0.48.0/src/usdm_excel/study_design_encounter_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.48.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3075 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.235405 usdm-0.48.0/src/usdm_excel/study_design_epoch_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.48.0/src/usdm_excel/study_design_epoch_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1449 2023-11-27 15:49:16.000000 usdm-0.48.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.240195 usdm-0.48.0/src/usdm_excel/study_design_estimands_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.48.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3595 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.240919 usdm-0.48.0/src/usdm_excel/study_design_indication_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-27 15:49:16.000000 usdm-0.48.0/src/usdm_excel/study_design_indication_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1182 2024-01-02 13:11:00.000000 usdm-0.48.0/src/usdm_excel/study_design_indication_sheet/study_design_indication_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.242091 usdm-0.48.0/src/usdm_excel/study_design_intervention_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-27 15:49:16.000000 usdm-0.48.0/src/usdm_excel/study_design_intervention_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     5600 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/study_design_intervention_sheet/study_design_intervention_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.244581 usdm-0.48.0/src/usdm_excel/study_design_objective_endpoint_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.48.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     4569 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.246004 usdm-0.48.0/src/usdm_excel/study_design_population_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.48.0/src/usdm_excel/study_design_population_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3726 2024-03-29 08:02:31.000000 usdm-0.48.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.246980 usdm-0.48.0/src/usdm_excel/study_design_procedure_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.48.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1894 2024-01-02 13:11:00.000000 usdm-0.48.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.249319 usdm-0.48.0/src/usdm_excel/study_design_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.48.0/src/usdm_excel/study_design_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     9247 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.251141 usdm-0.48.0/src/usdm_excel/study_design_sites_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2024-01-02 13:11:00.000000 usdm-0.48.0/src/usdm_excel/study_design_sites_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2238 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_excel/study_design_sites_sheet/study_design_sites_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.252781 usdm-0.48.0/src/usdm_excel/study_design_timing_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-10-12 07:52:37.000000 usdm-0.48.0/src/usdm_excel/study_design_timing_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3928 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/study_design_timing_sheet/study_design_timing_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      758 2023-11-27 15:49:16.000000 usdm-0.48.0/src/usdm_excel/study_design_timing_sheet/window_type.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.253562 usdm-0.48.0/src/usdm_excel/study_identifiers_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.48.0/src/usdm_excel/study_identifiers_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2452 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.255492 usdm-0.48.0/src/usdm_excel/study_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.48.0/src/usdm_excel/study_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)    19339 2024-03-29 05:18:23.000000 usdm-0.48.0/src/usdm_excel/study_sheet/study_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.259493 usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-10-12 07:52:37.000000 usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      513 2023-11-01 11:43:59.000000 usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/activities.py
--rw-r--r--   0 daveih     (501) staff       (20)     4157 2024-02-22 05:10:08.000000 usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      686 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/conditons.py
--rw-r--r--   0 daveih     (501) staff       (20)     3758 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instance.py
--rw-r--r--   0 daveih     (501) staff       (20)     2452 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instances.py
--rw-r--r--   0 daveih     (501) staff       (20)      292 2023-10-12 07:52:37.000000 usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/soa_column_rows.py
--rw-r--r--   0 daveih     (501) staff       (20)     4155 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/study_soa_v2_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.259869 usdm-0.48.0/src/usdm_info/
--rw-r--r--   0 daveih     (501) staff       (20)       59 2024-03-29 08:02:31.000000 usdm-0.48.0/src/usdm_info/__init__.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.274243 usdm-0.48.0/src/usdm_model/
--rw-r--r--   0 daveih     (501) staff       (20)     2792 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      481 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      414 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/address.py
--rw-r--r--   0 daveih     (501) staff       (20)      328 2024-03-29 08:02:31.000000 usdm-0.48.0/src/usdm_model/administration_duration.py
--rw-r--r--   0 daveih     (501) staff       (20)      420 2024-03-29 08:02:31.000000 usdm-0.48.0/src/usdm_model/agent_administration.py
--rw-r--r--   0 daveih     (501) staff       (20)      238 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/alias_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      211 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/analysis_population.py
--rw-r--r--   0 daveih     (501) staff       (20)     1538 2024-02-09 13:14:36.000000 usdm-0.48.0/src/usdm_model/api_base_model.py
--rw-r--r--   0 daveih     (501) staff       (20)      409 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      353 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/biomedical_concept_category.py
--rw-r--r--   0 daveih     (501) staff       (20)      397 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/biomedical_concept_property.py
--rw-r--r--   0 daveih     (501) staff       (20)      259 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/biomedical_concept_surrogate.py
--rw-r--r--   0 daveih     (501) staff       (20)      152 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/characteristic.py
--rw-r--r--   0 daveih     (501) staff       (20)      208 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/code.py
--rw-r--r--   0 daveih     (501) staff       (20)      306 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/condition.py
--rw-r--r--   0 daveih     (501) staff       (20)      338 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/eligibility_criterion.py
--rw-r--r--   0 daveih     (501) staff       (20)      573 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/encounter.py
--rw-r--r--   0 daveih     (501) staff       (20)      192 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/endpoint.py
--rw-r--r--   0 daveih     (501) staff       (20)      414 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/estimand.py
--rw-r--r--   0 daveih     (501) staff       (20)      416 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/geographic_scope.py
--rw-r--r--   0 daveih     (501) staff       (20)      365 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/governance_date.py
--rw-r--r--   0 daveih     (501) staff       (20)      259 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/indication.py
--rw-r--r--   0 daveih     (501) staff       (20)      213 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/intercurrent_event.py
--rw-r--r--   0 daveih     (501) staff       (20)      195 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/masking.py
--rw-r--r--   0 daveih     (501) staff       (20)      362 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_model/narrative_content.py
--rw-r--r--   0 daveih     (501) staff       (20)      256 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_model/objective.py
--rw-r--r--   0 daveih     (501) staff       (20)      507 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/organization.py
--rw-r--r--   0 daveih     (501) staff       (20)      913 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_model/population_definition.py
--rw-r--r--   0 daveih     (501) staff       (20)      292 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/procedure.py
--rw-r--r--   0 daveih     (501) staff       (20)      241 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_model/quantity.py
--rw-r--r--   0 daveih     (501) staff       (20)      262 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/range.py
--rw-r--r--   0 daveih     (501) staff       (20)      209 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/response_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      589 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/schedule_timeline.py
--rw-r--r--   0 daveih     (501) staff       (20)      171 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/schedule_timeline_exit.py
--rw-r--r--   0 daveih     (501) staff       (20)      899 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_model/scheduled_instance.py
--rw-r--r--   0 daveih     (501) staff       (20)      523 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/study.py
--rw-r--r--   0 daveih     (501) staff       (20)      499 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/study_amendment.py
--rw-r--r--   0 daveih     (501) staff       (20)      253 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/study_amendment_reason.py
--rw-r--r--   0 daveih     (501) staff       (20)      305 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/study_arm.py
--rw-r--r--   0 daveih     (501) staff       (20)      212 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/study_cell.py
--rw-r--r--   0 daveih     (501) staff       (20)     2236 2024-02-22 05:10:08.000000 usdm-0.48.0/src/usdm_model/study_design.py
--rw-r--r--   0 daveih     (501) staff       (20)      397 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/study_element.py
--rw-r--r--   0 daveih     (501) staff       (20)      298 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/study_epoch.py
--rw-r--r--   0 daveih     (501) staff       (20)      260 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/study_identifier.py
--rw-r--r--   0 daveih     (501) staff       (20)      549 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_model/study_intervention.py
--rw-r--r--   0 daveih     (501) staff       (20)      337 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/study_protocol_document.py
--rw-r--r--   0 daveih     (501) staff       (20)      461 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/study_protocol_document_version.py
--rw-r--r--   0 daveih     (501) staff       (20)      295 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/study_site.py
--rw-r--r--   0 daveih     (501) staff       (20)      199 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/study_title.py
--rw-r--r--   0 daveih     (501) staff       (20)      876 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/study_version.py
--rw-r--r--   0 daveih     (501) staff       (20)      250 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/syntax_template.py
--rw-r--r--   0 daveih     (501) staff       (20)      422 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_model/syntax_template_dictionary.py
--rw-r--r--   0 daveih     (501) staff       (20)      505 2024-03-23 12:59:10.000000 usdm-0.48.0/src/usdm_model/timing.py
--rw-r--r--   0 daveih     (501) staff       (20)      203 2024-01-25 11:26:05.000000 usdm-0.48.0/src/usdm_model/transition_rule.py
--rw-r--r--   0 daveih     (501) staff       (20)      233 2024-03-29 05:18:23.000000 usdm-0.48.0/src/usdm_model/wrapper.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-03-29 08:05:34.287619 usdm-0.48.0/tests/
--rw-r--r--   0 daveih     (501) staff       (20)    21488 2024-03-23 12:59:10.000000 usdm-0.48.0/tests/test_base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     1030 2024-03-22 09:59:36.000000 usdm-0.48.0/tests/test_cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      238 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_cdisc_ct.py
--rw-r--r--   0 daveih     (501) staff       (20)     2631 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4983 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_cross_reference.py
--rw-r--r--   0 daveih     (501) staff       (20)     2249 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_data_factory.py
--rw-r--r--   0 daveih     (501) staff       (20)     1655 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_document.py
--rw-r--r--   0 daveih     (501) staff       (20)     1532 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_document_macros.py
--rw-r--r--   0 daveih     (501) staff       (20)    10074 2024-03-23 12:59:10.000000 usdm-0.48.0/tests/test_document_soa.py
--rw-r--r--   0 daveih     (501) staff       (20)     1537 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_document_template_plain.py
--rw-r--r--   0 daveih     (501) staff       (20)      941 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_document_utility.py
--rw-r--r--   0 daveih     (501) staff       (20)      861 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_error.py
--rw-r--r--   0 daveih     (501) staff       (20)     2230 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_errors.py
--rw-r--r--   0 daveih     (501) staff       (20)     1246 2024-03-29 07:25:34.000000 usdm-0.48.0/tests/test_export.py
--rw-r--r--   0 daveih     (501) staff       (20)      988 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_factory.py
--rw-r--r--   0 daveih     (501) staff       (20)     5789 2024-03-29 08:02:32.000000 usdm-0.48.0/tests/test_integration.py
--rw-r--r--   0 daveih     (501) staff       (20)     2090 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)     1759 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_iso_8601_duration.py
--rw-r--r--   0 daveih     (501) staff       (20)      410 2024-03-23 12:59:10.000000 usdm-0.48.0/tests/test_ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)     1447 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_option_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)     2182 2024-01-17 06:39:55.000000 usdm-0.48.0/tests/test_quantity_type.py
--rw-r--r--   0 daveih     (501) staff       (20)     1176 2023-11-27 15:49:16.000000 usdm-0.48.0/tests/test_range_type.py
--rw-r--r--   0 daveih     (501) staff       (20)     2152 2024-01-02 13:11:00.000000 usdm-0.48.0/tests/test_study_design_activity_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     5400 2023-11-27 15:49:16.000000 usdm-0.48.0/tests/test_study_design_arm_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4984 2024-01-25 11:26:05.000000 usdm-0.48.0/tests/test_study_design_conditions_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)    10044 2024-03-23 12:59:10.000000 usdm-0.48.0/tests/test_study_design_content_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4276 2024-03-23 12:59:10.000000 usdm-0.48.0/tests/test_study_design_dictionary_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     3643 2023-11-27 15:49:16.000000 usdm-0.48.0/tests/test_study_design_eligibility_criteria_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4735 2023-11-27 15:49:16.000000 usdm-0.48.0/tests/test_study_design_encounter_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4044 2023-11-27 15:49:16.000000 usdm-0.48.0/tests/test_study_design_epoch_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     3118 2023-11-27 15:49:16.000000 usdm-0.48.0/tests/test_study_design_indication_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     5756 2024-03-23 12:59:10.000000 usdm-0.48.0/tests/test_study_design_intervention_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4772 2024-03-29 08:02:32.000000 usdm-0.48.0/tests/test_study_design_oe_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4271 2024-01-25 11:26:05.000000 usdm-0.48.0/tests/test_study_design_sites_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4877 2023-11-27 15:49:16.000000 usdm-0.48.0/tests/test_study_design_timing_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     7318 2023-11-27 15:49:16.000000 usdm-0.48.0/tests/test_study_identifiers_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     1391 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_study_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      199 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_study_soa_v2_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      429 2024-02-22 05:10:08.000000 usdm-0.48.0/tests/test_utility.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.485732 usdm-0.49.0/
+-rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.49.0/LICENSE
+-rw-r--r--   0 daveih     (501) staff       (20)    38155 2024-04-20 07:15:44.485353 usdm-0.49.0/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)    37497 2024-04-19 04:39:42.000000 usdm-0.49.0/README.md
+-rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.49.0/pyproject.toml
+-rw-r--r--   0 daveih     (501) staff       (20)       38 2024-04-20 07:15:44.485790 usdm-0.49.0/setup.cfg
+-rw-r--r--   0 daveih     (501) staff       (20)      972 2023-10-12 07:52:37.000000 usdm-0.49.0/setup.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.423192 usdm-0.49.0/src/
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.484742 usdm-0.49.0/src/usdm.egg-info/
+-rw-r--r--   0 daveih     (501) staff       (20)    38155 2024-04-20 07:15:44.000000 usdm-0.49.0/src/usdm.egg-info/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)     8436 2024-04-20 07:15:44.000000 usdm-0.49.0/src/usdm.egg-info/SOURCES.txt
+-rw-r--r--   0 daveih     (501) staff       (20)        1 2024-04-20 07:15:44.000000 usdm-0.49.0/src/usdm.egg-info/dependency_links.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       73 2024-04-20 07:15:44.000000 usdm-0.49.0/src/usdm.egg-info/requires.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       40 2024-04-20 07:15:44.000000 usdm-0.49.0/src/usdm.egg-info/top_level.txt
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.426323 usdm-0.49.0/src/usdm_db/
+-rw-r--r--   0 daveih     (501) staff       (20)     2478 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_db/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1454 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_db/cross_reference.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.427121 usdm-0.49.0/src/usdm_db/document/
+-rw-r--r--   0 daveih     (501) staff       (20)       27 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_db/document/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)    13622 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_db/document/document.py
+-rw-r--r--   0 daveih     (501) staff       (20)      758 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_db/document/utility.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.428273 usdm-0.49.0/src/usdm_db/errors_and_logging/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_db/errors_and_logging/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      602 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_db/errors_and_logging/error.py
+-rw-r--r--   0 daveih     (501) staff       (20)      696 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_db/errors_and_logging/errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1013 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_db/errors_and_logging/errors_and_logging.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3331 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_db/neo4j_dict.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3608 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_db/timeline.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.434368 usdm-0.49.0/src/usdm_excel/
+-rw-r--r--   0 daveih     (501) staff       (20)    12623 2024-04-19 04:16:10.000000 usdm-0.49.0/src/usdm_excel/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      364 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/alias.py
+-rw-r--r--   0 daveih     (501) staff       (20)    18660 2024-04-19 04:16:10.000000 usdm-0.49.0/src/usdm_excel/base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)    16463 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/cdisc_bc_library.py
+-rw-r--r--   0 daveih     (501) staff       (20)      987 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/cdisc_ct.py
+-rw-r--r--   0 daveih     (501) staff       (20)     7304 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/cdisc_ct_library.py
+-rw-r--r--   0 daveih     (501) staff       (20)      523 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/code_base.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1795 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2987 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/cross_ref.py
+-rw-r--r--   0 daveih     (501) staff       (20)      478 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/ct_version_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.443805 usdm-0.49.0/src/usdm_excel/data/
+-rw-r--r--   0 daveih     (501) staff       (20)   833791 2024-03-29 05:59:21.000000 usdm-0.49.0/src/usdm_excel/data/cdisc_bcs.yaml
+-rw-r--r--   0 daveih     (501) staff       (20)   994684 2024-03-29 08:02:31.000000 usdm-0.49.0/src/usdm_excel/data/cdisc_ct_2023-12-15.yaml
+-rw-r--r--   0 daveih     (501) staff       (20)     1771 2024-03-29 08:02:31.000000 usdm-0.49.0/src/usdm_excel/data/cdisc_ct_config.yaml
+-rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.49.0/src/usdm_excel/data/iso_3166.json
+-rw-r--r--   0 daveih     (501) staff       (20)    17843 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/data/missing_ct.yaml
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.446286 usdm-0.49.0/src/usdm_excel/document/
+-rw-r--r--   0 daveih     (501) staff       (20)      101 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/document/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5268 2024-04-19 04:16:10.000000 usdm-0.49.0/src/usdm_excel/document/elements.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5796 2024-04-19 14:44:40.000000 usdm-0.49.0/src/usdm_excel/document/macros.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5087 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/document/soa.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1065 2024-04-05 04:37:08.000000 usdm-0.49.0/src/usdm_excel/document/template_base.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4803 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/document/template_m11.py
+-rw-r--r--   0 daveih     (501) staff       (20)     6608 2024-04-19 11:24:09.000000 usdm-0.49.0/src/usdm_excel/document/template_plain.py
+-rw-r--r--   0 daveih     (501) staff       (20)      658 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/document/utility.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.447233 usdm-0.49.0/src/usdm_excel/errors_and_logging/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/errors_and_logging/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      933 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/errors_and_logging/error.py
+-rw-r--r--   0 daveih     (501) staff       (20)      632 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/errors_and_logging/errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1735 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/errors_and_logging/errors_and_logging.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1156 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/globals.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2040 2024-04-19 04:16:10.000000 usdm-0.49.0/src/usdm_excel/id_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1250 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      883 2023-10-12 07:51:31.000000 usdm-0.49.0/src/usdm_excel/iso_8601_duration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      376 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)      854 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/option_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)      200 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/other_ct.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1501 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/quantity_type.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1604 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/range_type.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.447642 usdm-0.49.0/src/usdm_excel/study_design_activity_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-05-03 10:02:41.000000 usdm-0.49.0/src/usdm_excel/study_design_activity_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1305 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.448001 usdm-0.49.0/src/usdm_excel/study_design_amendment_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-01 11:43:59.000000 usdm-0.49.0/src/usdm_excel/study_design_amendment_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     7916 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_amendment_sheet/study_design_amendment_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.448558 usdm-0.49.0/src/usdm_excel/study_design_arm_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.49.0/src/usdm_excel/study_design_arm_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1702 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.448876 usdm-0.49.0/src/usdm_excel/study_design_characteristics_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2024-04-19 04:16:10.000000 usdm-0.49.0/src/usdm_excel/study_design_characteristics_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1527 2024-04-19 04:16:10.000000 usdm-0.49.0/src/usdm_excel/study_design_characteristics_sheet/study_design_characteristics_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.449225 usdm-0.49.0/src/usdm_excel/study_design_conditions_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2024-01-17 06:39:55.000000 usdm-0.49.0/src/usdm_excel/study_design_conditions_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2714 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_conditions_sheet/study_design_conditions_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.449574 usdm-0.49.0/src/usdm_excel/study_design_content_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-10-12 07:51:31.000000 usdm-0.49.0/src/usdm_excel/study_design_content_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3275 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_content_sheet/study_design_content_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.449910 usdm-0.49.0/src/usdm_excel/study_design_dictionary_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-01 11:43:59.000000 usdm-0.49.0/src/usdm_excel/study_design_dictionary_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2977 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_dictionary_sheet/study_design_dictionary_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.450286 usdm-0.49.0/src/usdm_excel/study_design_element_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.49.0/src/usdm_excel/study_design_element_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2051 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.450881 usdm-0.49.0/src/usdm_excel/study_design_eligibility_criteria_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-01 11:43:59.000000 usdm-0.49.0/src/usdm_excel/study_design_eligibility_criteria_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1872 2024-04-19 04:16:10.000000 usdm-0.49.0/src/usdm_excel/study_design_eligibility_criteria_sheet/study_design_eligibility_criteria_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.451253 usdm-0.49.0/src/usdm_excel/study_design_encounter_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.49.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3005 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.451658 usdm-0.49.0/src/usdm_excel/study_design_epoch_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.49.0/src/usdm_excel/study_design_epoch_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1342 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.451954 usdm-0.49.0/src/usdm_excel/study_design_estimands_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.49.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3397 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.452468 usdm-0.49.0/src/usdm_excel/study_design_indication_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-27 15:49:16.000000 usdm-0.49.0/src/usdm_excel/study_design_indication_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1125 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_indication_sheet/study_design_indication_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.452910 usdm-0.49.0/src/usdm_excel/study_design_intervention_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-27 15:49:16.000000 usdm-0.49.0/src/usdm_excel/study_design_intervention_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5431 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_intervention_sheet/study_design_intervention_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.453357 usdm-0.49.0/src/usdm_excel/study_design_objective_endpoint_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.49.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3502 2024-04-19 04:16:10.000000 usdm-0.49.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.453733 usdm-0.49.0/src/usdm_excel/study_design_population_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.49.0/src/usdm_excel/study_design_population_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3964 2024-04-19 04:16:10.000000 usdm-0.49.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.454060 usdm-0.49.0/src/usdm_excel/study_design_procedure_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.49.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1538 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.454370 usdm-0.49.0/src/usdm_excel/study_design_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.49.0/src/usdm_excel/study_design_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     9083 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.455001 usdm-0.49.0/src/usdm_excel/study_design_sites_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2024-01-02 13:11:00.000000 usdm-0.49.0/src/usdm_excel/study_design_sites_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2187 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_sites_sheet/study_design_sites_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.456081 usdm-0.49.0/src/usdm_excel/study_design_timing_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-10-12 07:52:37.000000 usdm-0.49.0/src/usdm_excel/study_design_timing_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3851 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_timing_sheet/study_design_timing_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      819 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_design_timing_sheet/window_type.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.456407 usdm-0.49.0/src/usdm_excel/study_identifiers_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.49.0/src/usdm_excel/study_identifiers_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2074 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.456726 usdm-0.49.0/src/usdm_excel/study_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.49.0/src/usdm_excel/study_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     9005 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_sheet/study_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.459389 usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-10-12 07:52:37.000000 usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      514 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/activities.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4230 2024-04-19 14:44:40.000000 usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      686 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/conditons.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3872 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instance.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2494 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instances.py
+-rw-r--r--   0 daveih     (501) staff       (20)      292 2023-10-12 07:52:37.000000 usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/soa_column_rows.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4035 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/study_soa_v2_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1541 2024-04-19 04:16:10.000000 usdm-0.49.0/src/usdm_excel/syntax_template_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.459641 usdm-0.49.0/src/usdm_info/
+-rw-r--r--   0 daveih     (501) staff       (20)       59 2024-04-18 13:50:02.000000 usdm-0.49.0/src/usdm_info/__init__.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.472257 usdm-0.49.0/src/usdm_model/
+-rw-r--r--   0 daveih     (501) staff       (20)     2792 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      481 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      414 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/address.py
+-rw-r--r--   0 daveih     (501) staff       (20)      328 2024-03-29 08:02:31.000000 usdm-0.49.0/src/usdm_model/administration_duration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      420 2024-03-29 08:02:31.000000 usdm-0.49.0/src/usdm_model/agent_administration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      238 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/alias_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      211 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/analysis_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1538 2024-02-09 13:14:36.000000 usdm-0.49.0/src/usdm_model/api_base_model.py
+-rw-r--r--   0 daveih     (501) staff       (20)      409 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      353 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/biomedical_concept_category.py
+-rw-r--r--   0 daveih     (501) staff       (20)      397 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/biomedical_concept_property.py
+-rw-r--r--   0 daveih     (501) staff       (20)      259 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/biomedical_concept_surrogate.py
+-rw-r--r--   0 daveih     (501) staff       (20)      152 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/characteristic.py
+-rw-r--r--   0 daveih     (501) staff       (20)      208 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      306 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/condition.py
+-rw-r--r--   0 daveih     (501) staff       (20)      338 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/eligibility_criterion.py
+-rw-r--r--   0 daveih     (501) staff       (20)      573 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/encounter.py
+-rw-r--r--   0 daveih     (501) staff       (20)      192 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/endpoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)      414 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/estimand.py
+-rw-r--r--   0 daveih     (501) staff       (20)      416 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/geographic_scope.py
+-rw-r--r--   0 daveih     (501) staff       (20)      365 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/governance_date.py
+-rw-r--r--   0 daveih     (501) staff       (20)      259 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/indication.py
+-rw-r--r--   0 daveih     (501) staff       (20)      213 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/intercurrent_event.py
+-rw-r--r--   0 daveih     (501) staff       (20)      195 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/masking.py
+-rw-r--r--   0 daveih     (501) staff       (20)      362 2024-03-23 12:59:10.000000 usdm-0.49.0/src/usdm_model/narrative_content.py
+-rw-r--r--   0 daveih     (501) staff       (20)      256 2024-03-23 12:59:10.000000 usdm-0.49.0/src/usdm_model/objective.py
+-rw-r--r--   0 daveih     (501) staff       (20)      507 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/organization.py
+-rw-r--r--   0 daveih     (501) staff       (20)      913 2024-03-23 12:59:10.000000 usdm-0.49.0/src/usdm_model/population_definition.py
+-rw-r--r--   0 daveih     (501) staff       (20)      292 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/procedure.py
+-rw-r--r--   0 daveih     (501) staff       (20)      241 2024-03-23 12:59:10.000000 usdm-0.49.0/src/usdm_model/quantity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      262 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/range.py
+-rw-r--r--   0 daveih     (501) staff       (20)      209 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/response_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      589 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/schedule_timeline.py
+-rw-r--r--   0 daveih     (501) staff       (20)      171 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/schedule_timeline_exit.py
+-rw-r--r--   0 daveih     (501) staff       (20)      899 2024-03-23 12:59:10.000000 usdm-0.49.0/src/usdm_model/scheduled_instance.py
+-rw-r--r--   0 daveih     (501) staff       (20)      523 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/study.py
+-rw-r--r--   0 daveih     (501) staff       (20)      499 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/study_amendment.py
+-rw-r--r--   0 daveih     (501) staff       (20)      253 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/study_amendment_reason.py
+-rw-r--r--   0 daveih     (501) staff       (20)      305 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/study_arm.py
+-rw-r--r--   0 daveih     (501) staff       (20)      212 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/study_cell.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2236 2024-02-22 05:10:08.000000 usdm-0.49.0/src/usdm_model/study_design.py
+-rw-r--r--   0 daveih     (501) staff       (20)      397 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/study_element.py
+-rw-r--r--   0 daveih     (501) staff       (20)      298 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/study_epoch.py
+-rw-r--r--   0 daveih     (501) staff       (20)      260 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/study_identifier.py
+-rw-r--r--   0 daveih     (501) staff       (20)      549 2024-03-23 12:59:10.000000 usdm-0.49.0/src/usdm_model/study_intervention.py
+-rw-r--r--   0 daveih     (501) staff       (20)      337 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/study_protocol_document.py
+-rw-r--r--   0 daveih     (501) staff       (20)      461 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/study_protocol_document_version.py
+-rw-r--r--   0 daveih     (501) staff       (20)      295 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/study_site.py
+-rw-r--r--   0 daveih     (501) staff       (20)      199 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/study_title.py
+-rw-r--r--   0 daveih     (501) staff       (20)      876 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/study_version.py
+-rw-r--r--   0 daveih     (501) staff       (20)      250 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/syntax_template.py
+-rw-r--r--   0 daveih     (501) staff       (20)      422 2024-03-23 12:59:10.000000 usdm-0.49.0/src/usdm_model/syntax_template_dictionary.py
+-rw-r--r--   0 daveih     (501) staff       (20)      505 2024-03-23 12:59:10.000000 usdm-0.49.0/src/usdm_model/timing.py
+-rw-r--r--   0 daveih     (501) staff       (20)      203 2024-01-25 11:26:05.000000 usdm-0.49.0/src/usdm_model/transition_rule.py
+-rw-r--r--   0 daveih     (501) staff       (20)      233 2024-03-29 05:18:23.000000 usdm-0.49.0/src/usdm_model/wrapper.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:15:44.484462 usdm-0.49.0/tests/
+-rw-r--r--   0 daveih     (501) staff       (20)    22464 2024-04-19 04:16:10.000000 usdm-0.49.0/tests/test_base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1102 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      274 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_cdisc_ct.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2684 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5360 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_cross_reference.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3035 2024-04-19 04:16:10.000000 usdm-0.49.0/tests/test_data_factory.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1521 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_document.py
+-rw-r--r--   0 daveih     (501) staff       (20)      561 2024-04-19 04:16:10.000000 usdm-0.49.0/tests/test_document_elements.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4606 2024-04-19 14:44:40.000000 usdm-0.49.0/tests/test_document_macros.py
+-rw-r--r--   0 daveih     (501) staff       (20)    10171 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_document_soa.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1413 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_document_template_plain.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1098 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_document_utility.py
+-rw-r--r--   0 daveih     (501) staff       (20)      873 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_error.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2278 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1311 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_export.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1486 2024-04-19 14:44:40.000000 usdm-0.49.0/tests/test_factory.py
+-rw-r--r--   0 daveih     (501) staff       (20)      377 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_globals.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5048 2024-04-19 13:15:43.000000 usdm-0.49.0/tests/test_integration.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2143 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1768 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_iso_8601_duration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      437 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1693 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_option_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2293 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_quantity_type.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1251 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_range_type.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1905 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_design_activity_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5542 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_design_arm_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3317 2024-04-19 04:16:10.000000 usdm-0.49.0/tests/test_study_design_characteristic_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     7055 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_design_conditions_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)    10476 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_design_content_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4310 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_design_dictionary_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3750 2024-04-18 14:04:27.000000 usdm-0.49.0/tests/test_study_design_eligibility_criteria_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4901 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_design_encounter_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4206 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_design_epoch_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3226 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_design_indication_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5830 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_design_intervention_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4848 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_design_oe_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4503 2024-04-19 04:16:10.000000 usdm-0.49.0/tests/test_study_design_population_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4364 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_design_sites_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5029 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_design_timing_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     9759 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_identifiers_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1400 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_study_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      199 2024-02-22 05:10:08.000000 usdm-0.49.0/tests/test_study_soa_v2_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      513 2024-04-18 13:50:02.000000 usdm-0.49.0/tests/test_utility.py
```

### Comparing `usdm-0.48.0/LICENSE` & `usdm-0.49.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/PKG-INFO` & `usdm-0.49.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.48.0
+Version: 0.49.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -80,14 +80,15 @@
 - Study Design sheet
 - One or more Timeline sheets
 - Study Design Timing sheet
 - Study Design Activities sheet (optional)
 - Study Design Indications sheet
 - Study Design Interventions sheet
 - Study Design Populations sheet
+- Study Design Characteristcis sheet
 - Study Design Objectives and Endpoints sheet
 - Study Design Eligibility Criteria sheet
 - Study Design Estimands sheet
 - Study Design Procedures sheet
 - Study Design Encounters sheet
 - Study Design Elements sheet
 - Study Design Content sheet
@@ -136,17 +137,17 @@
 - Minutes: 'M', 'MINS', 'MIN', 'MINUTES', 'MINUTE'
 - Seconds: 'S', 'SECS', 'SEC', 'SECONDS', 'SECOND'
 
 So ```3 Y```, ```3 YRS```, ```3 YR```, ```3 YEARS```, ```3 YEAR``` are all equivalent. Only a single value and unit should be entered, i.e. combination values are not supported.
 
 ### Templated Text
 
-Some entries can include "tags" that allow the text to reference structured content from elsewhere in the model. An example is an activity name. These sections of text are formatted as `[tag_name]` within the text. The `tag_name` refers to an entry within a dictionary (see the dictionaries sheet)
+Some entries can include "tags" that allow the text to reference structured content from elsewhere in the model. An example is an eligibility criterion referring to population definitions or an activity name. These sections of text are formatted as `<usdm:tag name="...tag_name..."/>` within the text. The `...tag_name...` refers to an entry within a dictionary (see the dictionaries sheet)
 
-An example of Templated Text is `Subjects shall be between [min_age] and [max_age]` where the min and max ages will be inserted using the dictionary entries that refer to particular attribute values from within the structured parts of the model.
+An example of Templated Text is `Subjects shall be between <usdm:tag name="min_age"/> and <usdm:tag name="max_age"/>` where the min and max ages will be inserted using the dictionary entries that refer to particular attribute values from within the structured parts of the model.
 
 ### Sheet Descriptions
 
 The sheet descriptions detail the fields found within each sheet and the details of the data required. Note:
 
 - Some fields have multiple names due to model changes and a desire to preserve backwards compatibility. Any of the choices documented can be used. 
 - Some columns are optional and thus can be included or omitted. Again this is to preserve backwards compatibility. A default value is specified if the column is not included.
@@ -201,21 +202,21 @@
 
 #### Sheet Contents
 
 A header row in row 1 followed by repeating rows from row 2, each containing a study identifier: 
 
 | Column | Column Name | Purpose | Format and Values |
 | :--- | :--- | :--- | :--- |
-| A | organisationIdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
-| B | organisationIdentifier | Organisation identifier | Text string |
+| A | organisationIdentifierScheme, organizationIdentifierScheme or IdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
+| B | organisationIdentifier or identifier | Organisation identifier | Text string |
 | C | organisationName or name | Organisation name | Text string |
 | D (optional) | label | Display label | Text string, can be empty. Default value is '' |
-| E | organisationType or type | Organisation type | CDISC code reference |
+| E | organisationType, organizationType or type | Organisation type | CDISC code reference |
 | F | studyIdentifier | The identifier for the study | Text string |
-| G | organisationAddress | The organisation address | Address |
+| G | organisationAddress, organizationAddress or address | The organisation address | Address |
 
 
 ### Study Amendments	Sheet
 	
 #### Sheet Name
 
 `studyAmendments`
@@ -494,27 +495,46 @@
 
 #### Sheet Name
 
 `studyDesignPopulations`
 
 #### Sheet Contents
 
-A header row in row 1 followed by repeating rows from row 2 containing population or sub-population definitions. Note that not every entry in columns E through I need to be filled in, just enough to define  either the whole population of the sub-populations. Sub-population need not be specificed.
+A header row in row 1 followed by repeating rows from row 2 containing population or sub-population definitions. Note that not every entry in columns E through I need to be filled in, just enough to define  either the whole population of the sub-populations. Sub-populations need not be specificed.
 
 | Column | Column Name | Purpose | Format and Values |
 | :--- | :--- | :--- | :--- |
 | A | level	| Level of entry | Set to either `MAIN` for the main population entry. All other values equate to a cohort (sub population) entry | 
 | B | name	| Identifier | Text string | 
 | C | description| Description | Text string, can be empty | 
 | D | label | Display label | Text string, can be empty |
 | E | plannedCompletionNumber	| Number of participants to complete the study | Integer | 
 | F | plannedEnrollmentNumber	| Number of participants to be enrolled | Integer | 
 | G | plannedAge	| Age range of participants | Range |
 | H | plannedSexOfParticipants | Sex of participants | CDISC code reference |
 | I | includesHealthSubjects | Healthy subjects flag | Boolean |
+| I | characterisitcs | List of characteristics for the cohort (ignored for main population) | Comma separated list of charcateristics name references |
+
+### Study Design Characteristics sheet
+
+#### Sheet Name
+
+`studyDesignCharacteristics`
+
+#### Sheet Contents
+
+A header row in row 1 followed by repeating rows from row 2 containing characteristics for cohorts.
+
+| Column | Column Name | Purpose | Format and Values |
+| :--- | :--- | :--- | :--- |
+| A | name	| Identifier | Text string | 
+| B | description| Description | Text string, can be empty | 
+| C | label | Display label | Text string, can be empty |
+| D | text	| Criteria text | Templated text |
+| E | dictionary| Dictionary cross reference | The dictionary from which the templated text tags are taken. If no tags are used can be empty |
 
 ### Study Design Objectives and Endpoints sheet
 
 #### Sheet Name
 
 `studyDesignOE`
 
@@ -668,18 +688,23 @@
 | element | Refer to a predefined element | 'name' of the element. Supported element names are 'study_phase', 'study_short_title', 'study_full_title', 'study_acronym', 'study_rationale', 'study_version_identifier', 'study_identifier', 'study_regulatory_identifiers', 'study_date', 'approval_date', 'organization_name_and_address', 'amendment' and 'amendment_scope' |
 | section | Add a pre defined section into the document | 'name' and 'template'. Supported section are 'title_page', 'inclusion', 'exclusion' and 'objective_endpoints'. Supported templates are 'm11' and 'plain' |
 | note | Insert a note into the document | 'text' |
 
 Examples of macros are:
 
 ```<usdm:macro id="xref" klass="Objective" name="OBJ1" attribute="text"/>```
+
 ```<usdm:macro id="xref" klass="StudyDesignPopulation" name="STUDY_POP" attribute="@plannedCompletionNumber/Range/maxValue"/>```
+
 ```<usdm:macro id="element" name="study_identifier"/>```
+
 ```<usdm:macro id="image" file="design.png" type="png"/>```
+
 ```<usdm:macro id="section" name="inclusion" template="plain"/>```
+
 ```<usdm:macro id="note" text="A note here please"/>```
 
 ### Study Design Sites sheet
 
 #### Sheet Name
 
 `studyDesignSites`
```

### Comparing `usdm-0.48.0/README.md` & `usdm-0.49.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 - Study Design sheet
 - One or more Timeline sheets
 - Study Design Timing sheet
 - Study Design Activities sheet (optional)
 - Study Design Indications sheet
 - Study Design Interventions sheet
 - Study Design Populations sheet
+- Study Design Characteristcis sheet
 - Study Design Objectives and Endpoints sheet
 - Study Design Eligibility Criteria sheet
 - Study Design Estimands sheet
 - Study Design Procedures sheet
 - Study Design Encounters sheet
 - Study Design Elements sheet
 - Study Design Content sheet
@@ -113,17 +114,17 @@
 - Minutes: 'M', 'MINS', 'MIN', 'MINUTES', 'MINUTE'
 - Seconds: 'S', 'SECS', 'SEC', 'SECONDS', 'SECOND'
 
 So ```3 Y```, ```3 YRS```, ```3 YR```, ```3 YEARS```, ```3 YEAR``` are all equivalent. Only a single value and unit should be entered, i.e. combination values are not supported.
 
 ### Templated Text
 
-Some entries can include "tags" that allow the text to reference structured content from elsewhere in the model. An example is an activity name. These sections of text are formatted as `[tag_name]` within the text. The `tag_name` refers to an entry within a dictionary (see the dictionaries sheet)
+Some entries can include "tags" that allow the text to reference structured content from elsewhere in the model. An example is an eligibility criterion referring to population definitions or an activity name. These sections of text are formatted as `<usdm:tag name="...tag_name..."/>` within the text. The `...tag_name...` refers to an entry within a dictionary (see the dictionaries sheet)
 
-An example of Templated Text is `Subjects shall be between [min_age] and [max_age]` where the min and max ages will be inserted using the dictionary entries that refer to particular attribute values from within the structured parts of the model.
+An example of Templated Text is `Subjects shall be between <usdm:tag name="min_age"/> and <usdm:tag name="max_age"/>` where the min and max ages will be inserted using the dictionary entries that refer to particular attribute values from within the structured parts of the model.
 
 ### Sheet Descriptions
 
 The sheet descriptions detail the fields found within each sheet and the details of the data required. Note:
 
 - Some fields have multiple names due to model changes and a desire to preserve backwards compatibility. Any of the choices documented can be used. 
 - Some columns are optional and thus can be included or omitted. Again this is to preserve backwards compatibility. A default value is specified if the column is not included.
@@ -178,21 +179,21 @@
 
 #### Sheet Contents
 
 A header row in row 1 followed by repeating rows from row 2, each containing a study identifier: 
 
 | Column | Column Name | Purpose | Format and Values |
 | :--- | :--- | :--- | :--- |
-| A | organisationIdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
-| B | organisationIdentifier | Organisation identifier | Text string |
+| A | organisationIdentifierScheme, organizationIdentifierScheme or IdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
+| B | organisationIdentifier or identifier | Organisation identifier | Text string |
 | C | organisationName or name | Organisation name | Text string |
 | D (optional) | label | Display label | Text string, can be empty. Default value is '' |
-| E | organisationType or type | Organisation type | CDISC code reference |
+| E | organisationType, organizationType or type | Organisation type | CDISC code reference |
 | F | studyIdentifier | The identifier for the study | Text string |
-| G | organisationAddress | The organisation address | Address |
+| G | organisationAddress, organizationAddress or address | The organisation address | Address |
 
 
 ### Study Amendments	Sheet
 	
 #### Sheet Name
 
 `studyAmendments`
@@ -471,27 +472,46 @@
 
 #### Sheet Name
 
 `studyDesignPopulations`
 
 #### Sheet Contents
 
-A header row in row 1 followed by repeating rows from row 2 containing population or sub-population definitions. Note that not every entry in columns E through I need to be filled in, just enough to define  either the whole population of the sub-populations. Sub-population need not be specificed.
+A header row in row 1 followed by repeating rows from row 2 containing population or sub-population definitions. Note that not every entry in columns E through I need to be filled in, just enough to define  either the whole population of the sub-populations. Sub-populations need not be specificed.
 
 | Column | Column Name | Purpose | Format and Values |
 | :--- | :--- | :--- | :--- |
 | A | level	| Level of entry | Set to either `MAIN` for the main population entry. All other values equate to a cohort (sub population) entry | 
 | B | name	| Identifier | Text string | 
 | C | description| Description | Text string, can be empty | 
 | D | label | Display label | Text string, can be empty |
 | E | plannedCompletionNumber	| Number of participants to complete the study | Integer | 
 | F | plannedEnrollmentNumber	| Number of participants to be enrolled | Integer | 
 | G | plannedAge	| Age range of participants | Range |
 | H | plannedSexOfParticipants | Sex of participants | CDISC code reference |
 | I | includesHealthSubjects | Healthy subjects flag | Boolean |
+| I | characterisitcs | List of characteristics for the cohort (ignored for main population) | Comma separated list of charcateristics name references |
+
+### Study Design Characteristics sheet
+
+#### Sheet Name
+
+`studyDesignCharacteristics`
+
+#### Sheet Contents
+
+A header row in row 1 followed by repeating rows from row 2 containing characteristics for cohorts.
+
+| Column | Column Name | Purpose | Format and Values |
+| :--- | :--- | :--- | :--- |
+| A | name	| Identifier | Text string | 
+| B | description| Description | Text string, can be empty | 
+| C | label | Display label | Text string, can be empty |
+| D | text	| Criteria text | Templated text |
+| E | dictionary| Dictionary cross reference | The dictionary from which the templated text tags are taken. If no tags are used can be empty |
 
 ### Study Design Objectives and Endpoints sheet
 
 #### Sheet Name
 
 `studyDesignOE`
 
@@ -645,18 +665,23 @@
 | element | Refer to a predefined element | 'name' of the element. Supported element names are 'study_phase', 'study_short_title', 'study_full_title', 'study_acronym', 'study_rationale', 'study_version_identifier', 'study_identifier', 'study_regulatory_identifiers', 'study_date', 'approval_date', 'organization_name_and_address', 'amendment' and 'amendment_scope' |
 | section | Add a pre defined section into the document | 'name' and 'template'. Supported section are 'title_page', 'inclusion', 'exclusion' and 'objective_endpoints'. Supported templates are 'm11' and 'plain' |
 | note | Insert a note into the document | 'text' |
 
 Examples of macros are:
 
 ```<usdm:macro id="xref" klass="Objective" name="OBJ1" attribute="text"/>```
+
 ```<usdm:macro id="xref" klass="StudyDesignPopulation" name="STUDY_POP" attribute="@plannedCompletionNumber/Range/maxValue"/>```
+
 ```<usdm:macro id="element" name="study_identifier"/>```
+
 ```<usdm:macro id="image" file="design.png" type="png"/>```
+
 ```<usdm:macro id="section" name="inclusion" template="plain"/>```
+
 ```<usdm:macro id="note" text="A note here please"/>```
 
 ### Study Design Sites sheet
 
 #### Sheet Name
 
 `studyDesignSites`
```

### Comparing `usdm-0.48.0/setup.py` & `usdm-0.49.0/setup.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm.egg-info/PKG-INFO` & `usdm-0.49.0/src/usdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.48.0
+Version: 0.49.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -80,14 +80,15 @@
 - Study Design sheet
 - One or more Timeline sheets
 - Study Design Timing sheet
 - Study Design Activities sheet (optional)
 - Study Design Indications sheet
 - Study Design Interventions sheet
 - Study Design Populations sheet
+- Study Design Characteristcis sheet
 - Study Design Objectives and Endpoints sheet
 - Study Design Eligibility Criteria sheet
 - Study Design Estimands sheet
 - Study Design Procedures sheet
 - Study Design Encounters sheet
 - Study Design Elements sheet
 - Study Design Content sheet
@@ -136,17 +137,17 @@
 - Minutes: 'M', 'MINS', 'MIN', 'MINUTES', 'MINUTE'
 - Seconds: 'S', 'SECS', 'SEC', 'SECONDS', 'SECOND'
 
 So ```3 Y```, ```3 YRS```, ```3 YR```, ```3 YEARS```, ```3 YEAR``` are all equivalent. Only a single value and unit should be entered, i.e. combination values are not supported.
 
 ### Templated Text
 
-Some entries can include "tags" that allow the text to reference structured content from elsewhere in the model. An example is an activity name. These sections of text are formatted as `[tag_name]` within the text. The `tag_name` refers to an entry within a dictionary (see the dictionaries sheet)
+Some entries can include "tags" that allow the text to reference structured content from elsewhere in the model. An example is an eligibility criterion referring to population definitions or an activity name. These sections of text are formatted as `<usdm:tag name="...tag_name..."/>` within the text. The `...tag_name...` refers to an entry within a dictionary (see the dictionaries sheet)
 
-An example of Templated Text is `Subjects shall be between [min_age] and [max_age]` where the min and max ages will be inserted using the dictionary entries that refer to particular attribute values from within the structured parts of the model.
+An example of Templated Text is `Subjects shall be between <usdm:tag name="min_age"/> and <usdm:tag name="max_age"/>` where the min and max ages will be inserted using the dictionary entries that refer to particular attribute values from within the structured parts of the model.
 
 ### Sheet Descriptions
 
 The sheet descriptions detail the fields found within each sheet and the details of the data required. Note:
 
 - Some fields have multiple names due to model changes and a desire to preserve backwards compatibility. Any of the choices documented can be used. 
 - Some columns are optional and thus can be included or omitted. Again this is to preserve backwards compatibility. A default value is specified if the column is not included.
@@ -201,21 +202,21 @@
 
 #### Sheet Contents
 
 A header row in row 1 followed by repeating rows from row 2, each containing a study identifier: 
 
 | Column | Column Name | Purpose | Format and Values |
 | :--- | :--- | :--- | :--- |
-| A | organisationIdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
-| B | organisationIdentifier | Organisation identifier | Text string |
+| A | organisationIdentifierScheme, organizationIdentifierScheme or IdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
+| B | organisationIdentifier or identifier | Organisation identifier | Text string |
 | C | organisationName or name | Organisation name | Text string |
 | D (optional) | label | Display label | Text string, can be empty. Default value is '' |
-| E | organisationType or type | Organisation type | CDISC code reference |
+| E | organisationType, organizationType or type | Organisation type | CDISC code reference |
 | F | studyIdentifier | The identifier for the study | Text string |
-| G | organisationAddress | The organisation address | Address |
+| G | organisationAddress, organizationAddress or address | The organisation address | Address |
 
 
 ### Study Amendments	Sheet
 	
 #### Sheet Name
 
 `studyAmendments`
@@ -494,27 +495,46 @@
 
 #### Sheet Name
 
 `studyDesignPopulations`
 
 #### Sheet Contents
 
-A header row in row 1 followed by repeating rows from row 2 containing population or sub-population definitions. Note that not every entry in columns E through I need to be filled in, just enough to define  either the whole population of the sub-populations. Sub-population need not be specificed.
+A header row in row 1 followed by repeating rows from row 2 containing population or sub-population definitions. Note that not every entry in columns E through I need to be filled in, just enough to define  either the whole population of the sub-populations. Sub-populations need not be specificed.
 
 | Column | Column Name | Purpose | Format and Values |
 | :--- | :--- | :--- | :--- |
 | A | level	| Level of entry | Set to either `MAIN` for the main population entry. All other values equate to a cohort (sub population) entry | 
 | B | name	| Identifier | Text string | 
 | C | description| Description | Text string, can be empty | 
 | D | label | Display label | Text string, can be empty |
 | E | plannedCompletionNumber	| Number of participants to complete the study | Integer | 
 | F | plannedEnrollmentNumber	| Number of participants to be enrolled | Integer | 
 | G | plannedAge	| Age range of participants | Range |
 | H | plannedSexOfParticipants | Sex of participants | CDISC code reference |
 | I | includesHealthSubjects | Healthy subjects flag | Boolean |
+| I | characterisitcs | List of characteristics for the cohort (ignored for main population) | Comma separated list of charcateristics name references |
+
+### Study Design Characteristics sheet
+
+#### Sheet Name
+
+`studyDesignCharacteristics`
+
+#### Sheet Contents
+
+A header row in row 1 followed by repeating rows from row 2 containing characteristics for cohorts.
+
+| Column | Column Name | Purpose | Format and Values |
+| :--- | :--- | :--- | :--- |
+| A | name	| Identifier | Text string | 
+| B | description| Description | Text string, can be empty | 
+| C | label | Display label | Text string, can be empty |
+| D | text	| Criteria text | Templated text |
+| E | dictionary| Dictionary cross reference | The dictionary from which the templated text tags are taken. If no tags are used can be empty |
 
 ### Study Design Objectives and Endpoints sheet
 
 #### Sheet Name
 
 `studyDesignOE`
 
@@ -668,18 +688,23 @@
 | element | Refer to a predefined element | 'name' of the element. Supported element names are 'study_phase', 'study_short_title', 'study_full_title', 'study_acronym', 'study_rationale', 'study_version_identifier', 'study_identifier', 'study_regulatory_identifiers', 'study_date', 'approval_date', 'organization_name_and_address', 'amendment' and 'amendment_scope' |
 | section | Add a pre defined section into the document | 'name' and 'template'. Supported section are 'title_page', 'inclusion', 'exclusion' and 'objective_endpoints'. Supported templates are 'm11' and 'plain' |
 | note | Insert a note into the document | 'text' |
 
 Examples of macros are:
 
 ```<usdm:macro id="xref" klass="Objective" name="OBJ1" attribute="text"/>```
+
 ```<usdm:macro id="xref" klass="StudyDesignPopulation" name="STUDY_POP" attribute="@plannedCompletionNumber/Range/maxValue"/>```
+
 ```<usdm:macro id="element" name="study_identifier"/>```
+
 ```<usdm:macro id="image" file="design.png" type="png"/>```
+
 ```<usdm:macro id="section" name="inclusion" template="plain"/>```
+
 ```<usdm:macro id="note" text="A note here please"/>```
 
 ### Study Design Sites sheet
 
 #### Sheet Name
 
 `studyDesignSites`
```

### Comparing `usdm-0.48.0/src/usdm.egg-info/SOURCES.txt` & `usdm-0.49.0/src/usdm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,59 +3,70 @@
 pyproject.toml
 setup.py
 src/usdm.egg-info/PKG-INFO
 src/usdm.egg-info/SOURCES.txt
 src/usdm.egg-info/dependency_links.txt
 src/usdm.egg-info/requires.txt
 src/usdm.egg-info/top_level.txt
+src/usdm_db/__init__.py
+src/usdm_db/cross_reference.py
+src/usdm_db/neo4j_dict.py
+src/usdm_db/timeline.py
+src/usdm_db/document/__init__.py
+src/usdm_db/document/document.py
+src/usdm_db/document/utility.py
+src/usdm_db/errors_and_logging/__init__.py
+src/usdm_db/errors_and_logging/error.py
+src/usdm_db/errors_and_logging/errors.py
+src/usdm_db/errors_and_logging/errors_and_logging.py
 src/usdm_excel/__init__.py
 src/usdm_excel/alias.py
 src/usdm_excel/base_sheet.py
-src/usdm_excel/cdisc_biomedical_concept.py
+src/usdm_excel/cdisc_bc_library.py
 src/usdm_excel/cdisc_ct.py
 src/usdm_excel/cdisc_ct_library.py
 src/usdm_excel/code_base.py
 src/usdm_excel/configuration_sheet.py
 src/usdm_excel/cross_ref.py
 src/usdm_excel/ct_version_manager.py
-src/usdm_excel/export_as_neo4j_dict.py
-src/usdm_excel/export_as_timeline.py
-src/usdm_excel/export_as_yworks_dict.py
+src/usdm_excel/globals.py
 src/usdm_excel/id_manager.py
 src/usdm_excel/iso_3166.py
 src/usdm_excel/iso_8601_duration.py
-src/usdm_excel/logger.py
 src/usdm_excel/ncit.py
 src/usdm_excel/option_manager.py
 src/usdm_excel/other_ct.py
 src/usdm_excel/quantity_type.py
 src/usdm_excel/range_type.py
+src/usdm_excel/syntax_template_sheet.py
 src/usdm_excel/data/cdisc_bcs.yaml
 src/usdm_excel/data/cdisc_ct_2023-12-15.yaml
 src/usdm_excel/data/cdisc_ct_config.yaml
 src/usdm_excel/data/iso_3166.json
 src/usdm_excel/data/missing_ct.yaml
 src/usdm_excel/document/__init__.py
-src/usdm_excel/document/document.py
 src/usdm_excel/document/elements.py
 src/usdm_excel/document/macros.py
 src/usdm_excel/document/soa.py
 src/usdm_excel/document/template_base.py
 src/usdm_excel/document/template_m11.py
 src/usdm_excel/document/template_plain.py
 src/usdm_excel/document/utility.py
-src/usdm_excel/errors/__init__.py
-src/usdm_excel/errors/error.py
-src/usdm_excel/errors/errors.py
+src/usdm_excel/errors_and_logging/__init__.py
+src/usdm_excel/errors_and_logging/error.py
+src/usdm_excel/errors_and_logging/errors.py
+src/usdm_excel/errors_and_logging/errors_and_logging.py
 src/usdm_excel/study_design_activity_sheet/__init__.py
 src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py
 src/usdm_excel/study_design_amendment_sheet/__init__.py
 src/usdm_excel/study_design_amendment_sheet/study_design_amendment_sheet.py
 src/usdm_excel/study_design_arm_sheet/__init__.py
 src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
+src/usdm_excel/study_design_characteristics_sheet/__init__.py
+src/usdm_excel/study_design_characteristics_sheet/study_design_characteristics_sheet.py
 src/usdm_excel/study_design_conditions_sheet/__init__.py
 src/usdm_excel/study_design_conditions_sheet/study_design_conditions_sheet.py
 src/usdm_excel/study_design_content_sheet/__init__.py
 src/usdm_excel/study_design_content_sheet/study_design_content_sheet.py
 src/usdm_excel/study_design_dictionary_sheet/__init__.py
 src/usdm_excel/study_design_dictionary_sheet/study_design_dictionary_sheet.py
 src/usdm_excel/study_design_element_sheet/__init__.py
@@ -156,39 +167,43 @@
 tests/test_base_sheet.py
 tests/test_cdisc_biomedical_concept.py
 tests/test_cdisc_ct.py
 tests/test_configuration_sheet.py
 tests/test_cross_reference.py
 tests/test_data_factory.py
 tests/test_document.py
+tests/test_document_elements.py
 tests/test_document_macros.py
 tests/test_document_soa.py
 tests/test_document_template_plain.py
 tests/test_document_utility.py
 tests/test_error.py
 tests/test_errors.py
 tests/test_export.py
 tests/test_factory.py
+tests/test_globals.py
 tests/test_integration.py
 tests/test_iso_3166.py
 tests/test_iso_8601_duration.py
 tests/test_ncit.py
 tests/test_option_manager.py
 tests/test_quantity_type.py
 tests/test_range_type.py
 tests/test_study_design_activity_sheet.py
 tests/test_study_design_arm_sheet.py
+tests/test_study_design_characteristic_sheet.py
 tests/test_study_design_conditions_sheet.py
 tests/test_study_design_content_sheet.py
 tests/test_study_design_dictionary_sheet.py
 tests/test_study_design_eligibility_criteria_sheet.py
 tests/test_study_design_encounter_sheet.py
 tests/test_study_design_epoch_sheet.py
 tests/test_study_design_indication_sheet.py
 tests/test_study_design_intervention_sheet.py
 tests/test_study_design_oe_sheet.py
+tests/test_study_design_population_sheet.py
 tests/test_study_design_sites_sheet.py
 tests/test_study_design_timing_sheet.py
 tests/test_study_identifiers_sheet.py
 tests/test_study_sheet.py
 tests/test_study_soa_v2_sheet.py
 tests/test_utility.py
```

### Comparing `usdm-0.48.0/src/usdm_excel/base_sheet.py` & `usdm-0.49.0/src/usdm_excel/base_sheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 import os
-import traceback
 import pandas as pd
 from openpyxl import load_workbook
-from usdm_excel.id_manager import id_manager
 from usdm_excel.cdisc_ct import CDISCCT
 from usdm_excel.other_ct import OtherCT
-from usdm_excel.ct_version_manager import ct_version_manager
-from usdm_excel.errors.errors import error_manager
-from usdm_excel.logger import package_logger
-from usdm_excel.option_manager import *
-from usdm_excel.cross_ref import cross_references
+from usdm_excel.option_manager import Options
 from usdm_excel.quantity_type import QuantityType
 from usdm_excel.range_type import RangeType
 from usdm_excel.iso_3166 import ISO3166
 from usdm_model.quantity import Quantity
 from usdm_model.range import Range
 from usdm_model.address import Address
 from usdm_excel.alias import Alias
+from usdm_excel.option_manager import EmptyNoneOption
+from usdm_excel.globals import Globals
 
 class BaseSheet():
 
   class StateError(Exception):
     pass
 
   class FormatError(Exception):
     pass
 
-  def __init__(self, file_path, sheet_name, header=0, optional=False, converters={}, require={}):
+  def __init__(self, file_path: str, globals: Globals, sheet_name: str, header: int=0, optional: bool=False, converters: dict={}, require: dict={}):
     self.file_path = file_path
+    self.globals = globals
     self.dir_path, self.filename = os.path.split(file_path)
     self.sheet_name = sheet_name
     self.sheet = None
     self.success = False
     if optional and not self._sheet_present(file_path, sheet_name):
       self._general_info(f"{sheet_name} not found but optional")
     else:
@@ -58,37 +55,37 @@
 
   def read_cell_by_name(self, row_index, field_name, default=None, must_be_present=True):
     try:
       col_index = self.column_present(field_name)
       return self.read_cell(row_index, col_index)
     except Exception as e:
       if not must_be_present:
-        return "" #if option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value else None
+        return "" #if self.globals.option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value else None
       elif default:
         return default
       else:
         self._error(row_index, -2, f"Error '{e}' reading cell '{field_name}'")
-        return "" #if option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value else None
+        return "" #if self.globals.option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value else None
 
   def read_cell(self, row_index, col_index, default=None):
     try:
       if pd.isnull(self.sheet.iloc[row_index, col_index]):
         if default:
           return default
         else:
-          return "" #if option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value else None
+          return "" #if self.globals.option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value else None
       else:
         return str(self.sheet.iloc[row_index, col_index]).strip()
     except Exception as e:
-      self._error(row_index, col_index, f"Error '{e}' reading cell")
-      self._traceback(f"{e}\n{traceback.format_exc()}")
+      #print(f"ROW / COL: {row_index}, {col_index}")
+      self._exception(row_index, col_index, 'Error reading cell', e)
       if default:
         return default
       else:
-        return "" #if option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value else None
+        return "" #if self.globals.option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value else None
 
   # Deprecate this method
   def read_cell_empty_legacy(self, row_index, col_index):
     if self.cell_empty(row_index, col_index):
       return "", True
     else:
       value = self.read_cell_empty(row_index, col_index, '-')
@@ -99,28 +96,41 @@
 
   # Deprecate this method
   def read_cell_empty(self, row_index, col_index, empty_character):
     value = self.read_cell(row_index, col_index)
     value = "" if (value == empty_character) or (value == None) else value
     return value
 
+  def read_cell_multiple_by_name(self, row_index, field_name, must_be_present=True):
+    try:
+      col_index = self.column_present(field_name)
+      return self.read_cell_multiple(row_index, col_index)
+    except Exception as e:
+      if not must_be_present:
+        return []
+      else:
+        self._error(row_index, -2, f"Error '{e}' reading cell multiple '{field_name}'")
+        return []
+
   def read_cell_multiple(self, rindex, cindex):
     try:
       results = []
       value = self.read_cell(rindex, cindex)
       if value.strip() == '':
         return results
       for part in self._state_split(value):
         results.append(part.strip())
       return results
     except BaseSheet.StateError as e:
       self._error(rindex, cindex, f"Internal state error '{e}' reading cell")
+      return []
     except BaseSheet.FormatError as e:
       self._error(rindex, cindex, "Format error reading cell, check the format of the cell")
-
+      return []
+    
   def read_cell_with_previous(self, row_index, col_index, first_col_index):
     try:
       i = col_index
       while i >= first_col_index:
         if pd.isnull(self.sheet.iloc[row_index, i]):
           i -= 1
         else:
@@ -142,44 +152,41 @@
   def read_quantity_cell_by_name(self, row_index, field_name, allow_missing_units=True, allow_empty=True):
     col_index = self.column_present(field_name)
     return self.read_quantity_cell(row_index, col_index, allow_missing_units, allow_empty)
 
   def read_quantity_cell(self, row_index, col_index, allow_missing_units=True, allow_empty=True):
     try:
       text = self.read_cell(row_index, col_index)
-      quantity = QuantityType(text, allow_missing_units, allow_empty)
+      quantity = QuantityType(text, self.globals, allow_missing_units, allow_empty)
       if not quantity.errors:
-        unit = Alias.code(quantity.units_code, [])
-        return None if quantity.empty else Quantity(id=id_manager.build_id(Quantity), value=float(quantity.value), unit=unit)
+        unit = Alias(self.globals).code(quantity.units_code, [])
+        return None if quantity.empty else Quantity(id=self.globals.id_manager.build_id(Quantity), value=float(quantity.value), unit=unit)
       else:
         self._add_errors(quantity.errors, row_index, col_index)
         return None
     except Exception as e:
-      self._error(row_index, col_index, f"Failed to decode quantity data '{text}'")
-      self._traceback(f"{e}\n{traceback.format_exc()}")
+      self.globals.errors_and_logging.exception(f"Failed to decode quantity data '{text}'", e, self.sheet, row_index, col_index)
       return None
 
   def read_range_cell_by_name(self, row_index, field_name, require_units=True, allow_empty=True):
     col_index = self.column_present(field_name)
     return self.read_range_cell(row_index, col_index, require_units, allow_empty)
 
   def read_range_cell(self, row_index, col_index, require_units=True, allow_empty=True):
     try:
       text = self.read_cell(row_index, col_index)
-      range = RangeType(text, require_units, allow_empty)
+      range = RangeType(text, self.globals, require_units, allow_empty)
       if not range.errors:
         #print(f"RANGE: {range.lower} {range.upper} {range.units} {range.units_code} {range.empty} ")
-        return None if range.empty else Range(id=id_manager.build_id(Range), minValue=float(range.lower), maxValue=float(range.upper), unit=range.units_code, isApproximate=False)
+        return None if range.empty else Range(id=self.globals.id_manager.build_id(Range), minValue=float(range.lower), maxValue=float(range.upper), unit=range.units_code, isApproximate=False)
       else:
         self._add_errors(range.errors, row_index, col_index)
         return None
     except Exception as e:
-      self._error(row_index, col_index, f"Failed to decode range data '{text}'")
-      #print(f"{e}\n{traceback.format_exc()}")
-      self._traceback(f"{e}\n{traceback.format_exc()}")
+      self.globals.errors_and_logging.exception(f"Failed to decode range data '{text}'", e, self.sheet, row_index, col_index)
       return None
 
   def read_address_cell_by_name(self, row_index, field_name, allow_empty=False):
     raw_address = self.read_cell_by_name(row_index, field_name)
     # TODO The '|' separator is preserved for legacy reasons but should be removed in the future
     if not raw_address:
       sep = ','
@@ -188,63 +195,60 @@
       sep = '|'
       parts = raw_address.split(sep)
     else:
       sep = ','
       parts = self._state_split(raw_address)
     if len(parts) == 6:
       result = self._to_address(
-          id_manager.build_id(Address),
+          self.globals.id_manager.build_id(Address),
           line=parts[0].strip(), 
           district=parts[1].strip(), 
           city=parts[2].strip(), 
           state=parts[3].strip(), 
           postal_code=parts[4].strip(), 
-          country=ISO3166().code(parts[5].strip())
+          country=ISO3166(self.globals).code(parts[5].strip())
         )
       return result
     elif allow_empty:
       pass
     else:
-      col_index = self.sheet.columns.get_loc(field_name)
-      self._error(row_index, col_index, f"Address does not contain the required fields (line, district, city, state, postal code and country code) using '{sep}' separator characters, only {len(parts)} found")
+      col_index = self.column_present(field_name)
+      self._error(row_index, col_index, f"Address '{raw_address}' does not contain the required fields (first line, district, city, state, postal code and country code) using '{sep}' separator characters, only {len(parts)} found")
       return None
 
   def _to_address(self, id, line, city, district, state, postal_code, country):
     text = "%s, %s, %s, %s, %s, %s" % (line, city, district, state, postal_code, country.decode)
     text = text.replace(' ,', '')
     try:
       result = Address(id=id, text=text, line=line, city=city, district=district, state=state, postalCode=postal_code, country=country)
     except Exception as e:
-      self._general_error(f"Failed to create Address object, exception {e}")
-      self._traceback(f"{traceback.format_exc()}")
+      self._general_exception(f"Failed to create Address object", e)
       result = None
     return result
 
   def create_object(self, cls, params):
     try:
-      params['id'] = id_manager.build_id(cls)
+      params['id'] = self.globals.id_manager.build_id(cls)
       return cls(**params)
     except Exception as e:
-      self._general_error(f"Failed to create {cls.__name__} object, exception {e}")
-      self._traceback(f"{traceback.format_exc()}")
+      self._general_exception(f"Failed to create {cls.__name__} object", e)
       return None
 
   def read_other_code_cell_by_name(self, row_index, field_name):
-    #col_index = self.sheet.columns.get_loc(field_name)
     col_index = self.column_present(field_name)
     return self.read_other_code_cell(row_index, col_index)
 
   def read_other_code_cell(self, row_index, col_index):
     value = self.read_cell(row_index, col_index)
     if value.strip() == "":
       return None
     return self._decode_other_code(value, row_index, col_index)
 
   def read_other_code_cell_multiple_by_name(self, row_index, field_name):
-    col_index = self.sheet.columns.get_loc(field_name)
+    col_index = self.column_present(field_name)
     return self.read_other_code_cell_mutiple(row_index, col_index)
 
   def read_other_code_cell_mutiple(self, row_index, col_index):
     value = self.read_cell(row_index, col_index)
     result = []
     if value.strip() == '':
       return result
@@ -258,150 +262,151 @@
     col_index = self.column_present(field_name)
     return self.read_cdisc_klass_attribute_cell(klass, attribute, row_index, col_index, allow_empty)
 
   def read_cdisc_klass_attribute_cell(self, klass, attribute, row_index, col_index, allow_empty=False):
     code = None
     value = self.read_cell(row_index, col_index)
     if value:
-      code = CDISCCT().code_for_attribute(klass, attribute, value)
+      code = CDISCCT(self.globals).code_for_attribute(klass, attribute, value)
       if not code:
         self._error(row_index, col_index, f"CDISC CT not found for value '{value}'.")
     elif not allow_empty:
       self._error(row_index, col_index, "Empty cell detected where CDISC CT value expected.")
     return code
 
   def read_cdisc_klass_attribute_cell_multiple_by_name(self, klass, attribute, row_index, field_name):
-    #col_index = self.sheet.columns.get_loc(field_name)
     col_index = self.column_present(field_name)
     return self.read_cdisc_klass_attribute_cell_multiple(klass, attribute, row_index, col_index)
 
   def read_cdisc_klass_attribute_cell_multiple(self, klass, attribute, row_index, col_index):
     result = []
     value = self.read_cell(row_index, col_index)
     if value.strip() == "":
       self._error(row_index, col_index, "Empty cell detected where multiple CDISC CT values expected.")
       return result
     for item in self._state_split(value):
-      code = CDISCCT().code_for_attribute(klass, attribute, item.strip())
+      code = CDISCCT(self.globals).code_for_attribute(klass, attribute, item.strip())
       if code is not None:
         result.append(code)
       else:
         self._error(row_index, col_index, f"CDISC CT not found for value '{item.strip()}'.")
     return result
 
   def _get_cross_reference(self, klass, name, error_klass_name):
-    item = cross_references.get(klass, name)
+    item = self.globals.cross_references.get(klass, name)
     if item:
       return item.id
     else:
       self._general_error(f"Unable to find {error_klass_name} with name '{name}'")              
       return None
 
   def double_link(self, items, prev, next):
     try: 
       for idx, item in enumerate(items):
         if idx == 0:
-          if option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value:
+          if self.globals.option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value:
             setattr(item, prev, "")
           else:
             setattr(item, prev, None)
         else:
           the_id = getattr(items[idx-1], 'id')
           setattr(item, prev, the_id)
         if idx == len(items)-1:  
-          if option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value:
+          if self.globals.option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value:
             setattr(item, next, "")
           else:
             setattr(item, next, None)
         else:
           the_id = getattr(items[idx+1], 'id')
           setattr(item, next, the_id)
     except Exception as e:
-      self._general_error(f"Exception '{e}' in double_link: {items}")
+      self._general_exception(f"Error while doubly linking lists", e)
 
   def previous_link(self, items, prev):
     try: 
       for idx, item in enumerate(items):
         if idx == 0:
-          if option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value:
+          if self.globals.option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value:
             setattr(item, prev, "")
           else:
             setattr(item, prev, None)
         else:
           the_id = getattr(items[idx-1], 'id')
           setattr(item, prev, the_id)
     except Exception as e:
-      self._general_error(f"Exception '{e}' in previous_link: {items}")
+      self._general_exception(f"Error in previous link link {items}", e)
 
   def _decode_other_code(self, value, row_index, col_index):
     if value.strip() == "":
       return None
     outer_parts = value.split(":")
     if len(outer_parts) == 2:
       system = outer_parts[0].strip()
       inner_parts = outer_parts[1].strip().split("=")
       if len(inner_parts) == 2:
-        version = ct_version_manager.get(system)
-        return OtherCT().code(code=inner_parts[0].strip(), system=system, version=version, decode=inner_parts[1].strip())
+        version = self.globals.ct_version_manager.get(system)
+        return OtherCT(self.globals).code(code=inner_parts[0].strip(), system=system, version=version, decode=inner_parts[1].strip())
       else:
         self._error(row_index, col_index, "Failed to decode code data '%s', no '=' detected" % (value))
     else:
       self._error(row_index, col_index, "Failed to decode code data '%s', no ':' detected" % (value))
     return None
 
   def _to_int(self, value):
     try:
       return int(value)
     except:
       return None
 
+  def _get_column_index(self, column_name):
+    return self.sheet.columns.get_loc(column_name)
+
   def _add_errors(self, errors, row, column):
     for error in errors:
       self._error(row, column, error)
       
-  def _get_column_index(self, column_name):
-    return self.sheet.columns.get_loc(column_name)
-
   def _info(self, row, column, message):
-     package_logger.info(self._format(row + 1, column + 1, message))
+    self.globals.errors_and_logging.info(message, self.sheet_name, row + 1, column + 1)
      
   def _general_info(self, message):
-     package_logger.info(self._format(None, None, message))
+    self.globals.errors_and_logging.info(message, self.sheet_name)
      
   def _error(self, row, column, message):
+    #print(f"ROW / COL: {row}, {column}")
     try:
-      error_manager.add(self.sheet_name, row + 1, column + 1, message)
+      self.globals.errors_and_logging.error(message, self.sheet_name, row + 1, column + 1)
     except Exception as e:
-      error_manager.add(self.sheet_name, None, None, f"{e}\n{traceback.format_exc()}", error_manager.WARNING)
+      # Exception will tend to come from the row / column being none etc. Just a last 
+      # attempt to catch it
+      self.globals.errors_and_logging.exception(message, e, self.sheet_name)
 
   def _general_error(self, message):
-    error_manager.add(self.sheet_name, None, None, message)
+    self.globals.errors_and_logging.error(message, self.sheet_name)
 
   def _warning(self, row, column, message):
-    error_manager.add(self.sheet_name, row + 1, column + 1, message, error_manager.WARNING)
+    self.globals.errors_and_logging.warning(message, self.sheet_name, row + 1, column + 1)
 
   def _general_warning(self, message):
-    error_manager.add(self.sheet_name, None, None, message, error_manager.WARNING)
+    self.globals.errors_and_logging.warning(message, self.sheet_name)
 
   def _debug(self, row, column, message):
-    error_manager.add(self.sheet_name, row + 1, column + 1, message, error_manager.DEBUG)
+    self.globals.errors_and_logging.debug(message, self.sheet_name, row + 1, column + 1)
 
   def _general_debug(self, message):
-    error_manager.add(self.sheet_name, None, None, message, error_manager.DEBUG)
+    self.globals.errors_and_logging.debug(message, self.sheet_name)
 
-  def _traceback(self, message):
-    package_logger.error(message)
+  def _general_exception(self, message, e):
+    self.globals.errors_and_logging.exception(message, e, self.sheet_name)
 
-  def _format(self, row, column, message):
-    if self.sheet_name == None:
-      return f"{self.message}"
-    elif row == None:
-      return f"In sheet {self.sheet_name}: {message}"
-    else:
-      return f"In sheet {self.sheet_name} at [{row},{column}]: {message}"
+  def _exception(self, row, column, message, e):
+    #print(f"ROW / COL: {row}, {column}")
+    self.globals.errors_and_logging.exception(message, e, self.sheet_name, row + 1, column + 1)
+
+  def _sheet_exception(self, e):
+    self.globals.errors_and_logging.exception(f"Error [{e}] while reading sheet '{self.sheet_name}'", e, self.sheet_name)
 
   def _get_sheet_names(self, file_path):
     wb = load_workbook(file_path, read_only=True, keep_links=False)
     return wb.sheetnames
 
   def _sheet_present(self, file_path, sheet_name):
     sheet_names = self._get_sheet_names(file_path)
@@ -422,17 +427,20 @@
     ESC = "escape"
 
     state = OUT
     result = []
     current = []
     exit = ""
     for c in s:
+      #print(f"STATE: s: {state}, c: {c}")
       if state == OUT:
         current = []
-        if c in ['"', "'"]:
+        if c == ',':
+          result.append("")
+        elif c in ['"', "'"]:
           state = IN_QUOTED
           exit = c
         elif c.isspace():
           pass
         else:
           state = IN_NORMAL
           current.append(c)
```

### Comparing `usdm-0.48.0/src/usdm_excel/cdisc_biomedical_concept.py` & `usdm-0.49.0/src/usdm_excel/cdisc_bc_library.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from usdm_excel.cdisc_ct import CDISCCT
-from usdm_excel.cdisc_ct_library import cdisc_ct_library
-from usdm_excel.ncit import NCIt
-from usdm_excel.id_manager import id_manager
-from usdm_excel.alias import Alias
+import os
+import yaml
+import requests
+from usdm_excel.errors_and_logging.errors_and_logging import ErrorsAndLogging
+from usdm_excel.cdisc_ct_library import CDISCCTLibrary
+from usdm_excel.id_manager import IdManager
 from usdm_model.biomedical_concept import BiomedicalConcept
 from usdm_model.biomedical_concept_property import BiomedicalConceptProperty
 from usdm_model.response_code import ResponseCode
+from usdm_model.code import Code
 from usdm_model.alias_code import AliasCode
-from usdm_excel.logger import package_logger
 
-import os
-import yaml
-import requests
-import traceback
-
-class CDISCBiomedicalConcepts():
+class CDISCBCLibrary():
 
   API_ROOT = 'https://api.library.cdisc.org/api/cosmos/v2'    
   
-  def __init__(self):
-    self.api_key = os.getenv('CDISC_API_KEY')
-    self.headers =  {"Content-Type":"application/json", "api-key": self.api_key}
+  def __init__(self, errors_and_logging: ErrorsAndLogging, ct_library: CDISCCTLibrary, id_manager: IdManager):
+    self._errors_and_logging = errors_and_logging
+    self._ct_library = ct_library
+    self._id_manager = id_manager
+    self._api_key = os.getenv('CDISC_API_KEY')
+    self._headers =  {"Content-Type":"application/json", "api-key": self._api_key}
     self._package_metadata = {}
     self._package_items = {}
     self._bc_responses = {}
     self._bcs = {}
     self._bcs_raw = {}
     self._bc_index = {}
     self._map = {}
@@ -51,15 +50,15 @@
       self._set_ids(bc_copy)
       bc = BiomedicalConcept(**bc_copy)
     return bc
 
   def _set_ids(self, parent):
     if isinstance(parent, str) or isinstance(parent, bool):
       return
-    parent['id'] = id_manager.build_id(parent['instanceType'])
+    parent['id'] = self._id_manager.build_id(parent['instanceType'])
     for name, value in parent.items():
       if isinstance(value, list):
         for child in value:
           self._set_ids(child)    
       else:
         self._set_ids(value)
 
@@ -85,44 +84,44 @@
     urls = {
       'generic': '/mdr/bc/packages',
       'sdtm': '/mdr/specializations/sdtm/packages'
     } 
     for url_type, url in urls.items():
       try:
         api_url = self._url(url)
-        package_logger.info(f"CDISC BC Library: {url_type}: {url}")
-        raw = requests.get(api_url, headers=self.headers)
+        self._logger.info(f"CDISC BC Library: {url_type}: {url}")
+        raw = requests.get(api_url, headers=self._headers)
         response = raw.json()
         self._package_metadata[url_type] = response['_links']['packages']
       except Exception as e:
         self._exception(f"Exception '{e}', failed to retrieve CDISC BC package metadata from '{api_url}'", e)
-    package_logger.debug(f"PACKAGES: {self._package_metadata}")
+    self._logger.debug(f"PACKAGES: {self._package_metadata}")
         
   def _get_package_items(self) -> dict:
     #self._package_items, self._map
     for package_type in ['sdtm', 'generic']:
       self._package_items[package_type] = {}
       for package in self._package_metadata[package_type]:
         self._get_package(package, package_type)        
 
   def _get_package(self, package, package_type):
     try:
       response_field = {'sdtm': 'datasetSpecializations', 'generic': 'biomedicalConcepts'}
       api_url = self._url(package['href']) if 'href' in package else 'not set'
-      package_logger.info(f"CDISC BC Library: {package_type}, {api_url}")
-      raw = requests.get(api_url, headers=self.headers)
+      self._logger.info(f"CDISC BC Library: {package_type}, {api_url}")
+      raw = requests.get(api_url, headers=self._headers)
       response = raw.json()
       for item in response['_links'][response_field[package_type]]:
-        package_logger.debug(f"ITEM: {item}")
+        self._logger.debug(f"ITEM: {item}")
         key = item['title'].upper()
         if package_type == 'sdtm':
           self._package_items[package_type][key] = item
           #map[item['href']] = key
         elif package_type == 'generic' and not key in self._package_items:
-          package_logger.info(f"GENERIC: Detected generic only BC {key}")
+          self._logger.info(f"GENERIC: Detected generic only BC {key}")
           self._package_items[package_type][key] = item
           self._map[item['href']] = key
     except Exception as e:
       self._exception(f"Exception '{e}', failed to retrieve CDISC BC metadata from '{api_url}'", e)
       return {}
 
   def _get_sdtm_bcs(self):
@@ -142,15 +141,15 @@
           self._bcs[name] = bc
         if generic:
           href = generic['_links']['self']['href']
           if href in self._map:
             #print(f"POP: {href}")
             self._map.pop(generic['_links']['self']['href'])
           else:
-            package_logger.error(f"Missing reference when popping {href}")
+            self._logger.error(f"Missing reference when popping {href}")
     #print(f"REMAINING: {self._map}")
 
   def _get_generic_bcs(self) -> BiomedicalConcept:
     #print(f"GENRIC KEYS: {self._package_items['generic'].keys()}")
     for name, item in self._package_items['generic'].items():
       if self._process_genric_bc(name):
         #print(f"ITEM IN GET GENERIC BC: {item}")
@@ -161,125 +160,125 @@
             property = self._generic_bc_property_as_usdm(item)
             if property:
               bc.properties.append(property)
         self._bcs_raw[name] = bc.model_dump()
         self._bcs[name] = bc
 
   def _generic_bc_as_usdm(self, api_bc) -> BiomedicalConcept:
-    concept_code = CDISCCT().code(api_bc['conceptId'], api_bc['shortName'])
+    concept_code = self._cdisc_code(api_bc['conceptId'], api_bc['shortName'])
     synonyms = api_bc['synonyms'] if 'synonyms' in api_bc else []
     return self._biomedical_concept_object(api_bc['shortName'], api_bc['shortName'], synonyms, api_bc['_links']['self']['href'], concept_code)
 
   def _generic_bc_property_as_usdm(self, property) -> BiomedicalConceptProperty:
-    concept_code = CDISCCT().code(property['conceptId'], property['shortName'])
+    concept_code = self._cdisc_code(property['conceptId'], property['shortName'])
     responses = []
     if 'exampleSet' in property:
       for example in property['exampleSet']:
-        term = cdisc_ct_library.preferred_term(example)
+        term = self._ct_library.preferred_term(example)
         if term != None:
-          code = CDISCCT().code(term['conceptId'], term['preferredTerm'])
+          code = self._cdisc_code(term['conceptId'], term['preferredTerm'])
           code.id = "tbd"
           responses.append(ResponseCode(id="tbd", isEnabled=True, code=code))
     return self._biomedical_concept_property_object(property['shortName'], property['shortName'], property['dataType'], responses, concept_code)
 
   def _sdtm_bc_as_usdm(self, sdtm, generic) -> BiomedicalConcept:
     try:
       if self._process_sdtm_bc(sdtm['shortName']):
-        package_logger.debug(f"BC: {sdtm}\n\n{generic}")
+        self._logger.debug(f"BC: {sdtm}\n\n{generic}")
         role_variable = self._get_role_variable(sdtm)
         if role_variable:
           if 'assignedTerm' in role_variable:
             if 'conceptId' in role_variable['assignedTerm'] and 'value' in role_variable['assignedTerm']:
-              concept_code = CDISCCT().code(role_variable['assignedTerm']['conceptId'], role_variable['assignedTerm']['value'])
+              concept_code = self._cdisc_code(role_variable['assignedTerm']['conceptId'], role_variable['assignedTerm']['value'])
             else:
-              package_logger.error(f"Failed to set BC concept 1, {sdtm['shortName']}")
-              concept_code = CDISCCT().code('No Concept Code', role_variable['assignedTerm']['value'])
+              self._logger.error(f"Failed to set BC concept 1, {sdtm['shortName']}")
+              concept_code = self._cdisc_code('No Concept Code', role_variable['assignedTerm']['value'])
           else:
-            package_logger.error(f"Failed to set BC concept 2, {sdtm['shortName']}")
-            concept_code = CDISCCT().code(generic['conceptId'], generic['shortName'])
+            self._logger.error(f"Failed to set BC concept 2, {sdtm['shortName']}")
+            concept_code = self._cdisc_code(generic['conceptId'], generic['shortName'])
         else:
-          package_logger.error(f"Failed to set BC concept {sdtm['shortName']}")
-          concept_code = CDISCCT().code(generic['conceptId'], generic['shortName'])
+          self._logger.error(f"Failed to set BC concept {sdtm['shortName']}")
+          concept_code = self._cdisc_code(generic['conceptId'], generic['shortName'])
         synonyms = generic['synonyms'] if 'synonyms' in generic else []
         synonyms.append(generic['shortName'])
         return self._biomedical_concept_object(sdtm['shortName'], sdtm['shortName'], synonyms, sdtm['_links']['self']['href'], concept_code)
       else:
         return None
     except Exception as e:
       self._exception(f"Exception '{e}', failed to build BC {sdtm['shortName']}", e)
       return None
 
   def _sdtm_bc_property_as_usdm(self, sdtm_property, generic) -> BiomedicalConceptProperty:
     try:
-      package_logger.debug(f"NAME: {sdtm_property['name']}, {sdtm_property['name'][2:]}")
+      self._logger.debug(f"NAME: {sdtm_property['name']}, {sdtm_property['name'][2:]}")
       if self._process_property(sdtm_property['name']):
-        package_logger.debug(f"PROPERTY: {sdtm_property}")
+        self._logger.debug(f"PROPERTY: {sdtm_property}")
         if 'dataElementConceptId' in sdtm_property:
           generic_match = self._get_dec_match(generic, sdtm_property['dataElementConceptId'])
           if generic_match:
-            concept_code = CDISCCT().code(generic_match['conceptId'], generic_match['shortName'])
+            concept_code = self._cdisc_code(generic_match['conceptId'], generic_match['shortName'])
           else:
             if 'assignedTerm' in sdtm_property and 'conceptId' in sdtm_property['assignedTerm'] and 'value' in sdtm_property['assignedTerm']:
-              concept_code = CDISCCT().code(sdtm_property['dataElementConceptId'], sdtm_property['name'])
+              concept_code = self._cdisc_code(sdtm_property['dataElementConceptId'], sdtm_property['name'])
             else:
-              package_logger.error(f"Failed to set property concept 1, {sdtm_property}")
-              concept_code = CDISCCT().code(sdtm_property['dataElementConceptId'], sdtm_property['name'])
+              self._logger.error(f"Failed to set property concept 1, {sdtm_property}")
+              concept_code = self._cdisc_code(sdtm_property['dataElementConceptId'], sdtm_property['name'])
         else:
           if 'assignedTerm' in sdtm_property:
-            concept_code = CDISCCT().code(sdtm_property['assignedTerm']['conceptId'], sdtm_property['assignedTerm']['value'])
+            concept_code = self._cdisc_code(sdtm_property['assignedTerm']['conceptId'], sdtm_property['assignedTerm']['value'])
           else:
-            package_logger.error(f"Failed to set property concept 2, {sdtm_property}")
-            concept_code = CDISCCT().code('No Concept Code', sdtm_property['name'])
+            self._logger.error(f"Failed to set property concept 2, {sdtm_property}")
+            concept_code = self._cdisc_code('No Concept Code', sdtm_property['name'])
         responses = []
         codes = []
         if 'valueList' in sdtm_property:
           codelist = sdtm_property['codelist']['conceptId'] if 'codelist' in sdtm_property else None
           for value in sdtm_property['valueList']:
-            term = cdisc_ct_library.preferred_term(value, codelist)
+            term = self._ct_library.preferred_term(value, codelist)
             if term:
-              code = CDISCCT().code(term['conceptId'], term['preferredTerm'])
+              code = self._cdisc_code(term['conceptId'], term['preferredTerm'])
               code.id = "tbd"
               codes.append(code)
             else:
-              term = cdisc_ct_library.submission(value, codelist)
+              term = self._ct_library.submission(value, codelist)
               if term:
-                code = CDISCCT().code(term['conceptId'], term['preferredTerm'])
+                code = self._cdisc_code(term['conceptId'], term['preferredTerm'])
                 code.id = "tbd"
                 codes.append(code)
               else:
                 cl = f", code list {sdtm_property['codelist']['conceptId'] if 'codelist' in sdtm_property else '<not defined>'}"
-                package_logger.error(f"Failed to find submission or preferred term '{value}' {cl}")
+                self._logger.error(f"Failed to find submission or preferred term '{value}' {cl}")
         for code in codes:
          response_code = ResponseCode(id="tbd", isEnabled=True, code=code)
          responses.append(response_code)
         datatype = sdtm_property['dataType'] if 'dataType' in sdtm_property else ''
         return self._biomedical_concept_property_object(sdtm_property['name'], sdtm_property['name'], datatype, responses, concept_code)
       else:
         return None
     except Exception as e:
       self._exception(f"Exception '{e}', failed to build property {sdtm_property}", e)
       return None
 
   def _biomedical_concept_object(self, name, label, synonyms, reference, code) -> BiomedicalConcept:
     code.id = "tbd"
-    alias_code=Alias.code(code, [])
+    alias_code=self._alias_code(code, [])
     alias_code.id = "tbd"
     return BiomedicalConcept(
       id="tbd",
       name=name,
       label=label,
       synonyms=synonyms,
       reference=reference,
       properties=[],
       code=alias_code
     )
 
   def _biomedical_concept_property_object(self, name, label, datatype, responses, code):
     code.id = "tbd"
-    alias_code=Alias.code(code, [])
+    alias_code=self._alias_code(code, [])
     alias_code.id = "tbd"
     return BiomedicalConceptProperty(
       id="tbd",
       name=name,
       label=label,
       isRequired=True,
       isEnabled=True,
@@ -331,27 +330,27 @@
     return next((item for item in data['variables'] if item["role"] == "Topic"), None)
 
   def _get_dec_match(self, data, id):
     return next((item for item in data['dataElementConcepts'] if item["conceptId"] == id), None)
 
   def _get_from_url_all(self, name, details) -> dict:
     try:
-      package_logger.debug(f"DETAILS: {details}")
+      self._logger.debug(f"DETAILS: {details}")
       sdtm_response = self._get_from_url(details['href'])
       generic = sdtm_response["_links"]["parentBiomedicalConcept"]
       generic_response = self._get_from_url(generic['href'])
       return sdtm_response, generic_response
     except Exception as e:
       self._exception(f"Exception '{e}', failed to retrieve CDISC BC metadata for {name} from '{details['href']}'", e)
       return None, None
 
   def _get_from_url(self, url):
     api_url = self._url(url)
-    package_logger.info("CDISC BC Library: %s" % api_url)
-    raw = requests.get(api_url, headers=self.headers)
+    self._logger.info("CDISC BC Library: %s" % api_url)
+    raw = requests.get(api_url, headers=self._headers)
     result = raw.json()
     return result
 
   def _url(self, relative_url) -> str:
     return "%s%s" % (self.__class__.API_ROOT, relative_url)
 
   def _save_bcs(self, data):
@@ -363,23 +362,31 @@
 
   def _read_bcs(self):
     try:
       if self._bcs_exist():
         with open(self._bcs_filename()) as f:
           return yaml.load(f, Loader=yaml.FullLoader)
       else:
-        package_logger.error(f"Failed to read CDSIC BC file, does not exist")
+        self._logger.error(f"Failed to read CDSIC BC file, does not exist")
         return None
     except Exception as e:
       self._exception(f"Exception '{e}', failed to read CDSIC CT file", e)
 
   def _bcs_exist(self):
     return os.path.isfile(self._bcs_filename()) 
 
   def _bcs_filename(self):
     return os.path.join(os.path.dirname(__file__), 'data', f"cdisc_bcs.yaml")
 
+  def _cdisc_code(self, code, decode):
+    id = self._id_manager.build_id(Code)
+    instance = Code(id=id, code=code, codeSystem=self._library.system, codeSystemVersion=self._library.version, decode=decode)
+    self._cross_references.add(instance.id, instance)
+    return instance
+
+  def _alias_code(self, standard_code, aliases):
+    return AliasCode(id=self._id_manager.build_id(AliasCode), standardCode=standard_code, standardCodeAliases=aliases) if standard_code else None  
+  
   def _exception(self, message, e):
-    package_logger.error(message)
-    package_logger.error(f"{e}\n{traceback.format_exc()}")
+    self._logger.error(message)
+    self._logger.error(f"{e}\n{traceback.format_exc()}")
 
-cdisc_bc_library = CDISCBiomedicalConcepts()
```

### Comparing `usdm-0.48.0/src/usdm_excel/cdisc_ct_library.py` & `usdm-0.49.0/src/usdm_excel/cdisc_ct_library.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import os
 import yaml
 import traceback
 import requests
-#from usdm_excel.id_manager import id_manager
-#from usdm_model.code import Code
-from usdm_excel.logger import package_logger
+from usdm_excel.errors_and_logging.errors_and_logging import ErrorsAndLogging
 
 class CDISCCTLibrary():
 
   API_ROOT = 'https://api.library.cdisc.org/api'  
   HEADERS = { "Content-Type":"application/json", "api-key": os.getenv('CDISC_API_KEY') }
     
-  def __init__(self):
+  def __init__(self, errors_and_logging: ErrorsAndLogging):
+    self._errors_and_logging = errors_and_logging
     f = open(os.path.join(os.path.dirname(__file__), 'data', 'missing_ct.yaml'))
-    self.missing_ct = yaml.load(f, Loader=yaml.FullLoader)
+    self._missing_ct = yaml.load(f, Loader=yaml.FullLoader)
     f = open(os.path.join(os.path.dirname(__file__), 'data', 'cdisc_ct_config.yaml'))
-    self.cdisc_ct_config = yaml.load(f, Loader=yaml.FullLoader)
-    self.version = self.cdisc_ct_config['version']
-    self.system = "http://www.cdisc.org"
-    self.api_key = os.getenv('CDISC_API_KEY')
+    self._cdisc_ct_config = yaml.load(f, Loader=yaml.FullLoader)
     self._by_code_list = {}
     self._by_term = {}
     self._by_submission = {}
     self._by_pt = {}
     self._by_klass_attribute = {}
     if self._code_lists_exist():
       self._load_ct()
     else:
       self._get_ct()
       self._save_code_lists(self._by_code_list)
     self._get_missing_ct()
     self._get_klass_attribute()
+    # Visible properties
+    self.version = self._cdisc_ct_config['version']
+    self.system = "http://www.cdisc.org"
 
   def submission(self, value, cl=None):
     if value in list(self._by_submission.keys()):
       concept_ids = self._by_submission[value]
       if len(concept_ids) == 0:
         return None
       elif len(concept_ids) == 1:
@@ -64,88 +63,93 @@
         else:
           return None 
     else:
       return None
 
   def klass_and_attribute(self, klass, attribute, value):
     try:
+      #if value == "Protocol Treatment Arm":
+      #  print(f"Klass: {klass}, attribute: {attribute}, value: {value}")
       concept_id = self._by_klass_attribute[klass][attribute]
+      #if value == "Protocol Treatment Arm":
+      #  print(f"Concept: {concept_id}")
       code_list = self._by_code_list[concept_id]
+      #if value == "Protocol Treatment Arm":
+      #  print(f"Concept: {code_list}")
       return self._get_item(code_list, value)
     except Exception as e: 
-      package_logger.error(f"Failed to find '{value}' for klass '{klass}' attribute '{attribute}'")
-      package_logger.debug(f"{e}\n{traceback.format_exc()}")
+      self._errors_and_logging.exception(f"Failed to find '{value}' for klass '{klass}' attribute '{attribute}'", e)
       return None
 
   def unit(self, value):
     try:
       code_list = self._by_code_list['C71620']
       return self._get_item(code_list, value)
     except Exception as e: 
-      package_logger.error(f"Failed to find unit '{value}'") 
-      package_logger.debug(f"{e}\n{traceback.format_exc()}")
+      self._errors_and_logging.exception(f"Failed to find unit '{value}'") 
       return None
 
   def _get_item(self, code_list, value):
     try:
       for field in [ 'conceptId', 'preferredTerm', 'submissionValue']:
+        #if value == "Protocol Treatment Arm":
+        #  print(f"GET: {field}")
         result = next((item for item in code_list['terms'] if item[field].upper() == value.upper()), None)
         if result:
           return result
       return None
     except Exception as e:
-      package_logger.error(f"Failed to find CDSIC CT for '{value}' in code ist '{code_list}'") 
-      package_logger.debug(f"{e}\n{traceback.format_exc()}")
+      self._errors_and_logging.exception(f"Failed to find CDSIC CT for '{value}' in code ist '{code_list}'", e)
       return None
 
   def _get_ct(self):
-    for item in self.cdisc_ct_config['required']:
+    for item in self._cdisc_ct_config['required']:
       self._get_code_list(item)
 
   def _load_ct(self):
     self._by_code_list = self._read_code_lists()
     for c_code, entry in self._by_code_list.items():
       for item in entry['terms']:
         self._check_in_and_add(self._by_term, item['conceptId'], c_code)
         self._check_in_and_add(self._by_submission, item['submissionValue'], c_code)
         self._check_in_and_add(self._by_pt, item['preferredTerm'], c_code)
  
   def _get_missing_ct(self):
-    for response in self.missing_ct:
+    for response in self._missing_ct:
       self._by_code_list[response['conceptId']] = response
       for item in response['terms']:
         self._check_in_and_add(self._by_term, item['conceptId'], response['conceptId'])
         self._check_in_and_add(self._by_submission, item['submissionValue'], response['conceptId'])
         self._check_in_and_add(self._by_pt, item['preferredTerm'], response['conceptId'])
 
   def _get_klass_attribute(self):
-    for klass, info in self.cdisc_ct_config['klass'].items():
+    for klass, info in self._cdisc_ct_config['klass'].items():
       if not klass in self._by_klass_attribute:
         self._by_klass_attribute[klass] = {}
       for attribute, cl in info.items():
         if not attribute in self._by_klass_attribute[klass]:
           self._by_klass_attribute[klass][attribute] = cl
 
   def _get_code_list(self, c_code):
-    for package in self.cdisc_ct_config['packages']:
+    for package in self._cdisc_ct_config['packages']:
       package_full_name = "%sct-%s" % (package, self.version)
       api_url = self._url('/mdr/ct/packages/%s/codelists/%s' % (package_full_name, c_code))
-      package_logger.info(f"CDISC CT Library: {api_url}")
+      self._logger.info(f"CDISC CT Library: {api_url}")
       raw = requests.get(api_url, headers=self.__class__.HEADERS)
       if raw.status_code == 200:
         response = raw.json()
         response.pop('_links', None)
         self._by_code_list[response['conceptId']] = response
         for item in response['terms']:
           self._check_in_and_add(self._by_term, item['conceptId'], response['conceptId'])
           self._check_in_and_add(self._by_submission, item['submissionValue'], response['conceptId'])
           self._check_in_and_add(self._by_pt, item['preferredTerm'], response['conceptId'])
         return
     # If none found in all of the packages, then log error.
-    package_logger.error(f"Failed to find CDSIC CT for C code '{c_code}'")
+    self._errors_and_logging.exception(f"Failed to find CDSIC CT for C code '{c_code}'")
 
   def _url(self, relative_url):
     return f"{self.__class__.API_ROOT}{relative_url}"
 
   def _check_in_and_add(self, collection, id, item):
     if not id in collection:
       collection[id] = []
@@ -153,29 +157,25 @@
 
   def _save_code_lists(self, data):
     try:
       if not self._code_lists_exist():
         with open(self._ct_filename(), 'w') as f:
           yaml.dump(data, f, indent=2, sort_keys=True)
     except Exception as e:
-      package_logger.error(f"Exception '{e}', failed to save CDSIC CT file")
-      package_logger.debug(f"{e}\n{traceback.format_exc()}")
+      self._errors_and_logging.exception("Failed to save CDSIC CT file", e)
 
   def _read_code_lists(self):
     try:
       if self._code_lists_exist():
         with open(self._ct_filename()) as f:
-          return yaml.load(f, Loader=yaml.FullLoader)
+          return yaml.safe_load(f)
       else:
-        package_logger.error(f"Failed to read CDSIC CT file, does not exist")
+        self._errors_and_logging.error(f"Failed to read CDSIC CT file, does not exist")
         return None
     except Exception as e:
-      package_logger.error(f"Exception '{e}', failed to read CDSIC CT file")
-      package_logger.debug(f"{e}\n{traceback.format_exc()}")
+      self._errors_and_logging.exception("Failed to read CDSIC CT file", e)
 
   def _code_lists_exist(self):
     return os.path.isfile(self._ct_filename()) 
 
   def _ct_filename(self):
-    return os.path.join(os.path.dirname(__file__), 'data', f"cdisc_ct_{self.cdisc_ct_config['version']}.yaml")
-
-cdisc_ct_library = CDISCCTLibrary()
+    return os.path.join(os.path.dirname(__file__), 'data', f"cdisc_ct_{self._cdisc_ct_config['version']}.yaml")
```

### Comparing `usdm-0.48.0/src/usdm_excel/configuration_sheet.py` & `usdm-0.49.0/src/usdm_excel/configuration_sheet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,42 @@
-from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.ct_version_manager import ct_version_manager
-from usdm_excel.option_manager import * 
 import traceback
-import pandas as pd
+from usdm_excel.base_sheet import BaseSheet
+from usdm_excel.option_manager import Options, EmptyNoneOption
+from usdm_excel.globals import Globals
 
 class ConfigurationSheet(BaseSheet):
 
+  SHEET_NAME = 'configuration'
+  
   PARAMS_NAME_COL = 0
   PARAMS_VALUE_COL = 1
 
-  def __init__(self, file_path):
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='configuration', header=None)
-      option_manager.set(Options.EMPTY_NONE, EmptyNoneOption.NONE)
-      option_manager.set(Options.USDM_VERSION, 3)
-      # option_manager.set(Options.PREVIOUS_NEXT, PrevNextOption.NONE)
-      # option_manager.set(Options.ROOT, RootOption.API_COMPLIANT)
-      # option_manager.set(Options.DESCRIPTION, "")
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME, header=None)
+      self.globals.option_manager.set(Options.EMPTY_NONE, EmptyNoneOption.NONE)
+      self.globals.option_manager.set(Options.USDM_VERSION, 3)
       self._process_sheet()
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
 
-  def om(self):
-    return option_manager
-  
   def _process_sheet(self):
     for rindex, row in self.sheet.iterrows():
       name = self.read_cell(rindex, self.PARAMS_NAME_COL).strip().upper()
       value = self.read_cell(rindex, self.PARAMS_VALUE_COL)
       if name == 'CT VERSION':
         parts = value.split('=')
         if len(parts) == 2:
-          ct_version_manager.add(parts[0].strip(), parts[1].strip())
+          self.globals.ct_version_manager.add(parts[0].strip(), parts[1].strip())
       elif name == 'EMPTY NONE':
         if value.strip().upper() == 'EMPTY':
-          option_manager.set(Options.EMPTY_NONE, EmptyNoneOption.EMPTY)
+          self.globals.option_manager.set(Options.EMPTY_NONE, EmptyNoneOption.EMPTY)
       elif name == 'USDM VERSION':
         text = value.strip().upper()
         if text in ['2', '3']:
-          option_manager.set(Options.USDM_VERSION, int(text))
+          self.globals.option_manager.set(Options.USDM_VERSION, int(text))
       elif name == 'SDR PREV NEXT':
         self._general_warning("The SDR PREV NEXT option is now deprecated and will be ignored.")
       elif name == 'SDR ROOT':
         self._general_warning("The SDR ROOT option is now deprecated and will be ignored.")
       elif name == 'SDR DESCRIPTION':
         self._general_warning("The SDR DESCRIPTION option is now deprecated and will be ignored.")
```

### Comparing `usdm-0.48.0/src/usdm_excel/cross_ref.py` & `usdm-0.49.0/src/usdm_excel/cross_ref.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import traceback
-from usdm_excel.errors.errors import error_manager
+from usdm_excel.errors_and_logging.errors_and_logging import ErrorsAndLogging
 
 class CrossRef():
 
   class PathError(Exception):
     pass
 
-  def __init__(self):
-    self.references = {}
-    self.identifiers = {}
+  def __init__(self, errors_and_logging: ErrorsAndLogging):
+    self._errors_and_logging = errors_and_logging
+    self._references = {}
+    self._identifiers = {}
 
   def clear(self):
-    self.references = {}
-    self.identifiers = {}
+    self._references = {}
+    self._identifiers = {}
 
   def add(self, name, object):
     klass = object.__class__
     try:
       key, id_key = self._key(klass, name, object.id)
-      if not key in self.references:
-        self.references[key] = object
-        self.identifiers[id_key] = object
+      if not key in self._references:
+        self._references[key] = object
+        self._identifiers[id_key] = object
       else:
-        error_manager.add(None, None, None, f"Duplicate cross reference detected, class '{self._klass_name(klass)}' with name '{name}'")
+        self._error(f"Duplicate cross reference detected, class '{self._klass_name(klass)}' with name '{name}'")
     except Exception as e:
-      error_manager.add(None, None, None, f"Failed to add cross reference detected, class '{self._klass_name(klass)}' with name '{name}'. Exception {e}")
+      self._exception(f"Failed to add cross reference detected, class '{self._klass_name(klass)}' with name '{name}'.", e)
 
   def get(self, klass, name):
     key, id_key = self._key(klass, name, "")
-    if key in self.references:
-      return self.references[key]
+    if key in self._references:
+      return self._references[key]
     else:
       return None
 
   def get_by_id(self, klass, id):
     key, id_key = self._key(klass, "", id)
-    if id_key in self.identifiers:
-      return self.identifiers[id_key]
+    if id_key in self._identifiers:
+      return self._identifiers[id_key]
     else:
       return None
 
   def get_by_path(self, klass, name, path):
     instance = self.get(klass, name)
     if instance:
       parts = path.split("/")
@@ -53,16 +53,16 @@
             instance = getattr(instance, attribute)
           except AttributeError as e:
             raise self.PathError(f"Failed to translate reference path '{path}', attribute '{attribute}' was not found")
           attribute = parts[index+1].replace('@', '')
           if not parts[index] == instance.__class__.__name__:
             raise self.PathError(f"Failed to translate reference path '{path}', class mismtach, expecting '{parts[index]}', found '{instance.__class__.__name__}'")
         if instance and attribute:
-          if not cross_references.get_by_id(instance.__class__, instance.id):
-            cross_references.add(instance.id, instance)
+          if not self.get_by_id(instance.__class__, instance.id):
+            self.add(instance.id, instance)
           return instance, attribute
         else:
           raise self.PathError(f"Failed to translate reference path '{path}', path was not found")
       else:
         raise self.PathError(f"Failed to translate reference path '{path}', format error")
     else:
       raise self.PathError(f"Failed to translate reference path '{path}', could not find start instance '{klass}', '{name}'")
@@ -70,8 +70,12 @@
   def _key(self, klass, name, id):
     klass_name = self._klass_name(klass)
     return f"{klass_name}.{name}", f"{klass_name}.{id}"
 
   def _klass_name(self, klass):
     return klass if isinstance(klass, str) else klass.__name__
 
-cross_references = CrossRef()
+  def _error(self, message):
+    self._errors_and_logging.error(message)
+
+  def _exception(self, message, e):
+    self._errors_and_logging.exception(message, e)
```

### Comparing `usdm-0.48.0/src/usdm_excel/data/cdisc_bcs.yaml` & `usdm-0.49.0/src/usdm_excel/data/cdisc_bcs.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_excel/data/cdisc_ct_2023-12-15.yaml` & `usdm-0.49.0/src/usdm_excel/data/cdisc_ct_2023-12-15.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_excel/data/cdisc_ct_config.yaml` & `usdm-0.49.0/src/usdm_excel/data/cdisc_ct_config.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_excel/data/iso_3166.json` & `usdm-0.49.0/src/usdm_excel/data/iso_3166.json`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_excel/data/missing_ct.yaml` & `usdm-0.49.0/src/usdm_excel/data/missing_ct.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -52,65 +52,65 @@
 #     synonyms: []
 #   - conceptId: C99901x3
 #     definition: A type of time point relationship that is fixed with respect to a
 #       timeline.
 #     preferredTerm: Fixed Reference
 #     submissionValue: ''
 #     synonyms: []
-- conceptId: C174222
-  definition: ''
-  extensible: false
-  name: ''
-  preferredTerm: ''
-  submissionValue: ''
-  synonyms: []
-  terms:
-  - conceptId: C174267
-    definition: An arm describing the active comparator.
-    preferredTerm: Active Comparator Arm
-    submissionValue: ''
-    synonyms: []
-  - conceptId: C174226
-    definition: An arm describing the intervention or treatment plan for a group of
-      participants in the study receiving a control. The control may comprise a non-investigational
-      product (active control) or regimen, placebo, or no treatment.
-    preferredTerm: Control Arm
-    submissionValue: ''
-    synonyms: []
-  - conceptId: C174266
-    definition: An arm describing the intervention or treatment plan for a group of
-      participants in the study receiving test product(s).
-    preferredTerm: Experimental Arm
-    submissionValue: ''
-    synonyms:
-    - Investigational Arm
-  - conceptId: C174270
-    definition: A study arm without an intervention or treatment.
-    preferredTerm: No Intervention Arm
-    submissionValue: ''
-    synonyms: []
-  - conceptId: C174268
-    definition: An arm describing the placebo comparator.
-    preferredTerm: Placebo Comparator Arm
-    submissionValue: ''
-    synonyms:
-    - Placebo Control Arm
-  - conceptId: C174269
-    definition: An arm describing the sham comparator.
-    preferredTerm: Sham Comparator Arm
-    submissionValue: ''
-    synonyms:
-    - Sham Intervention Arm
-  - conceptId: C15538
-    definition: An arm describing the intervention or treatment plan for a group of
-      participants in the study. Treatment may consist of either experimental or control
-      products under investigation.
-    preferredTerm: Treatment Arm
-    submissionValue: ''
-    synonyms: []
+# - conceptId: C174222
+#   definition: ''
+#   extensible: false
+#   name: ''
+#   preferredTerm: ''
+#   submissionValue: ''
+#   synonyms: []
+#   terms:
+#   - conceptId: C174267
+#     definition: An arm describing the active comparator.
+#     preferredTerm: Active Comparator Arm
+#     submissionValue: ''
+#     synonyms: []
+#   - conceptId: C174226
+#     definition: An arm describing the intervention or treatment plan for a group of
+#       participants in the study receiving a control. The control may comprise a non-investigational
+#       product (active control) or regimen, placebo, or no treatment.
+#     preferredTerm: Control Arm
+#     submissionValue: ''
+#     synonyms: []
+#   - conceptId: C174266
+#     definition: An arm describing the intervention or treatment plan for a group of
+#       participants in the study receiving test product(s).
+#     preferredTerm: Experimental Arm
+#     submissionValue: ''
+#     synonyms:
+#     - Investigational Arm
+#   - conceptId: C174270
+#     definition: A study arm without an intervention or treatment.
+#     preferredTerm: No Intervention Arm
+#     submissionValue: ''
+#     synonyms: []
+#   - conceptId: C174268
+#     definition: An arm describing the placebo comparator.
+#     preferredTerm: Placebo Comparator Arm
+#     submissionValue: ''
+#     synonyms:
+#     - Placebo Control Arm
+#   - conceptId: C174269
+#     definition: An arm describing the sham comparator.
+#     preferredTerm: Sham Comparator Arm
+#     submissionValue: ''
+#     synonyms:
+#     - Sham Intervention Arm
+#   - conceptId: C15538
+#     definition: An arm describing the intervention or treatment plan for a group of
+#       participants in the study. Treatment may consist of either experimental or control
+#       products under investigation.
+#     preferredTerm: Treatment Arm
+#     submissionValue: ''
+#     synonyms: []
 - conceptId: C99902x
   definition: ''
   extensible: false
   name: ''
   preferredTerm: ''
   submissionValue: ''
   synonyms: []
```

### Comparing `usdm-0.48.0/src/usdm_excel/document/document.py` & `usdm-0.49.0/src/usdm_db/document/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import os
-import traceback
 import docraptor
 from yattag import Doc
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.study_sheet.study_sheet import Study
-from .utility import get_soup
+from usdm_model.study import Study
+from usdm_db.cross_reference import CrossReference
+from usdm_db.errors_and_logging.errors_and_logging import ErrorsAndLogging
+from usdm_db.document.utility import get_soup
 
 class Document():
 
   class LogicError(Exception):
     pass
 
-  def __init__(self, parent: BaseSheet, doc_title: str, study: Study, filepath: str):
-    self.parent = parent
-    self.filepath = filepath
+  def __init__(self, doc_title: str, study: Study, errors_and_logging: ErrorsAndLogging):
     self.study = study
+    self._errors_and_logging = ErrorsAndLogging()
+    self._cross_ref = CrossReference(study, self._errors_and_logging)
     self.study_version = study.versions[0]
     self.study_design = self.study_version.studyDesigns[0]
     self.protocol_document_version = self.study.documentedBy.versions[0]
     self.doc_title = doc_title
     self.chapters = []
     self.modal_count = 1
     if self.protocol_document_version.id != self.study.versions[0].documentVersionId:
-      self.parent._general_error(f"Failed to initialise NarrativeContent for document creation, ids did not match")
       raise self.LogicError(f"Failed to initialise NarrativeContent for document creation, ids did not match")
 
   def to_pdf(self, test=True):
     doc_api = docraptor.DocApi()
     doc_api.api_client.configuration.username = os.getenv('DOCRAPTOR_API_KEY')
     document_content = self.to_html()
     try:
@@ -42,19 +40,19 @@
         #    'media': 'print', # @media 'screen' or 'print' CSS
         #    'baseurl': 'https://yoursite.com', # the base URL for any relative URLs
         # },
       })
       binary_formatted_response = bytearray(response)
       return binary_formatted_response
     except docraptor.rest.ApiException as e:
-      self.parent._traceback(f"Failed to create PDF document {e.status} {e.reason} {e.body}\n{traceback.format_exc()}")
-      self.parent._general_error(f"Something went wrong '{e.reason}' creating the PDF document")
+      self._errors_and_logging.exception(f"Exception raised generating PDF content. See logs for more details", e)
+      return None
     except Exception as e:
-      self.parent._general_error(f"Exception '{e}' raised generating PDF content.\n{traceback.format_exc()}")
-      self.parent._general_error(f"Exception '{e}' raised generating PDF content")
+      self._errors_and_logging.exception(f"Exception raised generating PDF content. See logs for more details", e)
+      return None
 
   def to_html(self, highlight=False):
     try:
       self.modal_count = 1
       self.chapters = []
       root = self.protocol_document_version.contents[0]
       doc = Doc()
@@ -112,16 +110,16 @@
           doc.asis(self._title_page())    
           for id in root.childIds:
             content = next((x for x in self.protocol_document_version.contents if x.id == id), None)
             if content:
               self._content_to_html(content, doc, highlight)
       return doc.getvalue()
     except Exception as e:
-      self.parent._traceback(f"Exception '{e}' raised generating HTML content.\n{traceback.format_exc()}")
-      self.parent._general_error(f"Exception '{e}' raised generating HTML content")
+      self._errors_and_logging.exception(f"Exception raised generating HTML content. See logs for more details", e)
+      return None
 
   def _content_to_html(self, content, doc, highlight=False):
     level = self._get_level(content.sectionNumber)
     klass = "page" if level == 1 else ""
     heading_id = f"section-{content.sectionNumber}"
     if (level == 1 and self._is_first_section(content.sectionNumber)):
       with doc.tag('div', klass=klass):
@@ -158,69 +156,65 @@
     try:
       sn = int(section_number)
       return True if sn == 1 else False
     except:
       return False
 
   def _translate_references(self, content_text, highlight=False):
-    soup = get_soup(content_text, self.parent)
+    soup = get_soup(content_text, self._errors_and_logging)
     for ref in soup(['usdm:ref']):
       try:
         attributes = ref.attrs
-        instance = cross_references.get_by_id(attributes['klass'], attributes['id'])
+        instance = self._cross_ref.get(attributes['klass'], attributes['id'])
         value = self._resolve_instance(instance, attributes['attribute'])
         translated_text = self._translate_references(value, highlight)
         self._replace_and_highlight(soup, ref, translated_text, highlight)
-        #ref.replace_with(translated_text)
       except Exception as e:
-        self.parent._traceback(f"Failed to translate reference '{attributes}'\n{traceback.format_exc()}")
-        self.parent._general_error(f"Exception '{e} while attempting to translate reference '{attributes}' while generating the HTML document")
+        self._errors_and_logging.exception(f"Exception raised while attempting to translate reference '{attributes}' while generating the HTML document, see the logs for more info", e)
         self._replace_and_highlight(soup, ref, 'Missing content: exception', highlight)
-        #ref.replace_with('Missing content: exception')
-    self.parent._general_debug(f"Translate references from {content_text} => {get_soup(str(soup), self.parent)}")
-    return get_soup(str(soup), self.parent)
+    self._errors_and_logging.debug(f"Translate references from {content_text} => {get_soup(str(soup), self._errors_and_logging)}")
+    return get_soup(str(soup), self._errors_and_logging)
 
   def _resolve_instance(self, instance, attribute, highlight=False):
     dictionary = self._get_dictionary(instance)
     value = str(getattr(instance, attribute))
-    soup = get_soup(value, self.parent)
+    soup = get_soup(value, self._errors_and_logging)
     for ref in soup(['usdm:tag']):
       try:
         attributes = ref.attrs
         if dictionary:
           entry = next((item for item in dictionary.parameterMaps if item.tag == attributes['name']), None)
-          self._replace_and_highlight(soup, ref, get_soup(entry.reference, self.parent), highlight)
+          self._replace_and_highlight(soup, ref, get_soup(entry.reference, self._errors_and_logging), highlight)
         else:
-          self.parent._general_error(f"Missing dictionary while attempting to resolve reference '{attributes}' while generating the HTML document")
+          self._errors_and_logging.error(f"Missing dictionary while attempting to resolve reference '{attributes}' while generating the HTML document")
           self._replace_and_highlight(soup, ref, 'Missing content: missing dictionary', highlight)
       except Exception as e:
-        self.parent._traceback(f"Failed to resolve reference '{attributes}'\n{traceback.format_exc()}")
-        self.parent._general_error(f"Exception '{e} while attempting to resolve reference '{attributes}' while generating the HTML document")
+        self._errors_and_logging.exception(f"Failed to resolve reference '{attributes} while generating the HTML document", e)
         self._replace_and_highlight(soup, ref, 'Missing content: exception', highlight)
     return str(soup)
 
   def _get_dictionary(self, instance):
     try:
-      return cross_references.get_by_id('SyntaxTemplateDictionary', instance.dictionaryId)
+      return self._cross_ref.get('SyntaxTemplateDictionary', instance.dictionaryId)
     except:
       return None  
 
   def _replace_and_highlight(self, soup, ref, text, highlight):
     if highlight:
       self._wrap_in_span_and_modal(soup, ref, text)
     else:
       ref.replace_with(text)
 
   def _wrap_in_span_and_modal(self, soup, ref, text):
     id = f"usdmContent{self.modal_count}"
     span = soup.new_tag('span', attrs={'class': "usdm-highlight"})
-    span.append(get_soup(self._link(id), self.parent))
+    span.append(get_soup(self._link(id), self._errors_and_logging))
     span.append(text)
     ref.replace_with(span)
-    span.append(get_soup(self._modal(ref, id), self.parent))
+    span.append(get_soup(self._modal(ref, id), self._errors_and_logging))
     self.modal_count += 1
 
   def _link(self, id):
     return f"""
       <a class="link-dark usdm-highlight-link" style="font-size: 12px;" data-bs-toggle="modal" data-bs-target="#{id}">
         <i class="ps-1 pe-1 bi bi-info-circle"/>
       </a>
```

### Comparing `usdm-0.48.0/src/usdm_excel/document/elements.py` & `usdm-0.49.0/src/usdm_excel/document/elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,28 @@
     identifier = self._sponsor_identifier()
     results = [
       {'instance': identifier.studyIdentifierScope, 'klass': 'Organization', 'attribute': 'name'},
       {'instance': identifier.studyIdentifierScope.legalAddress, 'klass': 'Address', 'attribute': 'text'},
     ]
     return self._set_of_references(results)
 
+  def organization_address(self):
+    identifier = self._sponsor_identifier()
+    results = [
+      {'instance': identifier.studyIdentifierScope.legalAddress, 'klass': 'Address', 'attribute': 'text'},
+    ]
+    return self._set_of_references(results)
+
+  def organization_name(self):
+    identifier = self._sponsor_identifier()
+    results = [
+      {'instance': identifier.studyIdentifierScope, 'klass': 'Organization', 'attribute': 'name'},
+    ]
+    return self._set_of_references(results)
+
   def amendment(self):
     amendments = self.study_version.amendments
     results = [{'instance': amendments[-1], 'klass': 'StudyAmendment', 'attribute': 'number'}]
     return self._set_of_references(results)
 
   def amendment_scopes(self):
     results = []
```

### Comparing `usdm-0.48.0/src/usdm_excel/document/macros.py` & `usdm-0.49.0/src/usdm_excel/document/macros.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import os
 import base64
-import traceback
-from .template_m11 import TemplateM11
-from .template_plain import TemplatePlain
-from .elements import Elements
-from usdm_excel.cross_ref import cross_references
+from usdm_excel.document.template_m11 import TemplateM11
+from usdm_excel.document.template_plain import TemplatePlain
+from usdm_excel.document.elements import Elements
 from usdm_excel.base_sheet import BaseSheet
-from .utility import get_soup
+from usdm_model.study import Study
+from usdm_model.activity import Activity
+from usdm_model.biomedical_concept import BiomedicalConcept
+from usdm_model.biomedical_concept_surrogate import BiomedicalConceptSurrogate
+from usdm_excel.document.utility import get_soup
 
 class Macros():
 
-  def __init__(self, parent: BaseSheet, study):
+  def __init__(self, parent: BaseSheet, study: Study):
     self.parent = parent
     self.study = study
     self.study_version = study.versions[0]
     self.study_design = self.study_version.studyDesigns[0]
     self.protocol_document_version = self.study.documentedBy.versions[0]
     self.elements = Elements(parent, self.study)
     self.m11 = TemplateM11(parent, self.study)
@@ -29,24 +31,48 @@
         method = f"_{attributes['id'].lower()}"
         if self._valid_method(method):
           result = getattr(self, method)(attributes, soup, ref)
         else:
           self.parent._general_error(f"Failed to resolve document macro '{attributes}', invalid method name {method}")
           ref.replace_with('Missing content: invalid method name')
       except Exception as e:
-        self.parent._traceback(f"Failed to resolve document macro '{attributes}'\n{traceback.format_exc()}")
-        self.parent._general_error(f"Exception '{e} while attempting to translate document macro '{attributes}'")
+        self.parent._general_exception(f"Failed to resolve document macro '{attributes}'", e)
         ref.replace_with('Missing content: exception')
     return str(soup)
 
   def _xref(self, attributes, soup, ref) -> None:
-    instance, attribute = cross_references.get_by_path(attributes['klass'], attributes['name'], attributes['attribute'])
+    instance, attribute = self.parent.globals.cross_references.get_by_path(attributes['klass'], attributes['name'], attributes['attribute'])
     ref_tag = soup.new_tag("usdm:ref")
     ref_tag.attrs = {'klass': instance.__class__.__name__, 'id': instance.id, 'attribute': attribute}
     ref.replace_with(ref_tag)
+      
+  def _bc(self, attributes, soup, ref) -> None:
+    bc_name = attributes['name'].upper().strip()
+    activity_name = attributes['activity'].strip()
+    activity = self.parent.globals.cross_references.get(Activity, activity_name)
+    if activity:
+      bc = None
+      for collection in [{'klass': BiomedicalConcept, 'ids': activity.biomedicalConceptIds, 'synonyms': True}, 
+                         {'klass': BiomedicalConceptSurrogate, 'ids': activity.bcSurrogateIds, 'synonyms': False}]:
+        for id in collection['ids']:
+          next_bc = self.parent.globals.cross_references.get_by_id(collection['klass'], id)
+          if next_bc:
+            if bc_name == next_bc.name.upper() or bc_name in [x.upper() for x in next_bc.synonyms]:
+              bc = next_bc
+              break
+      if bc:      
+        ref_tag = soup.new_tag("usdm:ref")
+        ref_tag.attrs = {'klass': bc.__class__.__name__, 'id': bc.id, 'attribute': 'label'}
+        ref.replace_with(ref_tag)
+      else:
+        self.parent._general_error(f"Failed to find BC name '{bc_name}' in activity '{activity_name}'")
+        ref.replace_with('Missing BC: failed to find BC in activity')
+    else:
+      self.parent._general_error(f"Failed to find  activity '{activity_name}'")
+      ref.replace_with('Missing activity: failed to find activity')
 
   def _image(self, attributes, soup, ref) -> None:
     type = {attributes['type']}
     data = self._encode_image(attributes['file'])
     if data:
       img_tag = soup.new_tag("img")
       img_tag.attrs['src'] = f"data:image/{type};base64,{data.decode('ascii')}"
@@ -64,15 +90,15 @@
       ref.replace_with('Missing content: invalid method name')
 
   def _section(self, attributes, soup, ref) -> None:
     method = attributes['name'].lower()
     template = attributes['template'] if 'template' in attributes else 'plain' 
     instance = self._resolve_template(template)
     if instance.valid_method(method):
-      text = getattr(instance, method)()
+      text = getattr(instance, method)(attributes)
       ref.replace_with(get_soup(text, self.parent))
     else:
       self.parent._general_error(f"Failed to translate section method name '{method}' in '{attributes}', invalid method")
       ref.replace_with('Missing content: invalid method name')       
 
   def _note(self, attributes, soup, ref) -> None:
     text = f"""
@@ -80,15 +106,15 @@
         <p class="usdm-warning">Note:</p>
         <p class="usdm-warning">{attributes['text']}</p>
       </div>
     """
     ref.replace_with(get_soup(text, self.parent))
 
   def _valid_method(self, name):
-    return name in ['_xref', '_image', '_element', '_section', '_note']
+    return name in ['_xref', '_image', '_element', '_section', '_note', '_bc']
   
   def _resolve_template(self, template) -> object:
     try:
       return self.template_map[template.lower()]
     except:
       self.parent._general_error(f"Failed to map template '{template}', using plain template")
       return self.plain
```

### Comparing `usdm-0.48.0/src/usdm_excel/document/soa.py` & `usdm-0.49.0/src/usdm_excel/document/soa.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from .utility import usdm_reference
-from usdm_excel.cross_ref import cross_references
 from usdm_excel.base_sheet import BaseSheet
-#from usdm_excel.study_sheet.study_sheet import Study
 from usdm_model.schedule_timeline import ScheduleTimeline
-from usdm_model.activity import Activity
-from usdm_model.scheduled_instance import ScheduledActivityInstance, ScheduledDecisionInstance
+#from usdm_model.activity import Activity
+#from usdm_model.scheduled_instance import ScheduledActivityInstance, ScheduledDecisionInstance
 from usdm_model.study_design import StudyDesign
 
 class SoA():
 
   def __init__(self, parent: BaseSheet, study_design: StudyDesign, timeline: ScheduleTimeline):
     self.parent = parent
     self.study_design = study_design
@@ -43,17 +41,18 @@
     # ScheduleActivityInstance order
     required_activities = []
     sai_order = []
     item = self._find(self.timeline.instances, self.timeline.entryId)
     more = True
     while more:
       sai_order.append(item)
-      for id in item.activityIds:
-        if id not in required_activities:
-          required_activities.append(id)
+      if hasattr(item, 'activityIds'):
+        for id in item.activityIds:
+          if id not in required_activities:
+            required_activities.append(id)
       more = False if not item.defaultConditionId else True
       item = self._find(self.timeline.instances, item.defaultConditionId)
     #print(f"SAI ORDER: {sai_order}\n\n")
     #print(f"ACTIVITIES: {required_activities}\n\n")
 
     # Activity order
     activity_order = []
@@ -81,24 +80,25 @@
     # for index, sai in enumerate(sai_order):
     #   row[index + sai_start_index]['label'] = index
     # results.append(row)
 
     row = self._template_copy(row_template)    
     for index, sai in enumerate(sai_order):
       if sai.epochId:
-        item = cross_references.get_by_id("StudyEpoch", sai.epochId)
+        item = self.parent.globals.cross_references.get_by_id("StudyEpoch", sai.epochId)
         row[index + sai_start_index]['label'] = usdm_reference(item, 'label') if item else "???"
     if self._has_non_empty(row):
       results.append(row)
 
     row = self._template_copy(row_template)
     for index, sai in enumerate(sai_order):
-      if sai.encounterId:
-        item = cross_references.get_by_id("Encounter", sai.encounterId)
-        row[index + sai_start_index]['label'] = usdm_reference(item, 'label') if item else "???"
+      if hasattr(sai, 'encounterId'):
+        if sai.encounterId:
+          item = self.parent.globals.cross_references.get_by_id("Encounter", sai.encounterId)
+          row[index + sai_start_index]['label'] = usdm_reference(item, 'label') if item else "???"
     if self._has_non_empty(row):
       results.append(row)
 
     row = self._template_copy(row_template)
     for index, sai in enumerate(sai_order):
       timing = self._timing_from(self.timeline.timings, sai)
       if timing:
@@ -118,15 +118,16 @@
       row = self._template_copy(row_template)
       row[0]['label'] = usdm_reference(activity, 'label')
       condition = self._condition_no_context(self.study_design.conditions, activity)
       if condition:
         row[0]['condition'] = condition
       for index, sai in enumerate(sai_order):
         row[index + sai_start_index]['set'] = False
-        if activity.id in sai.activityIds:
-          row[index + sai_start_index]['set'] = True
-          condition = self._condition_with_context(self.study_design.conditions, activity, sai)
-          if condition:
-            row[index + sai_start_index]['condition'] = condition
+        if hasattr(sai, 'activityIds'):
+          if activity.id in sai.activityIds:
+            row[index + sai_start_index]['set'] = True
+            condition = self._condition_with_context(self.study_design.conditions, activity, sai)
+            if condition:
+              row[index + sai_start_index]['condition'] = condition
       results.append(row)
 
     return results
```

### Comparing `usdm-0.48.0/src/usdm_excel/document/template_base.py` & `usdm-0.49.0/src/usdm_excel/document/template_base.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_excel/document/template_m11.py` & `usdm-0.49.0/src/usdm_excel/document/template_m11.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import re
 from yattag import Doc
 #from .elements import Elements
 from .template_base import TemplateBase
-#from usdm_excel.cross_ref import cross_references
+##from usdm_excel.cross_ref import cross_references
 from usdm_excel.base_sheet import BaseSheet
 
 class TemplateM11(TemplateBase):
 
   def __init__(self, parent: BaseSheet, study):
     super().__init__(parent, study)
 
-  def title_page(self):
+  def title_page(self, attributes):
     doc = Doc()
     with doc.tag('table'):
       self._title_page_entry(doc, 'Sponsor Confidentiality Statement:', '')
       self._title_page_entry(doc, 'Full Title:', f'{self.elements.study_full_title()}')
       self._title_page_entry(doc, 'Trial Acronym:', f'{self.elements.study_acronym()}')
       self._title_page_entry(doc, 'Protocol Identifier:', f'{self.elements.study_identifier()}')
       self._title_page_entry(doc, 'Original Protocol:', '')
@@ -37,21 +37,21 @@
       # Region Identifier
       # Secondary Reason for Amendment
 
     result = doc.getvalue()
     #print(f"DOC: {result}")
     return result
 
-  def inclusion(self):  
+  def inclusion(self, attributes):  
     return self._criteria("C25532")
   
-  def exclusion(self):  
+  def exclusion(self, attributes):  
     return self._criteria("C25370")
 
-  def objective_endpoints(self):
+  def objective_endpoints(self, attributes):
     #print(f"M11 TP:")
     doc = Doc()
     with doc.tag('table'):
       for item in self._objective_endpoints_list():
         self._objective_endpoints_entry(doc, item['objective'], item['endpoints'])
     return doc.getvalue()
```

### Comparing `usdm-0.48.0/src/usdm_excel/document/template_plain.py` & `usdm-0.49.0/src/usdm_excel/document/template_plain.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-import traceback
 from yattag import Doc
-#from .elements import Elements
-from .template_base import TemplateBase
-from .soa import SoA
-#from usdm_excel.cross_ref import cross_references
+from usdm_excel.document.template_base import TemplateBase
+from usdm_excel.document.soa import SoA
 from usdm_excel.base_sheet import BaseSheet
+from usdm_model.schedule_timeline import ScheduleTimeline
 
 class TemplatePlain(TemplateBase):
 
   def __init__(self, parent: BaseSheet, study):
     super().__init__(parent, study)
 
-  def title_page(self):
+  def title_page(self, attributes):
     doc = Doc()
     with doc.tag('table'):
       self._title_page_entry(doc, 'Full Title:', f'{self.elements.study_full_title()}')
       self._title_page_entry(doc, 'Trial Acronym:', f'{self.elements.study_acronym()}')
       self._title_page_entry(doc, 'Protocol Identifier:', f'{self.elements.study_identifier()}')
       self._title_page_entry(doc, 'Version Number:', f'{self.elements.study_version_identifier()}')
       self._title_page_entry(doc, 'Version Date:', f'{self.elements.study_date()}')
@@ -25,73 +23,91 @@
       self._title_page_entry(doc, 'Short Title:', f'{self.elements.study_short_title()}')
       self._title_page_entry(doc, 'Sponsor Name and Address:', f'{self.elements.organization_name_and_address()}')
       self._title_page_entry(doc, 'Regulatory Agency Identifier Number(s):', f'{self.elements.study_regulatory_identifiers()}')
       self._title_page_entry(doc, 'Spondor Approval Date:', f'{self.elements.approval_date()}')
     result = doc.getvalue()
     return result
 
-  def inclusion(self):  
+  def inclusion(self, attributes: dict):  
     return self._criteria("C25532")
   
-  def exclusion(self):  
+  def exclusion(self, attributes: dict):  
     return self._criteria("C25370")
 
-  def objective_endpoints(self):
+  def objective_endpoints(self, attributes: dict):
     doc = Doc()
     with doc.tag('table', klass='table'):
       for item in self._objective_endpoints_list():
         self._objective_endpoints_entry(doc, item['objective'], item['endpoints'])
     return doc.getvalue()
 
-  def soa(self):
+  def soa(self, attributes: dict):
     try:
       doc = Doc()
       for timeline in self.study_design.scheduleTimelines:      
-        footnote = 1
-        footnotes = []
-        soa = SoA(self.parent, self.study_design, timeline)
-        result = soa.generate()
-        with doc.tag('div', klass="page soa-page table-responsive"):
-          with doc.tag('p'):
-            with doc.tag('b'):
-              doc.asis(f"Timeline: {timeline.label}, {timeline.entryCondition}")
-          with doc.tag('table', klass='table table-bordered table-sm', style="width:100%"):
-            for row in range(len(result)):
-              with doc.tag('tr'):
-                for col in range(len(result[row])):
-                  if 'set' in result[row][col].keys():
-                    label = 'X' if result[row][col]['set'] else ''
-                  else:
-                    label = result[row][col]['label']
-                  with doc.tag('td'):
-                    klass = 'soa-activity-text' if col == 0 else 'soa-body-text'
-                    with doc.tag('p', klass=klass):
-                      doc.asis(label)
-                      if 'condition' in result[row][col].keys():
-                        with doc.tag('sup'):
-                          footnote_str = str(footnote)
-                          doc.text(footnote_str)
-                        footnotes.append({'number': footnote_str, 'text': result[row][col]['condition'].text})
-                        footnote += 1
-          if footnotes:
-            with doc.tag('table', klass='table table-borderless table-sm'):
-              for item in footnotes:
-                with doc.tag('tr'):
-                  with doc.tag('td'):
-                    with doc.tag('p', klass="soa-footnote-text"):
+        doc.asis(self.timeline({'timeline': timeline}))
+    except Exception as e:
+      self.parent._general_exception(f"Error raised generating SoA", e)
+    return doc.getvalue()
+
+  def timeline(self, attributes: dict):
+    try:
+      doc = Doc()
+      timeline = None
+      timeline = self._resolve_timeline(attributes)
+      footnote = 1
+      footnotes = []
+      soa = SoA(self.parent, self.study_design, timeline)
+      result = soa.generate()
+      with doc.tag('div', klass="page soa-page table-responsive"):
+        with doc.tag('p'):
+          with doc.tag('b'):
+            doc.asis(f"Timeline: {timeline.label}, {timeline.entryCondition}")
+        with doc.tag('table', klass='table table-bordered table-sm', style="width:100%"):
+          for row in range(len(result)):
+            with doc.tag('tr'):
+              for col in range(len(result[row])):
+                if 'set' in result[row][col].keys():
+                  label = 'X' if result[row][col]['set'] else ''
+                else:
+                  label = result[row][col]['label']
+                with doc.tag('td'):
+                  klass = 'soa-activity-text' if col == 0 else 'soa-body-text'
+                  with doc.tag('p', klass=klass):
+                    doc.asis(label)
+                    if 'condition' in result[row][col].keys():
                       with doc.tag('sup'):
-                        doc.text(item['number'])
-                  with doc.tag('td'):
-                    with doc.tag('p', klass="soa-footnote-text"):
-                      doc.asis(item['text'])
+                        footnote_str = str(footnote)
+                        doc.text(footnote_str)
+                      footnotes.append({'number': footnote_str, 'text': result[row][col]['condition'].text})
+                      footnote += 1
+        if footnotes:
+          with doc.tag('table', klass='table table-borderless table-sm'):
+            for item in footnotes:
+              with doc.tag('tr'):
+                with doc.tag('td'):
+                  with doc.tag('p', klass="soa-footnote-text"):
+                    with doc.tag('sup'):
+                      doc.text(item['number'])
+                with doc.tag('td'):
+                  with doc.tag('p', klass="soa-footnote-text"):
+                    doc.asis(item['text'])
     except Exception as e:
-      self.parent._traceback(f"Exception '{e}' raised generating SoA content.\n{traceback.format_exc()}")
-      self.parent._general_error(f"Exception '{e}' raised generating SoA content")
+      if timeline:
+        self.parent._general_exception(f"Error raised generating timeline '{timeline.name}'", e)
+        return "Error encountered creating timeline {timeline.name}"  
+      else:  
+        self.parent._general_exception(f"Error raised generating timeline, name not available", e)
+        return "Error encountered creating timeline"  
     return doc.getvalue()
-  
+
+  def _resolve_timeline(self, attributes):
+    return attributes['timeline'] if isinstance(attributes['timeline'], ScheduleTimeline) else self.parent.globals.cross_references.get(ScheduleTimeline, attributes['timeline'])
+
+
   def _criteria(self, type):
     doc = Doc()
     with doc.tag('table', klass='table'):
       for criterion in self._criteria_list(type):
         self._critieria_entry(doc, criterion['identifier'], criterion['text'])
     return doc.getvalue()
```

### Comparing `usdm-0.48.0/src/usdm_excel/document/utility.py` & `usdm-0.49.0/src/usdm_db/document/utility.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import warnings
-import traceback
-from bs4 import BeautifulSoup   
+from bs4 import BeautifulSoup
+from usdm_db.errors_and_logging.errors_and_logging import ErrorsAndLogging
 
 def usdm_reference(item, attribute):
   return f'<usdm:ref klass="{item.__class__.__name__}" id="{item.id}" attribute="{attribute}"></usdm:ref>'
 
-def get_soup(text, parent):
+def get_soup(text: str, errors_and_logging: ErrorsAndLogging):
   try:
     with warnings.catch_warnings(record=True) as warning_list:
       result =  BeautifulSoup(text, 'html.parser')
     if warning_list:
       for item in warning_list:
-        parent._general_warning(f"Warning raised within Soup package, processing '{text}'\nMessage returned '{item.message}'")
+        errors_and_logging.debug(f"Warning raised within Soup package, processing '{text}'\nMessage returned '{item.message}'")
     return result
   except Exception as e:
-    parent._traceback(f"Exception '{e}' raised parsing '{text}'\n{traceback.format_exc()}")
-    parent._general_error(f"Exception raised parsing '{text}'. Ignoring value")
+    errors_and_logging.exception(f"Parsing '{text}' with soup", e)
     return ""
```

### Comparing `usdm-0.48.0/src/usdm_excel/errors/error.py` & `usdm-0.49.0/src/usdm_excel/errors_and_logging/error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_excel/errors/errors.py` & `usdm-0.49.0/src/usdm_excel/errors_and_logging/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+import logging
 from .error import Error
-from usdm_excel.logger import package_logger
 
 class Errors():
 
   WARNING = Error.WARNING
   ERROR = Error.ERROR
   DEBUG = Error.DEBUG
   INFO = Error.INFO
@@ -13,20 +13,18 @@
 
   def clear(self):
     self.items = []
 
   def add(self, sheet: str, row: int, column: int, message: str, level: int=Error.ERROR) -> None:
     error = Error(sheet, row, column, message, level)
     self.items.append(error)      
-    package_logger.log(level, error.to_log())
 
   def count(self) -> int:
     return len(self.items)
   
   def dump(self, level):
     result = []
     for item in self.items:
       if item.level >= level:
         result.append(item.to_dict())
     return result
 
-error_manager = Errors()
```

### Comparing `usdm-0.48.0/src/usdm_excel/export_as_neo4j_dict.py` & `usdm-0.49.0/src/usdm_db/neo4j_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import stringcase
 import json
+import stringcase
 from uuid import uuid4
 
-class ExportAsNeo4jDict():
+class Neo4jDict():
 
   class LogicError(Exception):
     pass
   
   def __init__(self, study):
     self.study = study
     self.nodes = {}
     self.edges = {}
     self.add_edges = []
     self.node_id_to_uuid_map = {}
       
-  def export(self):
+  def to_dict(self):
     node = json.loads(self.study.to_json_with_type())
     self._process_node(node)
     for edge in self.add_edges:
       if edge['end'] in self.node_id_to_uuid_map:
         self._add_edge(edge['start'], self.node_id_to_uuid_map[edge['end']], edge['raw_relation'])
       else:
         raise self.LogicError(f"{edge['start']} --edge-> {edge['end']} [{edge}]")
```

### Comparing `usdm-0.48.0/src/usdm_excel/export_as_timeline.py` & `usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/study_soa_v2_sheet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,106 @@
-from yattag import Doc
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.logger import package_logger
+import traceback
+from usdm_excel.base_sheet import BaseSheet
+from usdm_excel.study_soa_v2_sheet.activities import Activities
+from usdm_excel.study_soa_v2_sheet.scheduled_instances import ScheduledInstances
+from usdm_model.scheduled_instance import ScheduledActivityInstance, ScheduledDecisionInstance
 from usdm_model.schedule_timeline import ScheduleTimeline
-from usdm_model.scheduled_instance import ScheduledActivityInstance, ScheduledDecisionInstance, ScheduledInstance
-from usdm_model.schedule_timeline_exit import ScheduleTimelineExit
+from usdm_excel.globals import Globals
 
-import traceback
+class StudySoAV2Sheet(BaseSheet):
 
-class ExportAsTimeline():
+  NAME_ROW = 0
+  DESCRIPTION_ROW = 1
+  CONDITION_ROW = 2
+  PARAMS_DATA_COL = 1
+
+  def __init__(self, file_path: str, globals: Globals, sheet_name: str, main: bool=False, require: dict={}):
+    try:
+      super().__init__(file_path=file_path, globals=globals, sheet_name=sheet_name, header=None, require=require)
+      self.name = ""
+      self.description = ""
+      self.condition = ""
+      self.timeline = None
+      self.main_timeline = main
+      self.encounters = []
+      self.activities = []
+      self.timelines = []
+      self.biomedical_concept_surrogates = []
+      self.biomedical_concepts = []
+      self._process_sheet()
+      self._raw_activities = Activities(self) # Order important, activities then instances
+      self._raw_instances = ScheduledInstances(self)
+
+      # @TODO Move block to Activities class
+      for item in self._raw_activities.items:
+        activity = item.usdm_activity
+        self.activities.append(activity)
+        self.biomedical_concept_surrogates += item.usdm_biomedical_concept_surrogates
+        self.biomedical_concepts += item.usdm_biomedical_concepts
+      self.double_link(self.activities, 'previousId', 'nextId')
+      
+      self.timeline = self._add_timeline(self.name, self.description, self.condition, self._raw_instances.instances, self._raw_instances.exits)
 
-  FULL = "full"
-  BODY = "body"
+    except Exception as e:
+      self._sheet_exception(e)
 
-  def __init__(self, study):
-    self.study = study
+  def check_timing_references(self, timings, timing_check):
+    timing_set = []
+    for instance in self._raw_instances.items:
+      item = instance.item
+      #print(f"TIMING1: {item.id}, {instance.name}")
+      if isinstance(item, ScheduledActivityInstance):
+        found = False
+        for timing in timings:
+          ids = [timing.relativeFromScheduledInstanceId, timing.relativeToScheduledInstanceId]
+          #print(f"TIMING2: {timing.name}, {ids}")
+          if item.id in ids:
+            #print(f"TIMING3: found")
+            found = True
+            if not timing_check[timing.name]:
+              timing_check[timing.name] = self.name
+              timing_set.append(timing)
+            elif timing_check[timing.name] == self.name:
+              pass
+            else:
+              self._general_warning(f"Duplicate use of timing with name '{timing.name}' across timelines detected")
+            #break
+        if not found:
+          self._general_warning(f"Unable to find timing reference for instance with name '{instance.name}'")
+    return timing_set
+  
+  def timing_match(self, ref):
+    return self._raw_instances.match(ref)
 
-  def export(self, level=FULL):
-    try:
-      doc = Doc()
-      study_design = self.study.versions[0].studyDesigns[0]
-      if level == self.BODY:
-        self._body(doc, study_design)
+  def _process_sheet(self):
+    for rindex in range(self.NAME_ROW, self.CONDITION_ROW + 1):
+      if rindex == self.NAME_ROW:
+        self.name = self.read_cell(rindex, self.PARAMS_DATA_COL)
+      elif rindex == self.DESCRIPTION_ROW:
+        self.description = self.read_cell(rindex, self.PARAMS_DATA_COL)
+      elif rindex == self.CONDITION_ROW:
+        self.condition = self.read_cell(rindex, self.PARAMS_DATA_COL)
       else:
-        self._full(doc, study_design)
-      return doc.getvalue()
+        pass
+
+  def _add_timeline(self, name, description, condition, instances, exit):
+    try:
+      timeline = ScheduleTimeline(
+        id=self.globals.id_manager.build_id(ScheduleTimeline),
+        mainTimeline=self.main_timeline,
+        name=name,
+        description=description,
+        label=name,
+        entryCondition=condition,
+        entryId=instances[0].id,
+        exits=exit,
+        instances=instances
+      )
+      self.globals.cross_references.add(timeline.name, timeline)
+      return timeline
     except Exception as e:
-      package_logger.error(f"Exception '{e}' raised generating HTML page {level}.")
-      package_logger.debug(f"{traceback.format_exc()}")
+      self._general_exception(f"Failed to create ScheduleTimeline object", e)
+      return None
+
+
 
-  def _full(self, doc, study_design):
-    doc.asis('<!DOCTYPE html>')
-    with doc.tag('html'):
-      with doc.tag('head'):
-        pass
-      with doc.tag('body'):
-        self._body(doc, study_design)
-  
-  def _body(self, doc, study_design):
-    for timeline in study_design.scheduleTimelines:
-      timings = timeline.timings
-      with doc.tag(f'h1'):
-        doc.asis(f'{timeline.name}')
-      with doc.tag('pre', klass='mermaid'):
-        doc.asis('\ngraph LR\n')
-        doc.asis(f'{timeline.id}([{timeline.entryCondition}])\n')
-        instance = cross_references.get_by_id(ScheduledActivityInstance, timeline.entryId)
-        if instance.instanceType == ScheduledActivityInstance.__name__: 
-          doc.asis(f'{instance.id}(ScheduledActivityInstance)\n')
-        else:
-          doc.asis(f'{instance.id}{{{{ScheduledDecisionInstance}}}}\n')
-        doc.asis(f'{timeline.id} -->|first| {instance.id}\n')
-        prev_instance = instance
-        instance = cross_references.get_by_id(ScheduledActivityInstance, instance.defaultConditionId)
-        while instance:
-          if instance.instanceType == ScheduledActivityInstance.__name__: 
-            doc.asis(f'{instance.id}(ScheduledActivityInstance)\n')
-          else:
-            doc.asis(f'{instance.id}{{{{ScheduledDecisionInstance}}}}\n')
-            for condition in instance.conditionAssignments:
-              doc.asis(f'{instance.id} -->|{condition.condition}| {condition.conditionTargetId}\n') 
-          doc.asis(f'{prev_instance.id} -->|default| {instance.id}\n')      
-          prev_instance = instance
-          instance = self._get_cross_reference(prev_instance.defaultConditionId)
-        exit = cross_references.get_by_id(ScheduleTimelineExit, prev_instance.timelineExitId)
-        doc.asis(f'{exit.id}([Exit])\n')
-        doc.asis(f'{prev_instance.id} -->|exit| {exit.id}\n')      
-        for timing in timings:
-          doc.asis(f'{timing.id}(({timing.label}\n{timing.type.decode}\n{timing.value}\n{timing.windowLower}..{timing.windowUpper}))\n')            
-          doc.asis(f'{timing.id} -->|from| {timing.relativeFromScheduledInstanceId}\n')      
-          doc.asis(f'{timing.id} -->|to| {timing.relativeToScheduledInstanceId}\n')      
-    with doc.tag('script', type='module'):
-      doc.asis("import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';\n")   
-      doc.asis("mermaid.initialize({ startOnLoad: true });\n")   
-
-  def _get_cross_reference(self, id):
-    for klass in [ScheduledActivityInstance, ScheduledDecisionInstance]:
-      instance = cross_references.get_by_id(klass, id)
-      if instance:
-        return instance 
-    return None
```

### Comparing `usdm-0.48.0/src/usdm_excel/id_manager.py` & `usdm-0.49.0/src/usdm_excel/id_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from usdm_excel.errors_and_logging.errors_and_logging import ErrorsAndLogging
+
 class IdManager():
 
-  def __init__(self):
-    self.id_index = {}
+  def __init__(self, errors_and_logging: ErrorsAndLogging):
+    self._errors_and_logging = errors_and_logging
+    self._id_index = {}
     self.clear()
 
   def clear(self):
-    self.id_index = {
+    self._id_index = {
       'Address': 0,
       'Code': 0,
       'AliasCode': 0,
       'Organization': 0,
       'StudyIdentifier': 0,
       'StudyEpoch': 0,
       'StudyArm': 0,
@@ -57,17 +60,17 @@
       'StudyCohort': 0,
       'StudyTitle': 0,
       'Masking': 0,
       'ResearchOrganization': 0,
       'StudySite': 0,
       'Condition': 0,
       'ParameterMap': 0,
-      'ConditionAssignment': 0
+      'ConditionAssignment': 0,
+      'Characteristic': 0
     }
 
   def build_id(self, klass):
     klass_name = klass if isinstance(klass, str) else str(klass.__name__)
-    self.id_index[klass_name] += 1
-    return "%s_%s" % (klass_name, self.id_index[klass_name])
+    self._id_index[klass_name] += 1
+    return f"{klass_name}_{self._id_index[klass_name]}"
 
-id_manager = IdManager()
```

### Comparing `usdm-0.48.0/src/usdm_excel/iso_3166.py` & `usdm-0.49.0/src/usdm_excel/iso_3166.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import os
-from usdm_excel.id_manager import id_manager
+from usdm_excel.globals import Globals
 from usdm_excel.code_base import CodeBase
 
 class ISO3166(CodeBase):
 
-  def __init__(self):
+  def __init__(self, globals: Globals):
+    super().__init__(globals)
     f = open(os.path.join(os.path.dirname(__file__), 'data', 'iso_3166.json'))
     self.db = json.load(f)
 
   def code(self, code):
     code, decode = self._get_decode(code)
     return self._build(code=code, system='ISO 3166 1 alpha3', version='2020-08', decode=decode)
```

### Comparing `usdm-0.48.0/src/usdm_excel/iso_8601_duration.py` & `usdm-0.49.0/src/usdm_excel/iso_8601_duration.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_excel/quantity_type.py` & `usdm-0.49.0/src/usdm_excel/quantity_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+import traceback
 import re
 from usdm_excel.cdisc_ct import CDISCCT
+from usdm_excel.globals import Globals
 
 class QuantityType():
 
-  def __init__(self, quantity_info, allow_missing_units=True, allow_empty=True):
+  def __init__(self, quantity_info: str, globals: Globals, allow_missing_units: bool=True, allow_empty: bool=True):
     try:
       self.value = None
       self.units = None
       self.units_code = None
       self.errors = []
       self.empty = False
       self.label = quantity_info.strip()
+ 
       if quantity_info:
         match = re.match(r"(?P<value>[+|-]*\d+)(\s*(?P<units>.+))?", self.label)
         if match :
           parts = match.groupdict()
           self.value = parts['value'].strip()
           if parts['units']:
             self.units = parts['units'].strip()
-            self.units_code = CDISCCT().code_for_unit(self.units)
+            self.units_code = CDISCCT(globals).code_for_unit(self.units)
             if not self.units_code:        
               self.errors.append(f"Unable to set the units code for the quantity '{quantity_info}'")
           elif allow_missing_units:
             pass
           else:
             self.errors.append(f"Could not decode the quantity value, possible typographical errors '{quantity_info}'")
         else:
```

### Comparing `usdm-0.48.0/src/usdm_excel/range_type.py` & `usdm-0.49.0/src/usdm_excel/range_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
+from usdm_excel.globals import Globals
 from usdm_excel.cdisc_ct import CDISCCT
 
 class RangeType():
 
-  def __init__(self, range_info, units_reqd=True, allow_empty=True):
+  def __init__(self, range_info: str, globals: Globals, units_reqd: bool=True, allow_empty: bool=True):
     try:
       self.upper = None
       self.lower = None
       self.units = None
       self.units_code = None
       self.errors = []
       self.empty = False
@@ -20,15 +21,15 @@
           if parts['upper']:
             self.upper = parts['upper'].strip()
           else:
             self.upper = self.lower
           if units_reqd:
             if parts['units']:
               self.units = parts['units'].strip()
-              self.units_code = CDISCCT().code_for_unit(self.units)
+              self.units_code = CDISCCT(globals).code_for_unit(self.units)
               if not self.units_code:        
                 self.errors.append(f"Unable to set the units code for the range '{range_info}'")
             else:
               self.errors.append(f"Could not decode the range value, possible typographical errors '{range_info}'")
         else:
           self.errors.append(f"Could not decode the range value '{range_info}'")
       elif not allow_empty:
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.id_manager import id_manager
 import traceback
-import pandas as pd
+from usdm_excel.base_sheet import BaseSheet
 from usdm_model.activity import Activity
+from usdm_excel.globals import Globals
 
 class StudyDesignActivitySheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignActivities'
+
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesignActivities', optional=True)
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME, optional=True)
       self.items = []
       if self.success:
         for index, row in self.sheet.iterrows():
           name = self.read_cell_by_name(index, ['activityName', 'name'])
           description = self.read_cell_by_name(index, ['activityDescription', 'description'])
           label = self.read_cell_by_name(index, 'label', default="", must_be_present=False)
           try:
             item = Activity(
-              id=id_manager.build_id(Activity), 
+              id=self.globals.id_manager.build_id(Activity), 
               name=name,
               description=description,
               label=label
             )
           except Exception as e:
-            self._general_error(f"Failed to create Activity object, exception {e}")
-            self._traceback(f"{traceback.format_exc()}")
+            self._general_exception(f"Failed to create Activity object", e)
           else:
             self.items.append(item)
-            cross_references.add(name, item)     
+            self.globals.cross_references.add(name, item)     
         self.double_link(self.items, 'previousId', 'nextId')   
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_amendment_sheet/study_design_amendment_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_amendment_sheet/study_design_amendment_sheet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
+import traceback
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.id_manager import id_manager
-from usdm_excel.cross_ref import cross_references
 from usdm_model.study_amendment import StudyAmendment
 from usdm_model.study_amendment_reason import StudyAmendmentReason
 from usdm_model.geographic_scope import SubjectEnrollment
 from usdm_model.quantity import Quantity
 from usdm_excel.cdisc_ct import CDISCCT
 from usdm_excel.iso_3166 import ISO3166
 from usdm_excel.alias import Alias
 from usdm_excel.quantity_type import QuantityType
-
-import traceback
+from usdm_excel.globals import Globals
 
 class StudyDesignAmendmentSheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyAmendments'
+  
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyAmendments', optional=True)
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME, optional=True)
       self.items = []
       if self.success:
         for index, row in self.sheet.iterrows():
           secondaries = []
           number = self.read_cell_by_name(index, 'number')
           summary = self.read_cell_by_name(index, 'summary')
           substantial = self.read_boolean_cell_by_name(index, 'substantialImpact')
@@ -34,88 +34,83 @@
               #print(f"SECONDARY: {amendment_reason}")
               secondaries.append(amendment_reason)
           enrollment = self._read_enrollment_cell(index)
           enrollments = self._enrollments(enrollment)
           #print(f"ENROLLMENT: {enrollment}")
           try:
             item = StudyAmendment(
-              id=id_manager.build_id(StudyAmendment), 
+              id=self.globals.id_manager.build_id(StudyAmendment), 
               number=number,
               summary=summary,
               substantialImpact=substantial,
               primaryReason=primary,
               secondaryReasons=secondaries,
               enrollments=enrollments
             )
           except Exception as e:
-            self._general_error(f"Failed to create StudyAmendment object, exception {e}")
-            self._traceback(f"{traceback.format_exc()}")
+            self._general_exception(f"Failed to create StudyAmendment object", e)
           else:
             self.items.append(item)
-            cross_references.add(item.number, item)
+            self.globals.cross_references.add(item.number, item)
         self.items.sort(key=lambda d: int(d.number))
         self.previous_link(self.items, 'previousId')
         
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
 
   def _enrollments(self, enrollments):
     results = []
     for enrollment in enrollments:
       try:
         #print(f"ENROLL: {enrollment}")
         item = SubjectEnrollment(
-          id=id_manager.build_id(SubjectEnrollment),
+          id=self.globals.id_manager.build_id(SubjectEnrollment),
           type=enrollment['type'],
           code=enrollment['code'],
           quantity=enrollment['quantity']
         )
       except Exception as e:
-        self._general_error(f"Failed to create SubjectEnrollment object, exception {e}")
-        self._traceback(f"{traceback.format_exc()}")
+        self._general_exception(f"Failed to create SubjectEnrollment object", e)
         return None
       else:
         results.append(item)
     return results
 
   def _amendment_reason(self, reason):
     #print(f"AR1: {reason}")
     try:
       item = StudyAmendmentReason(
-        id=id_manager.build_id(StudyAmendmentReason), 
+        id=self.globals.id_manager.build_id(StudyAmendmentReason), 
         code=reason['code'],
         otherReason=reason['other']
       )
     except Exception as e:
-      self._general_error(f"Failed to create StudyAmendmentReason object, exception {e}")
-      self._traceback(f"{traceback.format_exc()}")
-      print(f"AR2: {traceback.format_exc()}")
+      self._general_exception(f"Failed to create StudyAmendmentReason object", e)
       return None
     else:
       return item
     
   def _read_enrollment_cell(self, row_index):
     result = []
     col_index = self.sheet.columns.get_loc('enrollment')
     value = self.read_cell(row_index, col_index)
     #print(f"ENROL1: {value}")
     if value.strip() == "":
       self._error(row_index, col_index, "Empty cell detected where geographic enrollment values expected")
-      return [{'type': CDISCCT().code_for_attribute('GeographicScope', 'type', 'Global'), 'code': None, 'quantity': '0'}]
+      return [{'type': CDISCCT(self.globals).code_for_attribute('GeographicScope', 'type', 'Global'), 'code': None, 'quantity': '0'}]
     else:
       for item in self._state_split(value):
         #print(f"ENROL2: {item}")
         if item.strip().upper().startswith("GLOBAL"):
           # If we ever find global just return the one code
           text = item.strip()
           parts = text.split(":")
           if len(parts) == 2:
             quantity = self._get_quantitiy(parts[1].strip())
-            return [{'type': CDISCCT().code_for_attribute('GeographicScope', 'type', 'Global'), 'code': None, 'quantity': quantity}]
+            return [{'type': CDISCCT(self.globals).code_for_attribute('GeographicScope', 'type', 'Global'), 'code': None, 'quantity': quantity}]
           else:
             self._error(row_index, col_index, f"Failed to decode enrollment data {item}, no '=' detected")
           return 
         else: 
           code = None
           if item.strip():
             outer_parts = item.split(":")
@@ -124,35 +119,35 @@
               value = outer_parts[1].strip()
               name_value = value.split('=')
               if len(name_value) == 2:
                 #quantity = name_value[1].strip()
                 quantity = self._get_quantitiy(name_value[1].strip())
                 if system.upper() == "REGION":
                   pt = 'Region'
-                  code = ISO3166().region_code(value)
+                  code = ISO3166(self.globals).region_code(value)
                 elif system.upper() == "COUNTRY":
                   pt = 'Country'
-                  code = ISO3166().code(value)
+                  code = ISO3166(self.globals).code(value)
                 else:
                   self._error(row_index, col_index, f"Failed to decode geographic enrollment data {name_value}, must be either Region or Country using ISO3166 codes")
               else:
                 self._error(row_index, col_index, f"Failed to decode geographic enrollment data {name_value}, no '=' detected")
             else:
               self._error(row_index, col_index, f"Failed to decode geographic enrollment data {outer_parts}, no ':' detected")
           else:
             self._error(row_index, col_index, f"Failed to decode geographic enrollment data {item}, appears empty")
           if code:
-            result.append({'type': CDISCCT().code_for_attribute('GeographicScope', 'type', pt), 'code': Alias.code(code, []), 'quantity': quantity})
+            result.append({'type': CDISCCT(self.globals).code_for_attribute('GeographicScope', 'type', pt), 'code': Alias(self.globals).code(code, []), 'quantity': quantity})
       return result
 
   def _get_quantitiy(self, text):
     #print(f"QUANTITY1: {text}")
-    quantity = QuantityType(text, True, False)
-    unit = Alias.code(quantity.units_code, [])
-    #print(f"QUANTITY2: {quantity_details}")
+    quantity = QuantityType(text, self.globals, True, False)
+    unit = Alias(self.globals).code(quantity.units_code, [])
+    #print(f"QUANTITY2: {quantity} {quantity.units_code}")
     return self.create_object(Quantity, {'value': float(quantity.value), 'unit': unit})
 
   def _read_secondary_reason_cell(self, row_index):
     results = []
     col_index = self.sheet.columns.get_loc('secondaryReasons')
     value = self.read_cell(row_index, col_index)
     if not value.strip():
@@ -173,15 +168,15 @@
     if value.strip() == "":
       self._error(row_index, col_index, "Empty cell detected where CDISC CT value expected.")
       return None
     elif value.strip().upper().startswith('OTHER'):
       text = value.strip()
       parts = text.split("=")
       if len(parts) == 2:
-        return {'code': CDISCCT().code_for_attribute('StudyAmendmentReason', 'code', 'Other'), 'other': parts[1].strip()}
+        return {'code': CDISCCT(self.globals).code_for_attribute('StudyAmendmentReason', 'code', 'Other'), 'other': parts[1].strip()}
       else:
         self._error(row_index, col_index, f"Failed to decode reason data {text}, no '=' detected")
     else:
-      code = CDISCCT().code_for_attribute('StudyAmendmentReason', 'code', value)
+      code = CDISCCT(self.globals).code_for_attribute('StudyAmendmentReason', 'code', value)
       if code is None:
         self._error(row_index, col_index, f"CDISC CT not found for value '{value}'.")
       return {'code': code, 'other': None}
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,38 @@
+import traceback
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.id_manager import id_manager
 from usdm_model.study_arm import StudyArm
-import traceback
+from usdm_excel.globals import Globals
 
 class StudyDesignArmSheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignArms'
+  
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesignArms')
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME)
       self.items = []
       for index, row in self.sheet.iterrows():
         name = self.read_cell_by_name(index, ['studyArmName', 'name'])
         description = self.read_cell_by_name(index, ['studyArmDescription', 'description'])
         label = self.read_cell_by_name(index, 'label', default="", must_be_present=False)
         arm_type = self.read_cdisc_klass_attribute_cell_by_name('StudyArm', 'studyArmType', index, ['studyArmType', 'type'])
         arm_origin_description = self.read_cell_by_name(index, ['studyArmDataOriginDescription', 'dataOriginDescription'])
         arm_origin_type = self.read_cdisc_klass_attribute_cell_by_name('StudyArm', 'studyArmDataOriginType', index, ['studyArmDataOriginType', 'dataOriginType'])
         try:
           item = StudyArm(
-            id=id_manager.build_id(StudyArm), 
+            id=self.globals.id_manager.build_id(StudyArm), 
             name=name,
             description=description,
             label=label,
             type=arm_type,
             dataOriginDescription=arm_origin_description,
             dataOriginType=arm_origin_type
           )
         except Exception as e:
-          self._general_error(f"Failed to create StudyArm object, exception {e}")
-          self._traceback(f"{traceback.format_exc()}")
+          self._general_exception(f"Failed to create StudyArm object", e)
         else:
           self.items.append(item)
-          cross_references.add(name, item)     
+          self.globals.cross_references.add(name, item)     
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_conditions_sheet/study_design_conditions_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_conditions_sheet/study_design_conditions_sheet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import traceback
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.cross_ref import cross_references
 from usdm_model.condition import Condition
+from usdm_excel.globals import Globals
 
 class StudyDesignConditionSheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignConditions'
+
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesignConditions', optional=True)
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME, optional=True)
       self.items = []
       if self.success:
         for index, row in self.sheet.iterrows():
           name = self.read_cell_by_name(index, 'name')
           description = self.read_cell_by_name(index, 'description')
           label = self.read_cell_by_name(index, 'label')
           text = self.read_cell_by_name(index, 'text')
@@ -19,33 +21,33 @@
           context_refs = self._process_context_references(context, index)
           applies_to = self.read_cell_by_name(index, 'appliesTo')
           applies_refs = self._process_applies_to_references(applies_to, index)
           params = {'name': name, 'description': description, 'label': label, 'text': text, 'appliesToIds': applies_refs, 'contextIds': context_refs}
           item = self.create_object(Condition, params)
           if item:
             self.items.append(item)
-            cross_references.add(name, item)     
+            self.globals.cross_references.add(name, item)     
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
 
   def _process_context_references(self, references_list, index):
     return self._process_references(references_list, ['ScheduledActivityInstance', 'Activity'], index, 'context', False)
   
   def _process_applies_to_references(self, references_list, index):
     return self._process_references(references_list, ['Procedure', 'Activity', 'BiomedicalConcept', 'BiomedicalConceotCategory', 'BiomedicalConceptSurrogate'], index, 'appliesTo')
   
   def _process_references(self, references_list, klasses, index, column_name, references_required=True):
-    references = [x.strip() for x in references_list.split(',')]
+    references = [x.strip() for x in self._state_split(references_list)]
+    #references = [x.strip() for x in references_list.split(',')]
     results = []
     for reference in references:
       if reference:
         found = False
         for klass in klasses:
-          xref = cross_references.get(klass, reference)
+          xref = self.globals.cross_references.get(klass, reference)
           if xref:
             results.append(xref.id)
             found = True
             break
         if not found:
           self._error(index, self._get_column_index(column_name), f"Could not resolve condition reference '{reference}'")
     if not results and references_required:
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_content_sheet/study_design_content_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_content_sheet/study_design_content_sheet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+import traceback
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.id_manager import id_manager
-from usdm_excel.document.macros import Macros
 from usdm_model.narrative_content import NarrativeContent
-import traceback
+from usdm_excel.globals import Globals
+from usdm_excel.document.macros import Macros
 
 class StudyDesignContentSheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignContent'
+
+  def __init__(self, file_path: str, globals: Globals):
     try:
       self.items = []
-      super().__init__(file_path=file_path, sheet_name='studyDesignContent', optional=True, converters={"sectionName": str})
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME, optional=True, converters={"sectionName": str})
       if self.success:
         current_level = 0
         new_level = 0
         current_parent = []
         previous_item = NarrativeContent(
-          id=id_manager.build_id(NarrativeContent), 
+          id=self.globals.id_manager.build_id(NarrativeContent), 
           name="ROOT",
           sectionNumber="0",
           sectionTitle="Root",
           text="",
           childIds=[]
         )
         self.items.append(previous_item)
@@ -28,24 +30,23 @@
           new_level = self._get_level(section_number)
           title = self.read_cell_by_name(index, 'sectionTitle')
           text = self.read_cell_by_name(index, 'text')
           name = self.read_cell_by_name(index, 'name')
           name = f"SECTION {section_number}" if not name else name
           try:
             item = NarrativeContent(
-              id=id_manager.build_id(NarrativeContent), 
+              id=self.globals.id_manager.build_id(NarrativeContent), 
               name=name,
               sectionNumber=section_number,
               sectionTitle=title,
               text=self._wrap_div(text),
               childIds=[]
             )
           except Exception as e:  
-            self._general_error(f"Failed to create Content object, exception {e}")
-            self._traceback(f"{traceback.format_exc()}")
+            self._general_exception(f"Failed to create Content object", e)
           else:
             self.items.append(item)
             if new_level == current_level:
               # Same level
               parent = current_parent[-1]
               parent.childIds.append(item.id)
             elif new_level > current_level:
@@ -63,16 +64,15 @@
                 popped = current_parent.pop()
               parent = current_parent[-1]
               parent.childIds.append(item.id)
               current_level = new_level
             previous_item = item
           self.double_link(self.items, 'previousId', 'nextId')
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
 
   def resolve(self, study):
     macros = Macros(self, study)
     for item in self.items:
       item.text = macros.resolve(item.text)
 
   def _get_level(self, section_number):
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_dictionary_sheet/study_design_dictionary_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_dictionary_sheet/study_design_dictionary_sheet.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+import traceback
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.id_manager import id_manager
-from usdm_excel.cross_ref import cross_references
 from usdm_model.syntax_template_dictionary import SyntaxTemplateDictionary, ParameterMap
-
-import traceback
+from usdm_excel.globals import Globals
 
 class StudyDesignDictionarySheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'dictionaries'
+
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='dictionaries', optional=True)
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME, optional=True)
       self.items = []
       if self.success:
         current_name = None
         current_dictionary = None
         current_map = []
         for index, row in self.sheet.iterrows():
           name = self.read_cell_by_name(index, 'name')
@@ -29,15 +29,15 @@
           key = self.read_cell_by_name(index, 'key')
           klass = self.read_cell_by_name(index, 'class', default="")
           xref_name = self.read_cell_by_name(index, 'xref', default="")
           attribute_path = self.read_cell_by_name(index, ['attribute', 'path'], default="")
           value = self.read_cell_by_name(index, 'value', default="", must_be_present=False)
           if klass:
             try:
-              instance, attribute = cross_references.get_by_path(klass, xref_name, attribute_path)
+              instance, attribute = self.globals.cross_references.get_by_path(klass, xref_name, attribute_path)
             except Exception as e:
               instance = None
               col = self.column_present(['attribute', 'path'])
               self._error(index, col, str(e))
             if instance:
               map = self.create_object(ParameterMap, {'tag': key, 'reference': f'<usdm:ref klass="{instance.__class__.__name__}" id="{instance.id}" attribute="{attribute}"></usdm:ref>'})
               if map:
@@ -47,27 +47,25 @@
             if map:
               current_map.append(map)
         # Clean up last dictionary if present
         if current_dictionary:
           current_dictionary.parameterMaps = current_map
         
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
 
   def _dictionary(self, name, description, label):
     try:
       item = SyntaxTemplateDictionary(
-        id=id_manager.build_id(SyntaxTemplateDictionary), 
+        id=self.globals.id_manager.build_id(SyntaxTemplateDictionary), 
         name=name,
         description=description,
         label=label,
         parameterMaps=[]
       )
     except Exception as e:
-      self._general_error(f"Failed to create SyntaxTemplateDictionary object, exception {e}")
-      self._traceback(f"{traceback.format_exc()}")
+      self._general_exception(f"Failed to create SyntaxTemplateDictionary object", e)
       return None
     else:
       self.items.append(item)
-      cross_references.add(name, item)
+      self.globals.cross_references.add(name, item)
       return item
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,61 @@
-from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.id_manager import id_manager
 import traceback
 import pandas as pd
-from usdm_model.study_element import StudyElement
+from usdm_excel.base_sheet import BaseSheet
+from usdm_model.encounter import Encounter
 from usdm_model.transition_rule import TransitionRule
+from usdm_model.timing import Timing
+from usdm_excel.globals import Globals
 
-class StudyDesignElementSheet(BaseSheet):
+class StudyDesignEncounterSheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignEncounters'
+
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesignElements')
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME)
       self.items = []
       for index, row in self.sheet.iterrows():
         start_rule = None
         end_rule = None
-        xref = self.read_cell_by_name(index, 'xref', default="", must_be_present=False)
-        name = self.read_cell_by_name(index, ['studyElementName', 'name'])
-        description = self.read_cell_by_name(index, ['studyElementDescription', 'description'])
-        label = self.read_cell_by_name(index, 'label', default="", must_be_present=False)
+        xref = self.read_cell_by_name(index, 'xref', must_be_present=False)
+        name = self.read_cell_by_name(index, ['encounterName', 'name'])
+        description = self.read_cell_by_name(index, ['encounterDescription', 'description'])
+        label = self.read_cell_by_name(index, 'label', default='', must_be_present=False)
+        type = self.read_cdisc_klass_attribute_cell_by_name('Encounter', 'encounterType', index, ['encounterType', 'type'])
+        settings = self.read_cdisc_klass_attribute_cell_multiple_by_name('Encounter', 'encounterEnvironmentalSetting', index, ['encounterEnvironmentalSetting', 'environmentalSetting'])
+        modes = self.read_cdisc_klass_attribute_cell_multiple_by_name('Encounter', 'encounterContactModes', index, ['encounterContactModes', 'contactModes'])
         start_rule_text = self.read_cell_by_name(index, 'transitionStartRule')
         end_rule_text = self.read_cell_by_name(index, 'transitionEndRule')
+        timing_xref = self.read_cell_by_name(index, 'window', must_be_present=False)
         if start_rule_text:
-          start_rule = TransitionRule(id=id_manager.build_id(TransitionRule), name=f"ELEMENT_START_RULE_{index + 1}", text=start_rule_text)
+          start_rule = TransitionRule(id=self.globals.id_manager.build_id(TransitionRule), name=f"ENCOUNTER_START_RULE_{index + 1}", text=start_rule_text)
         if end_rule_text:
-          end_rule = TransitionRule(id=id_manager.build_id(TransitionRule), name=f"ELEMENT_END_RULE_{index + 1}", text=end_rule_text)
+          end_rule = TransitionRule(id=self.globals.id_manager.build_id(TransitionRule), name=f"ENCOUNTER_START_RULE_{index + 1}", text=end_rule_text)
+        if timing_xref:
+          timing = self.globals.cross_references.get(Timing, timing_xref)
+          timing_id = timing.id if timing else None
+        else:
+          timing_id = None
         try:
-          item = StudyElement(
-            id=id_manager.build_id(StudyElement), 
+          item = Encounter(
+            id=self.globals.id_manager.build_id(Encounter), 
             name=name,
             description=description,
             label=label,
+            type=type, 
+            environmentalSetting=settings,
+            contactModes=modes,
             transitionStartRule=start_rule,
-            transitionEndRule=end_rule
+            transitionEndRule=end_rule,
+            scheduledAtId=timing_id
           )
         except Exception as e:
-          self._general_error(f"Failed to create StudyElement object, exception {e}")
-          self._traceback(f"{traceback.format_exc()}")
+          self._general_exception(f"Failed to create Encounter object", e)
         else:
           self.items.append(item)
           cross_ref = xref if xref else name
-          cross_references.add(cross_ref, item)     
+          self.globals.cross_references.add(cross_ref, item)     
+      self.double_link(self.items, 'previousId', 'nextId')   
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_eligibility_criteria_sheet/study_design_eligibility_criteria_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,72 @@
-from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.id_manager import id_manager
-from usdm_excel.cross_ref import cross_references
-from usdm_model.eligibility_criterion import EligibilityCriterion
+from usdm_excel.globals import Globals
+from usdm_excel.syntax_template_sheet import SyntaxTemplateSheet
+from usdm_model.objective import Objective
+from usdm_model.endpoint import Endpoint
 from usdm_model.syntax_template_dictionary import SyntaxTemplateDictionary
+from usdm_excel.globals import Globals
 
-import traceback
-import re
+class StudyDesignObjectiveEndpointSheet(SyntaxTemplateSheet):
 
-class StudyDesignEligibilityCriteriaSheet(BaseSheet):
-
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignOE'
+  
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesignEligibilityCriteria', optional=True)
-      self.items = []
-      if self.success:
-        for index, row in self.sheet.iterrows():
-          category = self.read_cdisc_klass_attribute_cell_by_name('EligibilityCriteria', 'category', index, 'category')
-          identifier = self.read_cell_by_name(index, 'identifier')
-          name = self.read_cell_by_name(index, 'name')
-          description = self.read_cell_by_name(index, 'description')
-          label = self.read_cell_by_name(index, 'label')
-          text = self.read_cell_by_name(index, 'text')
-          dictionary_name = self.read_cell_by_name(index, 'dictionary')
-          self._validate_references(index, 'text', text, dictionary_name)
-          criteria = self._criteria(name, description, label, text, category, identifier, dictionary_name)
-          if criteria:
-            self.items.append(criteria)
-        
-    except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME)
+      self.objectives = []
+      current = None
+      for index, row in self.sheet.iterrows():
+        o_text = self.read_cell_by_name(index, 'objectiveText') 
+        ep_name = self.read_cell_by_name(index, ['endpointXref', 'endpointName'])
+        ep_description = self.read_cell_by_name(index, 'endpointDescription')
+        ep_label = self.read_cell_by_name(index, ["endpointLabel"], must_be_present=False) 
+        ep_text = self.read_cell_by_name(index, 'endpointText') 
+        ep_purpose = self.read_cell_by_name(index, ['endpointPurposeDescription', 'endpointPurpose'], default='None provided')
+        ep_level = self.read_cdisc_klass_attribute_cell_by_name('Endpoint', 'endpointLevel', index, "endpointLevel")
+        ep_dictionary_name = self.read_cell_by_name(index, 'endpointDictionary', must_be_present=False)
+        self._validate_references(index, 'endpointText', ep_text, ep_dictionary_name)
 
-  def _criteria(self, name, description, label, text, category, identifier, dictionary_name):
-    try:
-      dictionary_id = self._get_dictionary_id(dictionary_name)
-      item = EligibilityCriterion(
-        id=id_manager.build_id(EligibilityCriterion),
-        name=name,
-        description=description,
-        label=label,
-        text=text,
-        category=category,
-        identifier=identifier,
-        dictionaryId=dictionary_id
-      )
-    except Exception as e:
-      self._general_error(f"Failed to create EligibilityCriteria object, exception {e}")
-      self._traceback(f"{traceback.format_exc()}")
-      return None
-    else:
-      cross_references.add(item.id, item)
-      return item
+        if o_text:
+          o_name = self.read_cell_by_name(index, ["objectiveXref", "objectiveName"]) 
+          o_description = self.read_cell_by_name(index, 'objectiveDescription')
+          o_label = self.read_cell_by_name(index, ["objectiveLabel"], must_be_present=False) 
+          o_level = self.read_cdisc_klass_attribute_cell_by_name('Objective', 'objectiveLevel', index, "objectiveLevel")
+          o_dictionary_name = self.read_cell_by_name(index, 'objectiveDictionary', must_be_present=False)
+          self._validate_references(index, 'objectiveText', o_text, o_dictionary_name)
+          try:
+            dictionary_id = self._get_dictionary_id(o_dictionary_name)
+            current = Objective(id=self.globals.id_manager.build_id(Objective),
+              name=o_name,
+              description=o_description, 
+              label=o_label,
+              text=o_text,
+              level=o_level,
+              endpoints=[],
+              dictionaryId=dictionary_id
+            )
+          except Exception as e:
+            self._general_error(f"Failed to create Objective object", e)
+          else:
+            self.objectives.append(current)
+            self.globals.cross_references.add(o_name, current)
+        if current is not None:
+          try:
+            dictionary_id = self._get_dictionary_id(ep_dictionary_name)
+            ep = Endpoint(id=self.globals.id_manager.build_id(Endpoint),
+              name=ep_name,
+              description=ep_description,
+              label=ep_label,
+              text=ep_text, 
+              purpose=ep_purpose, 
+              level=ep_level,
+              dictionaryId=dictionary_id
+            )  
+          except Exception as e:
+            self._general_error(f"Failed to create Endpoint object", e)
+          else:
+            current.endpoints.append(ep)
+            self.globals.cross_references.add(ep_name, ep)
+        else:
+          self._general_error("Failed to add Endpoint, no Objective set")
 
-  def _validate_references(self, row, column_name, text, dictionary_name):
-    if dictionary_name:
-      column = self.column_present(column_name)
-      dictionary = cross_references.get(SyntaxTemplateDictionary, dictionary_name)
-      if not dictionary:
-        self._warning(row, column, f"Dictionary '{dictionary_name}' not found")
-        return
-      tags = re.findall(r'\[([^]]*)\]',text)
-      for tag in tags:
-        entry = next((item for item in dictionary.parameterMaps if item.tag == tag), None)
-        if not entry:
-        #if not tag in dictionary.parameterMap:
-          self._warning(row, column, f"Failed to find '{tag}' in dictionary '{dictionary_name}'")
-  
-  def _get_dictionary_id(self, dictionary_name):
-    if dictionary_name:
-      dictionary = cross_references.get(SyntaxTemplateDictionary, dictionary_name)
-      if dictionary:
-        return dictionary.id
-      else:
-        self._general_error(f"Unable to find dictionary with name '{dictionary_name}'")
-    return None
+    except Exception as e:
+      self._sheet_exception(e)
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,37 @@
-from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.id_manager import id_manager
 import traceback
-import pandas as pd
-from usdm_model.encounter import Encounter
-from usdm_model.transition_rule import TransitionRule
-from usdm_model.timing import Timing
+from usdm_model.organization import Organization
+from usdm_model.study_identifier import StudyIdentifier
+from usdm_excel.base_sheet import BaseSheet
+from usdm_excel.globals import Globals
 
-class StudyDesignEncounterSheet(BaseSheet):
 
-  def __init__(self, file_path):
+class StudyIdentifiersSheet(BaseSheet):
+
+  SHEET_NAME = 'studyIdentifiers'
+  
+  def __init__(self, file_path, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesignEncounters')
-      self.items = []
-      for index, row in self.sheet.iterrows():
-        start_rule = None
-        end_rule = None
-        xref = self.read_cell_by_name(index, 'xref', must_be_present=False)
-        name = self.read_cell_by_name(index, ['encounterName', 'name'])
-        description = self.read_cell_by_name(index, ['encounterDescription', 'description'])
-        label = self.read_cell_by_name(index, 'label', default='', must_be_present=False)
-        type = self.read_cdisc_klass_attribute_cell_by_name('Encounter', 'encounterType', index, ['encounterType', 'type'])
-        settings = self.read_cdisc_klass_attribute_cell_multiple_by_name('Encounter', 'encounterEnvironmentalSetting', index, ['encounterEnvironmentalSetting', 'environmentalSetting'])
-        modes = self.read_cdisc_klass_attribute_cell_multiple_by_name('Encounter', 'encounterContactModes', index, ['encounterContactModes', 'contactModes'])
-        start_rule_text = self.read_cell_by_name(index, 'transitionStartRule')
-        end_rule_text = self.read_cell_by_name(index, 'transitionEndRule')
-        timing_xref = self.read_cell_by_name(index, 'window', must_be_present=False)
-        if start_rule_text:
-          start_rule = TransitionRule(id=id_manager.build_id(TransitionRule), name=f"ENCOUNTER_START_RULE_{index + 1}", text=start_rule_text)
-        if end_rule_text:
-          end_rule = TransitionRule(id=id_manager.build_id(TransitionRule), name=f"ENCOUNTER_START_RULE_{index + 1}", text=end_rule_text)
-        if timing_xref:
-          timing = cross_references.get(Timing, timing_xref)
-          timing_id = timing.id if timing else None
-        else:
-          timing_id = None
-        try:
-          item = Encounter(
-            id=id_manager.build_id(Encounter), 
-            name=name,
-            description=description,
-            label=label,
-            type=type, 
-            environmentalSetting=settings,
-            contactModes=modes,
-            transitionStartRule=start_rule,
-            transitionEndRule=end_rule,
-            scheduledAtId=timing_id
-          )
-        except Exception as e:
-          self._general_error(f"Failed to create Encounter object, exception {e}")
-          self._traceback(f"{traceback.format_exc()}")
-        else:
-          self.items.append(item)
-          cross_ref = xref if xref else name
-          cross_references.add(cross_ref, item)     
-      self.double_link(self.items, 'previousId', 'nextId')   
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME)
+      self.identifiers = []
+      self.process_sheet()
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
-
+      self._sheet_exception(e)
+      
+  def process_sheet(self):
+    self.identifiers = []
+    for index, row in self.sheet.iterrows():
+      org_type = self.read_cdisc_klass_attribute_cell_by_name('Organization', 'organizationType', index, ['organisationType', 'organizationType', 'type'])     
+      org_id_scheme = self.read_cell_by_name(index, ['organisationIdentifierScheme', 'organizationIdentifierScheme', 'identifierScheme'])
+      org_identifier = self.read_cell_by_name(index, ['organisationIdentifier', 'organizationIdentifier'])
+      org_name = self.read_cell_by_name(index, ['organisationName', 'organizationName', 'name'])
+      org_label = self.read_cell_by_name(index, 'label', default="", must_be_present=False)
+      org_address = self.read_address_cell_by_name(index, ['organisationAddress', 'organizationAddress', 'address'])
+      if org_address:
+        self.globals.cross_references.add(org_address.id, org_address)   
+      organisation = self.create_object(Organization, {'identifierScheme': org_id_scheme, 'identifier': org_identifier, 'name': org_name, 'label': org_label, 'organizationType': org_type, 'legalAddress': org_address})
+      if organisation:
+        self.globals.cross_references.add(organisation.id, organisation)   
+        item = self.create_object(StudyIdentifier, {'studyIdentifier': self.read_cell_by_name(index, 'studyIdentifier'), 'studyIdentifierScope': organisation})
+        if item:
+          self.identifiers.append(item)
+          self.globals.cross_references.add(item.studyIdentifier, item)
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,33 @@
+import traceback
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.id_manager import id_manager
 from usdm_model.study_epoch import StudyEpoch
-import traceback
+from usdm_excel.globals import Globals
 
 class StudyDesignEpochSheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignEpochs'
+  
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesignEpochs')
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME)
       self.items = []
       for index, row in self.sheet.iterrows():
         name = self.read_cell_by_name(index, ['studyEpochName', 'name'])
         description = self.read_cell_by_name(index, ['studyEpochDescription', 'description'])
         label = self.read_cell_by_name(index, 'label', default="", must_be_present=False)
         epoch_type = self.read_cdisc_klass_attribute_cell_by_name('StudyEpoch', 'studyEpochType', index, ['studyEpochType', 'type'])
         try:
           item = StudyEpoch(
-            id=id_manager.build_id(StudyEpoch), 
+            id=self.globals.id_manager.build_id(StudyEpoch), 
             name=name, 
             description=description,
             label=label,
             type=epoch_type
           )
         except Exception as e:
-          self._general_error(f"Failed to create StudyEpoch object, exception {e}")
-          self._traceback(f"{traceback.format_exc()}")
+          self._general_exception(f"Failed to create StudyEpoch object", e)
         else:
           self.items.append(item)
-          cross_references.add(name, item)     
+          self.globals.cross_references.add(name, item)     
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.id_manager import id_manager
+#from usdm_excel.cross_ref import cross_references
+#from usdm_excel.id_manager import id_manager
 import traceback
 from usdm_model.intercurrent_event import IntercurrentEvent
 from usdm_model.analysis_population import AnalysisPopulation
 from usdm_model.estimand import Estimand
 from usdm_model.study_intervention import StudyIntervention
 from usdm_model.endpoint import Endpoint
+from usdm_excel.globals import Globals
 
 class StudyDesignEstimandsSheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignEstimands'
+  
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesignEstimands')
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME)
       self.estimands = []
       current = None
       current_ice_name = None
       current_ice_description = None
       for index, row in self.sheet.iterrows():
         e_summary = self.read_cell_by_name(index, "summaryMeasure")
         ap_description = self.read_cell_by_name(index, 'populationDescription')
@@ -24,46 +27,41 @@
         ice_description = self.read_cell_by_name(index, ['intercurrentEventDescription', 'description'])
         ice_label = self.read_cell_by_name(index, 'label', must_be_present=False)
         ice_strategy = self.read_cell_by_name(index, "intercurrentEventStrategy")
         treatment_xref = self.read_cell_by_name(index, "treatmentXref")
         endpoint_xref = self.read_cell_by_name(index, "endpointXref")
         if not e_summary == "":
           try:
-            ap = AnalysisPopulation(id=id_manager.build_id(AnalysisPopulation), name=f"AP_{index+1}", text=ap_description) 
+            ap = AnalysisPopulation(id=self.globals.id_manager.build_id(AnalysisPopulation), name=f"AP_{index+1}", text=ap_description) 
           except Exception as e:
-            self._general_error(f"Failed to create AnalysisPopulation object, exception {e}")
-            self._traceback(f"{traceback.format_exc()}")
+            self._general_error(f"Failed to create AnalysisPopulation object", e)
           else:
             try:
               treatment_id = self._get_treatment(treatment_xref)
               endpoint_id = self._get_endpoint(endpoint_xref)
-              current = Estimand(id=id_manager.build_id(Estimand), summaryMeasure=e_summary, analysisPopulation=ap, interventionId=treatment_id, variableOfInterestId=endpoint_id, intercurrentEvents=[])
+              current = Estimand(id=self.globals.id_manager.build_id(Estimand), summaryMeasure=e_summary, analysisPopulation=ap, interventionId=treatment_id, variableOfInterestId=endpoint_id, intercurrentEvents=[])
             except Exception as e:
-              self._general_error(f"Failed to create Estimand object, exception {e}")
-              self._traceback(f"{traceback.format_exc()}")
+              self._general_error(f"Failed to create Estimand object", e)
             else:
               self.estimands.append(current)  
         if current is not None:
           try:
             ice_name = current_ice_name if ice_name == "" else ice_name
             ice_description = current_ice_description if ice_description == "" else ice_description
-            ice = IntercurrentEvent(id=id_manager.build_id(IntercurrentEvent), name=ice_name, description=ice_description, label=ice_label, strategy=ice_strategy)
+            ice = IntercurrentEvent(id=self.globals.id_manager.build_id(IntercurrentEvent), name=ice_name, description=ice_description, label=ice_label, strategy=ice_strategy)
             current_ice_name = ice_name
             current_ice_description = ice_description
           except Exception as e:
-            self._general_error(f"Failed to create IntercurrentEvent object, exception {e}")
-            self._traceback(f"{traceback.format_exc()}")
+            self._general_error(f"Failed to create IntercurrentEvent object", e)
           else:
             current.intercurrentEvents.append(ice)
         else:
           self._general_error("Failed to add IntercurrentEvent, no Estimand set")
-          self._traceback(f"{traceback.format_exc()}")
 
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
 
   def _get_treatment(self, name):
     return self._get_cross_reference(StudyIntervention, name, 'study intervention')
 
   def _get_endpoint(self, name):
     return self._get_cross_reference(Endpoint, name, 'endpoint')
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_indication_sheet/study_design_indication_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_indication_sheet/study_design_indication_sheet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,26 @@
+import traceback
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.id_manager import id_manager
 from usdm_model.indication import Indication
-
-import traceback
+from usdm_excel.globals import Globals
 
 class StudyDesignIndicationSheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignIndications'
+  
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesignIndications')
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME )
       self.items = []
       for index, row in self.sheet.iterrows():
         name = self.read_cell_by_name(index, "name")
         description = self.read_cell_by_name(index, "description")
         label = self.read_cell_by_name(index, 'label', default="")
         rare = self.read_boolean_cell_by_name(index, 'isRareDisease', must_be_present=False)
         codes = self.read_other_code_cell_multiple_by_name(index, "codes")
         item = self.create_object(Indication, {'name': name, 'description': description, 'label': label, 'isRareDisease': rare, 'codes': codes})
         if item:
           self.items.append(item)
-          cross_references.add(name, item)
+          self.globals.cross_references.add(name, item)
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_intervention_sheet/study_design_intervention_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_intervention_sheet/study_design_intervention_sheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
+import traceback
 from usdm_excel.base_sheet import BaseSheet
 from usdm_excel.alias import Alias
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.id_manager import id_manager
-import traceback
-
 from usdm_model.study_intervention import StudyIntervention
 from usdm_model.agent_administration import AgentAdministration
 from usdm_model.administration_duration import AdministrationDuration
+from usdm_excel.globals import Globals
 
 class StudyDesignInterventionSheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignInterventions'
+
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesignInterventions')
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME)
       self.items = []
       self.current_name = None
       self.current_intervention = None
       for index, row in self.sheet.iterrows():
         # Read the adminstrations and durations
         admin_duration = self._create_administration_duration(index)
         agent_admin = self._create_agent_administration(index, admin_duration)
         # Read intervention in present
         self._create_intervention(index, agent_admin)
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
 
   def _create_intervention(self, index, agent_admin):
     name = self.read_cell_by_name(index, 'name')
     if name and name != self.current_name:
       self.current_name = name
       description = self.read_cell_by_name(index, 'description', must_be_present=False)
       label = self.read_cell_by_name(index, 'label', must_be_present=False)
@@ -41,76 +40,73 @@
       self.current_intervention = self._intervention(name, description, label, role, codes, type, pharm_class, product_designation, min_duration, agent_admin)
     else:
       self.current_intervention.administrations.append(agent_admin)
 
   def _intervention(self, name, description, label, role, codes, type, pharm_class, product_designation, minimum_duration, agent_administration):
     try:
       item = StudyIntervention(
-        id=id_manager.build_id(StudyIntervention), 
+        id=self.globals.id_manager.build_id(StudyIntervention), 
         name=name, 
         description=description, 
         label=label,
         role=role,
         type=type,
         minimumResponseDuration=minimum_duration,
         codes=codes,
         productDesignation=product_designation,
         pharmacologicClass=pharm_class,
         administrations=[agent_administration]
       )
     except Exception as e:
-      self._general_error(f"Failed to create StudyIntervention object, exception {e}")
-      self._traceback(f"{traceback.format_exc()}")
+      self._general_error(f"Failed to create StudyIntervention object", e)
     else:
       self.items.append(item)
-      cross_references.add(name, item)
+      self.globals.cross_references.add(name, item)
       return item    
 
   def _create_agent_administration(self, index, admin_duration):
     name = self.read_cell_by_name(index, 'administrationName')
     descriptiopn = self.read_cell_by_name(index, 'administrationDescription', must_be_present=False)
     label = self.read_cell_by_name(index, 'administrationLabel', must_be_present=False)
     route = self.read_cdisc_klass_attribute_cell_by_name("AgentAdministration", "route", index, "administrationRoute")
     dose = self.read_quantity_cell_by_name(index, "administrationDose")
     frequency = self.read_cdisc_klass_attribute_cell_by_name("AgentAdministration", "frequency", index, "administrationFrequency")
     return self._agent_administration(name, descriptiopn, label, route, dose, frequency, admin_duration)
 
   def _agent_administration(self, name, description, label, route, dose, frequency, admin_duration):
     try:
       item = AgentAdministration(
-        id=id_manager.build_id(AgentAdministration), 
+        id=self.globals.id_manager.build_id(AgentAdministration), 
         name=name, 
         description=description, 
         label=label,
         duration=admin_duration,
         dose=dose,
-        route=Alias.code(route, []),
-        frequency=Alias.code(frequency, [])
+        route=Alias(self.globals).code(route, []),
+        frequency=Alias(self.globals).code(frequency, [])
       )
     except Exception as e:
-      self._general_error(f"Failed to create AgentAdministration object, exception {e}")
-      self._traceback(f"{traceback.format_exc()}")
+      self._general_error(f"Failed to create AgentAdministration object", e)
     else:
-      cross_references.add(name, item)
+      self.globals.cross_references.add(name, item)
       return item
 
   def _create_administration_duration(self, index):
     description = self.read_cell_by_name(index, 'administrationDurationDescription', must_be_present=False)
     will_vary = self.read_boolean_cell_by_name(index, 'administrationDurationWillVary')
     will_vary_reason = self.read_cell_by_name(index, 'administrationDurationWillVaryReason')
     quantity = self.read_quantity_cell_by_name(index, 'administrationDurationQuantity')
     return self._administration_duration(description, will_vary, will_vary_reason, quantity)
 
   def _administration_duration(self, description, will_vary, will_vary_reason, quantity):
     try:
       item = AdministrationDuration(
-        id=id_manager.build_id(AdministrationDuration), 
+        id=self.globals.id_manager.build_id(AdministrationDuration), 
         description=description,
         durationWillVary=will_vary,
         reasonDurationWillVary=will_vary_reason,
         quantity=quantity
       )
     except Exception as e:
-      self._general_error(f"Failed to create AdministrationDuration object, exception {e}")
-      self._traceback(f"{traceback.format_exc()}")
+      self._general_error(f"Failed to create AdministrationDuration object", e)
     else:
       return item
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,85 @@
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.id_manager import id_manager
-from usdm_excel.cross_ref import cross_references
-import traceback
 from usdm_model.population_definition import StudyDesignPopulation, StudyCohort
 from usdm_model.range import Range
+from usdm_model.characteristic import Characteristic
+from usdm_excel.globals import Globals
 
 class StudyDesignPopulationSheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignPopulations'
+  
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesignPopulations')
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME)
       self.population = None
-      cohorts = []
+      self._cohorts = []
       for index, row in self.sheet.iterrows():
         level = self.read_cell_by_name(index, 'level')
         name = self.read_cell_by_name(index, 'name')
         description = self.read_cell_by_name(index, 'description')
         label = self.read_cell_by_name(index, 'label')
         required_number = self.read_range_cell_by_name(index, "plannedCompletionNumber", require_units=False, allow_empty=True)
         recruit_number = self.read_range_cell_by_name(index, "plannedEnrollmentNumber", require_units=False, allow_empty=True)
         planned_age = self.read_range_cell_by_name(index, "plannedAge", require_units=True, allow_empty=True)
         healthy = self.read_boolean_cell_by_name(index, 'includesHealthySubjects', must_be_present=False)
+        characteristics = self.read_cell_multiple_by_name(index, 'characteristics', must_be_present=False)
         codes = self._build_codes(row, index)
         if level.upper() == "MAIN":
           self.population = self._study_population(name, description, label, recruit_number, required_number, planned_age, healthy, codes)
         else:
-          cohort = self._study_cohort(name, description, label, recruit_number, required_number, planned_age, healthy, codes)
-          cohorts.append(cohort)
+          cohort = self._study_cohort(name, description, label, recruit_number, required_number, planned_age, healthy, codes, characteristics)
       if self.population: 
-        self.population.cohorts = cohorts
+        self.population.cohorts = self._cohorts
       else:
         self._general_error(f"Not main study population detected")
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet")
-      #print(f"{traceback.format_exc()}")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
 
   def _build_codes(self, row, index):
     code = self.read_cdisc_klass_attribute_cell_by_name('StudyDesignPopulation', "plannedSexOfParticipants", index, "plannedSexOfParticipants", allow_empty=True)
     return [code] if code else []
 
-  def _study_population(self, name, description, label, recruit_number, required_number, planned_age, healthy, codes):    
-    try:
-      item = StudyDesignPopulation(id=id_manager.build_id(StudyDesignPopulation),
-        name=name,
-        description=description,
-        label=label,
-        includesHealthySubjects=healthy,
-        plannedEnrollmentNumber=recruit_number,
-        plannedCompletionNumber=required_number,
-        plannedAge=planned_age,
-        plannedSex=codes
-      )
-    except Exception as e:
-      self._general_error(f"Failed to create StudyDesignPopulation object, exception {e}")
-      self._traceback(f"{traceback.format_exc()}")
-      return None
-    else:
-      cross_references.add(name, item)
-      return item
+  def _study_population(self, name: str, description: str, label: str, recruit_number: Range, required_number: Range, planned_age: Range, healthy: bool, codes: list) -> StudyDesignPopulation:    
+    params = {
+      'name': name,
+      'description': description,
+      'label': label,
+      'includesHealthySubjects': healthy,
+      'plannedEnrollmentNumber': recruit_number,
+      'plannedCompletionNumber': required_number,
+      'plannedAge': planned_age,
+      'plannedSex': codes
+    }
+    item = self.create_object(StudyDesignPopulation, params)
+    if item:
+      self.globals.cross_references.add(name, item)
+    return item
 
-  def _study_cohort(self, name, description, label, recruit_number, required_number, planned_age, healthy, codes):    
-    try:
-      item = StudyCohort(id=id_manager.build_id(StudyCohort),
-        name=name,
-        description=description,
-        label=label,
-        includesHealthySubjects=healthy,
-        plannedEnrollmentNumber=recruit_number,
-        plannedCompletionNumber=required_number,
-        plannedAge=planned_age,
-        plannedSex=codes,
-        characteristics=[]
-      )
-    except Exception as e:
-      self._general_error(f"Failed to create StudyCohort object, exception {e}")
-      #print(f"{traceback.format_exc()}")
-      self._traceback(f"{traceback.format_exc()}")
-      return None
-    else:
-      cross_references.add(name, item)
-      return item
+  def _study_cohort(self, name: str, description: str, label: str, recruit_number: Range, required_number: Range, planned_age: Range, healthy: bool, codes: list, characteristics: list) -> StudyCohort:    
+    characteristic_refs = self._resolve_characteristics(characteristics)
+    params = {  
+      'name': name,
+      'description': description,
+      'label': label,
+      'includesHealthySubjects': healthy,
+      'plannedEnrollmentNumber': recruit_number,
+      'plannedCompletionNumber': required_number,
+      'plannedAge': planned_age,
+      'plannedSex': codes,
+      'characteristics': characteristic_refs
+    }
+    item = self.create_object(StudyCohort, params)
+    if item:
+      self.globals.cross_references.add(name, item)
+      self._cohorts.append(item)
+    return item
+      
+  def _resolve_characteristics(self, names):
+    results = []
+    for name in names:
+      object = self.globals.cross_references.get(Characteristic, name)
+      if object:
+        results.append(object)
+      else:
+        self._general_warning(f"Characterisitc '{name}' not found")
+    return results
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.id_manager import id_manager
 import traceback
 import pandas as pd
+from usdm_excel.base_sheet import BaseSheet
 from usdm_model.procedure import Procedure
+from usdm_excel.globals import Globals
 
 class StudyDesignProcedureSheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignProcedures'
+  
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesignProcedures')
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME)
       self.procedures = []
       for index, row in self.sheet.iterrows():
         xref = self.read_cell_by_name(index, "xref", default="", must_be_present=False)
         name = self.read_cell_by_name(index, ["procedureName", 'name'])
         description = self.read_cell_by_name(index, ['procedureDescription', 'description'])
         label = self.read_cell_by_name(index, 'label', default="", must_be_present=False)
         type = self.read_cell_by_name(index, "procedureType")
         code = self.read_other_code_cell_by_name(index, ['procedureCode', 'code'])
-        #conditional = self.read_boolean_cell_by_name(index, 'procedureIsConditional')
-        #reason = self.read_cell_by_name(index, 'procedureIsConditionalReason')
         try:
-          item = Procedure(id=id_manager.build_id(Procedure),
+          item = Procedure(id=self.globals.id_manager.build_id(Procedure),
             name=name,
             description=description,
             label=label,
             procedureType=type, 
             code=code 
-            #isConditional=conditional, 
-            #isConditionalReason=reason
           )
         except Exception as e:
-          self._general_error(f"Failed to create Procedure object, exception {e}")
-          self._traceback(f"{traceback.format_exc()}")
+          self._general_exception(f"Failed to create Procedure object", e)
         else:
           self.procedures.append(item)
           cross_ref = xref if xref else name
-          cross_references.add(cross_ref, item)        
+          self.globals.cross_references.add(cross_ref, item)        
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_sheet/study_design_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_sheet/study_design_sheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
+import traceback
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.id_manager import id_manager
-from usdm_excel.cross_ref import cross_references
 from usdm_model.study_epoch import StudyEpoch
 from usdm_model.study_arm import StudyArm
 from usdm_model.study_element import StudyElement
 from usdm_model.study_cell import StudyCell
 from usdm_model.study_design import StudyDesign
 from usdm_model.masking import Masking
 from usdm_excel.alias import Alias
 from usdm_excel.option_manager import *
 from usdm_excel.cdisc_ct import CDISCCT
-import traceback
+from usdm_excel.globals import Globals
 
 class StudyDesignSheet(BaseSheet):
 
-#      'EPOCH_ARMS_START_LABEL =
+  SHEET_NAME = 'studyDesign'
+  
   NAME_LABEL = ['studyDesignName', 'name']
   DESCRIPTION_LABEL = ['studyDesignDescription', 'description']
   LABEL_LABEL = ['label']
   TA_LABEL = ['therapeuticAreas']
   RATIONALE_LABEL = ['studyDesignRationale']
   BLINDING_LABEL = ['studyDesignBlindingScheme']
   INTENT_LABEL = ['trialIntentTypes']
@@ -28,17 +28,17 @@
   OTHER_TIMELINES_LABEL = ['otherTimelines']
   MASKING_ROLE_LABEL = ['masking']
   CHARACTERISTICS_LABEL = ['characteristics']
 
   PARAMS_NAME_COL = 0
   PARAMS_DATA_COL = 1
 
-  def __init__(self, file_path):
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesign', header=None)
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME, header=None)
       self.name = "TEST"
       self.description = "An Microsoft Excel test study design"
       self.label=""
       self.epochs = []
       self.epoch_names = {}
       self.arms = []
       self.arm_names = {}
@@ -53,16 +53,15 @@
       self.trial_types = []
       self.intervention_model = None
       self.main_timeline = None
       self.other_timelines = []
       self.masks = []
       self.process_sheet()
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
 
   def process_sheet(self):
     general_params = True
     resolved_epochs = [None] * self.sheet.shape[1] 
     resolved_arms = [None] * self.sheet.shape[0] 
     for rindex, row in self.sheet.iterrows():
       key = self.read_cell(rindex, self.PARAMS_NAME_COL)
@@ -75,15 +74,15 @@
         elif key in self.DESCRIPTION_LABEL:
           self.description = self.read_cell(rindex, self.PARAMS_DATA_COL)
         elif key in self.TA_LABEL:
           self.therapeutic_areas = self.read_other_code_cell_mutiple(rindex, self.PARAMS_DATA_COL)
         elif key in self.RATIONALE_LABEL:
           self.rationale = self.read_cell(rindex, self.PARAMS_DATA_COL)
         elif key in self.BLINDING_LABEL:
-          self.blinding = Alias.code(self.read_cdisc_klass_attribute_cell('StudyDesign', 'studyDesignBlindingScheme',rindex, self.PARAMS_DATA_COL), [])
+          self.blinding = Alias(self.globals).code(self.read_cdisc_klass_attribute_cell('StudyDesign', 'studyDesignBlindingScheme',rindex, self.PARAMS_DATA_COL), [])
         elif key in self.INTENT_LABEL:
           self.trial_intents = self.read_cdisc_klass_attribute_cell_multiple('StudyDesign', 'trialIntentType', rindex, self.PARAMS_DATA_COL)
         elif key in self.CHARACTERISTICS_LABEL:
           self.characteristics = self.read_cdisc_klass_attribute_cell_multiple('StudyDesign', 'characteristics', rindex, self.PARAMS_DATA_COL)
           #print(f"CHARAC: {self.characteristics}")
         elif key in self.TYPES_LABEL:
           self.trial_types = self.read_cdisc_klass_attribute_cell_multiple('StudyDesign', 'trialType', rindex, self.PARAMS_DATA_COL)
@@ -130,62 +129,61 @@
                 
       self.double_link(self.epochs, 'previousId', 'nextId')
 
     study_design = self._create_design()
     self.study_designs.append(study_design)
 
   def _add_arm(self, name):
-    arm = cross_references.get(StudyArm, name)
+    arm = self.globals.cross_references.get(StudyArm, name)
     if arm is not None:
       if name not in self.arm_names:
         self.arm_names[name] = True
         self.arms.append(arm)
       return arm
     else:
       self._general_error(f"No arm definition found for arm '{name}'")
       return None
 
   def _add_epoch(self, name):
-    epoch = cross_references.get(StudyEpoch, name)
+    epoch = self.globals.cross_references.get(StudyEpoch, name)
     if epoch is not None:
       if name not in self.epoch_names:
         self.epoch_names[name] = True
         self.epochs.append(epoch)
       return epoch
     else:
       self._general_error(f"No epoch definition found for epoch '{name}'")
       return None
   
   def _add_element(self, name):
-    element = cross_references.get(StudyElement, name)
+    element = self.globals.cross_references.get(StudyElement, name)
     if element is not None:
       if name not in self.elements:
         self.elements[name] = element
       return element
     else:
       self._general_error(f"No element definition found for element '{name}'")
       return None
 
   def _add_cell(self, arm, epoch, elements):
     try:
       return StudyCell(
-        id=id_manager.build_id(StudyCell), 
+        id=self.globals.id_manager.build_id(StudyCell), 
         armId=arm,
         epochId=epoch,
         elementIds=elements
       )
     except Exception as e:
-      self._general_error("Failed to create StudyCell object, exception {e}")
-      self._traceback(f"{traceback.format_exc()}")
+      self._general_error("Failed to create StudyCell object", e)
       return None
 
   def _create_design(self):
     try:
       result = StudyDesign(
-        id=id_manager.build_id(StudyDesign), 
+        id=self.globals.id_manager.build_id(StudyDesign), 
         name=self.name,
         description=self.description,
         label=self.label,
         trialIntentTypes=self.trial_intents, 
         trialTypes=self.trial_types, 
         interventionModel=self.intervention_model,
         studyCells=self.cells,
@@ -198,36 +196,34 @@
         contents=[],
         maskingRoles=self.masks,
         characteristics=self.characteristics
       )
       #print(f"SD: {result.characteristics}")
       return result
     except Exception as e:
-      self._general_error("Failed to create StudyDesign object, exception {e}")
-      self._traceback(f"{traceback.format_exc()}")
+      self._general_error("Failed to create StudyDesign object", e)
       return None
   
 
   def _set_masking(self, rindex, cindex):
-    if option_manager.get(Options.USDM_VERSION) == '2':
+    if self.globals.option_manager.get(Options.USDM_VERSION) == '2':
       return None
     else:
       try:
         text = self.read_cell(rindex, cindex)
         parts = text.split('=')
         if len(parts) == 2: 
-          code = CDISCCT().code_for_attribute('Masking', 'role', parts[0].strip())
+          code = CDISCCT(self.globals).code_for_attribute('Masking', 'role', parts[0].strip())
           if code:
-            mask = Masking(id=id_manager.build_id(Masking), description=parts[1].strip(), role=code)
+            mask = Masking(id=self.globals.id_manager.build_id(Masking), description=parts[1].strip(), role=code)
             self.masks.append(mask)
-            cross_references.add(mask.id, mask)
+            self.globals.cross_references.add(mask.id, mask)
             return mask
           else:
             self._error(rindex, cindex, f"Failed to decode masking role data '{text}', must be a valid role code '{parts[0]}'")
             return None
         else:
           self._error(rindex, cindex, f"Failed to decode masking role data '{text}', no '=' detected")
           return None
       except Exception as e:
-        self._error(rindex, cindex, "Failed to create Masking object, exception {e}")
-        self._traceback(f"{traceback.format_exc()}")
+        self._error(rindex, cindex, "Failed to create Masking object", e)
         return None
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_sites_sheet/study_design_sites_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_eligibility_criteria_sheet/study_design_eligibility_criteria_sheet.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,34 @@
-from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.id_manager import id_manager
-import traceback
-import pandas as pd
-from usdm_model.organization import ResearchOrganization
-from usdm_model.study_site import StudySite
+from usdm_excel.globals import Globals
+from usdm_excel.syntax_template_sheet import SyntaxTemplateSheet
+from usdm_model.code import Code
+from usdm_model.eligibility_criterion import EligibilityCriterion
 
-class StudyDesignSitesSheet(BaseSheet):
+class StudyDesignEligibilityCriteriaSheet(SyntaxTemplateSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignEligibilityCriteria'
+  
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      self.organizations = []
-      self.sites = []
-      super().__init__(file_path=file_path, sheet_name='studyDesignSites', optional=True)
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME, optional=True)
+      self.items = []
       if self.success:
-        current_org = None
         for index, row in self.sheet.iterrows():
-          org_name = self.read_cell_by_name(index, 'name')
-          site_name = self.read_cell_by_name(index, 'siteName')
-          site_description = self.read_cell_by_name(index, 'siteDescription')
-          site_label = self.read_cell_by_name(index, 'siteLabel')
-          site = self.create_object(StudySite, {'name': site_name, 'description': site_description, 'label': site_label})
-          if site:
-            self.sites.append(site)
-            cross_references.add(site.id, site)     
-          if org_name:
-            org_label = self.read_cell_by_name(index, 'label')
-            org_type = self.read_cdisc_klass_attribute_cell_by_name('Organization', 'organizationType', index, ['type'])     
-            org_id_scheme = self.read_cell_by_name(index, 'identifierScheme')
-            org_identifier = self.read_cell_by_name(index, 'identifier')
-            org_address = self.read_address_cell_by_name(index, 'address')
-            if org_address:
-              cross_references.add(org_address.id, org_address)   
-            item = self.create_object(ResearchOrganization, {'identifierScheme': org_id_scheme, 'identifier': org_identifier, 'name': org_name, 'label': org_label, 'organizationType': org_type, 'legalAddress': org_address, 'manages': [site]})
-            if item:
-              self.organizations.append(item)
-              cross_references.add(item.id, item)     
-              current_org = item
-          else:
-            current_org.manages.append(site)
+          category = self.read_cdisc_klass_attribute_cell_by_name('EligibilityCriteria', 'category', index, 'category')
+          identifier = self.read_cell_by_name(index, 'identifier')
+          name = self.read_cell_by_name(index, 'name')
+          description = self.read_cell_by_name(index, 'description')
+          label = self.read_cell_by_name(index, 'label')
+          text = self.read_cell_by_name(index, 'text')
+          dictionary_name = self.read_cell_by_name(index, 'dictionary')
+          self._validate_references(index, 'text', text, dictionary_name)
+          item = self._criteria(name, description, label, text, category, identifier, dictionary_name)
+          if item:
+            self.globals.cross_references.add(item.name, item)
+            self.items.append(item)
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
 
+  def _criteria(self, name: str, description: str, label: str, text: str, category: Code, identifier: str, dictionary_name: str) -> EligibilityCriterion:
+    dictionary_id = self._get_dictionary_id(dictionary_name)
+    params = {'name': name, 'description': description, 'label': label, 'text': text, 'category': category, 'identifier': identifier, 'dictionaryId': dictionary_id}
+    return self.create_object(EligibilityCriterion, params)
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_timing_sheet/study_design_timing_sheet.py` & `usdm-0.49.0/src/usdm_excel/study_design_timing_sheet/study_design_timing_sheet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,61 @@
+import re
+import traceback
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.id_manager import id_manager
 from usdm_excel.iso_8601_duration import ISO8601Duration
 from usdm_excel.study_design_timing_sheet.window_type import WindowType
 from usdm_excel.cdisc_ct import CDISCCT
 from usdm_model.timing import Timing
-import traceback
-import re
+from usdm_excel.globals import Globals
 
 class StudyDesignTimingSheet(BaseSheet):
 
-  def __init__(self, file_path):
+  SHEET_NAME = 'studyDesignTiming'
+
+  def __init__(self, file_path: str, globals: Globals):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyDesignTiming', optional=True)
+      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME, optional=True)
       self.items = []
       if self.success:
         for index, row in self.sheet.iterrows():
           name = self.read_cell_by_name(index, 'name')
           description = self.read_cell_by_name(index, 'description')
           label = self.read_cell_by_name(index, 'label')
           type = self._set_type(self.read_cell_by_name(index, 'type'))
           from_name = self.read_cell_by_name(index, 'from')
           to_name = self.read_cell_by_name(index, 'to')
           timing_label = self.read_cell_by_name(index, 'timingValue')
           timing_value = self._set_text_and_encoded(self.read_cell_by_name(index, 'timingValue'))
           to_from_type = self._set_to_from_type(self.read_cell_by_name(index, 'toFrom'))
-          window = WindowType(self.read_cell_by_name(index, 'window'))
+          window = WindowType(self.read_cell_by_name(index, 'window'), self.globals)
           if window.errors:
             self._add_errors(window.errors, index, self._get_column_index('window'))
           try:
             item = Timing(
-              id=id_manager.build_id(Timing),
+              id=self.globals.id_manager.build_id(Timing),
               type=type,
               value=timing_value,
               valueLabel=timing_label,
               name=name,
               description=description,
               label=label,
               relativeToFrom=to_from_type,
               windowLabel=window.label,
               windowLower=window.lower,
               windowUpper=window.upper,
               relativeFromScheduledInstanceId=from_name,
               relativeToScheduledInstanceId=to_name
             )
           except Exception as e:
-            self._general_error(f"Failed to create Timing object, exception {e}")
-            self._traceback(f"{traceback.format_exc()}")
+            self._general_error(f"Failed to create Timing object", e)
           else:
-            cross_references.add(name, item)
+            self.globals.cross_references.add(name, item)
             self.items.append(item)
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
+      self._sheet_exception(e)
 
   def _set_text_and_encoded(self, duration):
     the_duration = duration.strip()
     original_duration = the_duration
     for char in ['+', '-']:
       if char in the_duration:
         the_duration = the_duration.replace(char, "")
@@ -73,18 +72,18 @@
   def _set_type(self, text):
     type_code = {
       "FIXED": {'c_code': 'C201358', 'pt': 'Fixed Reference'},
       "AFTER": {'c_code': 'C201356', 'pt': 'After'},
       "BEFORE": {'c_code': 'C201357', 'pt': 'Before'}
     }   
     key = text.strip().upper()
-    return CDISCCT().code(type_code[key]['c_code'], type_code[key]['pt'])
+    return CDISCCT(self.globals).code(type_code[key]['c_code'], type_code[key]['pt'])
 
   def _set_to_from_type(self, text):
     type_code = {
       "S2S": {'c_code': 'C201355', 'pt': 'Start to Start'},
       "S2E": {'c_code': 'C201354', 'pt': 'Start to End'},
       "E2S": {'c_code': 'C201353', 'pt': 'End to Start'},
       "E2E": {'c_code': 'C201352', 'pt': 'End to End'},
     }    
     key = "S2S" if not text else text.strip().upper()
-    return CDISCCT().code(type_code[key]['c_code'], type_code[key]['pt'])
+    return CDISCCT(self.globals).code(type_code[key]['c_code'], type_code[key]['pt'])
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_design_timing_sheet/window_type.py` & `usdm-0.49.0/src/usdm_excel/study_design_timing_sheet/window_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import re
 from usdm_excel.iso_8601_duration import ISO8601Duration
 from usdm_excel.range_type import RangeType
+from usdm_excel.globals import Globals
 
 class WindowType():
 
-  def __init__(self, timing_info):
+  def __init__(self, timing_info: str, globals: Globals):
     self.upper = None
     self.lower = None
     self.errors = []
     self.label = timing_info.strip() if timing_info else ""
     if self.label:
-      range = RangeType(self.label)
+      range = RangeType(self.label, globals)
       if not range.errors:
         self.lower = self._set_encoded(range.lower, range.units)
         self.upper = self._set_encoded(range.upper, range.units)     
       else:
         self.errors = range.errors
 
   def _set_encoded(self, value, units):
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py` & `usdm-0.49.0/src/usdm_db/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,86 @@
-from usdm_model.organization import Organization
-from usdm_model.study_identifier import StudyIdentifier
-from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.id_manager import id_manager
-from usdm_excel.cross_ref import cross_references
+import json
 import traceback
+from usdm_excel import USDMExcel
+from usdm_model.wrapper import Wrapper
+from usdm_db.document.document import Document
+from usdm_db.errors_and_logging.errors_and_logging import ErrorsAndLogging
+from usdm_db.neo4j_dict import Neo4jDict
+from usdm_db.timeline import Timeline
 
-class StudyIdentifiersSheet(BaseSheet):
+class USDMDb():
 
-  def __init__(self, file_path: str):
+  SYSTEM_NAME = "CDISC E2J"
+
+  FULL_HTML = Timeline.FULL
+  BODY_HTML = Timeline.BODY
+  
+  def __init__(self):
+    self._wrapper = None
+    self._excel = None
+    self._errors_and_logging = ErrorsAndLogging()
+
+  def errors(self):
+    return self._errors_and_logging.errors().dump()
+  
+  def wrapper(self):
+    return self._wrapper
+  
+  def excel(self):
+    return self._excel
+
+  def from_json(self, data):
+    self._wrapper = Wrapper.model_validate(data)
+    
+  def from_excel(self, file_path):
+    self._excel = USDMExcel(file_path)
+    self._wrapper = self._excel.execute()
+    return self._excel.errors()
+
+  def to_json(self):
+    try:
+      raw_json = self._wrapper.to_json()
+    except Exception as e:
+      message = self._format_exception("Failed to generate JSON output", e)
+      raw_json = json.dumps({'error': message}, indent = 2)
+    return raw_json
+
+  def to_html(self, highlight=False):
     try:
-      super().__init__(file_path=file_path, sheet_name='studyIdentifiers')
-      self.identifiers = []
-      self.process_sheet()
+      study = self._wrapper.study
+      title = self._get_title()
+      doc = Document(title, study, self._errors_and_logging)
+      html = doc.to_html(highlight)
     except Exception as e:
-      self._general_error(f"Exception '{e}' raised reading sheet.")
-      self._traceback(f"{traceback.format_exc()}")
-      
-  def process_sheet(self):
-    self.identifiers = []
-    for index, row in self.sheet.iterrows():
-      org_type = self.read_cdisc_klass_attribute_cell_by_name('Organization', 'organizationType', index, ['organisationType', 'type'])     
-      org_id_scheme = self.read_cell_by_name(index, 'organisationIdentifierScheme')
-      org_identifier = self.read_cell_by_name(index, 'organisationIdentifier')
-      org_name = self.read_cell_by_name(index, ['organisationName', 'name'])
-      org_label = self.read_cell_by_name(index, 'label', default="", must_be_present=False)
-      org_address = self.read_address_cell_by_name(index, 'organisationAddress')
-      if org_address:
-        cross_references.add(org_address.id, org_address)   
-      try:
-        organisation = Organization(
-          id=id_manager.build_id(Organization),
-          identifierScheme=org_id_scheme, 
-          identifier=org_identifier,
-          name=org_name,
-          label=org_label,
-          organizationType=org_type,
-          legalAddress=org_address
-        )
-      except Exception as e:
-        self._general_error(f"Failed to create Organization object, exception {e}")
-        self._traceback(f"{traceback.format_exc()}")
-      else:
-        cross_references.add(organisation.id, organisation)   
-        try:
-          item = StudyIdentifier(
-            id=id_manager.build_id(StudyIdentifier),
-            studyIdentifier=self.read_cell_by_name(index, 'studyIdentifier'), 
-            studyIdentifierScope=organisation
-          )
-        except Exception as e:
-          self._general_error(f"Failed to create StudyIdentifier object, exception {e}")
-          self._traceback(f"{traceback.format_exc()}")
-        else:
-          self.identifiers.append(item)
-          cross_references.add(item.studyIdentifier, item)         
+      message = self._format_exception("Failed to generate HTML output", e)
+      html = f"<p>{message}</p>"
+    return html
+
+  def to_pdf(self, test=True):
+    try:
+      study = self._wrapper.study
+      title = self._get_title()
+      doc = Document(title, study, self._errors_and_logging)
+      bytes = doc.to_pdf(test)
+    except Exception as e:
+      message = self._format_exception("Failed to generate PDF output", e)
+      bytes = bytearray()
+      bytes.extend(map(ord, message))    
+    return bytes
+
+  def to_neo4j_dict(self):
+    return Neo4jDict(self._wrapper.study).to_dict()
+
+  def to_timeline(self, level=FULL_HTML):
+    return Timeline(self._wrapper.study).to_html(level)
+
+  def _format_exception(self, message, e):
+    return f"{message}, exception {e}\n{traceback.format_exc()}"
+  
+  def _get_title(self):
+    study = self._wrapper.study
+    study_version = study.versions[0]
+    title_type = 'Official Study Title'
+    for title in study_version.titles:
+      if title.type.decode == title_type:
+        return title.text
+    return None
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/activities.py` & `usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/activities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from usdm_excel.id_manager import id_manager
+#from usdm_excel.id_manager import id_manager
 from usdm_excel.study_soa_v2_sheet.soa_column_rows import SoAColumnRows
 from usdm_excel.study_soa_v2_sheet.activity import Activity
 import pandas as pd
 
 class Activities():
   
   def __init__(self, parent):
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/activity.py` & `usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/activity.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,85 @@
-import traceback
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.id_manager import id_manager
-from usdm_excel.cross_ref import cross_references
 from usdm_excel.study_soa_v2_sheet.soa_column_rows import SoAColumnRows
 from usdm_model.activity import Activity as USDMActivity
 from usdm_model.biomedical_concept_surrogate import BiomedicalConceptSurrogate
-from usdm_excel.cdisc_biomedical_concept import cdisc_bc_library
 from usdm_model.procedure import Procedure
 from usdm_model.schedule_timeline import ScheduleTimeline
 
 class Activity():
   
-  def __init__(self, parent, row_index):
+  def __init__(self, parent: BaseSheet, row_index: int):
     self.parent = parent
     self.row_index = row_index
     self.usdm_biomedical_concept_surrogates = []
     self.usdm_biomedical_concepts = []
     self.name = parent.read_cell(row_index, SoAColumnRows.CHILD_ACTIVITY_COL)
     self._bcs, self._prs, self._tls = self._get_observation_cell(row_index, SoAColumnRows.BC_COL)
     self.parent._debug(row_index, SoAColumnRows.BC_COL, f"Activity {self.name} read. BC: {self._bcs}, PR: {self._prs}, TL: {self._tls}")
     self.usdm_activity = self._as_usdm()
     
   def _as_usdm(self):
     surrogate_bc_items = []
     full_bc_items = []
     procedures = []
     for bc in self._bcs:
-      if cdisc_bc_library.exists(bc):
-        full_bc = cdisc_bc_library.usdm(bc)
+      if self.parent.globals.cdisc_bc_library.exists(bc):
+        full_bc = self.parent.globals.cdisc_bc_library.usdm(bc)
         full_bc_items.append(full_bc.id)
         self.usdm_biomedical_concepts.append(full_bc)
+        self.parent.globals.cross_references.add(full_bc.id, full_bc)
       else:
         surrogate = self._to_bc_surrogates(bc)
         surrogate_bc_items.append(surrogate.id)
         self.usdm_biomedical_concept_surrogates.append(surrogate)
+        self.parent.globals.cross_references.add(surrogate.id, surrogate)
     timelineId = ""
     if len(self._tls) > 0:
-      timeline = cross_references.get(ScheduleTimeline, self._tls[0])
+      timeline = self.parent.globals.cross_references.get(ScheduleTimeline, self._tls[0])
       if timeline:
         timelineId = timeline.id
       else:
         timelineId = None
         self.parent._general_error(f"Unable to find timeline with name '{self._tls[0]}'")
     for procedure in self._prs:
-      ref = cross_references.get(Procedure, procedure)
+      ref = self.parent.globals.cross_references.get(Procedure, procedure)
       if ref is not None:
         procedures.append(ref)
       else:
         self.parent._warning(self.row_index, SoAColumnRows.BC_COL, f"Cross reference error for procedure {procedure}, not found")
-    activity = cross_references.get(Activity, self.name)
+    activity = self.parent.globals.cross_references.get(Activity, self.name)
     if activity is None:
       try:
         activity = USDMActivity(
-          id=id_manager.build_id(Activity),
+          id=self.parent.globals.id_manager.build_id(Activity),
           name=self.name,
           description=self.name,
           definedProcedures=procedures,
           #activityIsConditional=False,
           #activityIsConditionalReason="",
           biomedicalConceptIds=full_bc_items,
           bcCategoryIds=[],
           bcSurrogateIds=surrogate_bc_items,
           timelineId=timelineId
         )
-        cross_references.add(self.name, activity)     
+        self.parent.globals.cross_references.add(self.name, activity)     
         self.parent._warning(self.row_index, SoAColumnRows.BC_COL, f"No activity {self.name} found, so one has been created")
       except Exception as e:
         #print(f"NAME: {self.row_index}, {self.name}")
-        self.parent._general_error(f"Failed to create Activity object, exception {e}")
-        self.parent._traceback(f"{traceback.format_exc()}")  
+        self.parent._general_exception(f"Failed to create Activity object", e)
     else:
       activity.definedProcedures = procedures
       activity.biomedicalConceptIds = full_bc_items
       activity.bcSurrogateIds = surrogate_bc_items
       activity.timelineId = timelineId
     return activity
   
   def _to_bc_surrogates(self, name):
     return BiomedicalConceptSurrogate(
-      id=id_manager.build_id(BiomedicalConceptSurrogate),
+      id=self.parent.globals.id_manager.build_id(BiomedicalConceptSurrogate),
       name=name,
       description=name,
       label=name,
       reference='None set'
     )
   
   def _get_observation_cell(self, row_index, col_index):
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/conditons.py` & `usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/conditons.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instance.py` & `usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instance.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from usdm_excel.base_sheet import BaseSheet
 from usdm_excel.study_soa_v2_sheet.soa_column_rows import SoAColumnRows
 from usdm_excel.study_soa_v2_sheet.conditons import Conditons
-from usdm_excel.id_manager import id_manager
-from usdm_excel.cross_ref import cross_references
+#from usdm_excel.id_manager import id_manager
+#from usdm_excel.cross_ref import cross_references
 from usdm_model.scheduled_instance import ScheduledActivityInstance, ScheduledDecisionInstance
 from usdm_model.encounter import Encounter
 from usdm_model.study_epoch import StudyEpoch
 from usdm_model.activity import Activity
 import traceback
 
 class ScheduledInstance():
@@ -23,69 +23,68 @@
     label = self.parent.read_cell(SoAColumnRows.LABEL_ROW, col_index)
     epoch_name = self.parent.read_cell(SoAColumnRows.EPOCH_ROW, col_index)
     encounter_name = self.parent.read_cell(SoAColumnRows.ENCOUNTER_ROW, col_index)
     type = self.parent.read_cell(SoAColumnRows.TYPE_ROW, col_index)
     self.default_name = self.parent.read_cell(SoAColumnRows.DEFAULT_ROW, col_index)
     self.conditions = Conditons(self.parent.read_cell(SoAColumnRows.CONDITIONS_ROW, col_index))
     if encounter_name:
-      encounter = cross_references.get(Encounter, encounter_name)
+      encounter = self.parent.globals.cross_references.get(Encounter, encounter_name)
       if encounter:
         encounter_id = encounter.id
       else:
         self.parent._general_warning(f"Failed to find encounter with name '{encounter_name}'")
     if epoch_name:
-      epoch = cross_references.get(StudyEpoch, epoch_name)
+      epoch = self.parent.globals.cross_references.get(StudyEpoch, epoch_name)
       if epoch:
         epoch_id = epoch.id
       else:
         self.parent._general_warning(f"Failed to find epoch with name '{epoch_name}'")
     try:
       if type.upper() == "ACTIVITY":
         self.item = ScheduledActivityInstance(
-          id=id_manager.build_id(ScheduledActivityInstance),
+          id=self.parent.globals.id_manager.build_id(ScheduledActivityInstance),
           name=name,
           description=description,
           label=label,
           timelineExitId=None,
           encounterId=encounter_id,
           scheduledInstanceTimelineId=None,
           defaultConditionId=None,
           epochId=epoch_id,
           activityIds=self._add_activities()
         )
-        cross_references.add(self.item.id, self.item)
-        cross_references.add(self.name, self.item)
+        self.parent.globals.cross_references.add(self.item.id, self.item)
+        self.parent.globals.cross_references.add(self.name, self.item)
       elif type.upper() == "DECISION":
         self.item = ScheduledDecisionInstance(
-          id=id_manager.build_id(ScheduledDecisionInstance),
+          id=self.parent.globals.id_manager.build_id(ScheduledDecisionInstance),
           name=name,
           description=description,
           label=label,
           timelineExitId=None,
           scheduledInstanceTimelineId=None,
           defaultConditionId=None,
           conditionAssignments=[]
         )
-        cross_references.add(self.item.id, self.item)
-        cross_references.add(self.name, self.item)
+        self.parent.globals.cross_references.add(self.item.id, self.item)
+        self.parent.globals.cross_references.add(self.name, self.item)
       else:
         self.parent._general_warning(f"Unrecognized ScheduledInstance type: '{type}'")
     except Exception as e:
-      self.parent._general_error(f"Exception '{e}' raised reading sheet")
-      self.parent._traceback(f"{traceback.format_exc()}")
+      parent._sheet_exception(f"Error raised reading sheet", e)
 
   def _add_activities(self):
     activities = []
     row = 0
     column = self.parent.sheet.iloc[:, self.col_index]
     for cell in column:
       if row >= SoAColumnRows.FIRST_ACTIVITY_ROW:
         activity_name = self.parent.read_cell(row, SoAColumnRows.CHILD_ACTIVITY_COL)
         if str(cell).upper() == "X":
-          activity = cross_references.get(Activity, activity_name)
+          activity = self.parent.globals.cross_references.get(Activity, activity_name)
           if activity:
             activities.append(activity.id)
           else:
             self.parent._general_warning(f"Unable to find activity '{activity_name}' when adding to schedule instance")
       row += 1
     return activities
```

### Comparing `usdm-0.48.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instances.py` & `usdm-0.49.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instances.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from usdm_excel.study_soa_v2_sheet.soa_column_rows import SoAColumnRows
 from usdm_excel.study_soa_v2_sheet.scheduled_instance import ScheduledInstance
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.id_manager import id_manager
+#from usdm_excel.cross_ref import cross_references
+#from usdm_excel.id_manager import id_manager
 from usdm_model.schedule_timeline_exit import ScheduleTimelineExit
 from usdm_model.scheduled_instance import ConditionAssignment
 
 class ScheduledInstances():
   
   def __init__(self, parent):
     self.parent = parent
@@ -37,16 +37,16 @@
         exit = self._add_exit()
         item.timelineExitId = exit.id
         self.exits.append(exit)
       else:
         self.parent._general_error(f"Default reference from {instance.name} to {instance.default_name} cannot be made, not found on the same timeline")
 
   def _add_exit(self):
-    exit = ScheduleTimelineExit(id=id_manager.build_id(ScheduleTimelineExit))
-    cross_references.add(exit.id, exit)
+    exit = ScheduleTimelineExit(id=self.parent.globals.id_manager.build_id(ScheduleTimelineExit))
+    self.parent.globals.cross_references.add(exit.id, exit)
     return exit
 
   def _set_condition_references(self):
     for instance in self.items:
       item = instance.item
       if item.instanceType == 'ScheduledDecisionInstance':
         for condition in instance.conditions.items:
```

### Comparing `usdm-0.48.0/src/usdm_model/__init__.py` & `usdm-0.49.0/src/usdm_model/__init__.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_model/api_base_model.py` & `usdm-0.49.0/src/usdm_model/api_base_model.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_model/encounter.py` & `usdm-0.49.0/src/usdm_model/encounter.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_model/population_definition.py` & `usdm-0.49.0/src/usdm_model/population_definition.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_model/schedule_timeline.py` & `usdm-0.49.0/src/usdm_model/schedule_timeline.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_model/scheduled_instance.py` & `usdm-0.49.0/src/usdm_model/scheduled_instance.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_model/study.py` & `usdm-0.49.0/src/usdm_model/study.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_model/study_design.py` & `usdm-0.49.0/src/usdm_model/study_design.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_model/study_intervention.py` & `usdm-0.49.0/src/usdm_model/study_intervention.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/src/usdm_model/study_version.py` & `usdm-0.49.0/src/usdm_model/study_version.py`

 * *Files identical despite different names*

### Comparing `usdm-0.48.0/tests/test_base_sheet.py` & `usdm-0.49.0/tests/test_base_sheet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,222 +1,230 @@
 import pytest
 import pandas as pd
-
-xfail = pytest.mark.xfail
-
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.errors.errors import error_manager
 from usdm_model.code import Code
 
-# def test_sheet_cell_value(mocker):
-#   mocked_open = mocker.mock_open(read_data="File")
-#   mocker.patch("builtins.open", mocked_open)
-#   data = {'col_1': [3, 2, 1, 0], 'col_2': ['a', 'b', 'c', 'd']}
-#   mock_read = mocker.patch("openpyxl.load_workbook")
-#   mock_read.return_value = pd.DataFrame.from_dict(data)
-#   test_data = [
-#     ({'row': 0, 'column': 0, 'value': 4}, False),
-#     ({'row': 0, 'column': 1, 'value': 'e'}, False),
-#     ({'row': 0, 'column': 0, 'value': 3}, True),
-#     ({'row': 0, 'column': 1, 'value': 'a'}, True),
-#   ]
-#   for test in test_data:
-#     base = BaseSheet("", "sheet", require=test[0])
-#     if not test[1]:
-#       assert(base) == None
-#     else:
-#       assert(base) != None
+xfail = pytest.mark.xfail
 
-def test_cell_empty(mocker):
+def test_cell_empty(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': [3, 2, 1, 0], 'col_2': [None, 'b', 'c', None]}
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame.from_dict(data)
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     (0,0,False),
     (3,0,False),
     (0,1,True),
     (3,1,True)
   ]
   for test in test_data:
     assert(base.cell_empty(test[0],test[1])) == test[2]
 
-def test_cell_empty_legacy(mocker):
+def test_cell_empty_legacy(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': [3, 2, 1, 0], 'col_2': [None, 'b', '-', None]}
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame.from_dict(data)
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     (0,0,'3',False),
     (3,0,'0',False),
     (0,1,'',True),
     (2,1,'',True),
     (3,1,'',True)
   ]
   for test in test_data:
     value, is_null = base.read_cell_empty_legacy(test[0],test[1])
     assert(value) == test[2]
     assert(is_null) == test[3]
 
-def test_read_cell_empty(mocker):
+def test_read_cell_empty(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': [3, 2, 1, 0], 'col_2': [None, 'b', '-', None]}
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame.from_dict(data)
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     (0,0,'3','3'),
     (3,0,'0','0'),
     (0,1,'',''),
     (2,1,'','-'),
     (3,1,'','')
   ]
   for test in test_data:
     assert(base.read_cell_empty(test[0],test[1],'-')) == test[2]
     assert(base.read_cell_empty(test[0],test[1],'=')) == test[3]
 
-def test_read_cell(mocker):
+def test_read_cell(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': [3, 2, 1, 0], 'col_2': ['a', 'b', 'c', '']}
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame.from_dict(data)
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     (0,0,'3'),
     (3,0,'0'),
     (0,1,'a'),
     (3,1,'')
   ]
   for test in test_data:
     assert(base.read_cell(test[0],test[1])) == test[2]
 
-def test_read_cell_default(mocker):
+def test_read_cell_default(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': [3, 2, 1, 0], 'col_2': ['a', 'b', 'c', None]}
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame.from_dict(data)
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     (3,1,'100s','100s')
   ]
   for test in test_data:
     assert(base.read_cell(test[0],test[1], default=test[2])) == test[3]
 
-def test_read_cell_error(mocker):
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+def test_read_cell_error(mocker, globals):
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': [3, 2, 1, 0], 'col_2': ['a', 'b', 'c', '']}
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame.from_dict(data)
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   assert(base.read_cell(6,8)) == ""
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "sheet"
   assert mock_error.call_args[0][1] == 7
   assert mock_error.call_args[0][2] == 9
-  assert mock_error.call_args[0][3] == "Error 'index 8 is out of bounds for axis 0 with size 2' reading cell"
+  assert mock_error.call_args[0][3] == "Exception. Error reading cell. See log for additional details."
   
-def test_read_cell_by_name(mocker):
+def test_read_cell_by_name(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['tom', 10], ['nick', 15], ['juli', 14], ['fred', '']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Age'])
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     (0,'Name','tom'),
     (2,'Name','juli'),
     (0,'Age','10'),
     (2,'Age','14'),
     (3,'Age',''),
   ]
   for test in test_data:
     assert(base.read_cell_by_name(test[0],test[1])) == test[2]
 
-def test_read_cell_by_name_default(mocker):
+def test_read_cell_by_name_default(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['tom', 10], ['nick', 15], ['juli', 14], ['fred', '']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Age'])
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   assert(base.read_cell_by_name(0, 'NameX', 'Default')) == 'Default'
   assert(base.read_cell_by_name(0, 'Name', 'Default')) == 'tom'
   assert(base.read_cell_by_name(0, ['NameX', 'XXX'], 'Default')) == 'Default'
   assert(base.read_cell_by_name(0, ['NameX', 'XXX', 'Age'], 'Default')) == '10'
   assert(base.read_cell_by_name(3, 'Age', default='100')) == ''
 
-def test_read_cell_by_name_error(mocker):
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+def test_read_cell_by_name_error(mocker, globals):
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['tom', 10], ['nick', 15], ['juli', 14]]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Age'])
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   assert(base.read_cell_by_name(1,'Not There')) == ""
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "sheet"
   assert mock_error.call_args[0][1] == 2
   assert mock_error.call_args[0][2] == -1
   assert mock_error.call_args[0][3] == "Error 'Failed to detect column(s) 'Not There' in sheet' reading cell 'Not There'"
 
-def test_read_cell_by_name_present(mocker):
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+def test_read_cell_by_name_present(mocker, globals):
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['tom', 10], ['nick', 15], ['juli', 14]]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Age'])
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   assert(base.read_cell_by_name(1,'Not There',must_be_present=False)) == ""
   mock_error.assert_not_called()
 
-def test_read_cell_multiple(mocker):
+def test_read_cell_multiple(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     ['tom', ''], 
     ['nick', 'Sam'], 
     ['juli', ' Fred, Dick,   Harry  '], 
     ['andy', 'John  , Jane'], 
     ['andy', '"John, & Fred", Jane'],
     ['andy', '"John, \\" & Fred", Jane']
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Children'])
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     (0,1,[]),
     (2,1,['Fred', 'Dick', 'Harry']),
     (3,1,['John', 'Jane']),
     (4,1,['John, & Fred', 'Jane']),
     (5,1,['John, " & Fred', 'Jane'])
   ]
   for test in test_data:
     assert(base.read_cell_multiple(test[0],test[1])) == test[2]
 
+def test_read_cell_multiple_by_name(mocker, globals):
+  mocked_open = mocker.mock_open(read_data="File")
+  mocker.patch("builtins.open", mocked_open)
+  data = [
+    ['tom', ''], 
+    ['nick', 'Sam'], 
+    ['juli', ' Fred, Dick,   Harry  '], 
+    ['andy', 'John  , Jane'], 
+    ['andy', '"John, & Fred", Jane'],
+    ['andy', '"John, \\" & Fred", Jane']
+  ]
+  mock_read = mocker.patch("pandas.read_excel")
+  mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Children'])
+  base = BaseSheet("", globals, "sheet")
+  test_data = [
+    (0,[],                         True,  ""),
+    (2,['Fred', 'Dick', 'Harry'],  True,  ""),
+    (3,['John', 'Jane'],           True,  ""),
+    (4,['John, & Fred', 'Jane'],   True,  ""),
+    (5,['John, " & Fred', 'Jane'], True,  ""),
+    (6,[],                         False, "")
+  ]
+  for test in test_data:
+    errors = globals.errors_and_logging._errors
+    errors.clear()
+    assert(base.read_cell_multiple_by_name(test[0],'Children')) == test[1]
+    
+    #assert(errors.items[0].to_log()) == test[3]
+
 # read_cell_with_previous
 
-def test_read_boolean_cell_by_name(mocker):
+def test_read_boolean_cell_by_name(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   #data = [[0, 1, 2, 3, 4, 5, 6, 7, 8], ['a', 'y', 'Y', 'true', 'True', 'yes', 1, '1', '']]
   data = [[0, 'a'], [1, 'y'], [2, 'Y'], [3, 'true'], [4, 'True'], [5, 'yes'], [6, 1,], [7, '1'], [8, ''], [9, 'T']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Children'])
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     (0,'Children',False),
     (1,'Children',True),
     (2,'Children',True),
     (3,'Children',True),
     (4,'Children',True),
     (5,'Children',True),
@@ -224,90 +232,91 @@
     (7,'Children',True),
     (8,'Children',False),
     (9,'Children',True),
   ]
   for test in test_data:
     assert(base.read_boolean_cell_by_name(test[0],test[1])) == test[2]
 
-def test_read_quantity_cell_by_name(mocker):
+def test_read_quantity_cell_by_name(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [[''], ['1 days'], [' 1 weeks'], ['14 Hours'], ['14'], ['']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['Quantity'])
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     #  Name,       Allow Missing Units, Allow Empty, Errors, Empty,  Value,  Unit,     Error 
     (0,'Quantity', False,               False,       True,   False,  0.0,    '',       "Error in sheet sheet at [1,1]: Could not decode the quantity value, appears to be empty ''"),
     (1,'Quantity', False,               False,       False,  False,  1.0,    'C25301', ''),
     (2,'Quantity', False,               False,       False,  False,  1.0,    'C29844', ''),
     (3,'Quantity', False,               False,       False,  False,  14.0,   'C25529', ""),
     (4,'Quantity', True,                False,       False,  False,  14.0,   '',       ""),
     (5,'Quantity', False,               True,        False,  True,   0.0,    '',       ""),
   ]
   for test in test_data:
-    error_manager.clear()
+    errors = globals.errors_and_logging._errors
+    errors.clear()
     #print(f"INDEX: {test[0]}")
     item = base.read_quantity_cell_by_name(test[0],test[1],test[2],test[3]) 
     if not test[4] and not test[5]:
       assert(item.value) == test[6]
       if not test[2]:
         assert(item.unit.standardCode.code) == test[7]
-      assert(len(error_manager.items)) == 0
+      assert(len(errors.items)) == 0
     elif test[5]:
       assert(item) == None
     else:
       assert(item) == None
-      assert(error_manager.items[0].to_log()) == test[8]
+      assert(errors.items[0].to_log()) == test[8]
 
-def test_read_range_cell_by_name(mocker):
+def test_read_range_cell_by_name(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [[''], ['1..2 days'], [' 1 .. 3 weeks'], [' .. 3 weeks'], ['1 ..  weeks'], ['1 . 4 weeks'], ['14 Hours'], ['14'], ['']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['Range'])
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     #  Name,    Req Units, Allow Empty, Errors, Empty, Min,  Max,   Unit,     Error 
     (0,'Range', True,      False,       True,   False, 0.0,  0.0,   '',       "Error in sheet sheet at [1,1]: Could not decode the range value, appears to be empty ''"),
-    (1,'Range', True,      False,       False,  False,  1.0,  2.0,   'C25301', ''),
-    (2,'Range', True,      False,       False,  False,  1.0,  3.0,   'C29844', ''),
+    (1,'Range', True,      False,       False,  False, 1.0,  2.0,   'C25301', ''),
+    (2,'Range', True,      False,       False,  False, 1.0,  3.0,   'C29844', ''),
     (3,'Range', True,      False,       True,   False, 0.0,  0.0,   '',       "Error in sheet sheet at [4,1]: Could not decode the range value '.. 3 weeks'"),
     (4,'Range', True,      False,       True,   False, 0.0,  0.0,   '',       "Error in sheet sheet at [5,1]: Unable to set the units code for the range '1 ..  weeks'"),
     (5,'Range', True,      False,       True,   False, 0.0,  0.0,   '',       "Error in sheet sheet at [6,1]: Unable to set the units code for the range '1 . 4 weeks'"),
     (6,'Range', True,      False,       False,  False, 14.0, 14.0,  'C25529', ""),
     (7,'Range', False,     False,       False,  False, 14.0, 14.0,  '',       ""),
     (8,'Range', True,      True,        False,  True,  0.0,  0.0,   '',       ""),
   ]
   for test in test_data:
-    error_manager.clear()
+    globals.errors_and_logging.errors().clear()
     #print(f"INDEX: {test[0]}")
     range = base.read_range_cell_by_name(test[0],test[1],test[2],test[3]) 
     if not test[4] and not test[5]:
       assert(range.minValue) == test[6]
       assert(range.maxValue) == test[7]
       if test[2]:
         assert(range.unit.code) == test[8]
       assert(range.isApproximate) == False
-      assert(len(error_manager.items)) == 0
+      assert(len(globals.errors_and_logging.errors().items)) == 0
     elif test[5]:
       assert(range) == None
     else:
       assert(range) == None
-      assert(error_manager.items[0].to_log()) == test[9]
+      assert(globals.errors_and_logging.errors().items[0].to_log()) == test[9]
 
-# def test_read_description_by_name(mocker):
+# def test_read_description_by_name(mocker, globals):
 #   mock_option = mocker.patch("usdm_excel.om.get")
 #   mock_option.side_effect=['xxx', 'xxx', 'xxx']
 #   mocked_open = mocker.mock_open(read_data="File")
 #   mocker.patch("builtins.open", mocked_open)
 #   data = [[0, ''], [1, 'something'], [2, '  ']]
 #   mock_read = mocker.patch("pandas.read_excel")
 #   mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Children'])
-#   base = BaseSheet("", "sheet")
+#   base = BaseSheet("", globals, "sheet")
 #   test_data = [
 #     (0,'Children','xxx'),
 #     (1,'Children','something'),
 #     (2,'Children','xxx'),
 #   ]
 #   for test in test_data:
 #     assert(base.read_description_by_name(test[0],test[1])) == test[2]
@@ -328,64 +337,64 @@
 def test_read_other_code_cell_multiple_by_name():
   assert 0
 
 @xfail
 def test_read_other_code_cell_mutiple():
   assert 0
 
-def test_column_present(mocker):
+def test_column_present(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Children'])
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   assert(base.column_present("Name")) == 0
   assert(base.column_present(["Name"])) == 0
   assert(base.column_present(["Children"])) == 1
   assert(base.column_present(["ChildrenX", "Children"])) == 1
   with pytest.raises(BaseSheet.FormatError):
     assert(base.column_present(["Fred"]))
   
-def test_read_cdisc_klass_attribute_cell_by_name(mocker):
+def test_read_cdisc_klass_attribute_cell_by_name(mocker, globals):
   expected = Code(id='CodeX', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label")
   mock_code = mocker.patch("usdm_excel.cdisc_ct.CDISCCT.code_for_attribute")
   mock_code.side_effect=[expected, None]
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [[0, 'a'], [1, ''], [2, 'c']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Children'])
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     (0, 'Children', expected, ""),
     (1, 'Children', None, "sheet", 2, 2, "Empty cell detected where CDISC CT value expected."),
     (2, 'Children', None, "sheet", 3, 2, "CDISC CT not found for value 'c'.")
   ]
   for test in test_data:
     assert(base.read_cdisc_klass_attribute_cell_by_name( 'X', 'y', test[0], test[1])) == test[2]
     if not test[3] == "":
       mock_error.assert_called()
       assert mock_error.call_args[0][0] == test[3]
       assert mock_error.call_args[0][1] == test[4]
       assert mock_error.call_args[0][2] == test[5]
       assert mock_error.call_args[0][3] == test[6]
 
-def test_read_cdisc_klass_attribute_cell(mocker):
+def test_read_cdisc_klass_attribute_cell(mocker, globals):
   expected = Code(id='CodeX', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label")
   mock_code = mocker.patch("usdm_excel.cdisc_ct.CDISCCT.code_for_attribute")
   mock_code.side_effect=[expected, None]
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': [3, 2, 1, 0], 'col_2': ['a', '', 'c', '']}
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame.from_dict(data)
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     (0, 1, expected, ""),
     (1, 1, None, "sheet", 2, 2, "Empty cell detected where CDISC CT value expected."),
     (2, 1, None, "sheet", 3, 2, "CDISC CT not found for value 'c'.")
   ]
   for test in test_data:
     assert(base.read_cdisc_klass_attribute_cell( 'X', 'y', test[0], test[1])) == test[2]
@@ -393,82 +402,82 @@
       mock_error.assert_called()
       assert mock_error.call_args[0][0] == test[3]
       assert mock_error.call_args[0][1] == test[4]
       assert mock_error.call_args[0][2] == test[5]
       assert mock_error.call_args[0][3] == test[6]
      
 @xfail
-def test_read_cdisc_klass_attribute_cell_multiple_by_name(mocker):
+def test_read_cdisc_klass_attribute_cell_multiple_by_name(mocker, globals):
   assert 0
   
-def test_read_cdisc_klass_attribute_cell_multiple(mocker):
+def test_read_cdisc_klass_attribute_cell_multiple(mocker, globals):
   expected_1 = Code(id='CodeX1', code='code1', codeSystem='codesys', codeSystemVersion='3', decode="label1")
   expected_2 = Code(id='CodeX2', code='code2', codeSystem='codesys', codeSystemVersion='3', decode="label2")
   mock_code = mocker.patch("usdm_excel.cdisc_ct.CDISCCT.code_for_attribute")
   mock_code.side_effect=[expected_1, expected_2, None]
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': [3, 2, 1, 0], 'col_2': ['a,b', '', 'c', '']}
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame.from_dict(data)
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     (0, 1, [expected_1, expected_2], ""),
     (1, 1, [], "sheet", 2, 2, "Empty cell detected where multiple CDISC CT values expected."),
     (2, 1, [], "sheet", 3, 2, "CDISC CT not found for value 'c'.")
   ]
   for test in test_data:
     assert(base.read_cdisc_klass_attribute_cell_multiple( 'X', 'y', test[0], test[1])) == test[2]
     if not test[3] == "":
       mock_error.assert_called()
       assert mock_error.call_args[0][0] == test[3]
       assert mock_error.call_args[0][1] == test[4]
       assert mock_error.call_args[0][2] == test[5]
       assert mock_error.call_args[0][3] == test[6]
 
-def test_read_cdisc_klass_attribute_cell_multiple_by_name(mocker):
+def test_read_cdisc_klass_attribute_cell_multiple_by_name(mocker, globals):
   expected_1 = Code(id='CodeX1', code='code1', codeSystem='codesys', codeSystemVersion='3', decode="label1")
   expected_2 = Code(id='CodeX2', code='code2', codeSystem='codesys', codeSystemVersion='3', decode="label2")
   mock_code = mocker.patch("usdm_excel.cdisc_ct.CDISCCT.code_for_attribute")
   mock_code.side_effect=[expected_1, expected_2, None]
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [[0, 'a,b'], [1, ''], [2, 'c']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Children'])
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     (0, 'Children', [expected_1, expected_2], ""),
     (1, 'Children', [], "sheet", 2, 2, "Empty cell detected where multiple CDISC CT values expected."),
     (2, 'Children', [], "sheet", 3, 2, "CDISC CT not found for value 'c'.")
   ]
   for test in test_data:
     assert(base.read_cdisc_klass_attribute_cell_multiple_by_name( 'X', 'y', test[0], test[1])) == test[2]
     if not test[3] == "":
       mock_error.assert_called()
       assert mock_error.call_args[0][0] == test[3]
       assert mock_error.call_args[0][1] == test[4]
       assert mock_error.call_args[0][2] == test[5]
       assert mock_error.call_args[0][3] == test[6]
 
-def test__decode_other_cell(mocker):
+def test__decode_other_cell(mocker, globals):
   expected = Code(id='Code_1', code='c', codeSystem='a', codeSystemVersion='3', decode="d")
-  mock_version = mocker.patch("usdm_excel.ct_version_manager.get")
+  mock_version = mocker.patch("usdm_excel.ct_version_manager.CTVersionManager.get")
   mock_version.side_effect=['3']
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Code_1']
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data)
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     ("", 0, 0, None, ""),
     ("xxx", 1, 1, None, "sheet", 2, 2, "Failed to decode code data 'xxx', no ':' detected"),
     ("a:", 1, 1, None, "sheet", 2, 2, "Failed to decode code data 'a:', no '=' detected"),
     ("a:c", 1, 1, None, "sheet", 2, 2, "Failed to decode code data 'a:c', no '=' detected"),
     ("a:c=d", 1, 1, expected, "")
   ]
@@ -477,36 +486,37 @@
     if not test[4] == "":
       mock_error.assert_called()
       assert mock_error.call_args[0][0] == test[4]
       assert mock_error.call_args[0][1] == test[5]
       assert mock_error.call_args[0][2] == test[6]
       assert mock_error.call_args[0][3] == test[7]
 
-def test__state_split(mocker):
+def test__state_split(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data)
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   test_data = [
     ('111', ['111']),
     ('111,    ', ['111']),
     ('"111", 222, 333', ['111', '222', '333']),
     ('"111", 222, 333, "4"', ['111', '222', '333', '4']),
-    ('"111 \\" quote", 222, 333', ['111 " quote', '222', '333'])
+    ('"111 \\" quote", 222, 333', ['111 " quote', '222', '333']),
+    ('"111 \\" quote",,, 222, 333', ['111 " quote', '', '', '222', '333'])
   ]
   for test in test_data:
     assert(base._state_split(test[0])) == test[1]
 
   with pytest.raises(BaseSheet.FormatError):
     base._state_split('123, "456')
 
-def test__to_int(mocker):
+def test__to_int(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data)
-  base = BaseSheet("", "sheet")
+  base = BaseSheet("", globals, "sheet")
   assert(base._to_int("4")) == 4
   assert(base._to_int("dd")) == None
```

### Comparing `usdm-0.48.0/tests/test_cdisc_biomedical_concept.py` & `usdm-0.49.0/tests/test_cdisc_biomedical_concept.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
-from usdm_excel.cdisc_biomedical_concept import CDISCBiomedicalConcepts
+from usdm_excel.cdisc_bc_library import CDISCBCLibrary
 
 xfail = pytest.mark.xfail
 
-# def test_code(mocker):
-#     mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+# def test_code(mocker, globals):
+#     mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
 #     mock_id.side_effect=['Code_1']
 #     item = NCIt()
 #     code = item.code(code="CODE", decode="DECODE")
 #     assert code.codeId == "Code_1"
 #     assert code.code == "CODE"
 #     assert code.codeSystem == "NCI Thesaurus"
 #     assert code.codeSystemVersion == ""
@@ -34,18 +34,18 @@
 def test__get_package_metadata():
   assert 0
 
 @xfail
 def test__get_package_items(self):
   assert 0
   
-def test__url():
-  item = CDISCBiomedicalConcepts()
-  assert (item._url('something')) == f"{CDISCBiomedicalConcepts.API_ROOT}something"
+def test__url(globals):
+  item = CDISCBCLibrary(globals.errors_and_logging, globals.cdisc_ct_library, globals.id_manager)
+  assert (item._url('something')) == f"{CDISCBCLibrary.API_ROOT}something"
 
 @xfail
-def test__bc_as_usdm(mocker):
+def test__bc_as_usdm(mocker, globals):
   assert 0
 
 @xfail
 def test__bc_property_as_usdm(self, property, codes):
   assert 0
```

### Comparing `usdm-0.48.0/tests/test_configuration_sheet.py` & `usdm-0.49.0/tests/test_configuration_sheet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 import pandas as pd
 
 from usdm_excel.configuration_sheet import ConfigurationSheet
 from usdm_excel.option_manager import Options, EmptyNoneOption
-from usdm_excel import ct_version_manager as ctvm
-from usdm_excel import om
 
-def test_defaults(mocker):
+
+def test_defaults(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': ['Option X', 'Option 2', 'Option 3'], 'col_2': ['maybe', 'True', '']}
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data)
-  configuration = ConfigurationSheet("")
-  assert om.get(Options.EMPTY_NONE) == EmptyNoneOption.NONE.value
+  configuration = ConfigurationSheet("", globals)
+  assert globals.option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.NONE.value
 
-def test_sdr_deprecated(mocker):
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+def test_sdr_deprecated(mocker, globals):
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': ['sdr DESCRIPTION'], 'col_2': ['']}
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data)
-  configuration = ConfigurationSheet("")
+  configuration = ConfigurationSheet("", globals)
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "configuration"
   assert mock_error.call_args[0][1] == None
   assert mock_error.call_args[0][2] == None
   assert mock_error.call_args[0][3] == "The SDR DESCRIPTION option is now deprecated and will be ignored."
 
-def test_sdr_root_deprecated(mocker):
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+def test_sdr_root_deprecated(mocker, globals):
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': ['SDR root'], 'col_2': ['']}
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data)
-  configuration = ConfigurationSheet("")
+  configuration = ConfigurationSheet("", globals)
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "configuration"
   assert mock_error.call_args[0][1] == None
   assert mock_error.call_args[0][2] == None
   assert mock_error.call_args[0][3] == "The SDR ROOT option is now deprecated and will be ignored."
 
-def test_set_prev_next_deprecated(mocker):
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+def test_set_prev_next_deprecated(mocker, globals):
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': ['SDR prev next'], 'col_2': ['']}
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data)
-  configuration = ConfigurationSheet("")
+  configuration = ConfigurationSheet("", globals)
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "configuration"
   assert mock_error.call_args[0][1] == None
   assert mock_error.call_args[0][2] == None
   assert mock_error.call_args[0][3] == "The SDR PREV NEXT option is now deprecated and will be ignored."
```

### Comparing `usdm-0.48.0/tests/test_cross_reference.py` & `usdm-0.49.0/tests/test_cross_reference.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,83 +20,89 @@
 
   def __init__(self, id, name, instance):
     self.id = id
     self.name = name
     self.child = instance
     self.value = "VALUE"
 
-def test_create():
-  object = CrossRef()
-  assert len(object.references.keys()) == 0
-  assert object.references == {}
+def test_create(globals):
+  object = CrossRef(globals.errors_and_logging)
+  assert len(object._references.keys()) == 0
+  assert object._references == {}
 
-def test_clear():
+def test_clear(globals):
+  cross_references = globals.cross_references
   item = CRTest(id="1234", name="name")
-  cross_references.references = {}
-  cross_references.identifiers = {}
-  cross_references.references["CRTest.name"] = item
-  cross_references.identifiers["CRTest.1234"] = item
-  assert len(cross_references.references.keys()) == 1
-  assert len(cross_references.identifiers.keys()) == 1
+  cross_references._references = {}
+  cross_references._identifiers = {}
+  cross_references._references["CRTest.name"] = item
+  cross_references._identifiers["CRTest.1234"] = item
+  assert len(cross_references._references.keys()) == 1
+  assert len(cross_references._identifiers.keys()) == 1
   cross_references.clear()
-  assert len(cross_references.references.keys()) == 0
-  assert len(cross_references.identifiers.keys()) == 0
+  assert len(cross_references._references.keys()) == 0
+  assert len(cross_references._identifiers.keys()) == 0
 
-def test_add():
+def test_add(globals):
+  cross_references = globals.cross_references
   item = CRTest(id="1234", name="name")
   cross_references.clear()
-  assert len(cross_references.references.keys()) == 0
-  assert len(cross_references.identifiers.keys()) == 0
+  assert len(cross_references._references.keys()) == 0
+  assert len(cross_references._identifiers.keys()) == 0
   cross_references.add("name", item)
-  assert len(cross_references.references.keys()) == 1
-  assert cross_references.references["CRTest.name"] == item
-  assert len(cross_references.identifiers.keys()) == 1
-  assert cross_references.identifiers["CRTest.1234"] == item
+  assert len(cross_references._references.keys()) == 1
+  assert cross_references._references["CRTest.name"] == item
+  assert len(cross_references._identifiers.keys()) == 1
+  assert cross_references._identifiers["CRTest.1234"] == item
 
-def test_get():
+def test_get(globals):
+  cross_references = globals.cross_references
   item = CRTest(id="1234", name="name")
   cross_references.clear()
-  assert len(cross_references.references.keys()) == 0
-  assert len(cross_references.identifiers.keys()) == 0
-  cross_references.references["CRTest.name"] = item
+  assert len(cross_references._references.keys()) == 0
+  assert len(cross_references._identifiers.keys()) == 0
+  cross_references._references["CRTest.name"] = item
   assert cross_references.get(CRTest, "name") == item
 
-def test_get_by_id():
+def test_get_by_id(globals):
+  cross_references = globals.cross_references
   item = CRTest(id="1234", name="name")
   cross_references.clear()
-  assert len(cross_references.references.keys()) == 0
-  assert len(cross_references.identifiers.keys()) == 0
-  cross_references.identifiers["CRTest.1234"] = item
+  assert len(cross_references._references.keys()) == 0
+  assert len(cross_references._identifiers.keys()) == 0
+  cross_references._identifiers["CRTest.1234"] = item
   assert cross_references.get_by_id(CRTest, "1234") == item
   assert cross_references.get_by_id("CRTest", "1234") == item
 
-def test_get_by_path():
+def test_get_by_path(globals):
+  cross_references = globals.cross_references
   item1 = CRTest(id="1234", name="name1")
   item2 = CRTest2(id="1235", name="name2", instance=item1)
   item3 = CRTest3(id="1236", name="name3", instance=item2)
   cross_references.clear()
-  assert len(cross_references.references.keys()) == 0
-  assert len(cross_references.identifiers.keys()) == 0
+  assert len(cross_references._references.keys()) == 0
+  assert len(cross_references._identifiers.keys()) == 0
   cross_references.add("name1", item1)
   cross_references.add("name2", item2)  
   cross_references.add("name3", item3)
   instance, attribute = cross_references.get_by_path("CRTest3", "name3", "child/CRTest2/@child/CRTest/@value")
   assert instance.id == "1234"
   assert attribute == "value"
   instance, attribute = cross_references.get_by_path("CRTest3", "name3", "child/CRTest2/child/CRTest/@value")
   assert instance.id == "1234"
   assert attribute == "value"
 
-def test_get_by_path_errors():
+def test_get_by_path_errors(globals):
+  cross_references = globals.cross_references
   item1 = CRTest(id="1234", name="name1")
   item2 = CRTest2(id="1235", name="name2", instance=item1)
   item3 = CRTest3(id="1236", name="name3", instance=item2)
   cross_references.clear()
-  assert len(cross_references.references.keys()) == 0
-  assert len(cross_references.identifiers.keys()) == 0
+  assert len(cross_references._references.keys()) == 0
+  assert len(cross_references._identifiers.keys()) == 0
   cross_references.add("name1", item1)
   cross_references.add("name2", item2)  
   cross_references.add("name3", item3)
   with pytest.raises(cross_references.PathError) as ex_info:
     instance, attribute = cross_references.get_by_path("CRTest4", "name3", "child/CRTest2/@child/CRTest/@value")
   assert str(ex_info.value) == "Failed to translate reference path 'child/CRTest2/@child/CRTest/@value', could not find start instance 'CRTest4', 'name3'"
```

### Comparing `usdm-0.48.0/tests/test_data_factory.py` & `usdm-0.49.0/tests/test_data_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,28 +4,35 @@
 from usdm_model.study_arm import StudyArm
 from usdm_model.population_definition import *
 from usdm_model.study import Study
 from usdm_model.study_version import StudyVersion
 from usdm_model.study_title import StudyTitle
 from usdm_model.study_protocol_document import StudyProtocolDocument
 from usdm_model.study_protocol_document_version import StudyProtocolDocumentVersion
-
+from usdm_model.study_identifier import StudyIdentifier
+from usdm_model.organization import Organization
+from usdm_model.address import Address
+from usdm_excel.globals import Globals
 from tests.test_factory import Factory
 
 class MinimalStudy():
 
-  def __init__(self):
-    factory = Factory()
+  def __init__(self, globals: Globals):
+    globals.id_manager.clear()
+    factory = Factory(globals)
     self.population = factory.item(StudyDesignPopulation, {'name': 'POP1', 'label': '', 'description': '', 'includesHealthySubjects': True, 'criteria': []})
     cell = factory.item(StudyCell, {'armId': "X", 'epochId': "Y"})
     arm = factory.item(StudyArm, {'name': "Arm1", 'type': factory.cdisc_dummy(), 'dataOriginDescription': 'xxx', 'dataOriginType': factory.cdisc_dummy()})
     epoch = factory.item(StudyEpoch, {'name': 'EP1', 'label': 'Epoch A', 'description': '', 'type': factory.cdisc_dummy()})
     study_title = factory.item (StudyTitle, {'text': 'Title', 'type': factory.cdisc_dummy()})
     self.protocl_document_version = factory.item(StudyProtocolDocumentVersion, {'protocolVersion': '1', 'protocolStatus': factory.cdisc_dummy()})
     self.protocl_document = factory.item(StudyProtocolDocument, {'name': 'EP1', 'label': 'Epoch A', 'description': '', 'versions': [self.protocl_document_version]})
     self.study_design = factory.item(StudyDesign, {'name': 'Study Design', 'label': '', 'description': '', 
       'rationale': 'XXX', 'interventionModel': factory.cdisc_dummy(), 'arms': [arm], 'studyCells': [cell], 
       'epochs': [epoch], 'population': self.population})
+    address = factory.item(Address, {'line': 'line 1', 'city': 'City', 'district': 'District', 'state': 'State', 'postalCode': '12345', 'country': factory.code("UKK", "UKK_decode")})
+    organization = factory.item(Organization, {'name': 'Sponsor', 'organizationType': factory.cdisc_code("C70793", "sponsor"), 'identifier': "123456789", 'identifierScheme': "DUNS", 'legalAddress': address}) 
+    identifier = factory.item(StudyIdentifier, {'studyIdentifier': 'SPONSOR-1234', 'studyIdentifierScope': organization})
     self.study_version = factory.item(StudyVersion, {'versionIdentifier': '1', 'rationale': 'XXX', 'titles': [study_title], 'studyDesigns': [self.study_design], 
-                                                     'documentVersionId': self.protocl_document_version.id}) 
+                                                     'documentVersionId': self.protocl_document_version.id, 'studyIdentifiers': [identifier]}) 
     self.study = factory.item(Study, {'id': None, 'name': 'Study', 'label': '', 'description': '', 'versions': [self.study_version], 'documentedBy': self.protocl_document})
```

### Comparing `usdm-0.48.0/tests/test_document.py` & `usdm-0.49.0/tests/test_document.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,30 @@
 
 from yattag import Doc
 from usdm_model.eligibility_criterion import EligibilityCriterion
 from usdm_model.narrative_content import NarrativeContent
-from usdm_excel.document.document import Document
-
+from usdm_db.document.document import Document
 from tests.test_factory import Factory
-from tests.test_data_factory import MinimalStudy
-from tests.test_utility import clear as tu_clear
-
-factory = Factory()
 
-INCLUSION = factory.cdisc_code('C25532', 'Inc')
-EXCLUSION = factory.cdisc_code('C25370', 'Exc')
-
-def create_criteria():
+def create_criteria(factory):
+  INCLUSION = factory.cdisc_code('C25532', 'Inc')
+  EXCLUSION = factory.cdisc_code('C25370', 'Exc')
   item_list = [
     {'name': 'IE1', 'label': '', 'description': '', 'text': 'Only perform at baseline', 
      'dictionaryId': None, 'category': INCLUSION, 'identifier': '01', 'nextId': None, 'previousId': None, 'contextId': None
     },
     {'name': 'IE2', 'label': '', 'description': '', 'text': '<p>Only perform on males</p>', 
     'dictionaryId': None, 'category': INCLUSION, 'identifier': '02', 'nextId': None, 'previousId': None, 'contextId': None
     },
   ]
   results = factory.set(EligibilityCriterion, item_list)
   return results
 
-
-def test_create(mocker):
-  tu_clear()
-  minimal = MinimalStudy()
-  minimal.population.criteria = create_criteria()
-  bs = factory.base_sheet(mocker)
+def test_create(mocker, globals, minimal, factory):
+  minimal.population.criteria = create_criteria(factory)
   doc = Doc()
-  document = Document(bs, "xxx", minimal.study, "")
+  document = Document("xxx", minimal.study, globals.errors_and_logging)
   content = factory.item(NarrativeContent, {'name': "C1", 'sectionNumber': '1.1.1', 'sectionTitle': 'Section Title', 'text': '<usdm:macro id="section" name="inclusion"/>', 'childIds': []})
   document._content_to_html(content, doc)
   result = doc.getvalue()
   expected = '<div class=""><h3 id="section-1.1.1">1.1.1 Section Title</h3><usdm:macro id="section" name="inclusion"></usdm:macro></div>'
   assert result == expected
```

### Comparing `usdm-0.48.0/tests/test_document_macros.py` & `usdm-0.49.0/tests/test_document_template_plain.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,29 @@
+import pandas as pd
 from usdm_model.eligibility_criterion import EligibilityCriterion
-from usdm_excel.document.macros import Macros
+from usdm_excel.document.template_plain import TemplatePlain
 
-from tests.test_factory import Factory
-from tests.test_data_factory import MinimalStudy
-from tests.test_utility import clear as tu_clear
-
-factory = Factory()
-
-INCLUSION = factory.cdisc_code('C25532', 'Inc')
-EXCLUSION = factory.cdisc_code('C25370', 'Exc')
-
-def create_criteria():
+def create_criteria(factory):
+  INCLUSION = factory.cdisc_code('C25532', 'Inc')
+  EXCLUSION = factory.cdisc_code('C25370', 'Exc')
   item_list = [
     {'name': 'IE1', 'label': '', 'description': '', 'text': 'Only perform at baseline', 
      'dictionaryId': None, 'category': INCLUSION, 'identifier': '01', 'nextId': None, 'previousId': None, 'contextId': None
     },
     {'name': 'IE2', 'label': '', 'description': '', 'text': '<p>Only perform on males</p>', 
     'dictionaryId': None, 'category': INCLUSION, 'identifier': '02', 'nextId': None, 'previousId': None, 'contextId': None
     },
   ]
   results = factory.set(EligibilityCriterion, item_list)
   return results
 
-def test_create(mocker):
-  tu_clear()
-  minimal = MinimalStudy()
-  minimal.population.criteria = create_criteria()
+def test_create(mocker, globals, minimal, factory):
+  globals.id_manager.clear()
+  minimal.population.criteria = create_criteria(factory)
   bs = factory.base_sheet(mocker)
-  macro = Macros(bs, minimal.study)
-  result = macro.resolve('<usdm:macro id="section" name="inclusion"/>')
-  expected = '<table class="table"><tr><td>01</td><td><usdm:ref attribute="text" '\
-    'id="EligibilityCriterion_1" klass="EligibilityCriterion"></usdm:ref></td></tr><tr><td>02'\
-    '</td><td><usdm:ref attribute="text" id="EligibilityCriterion_2" klass="EligibilityCriterion">'\
-    '</usdm:ref></td></tr></table>'
+  template = TemplatePlain(bs, minimal.study)
+  result = template.inclusion({})
+  expected = '<table class="table"><tr><td>01</td><td><usdm:ref klass="EligibilityCriterion" '\
+    'id="EligibilityCriterion_1" attribute="text"></usdm:ref></td></tr><tr><td>02</td><td>'\
+    '<usdm:ref klass="EligibilityCriterion" id="EligibilityCriterion_2" attribute="text"></usdm:ref>'\
+    '</td></tr></table>'
   assert result == expected
```

### Comparing `usdm-0.48.0/tests/test_document_soa.py` & `usdm-0.49.0/tests/test_document_soa.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,26 @@
 from bs4 import BeautifulSoup   
-from usdm_excel.cross_ref import cross_references
-from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.cdisc_ct import CDISCCT
 from usdm_excel.document.soa import SoA
 from usdm_model.activity import Activity
 from usdm_model.study_epoch import StudyEpoch
 from usdm_model.study_cell import StudyCell
 from usdm_model.study_arm import StudyArm
 from usdm_model.encounter import Encounter
 from usdm_model.study_design import StudyDesign
 from usdm_model.schedule_timeline import ScheduleTimeline
 from usdm_model.scheduled_instance import ScheduledActivityInstance
 from usdm_model.schedule_timeline_exit import ScheduleTimelineExit
 from usdm_model.timing import Timing
 from usdm_model.condition import Condition
 
-from tests.test_factory import Factory
-from tests.test_utility import clear as tu_clear
-
-factory = Factory()
-
-FIXED = factory.cdisc_code('C201358', 'Fixed Reference')
-BEFORE = factory.cdisc_code('C201356', 'After')
-AFTER = factory.cdisc_code('C201357', 'Before')
-
-E2E = factory.cdisc_code('C201352', 'End to End')
-E2S = factory.cdisc_code('C201353', 'End to Start')
-S2E = factory.cdisc_code('C201354', 'Start to End')
-S2S = factory.cdisc_code('C201355', 'Start to Start')
-
-def translate_reference(text):
+def translate_reference(text, globals):
   soup = BeautifulSoup(str(text), 'html.parser')
   for ref in soup(['usdm:ref']):
     attributes = ref.attrs
-    instance = cross_references.get_by_id(attributes['klass'], attributes['id'])
+    instance = globals.cross_references.get_by_id(attributes['klass'], attributes['id'])
     value = str(getattr(instance, attributes['attribute']))
     ref.replace_with(value)
   return str(soup)
 
 def double_link(items, prev, next):
   for idx, item in enumerate(items):
     if idx == 0:
@@ -47,93 +30,102 @@
       setattr(item, prev, the_id)
     if idx == len(items)-1:  
       setattr(item, next, None)
     else:
       the_id = getattr(items[idx+1], 'id')
       setattr(item, next, the_id)
 
-def add_cross_ref(collection):
+def add_cross_ref(collection, globals):
   for item in collection:
-    cross_references.add(item.id, item)
+    globals.cross_references.add(item.id, item)
 
-def create_conditions():
+def create_conditions(factory, globals):
   item_list = [
     {'name': 'COND1', 'label': '', 'description': '', 'text': 'Only perform at baseline', 'appliesToIds': [], 'contextIds': []},
     {'name': 'COND2', 'label': '', 'description': '', 'text': 'Only perform on males', 'appliesToIds': [], 'contextIds': []},
   ]
   results = factory.set(Condition, item_list)
-  add_cross_ref(results)
+  add_cross_ref(results, globals)
   return results
 
-def create_timings():
+def create_timings(factory, globals):
+  FIXED = factory.cdisc_code('C201358', 'Fixed Reference')
+  BEFORE = factory.cdisc_code('C201356', 'After')
+  AFTER = factory.cdisc_code('C201357', 'Before')
+
+  E2E = factory.cdisc_code('C201352', 'End to End')
+  E2S = factory.cdisc_code('C201353', 'End to Start')
+  S2E = factory.cdisc_code('C201354', 'Start to End')
+  S2S = factory.cdisc_code('C201355', 'Start to Start')
+
   item_list = [
     {'name': 'T1', 'label': '-2 Days', 'description': '', 'type': BEFORE, 'value': '', 'valueLabel': '', 'relativeToFrom': S2S, 'relativeFromScheduledInstanceId': '', 'relativeToScheduledInstanceId': '', 'windowLower': '', 'windowUpper': '', 'windowLabel': ''},
     {'name': 'T2', 'label': 'Dose',    'description': '', 'type': FIXED,  'value': '', 'valueLabel': '', 'relativeToFrom': S2S, 'relativeFromScheduledInstanceId': '', 'relativeToScheduledInstanceId': '', 'windowLower': '', 'windowUpper': '', 'windowLabel': ''},
     {'name': 'T3', 'label': '7 Days',  'description': '', 'type': AFTER,  'value': '', 'valueLabel': '', 'relativeToFrom': S2S, 'relativeFromScheduledInstanceId': '', 'relativeToScheduledInstanceId': '', 'windowLower': '', 'windowUpper': '', 'windowLabel': '1..1 Days'}
   ]
   results = factory.set(Timing, item_list)
-  add_cross_ref(results)
+  add_cross_ref(results, globals)
   return results
 
-def create_activities():
+def create_activities(factory, globals):
   item_list = [
     {'name': 'A1', 'label': 'Activity 1', 'description': '', 'definedProcedures': [], 'biomedicalConceptIds': [], 'bcCategoryIds': [], 'bcSurrogateIds': [], 'timelineId': None},
     {'name': 'A2', 'label': 'Activity 2', 'description': '', 'definedProcedures': [], 'biomedicalConceptIds': [], 'bcCategoryIds': [], 'bcSurrogateIds': [], 'timelineId': None},
     {'name': 'A3', 'label': 'Activity 3', 'description': '', 'definedProcedures': [], 'biomedicalConceptIds': [], 'bcCategoryIds': [], 'bcSurrogateIds': [], 'timelineId': None},
     {'name': 'A4', 'label': 'Activity 4', 'description': '', 'definedProcedures': [], 'biomedicalConceptIds': [], 'bcCategoryIds': [], 'bcSurrogateIds': [], 'timelineId': None},
     {'name': 'A5', 'label': 'Activity 5', 'description': '', 'definedProcedures': [], 'biomedicalConceptIds': [], 'bcCategoryIds': [], 'bcSurrogateIds': [], 'timelineId': None}
   ]
   results = factory.set(Activity, item_list)
   double_link(results, 'previousId', 'nextId')
-  add_cross_ref(results)
+  add_cross_ref(results, globals)
   return results
 
-def create_epochs():
+def create_epochs(factory, globals):
   item_list = [
     {'name': 'EP1', 'label': 'Epoch A', 'description': '', 'type': factory.cdisc_dummy()},
     {'name': 'EP2', 'label': 'Epoch B', 'description': '', 'type': factory.cdisc_dummy()},
     {'name': 'EP3', 'label': 'Epoch C', 'description': '', 'type': factory.cdisc_dummy()},
   ]
   results = factory.set(StudyEpoch, item_list)
   double_link(results, 'previousId', 'nextId')
-  add_cross_ref(results)
+  add_cross_ref(results, globals)
   return results
 
-def create_encounters():
+def create_encounters(factory, globals):
   item_list = [
     {'name': 'E1', 'label': 'Screening', 'description': '', 'type': factory.cdisc_dummy(), 'environmentalSetting': [], 'contactModes': [], 'transitionStartRule': None, 'transitionEndRule': None, 'scheduledAtId': None},
     {'name': 'E2', 'label': 'Dose', 'description': '', 'type': factory.cdisc_dummy(), 'environmentalSetting': [], 'contactModes': [], 'transitionStartRule': None, 'transitionEndRule': None, 'scheduledAtId': None},
     {'name': 'E3', 'label': 'Check Up', 'description': '', 'type': factory.cdisc_dummy(), 'environmentalSetting': [], 'contactModes': [], 'transitionStartRule': None, 'transitionEndRule': None, 'scheduledAtId': None}
   ]
   results = factory.set(Encounter, item_list)
   double_link(results, 'previousId', 'nextId')
-  add_cross_ref(results)
+  add_cross_ref(results, globals)
   return results
 
-def create_activity_instances():
+def create_activity_instances(factory, globals):
   item_list = [
     {'name': 'SAI_1', 'description': '', 'label': '', 'timelineExitId': None, 'encounterId': None, 'scheduledInstanceTimelineId': None, 'defaultConditionId': None, 'epochId': None, 'activityIds': []},
     {'name': 'SAI_2', 'description': '', 'label': '', 'timelineExitId': None, 'encounterId': None, 'scheduledInstanceTimelineId': None, 'defaultConditionId': None, 'epochId': None, 'activityIds': []},
     {'name': 'SAI_3', 'description': '', 'label': '', 'timelineExitId': None, 'encounterId': None, 'scheduledInstanceTimelineId': None, 'defaultConditionId': None, 'epochId': None, 'activityIds': []}
   ]
   results = factory.set(ScheduledActivityInstance, item_list)
   results[0].defaultConditionId = results[1].id
   results[1].defaultConditionId = results[2].id
-  add_cross_ref(results)
+  add_cross_ref(results, globals)
   return results
 
-def scenario_1():
+def scenario_1(factory, globals):
   dummy_cell = factory.item(StudyCell, {'armId': "X", 'epochId': "Y"})
   dummy_arm = factory.item(StudyArm, {'name': "Arm1", 'type': factory.cdisc_dummy(), 'dataOriginDescription': 'xxx', 'dataOriginType': factory.cdisc_dummy()})
-  activities = create_activities()
-  epochs = create_epochs()
-  encounters = create_encounters()
-  activity_instances = create_activity_instances()
-  timings = create_timings()
-  conditions = create_conditions()
+  activities = create_activities(factory, globals)
+  epochs = create_epochs(factory, globals)
+  encounters = create_encounters(factory, globals)
+  activity_instances = create_activity_instances(factory, globals)
+  timings = create_timings(factory, globals)
+  conditions = create_conditions(factory, globals)
 
   activity_instances[0].activityIds = [activities[0].id, activities[1].id]
   activity_instances[0].encounterId = encounters[0].id
   activity_instances[0].epochId = epochs[0].id
   activity_instances[1].activityIds = [activities[1].id, activities[2].id]
   activity_instances[1].encounterId = encounters[1].id
   activity_instances[1].epochId = epochs[1].id
@@ -156,29 +148,28 @@
   study_design = factory.item(StudyDesign, {'name': 'Study Design', 'label': '', 'description': '', 
     'rationale': 'XXX', 'interventionModel': factory.cdisc_dummy(),
     'arms': [dummy_arm], 'studyCells': [dummy_cell], 'epochs': epochs,
     'activities': activities, 'scheduledTimelines': [timeline],
     'conditions': conditions})
   return study_design, timeline
 
-def test_create(mocker):
-  tu_clear()
+def test_create(mocker, globals, factory):
   bs = factory.base_sheet(mocker)
-  study_design, timeline = scenario_1()
+  study_design, timeline = scenario_1(factory, globals)
   soa = SoA(bs, study_design, timeline)
   result = soa.generate()
-  print(f"RESULT: {result}")
+  #print(f"RESULT: {result}")
   labels = []
   for row in range(len(result)):
     labels.append([])
     for col in range(len(result[row])):
       if 'set' in result[row][col].keys():
         label = 'X' if result[row][col]['set'] else ''
       else:
-        label = translate_reference(result[row][col]['label'])
+        label = translate_reference(result[row][col]['label'], globals)
       if 'condition' in result[row][col].keys():
         label = f"{label} [c]"
       labels[row].append(label)
   assert labels == [
     #['',           '0',            '1',            '2'], 
     ['',           'Epoch A',      'Epoch B',      'Epoch C'],
     ['',           'Screening',    'Dose',         'Check Up'],
```

### Comparing `usdm-0.48.0/tests/test_error.py` & `usdm-0.49.0/tests/test_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from usdm_excel.errors.error import Error
+from usdm_excel.errors_and_logging.error import Error
 
 def test_create():
   error = Error(sheet="My Sheet", row=1, column=99, message="XXXXX")
   assert error.sheet == "My Sheet"
   assert error.row == 1
   assert error.column == 99
   assert error.message == "XXXXX"
```

### Comparing `usdm-0.48.0/tests/test_errors.py` & `usdm-0.49.0/tests/test_errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-from usdm_excel.errors.errors import Errors
+from usdm_excel.errors_and_logging.errors import Errors
 
-def test_create():
+
+def test_create(globals):
   errors = Errors()
   assert errors.items == []
 
-def test_add():
+def test_add(globals):
   errors = Errors()
   assert len(errors.items) == 0
   errors.add(sheet="My Sheet", row=1, column=99, message="XXXXX")
   assert len(errors.items) == 1
   assert errors.items[0].message == "XXXXX"
     
-def test_count():
+def test_count(globals):
   errors = Errors()
   errors.add(sheet="My Sheet", row=1, column=99, message="XXXXX")
   errors.add(sheet="My Sheet", row=1, column=99, message="XXXXX")
   assert errors.count() == 2
 
-def test_clear():
+def test_clear(globals):
   errors = Errors()
   assert len(errors.items) == 0
   errors.add(sheet="My Sheet", row=1, column=99, message="XXXXX")
   assert len(errors.items) == 1
   errors.clear()
   assert len(errors.items) == 0
 
-def test_dumo():
+def test_dumo(globals):
   errors = Errors()
   errors.add(sheet="My Sheet", row=1, column=99, message="XXXXX1")
   errors.add(sheet="My Sheet", row=2, column=100, message="XXXXX2")
   errors.add(sheet="My Sheet", row=3, column=101, message="XXXXX3", level=Errors.WARNING)
   errors.add(sheet="My Sheet", row=4, column=102, message="XXXXX4", level=Errors.INFO)
   errors.add(sheet="My Sheet", row=5, column=103, message="XXXXX5", level=Errors.DEBUG)
   assert (errors.dump(Errors.DEBUG)) == [
```

### Comparing `usdm-0.48.0/tests/test_export.py` & `usdm-0.49.0/tests/test_export.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import yaml
 import csv
 from usdm_excel import USDMExcel
+from usdm_db import USDMDb
 from uuid import UUID
 
 SAVE_ALL = False
 
 def to_int(value):
   try:
     return int(value)
@@ -17,31 +18,32 @@
   for item in items:
     item['row'] = to_int(item['row'])
     item['column'] = to_int(item['column'])
   return items
 
 def run_test(filename, mocker, save=False):
   fake_uuids = (UUID(f'00000000-0000-4000-8000-{i:012}', version=4) for i in range(10000))
-  mocker.patch("usdm_excel.export_as_neo4j_dict.uuid4", side_effect=fake_uuids)
-  excel = USDMExcel(f"tests/integration_test_files/{filename}.xlsx")
-  result = excel.to_neo4j_dict()
+  mocker.patch("usdm_db.neo4j_dict.uuid4", side_effect=fake_uuids)
+  usdm = USDMDb()
+  usdm.from_excel(f"tests/integration_test_files/{filename}.xlsx")
+  result = usdm.to_neo4j_dict()
 
   # Useful if you want to see the results.
   if save or SAVE_ALL:
     with open(f"tests/integration_test_files/{filename}_neo4j_dict.yaml", 'w') as f:
       f.write(yaml.dump(result))
   
   with open(f"tests/integration_test_files/{filename}_neo4j_dict.yaml", 'r') as f:
     expected = yaml.safe_load(f) 
   assert result == expected
 
-def test_simple_1(mocker):
+def test_simple_1(mocker, globals):
   run_test('simple_1', mocker)
 
-def test_full_1(mocker):
+def test_full_1(mocker, globals):
   run_test('full_1', mocker)
 
-def test_full_2(mocker):
+def test_full_2(mocker, globals):
   run_test('full_2', mocker)
 
-def test_full_3(mocker):
+def test_full_3(mocker, globals):
   run_test('full_3', mocker)
```

### Comparing `usdm-0.48.0/tests/test_factory.py` & `usdm-0.49.0/tests/test_factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pandas as pd
-from usdm_excel.id_manager import id_manager
 from usdm_excel.base_sheet import BaseSheet
-from usdm_excel.cdisc_ct import CDISCCT
+from usdm_model.code import Code
+from usdm_model.alias_code import AliasCode
 
 class Factory():
 
-  def __init__(self):
-    self.cdisc_ct = CDISCCT()
-  
+  def __init__(self, globals):
+    self.globals = globals
+
   def item(self, cls, params):
-    params['id'] = params['id'] if 'id' in params else id_manager.build_id(cls)
+    params['id'] = params['id'] if 'id' in params else self.globals.id_manager.build_id(cls)
     params['instanceType'] = cls.__name__
     return cls(**params)
 
   def set(self, cls, item_list):
     results = []
     for item in item_list:
       results.append(self.item(cls, item))
@@ -21,14 +21,23 @@
 
   def base_sheet(self, mocker):
     mocked_open = mocker.mock_open(read_data="File")
     mocker.patch("builtins.open", mocked_open)
     data = []
     mock_read = mocker.patch("pandas.read_excel")
     mock_read.return_value = pd.DataFrame(data, columns=[])
-    return BaseSheet("", "")
+    return BaseSheet("", self.globals, "")
+
+  def code(self, code, decode):
+    return self._build_code(code=code, system="yyy", version="2", decode=decode)
 
   def cdisc_code(self, code, decode):
-    return self.cdisc_ct.code(code, decode)
+    return self._build_code(code=code, system="xxx", version="1", decode=decode)
   
   def cdisc_dummy(self):
-    return self.cdisc_ct.code("C12345", "decode")
+    return self.cdisc_code("C12345", "decode")
+
+  def alias_code(self, standard_code, alias_codes=[]):
+    return self.item(AliasCode, {'standardCode': standard_code, 'standardCodeAliases': alias_codes})
+
+  def _build_code(self, code, system, version, decode):
+    return self.item(Code, {'code': code, 'codeSystem': system, 'codeSystemVersion': version, 'decode': decode})
```

### Comparing `usdm-0.48.0/tests/test_integration.py` & `usdm-0.49.0/tests/test_integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import csv
 from usdm_excel import USDMExcel
+from usdm_db import USDMDb
 from bs4 import BeautifulSoup
 
-SAVE_ALL =False
+SAVE_ALL = False
 
 def save_error_csv(file, contents):
   writer = csv.DictWriter(file, fieldnames=['sheet','row','column','message','level'])
   writer.writeheader()
   writer.writerows(contents)
 
 def to_int(value):
@@ -30,17 +31,18 @@
   return errors
 
 def format_html(result):
   soup = BeautifulSoup(result, 'html.parser')
   return soup.prettify()
 
 def run_test(filename, save=False):
-  excel = USDMExcel(f"tests/integration_test_files/{filename}.xlsx")
-  result = excel.to_json()
-  errors = excel.errors()
+  usdm = USDMDb()
+  errors = usdm.from_excel(f"tests/integration_test_files/{filename}.xlsx")
+  result = usdm.to_json()
+  #errors = excel.errors()
 
   # Useful if you want to see the results.
   if save or SAVE_ALL:
     with open(f"tests/integration_test_files/{filename}.json", 'w', encoding='utf-8') as f:
       f.write(json.dumps(json.loads(result), indent=2))
     with open(f"tests/integration_test_files/{filename}_errors.csv", 'w',newline='') as f:
       save_error_csv(f, errors) 
@@ -50,17 +52,17 @@
   assert result == expected
   with open(f"tests/integration_test_files/{filename}_errors.csv", 'r') as f:
     expected = read_error_csv(f)
   assert prep_errors_for_csv_compare(errors) == expected
 
 def run_test_html(filename, save=False, highlight=False):
   suffix = "_highlight" if highlight else ""
-  excel = USDMExcel(f"tests/integration_test_files/{filename}.xlsx")
-  result = excel.to_html(highlight)
-  errors = excel.errors()
+  usdm = USDMDb()
+  errors = usdm.from_excel(f"tests/integration_test_files/{filename}.xlsx")
+  result = usdm.to_html(highlight)
 
   # Useful if you want to see the results.
   if save or SAVE_ALL:
     with open(f"tests/integration_test_files/{filename}{suffix}.html", 'w') as f:
       f.write(format_html(result))
     with open(f"tests/integration_test_files/{filename}{suffix}_html_errors.csv", 'w',newline='') as f:
       save_error_csv(f, errors) 
@@ -68,69 +70,55 @@
   with open(f"tests/integration_test_files/{filename}{suffix}.html", 'r') as f:
     expected = f.read()
   assert format_html(result) == expected
   with open(f"tests/integration_test_files/{filename}{suffix}_html_errors.csv", 'r') as f:
     expected = read_error_csv(f)
   assert prep_errors_for_csv_compare(errors) == expected
 
-def run_test_timeline(filename, level=USDMExcel.FULL_HTML, save=False):
-  excel = USDMExcel(f"tests/integration_test_files/{filename}.xlsx")
-  result = excel.to_timeline(level)
+def run_test_timeline(filename, level=USDMDb.FULL_HTML, save=False):
+  usdm = USDMDb()
+  usdm.from_excel(f"tests/integration_test_files/{filename}.xlsx")
+  result = usdm.to_timeline(level)
 
   # Useful if you want to see the results.
   if save or SAVE_ALL:
     with open(f"tests/integration_test_files/{filename}_timeline_{level}.html", 'w') as f:
       f.write(result)
   
   with open(f"tests/integration_test_files/{filename}_timeline_{level}.html", 'r') as f:
     expected = f.read()
   assert result == expected
 
-def run_test_ne(filename, save=False):
-  result = {}
-  excel = USDMExcel(f"tests/integration_test_files/{filename}.xlsx")
-  result['n'], result['e'] = excel.to_nodes_and_edges()
-  for type in ['n', 'e']:
-
-    # Useful if you want to see the results.
-    if save or SAVE_ALL:
-      with open(f"tests/integration_test_files/{filename}_{type}.json", 'w', encoding='utf-8') as f:
-        f.write(json.dumps(result[type], indent=2))
-    
-    with open(f"tests/integration_test_files/{filename}_{type}.json", 'r') as f:
-      expected = json.load(f)
-    assert result[type] == expected
-
 def test_full_1():
   run_test('full_1')
 
 def test_full_1_timeline():
   run_test_timeline('full_1')
 
 def test_full_1_timeline_body():
-  run_test_timeline('full_1', USDMExcel.BODY_HTML)
+  run_test_timeline('full_1', USDMDb.BODY_HTML)
 
 def test_full_1_html():
   run_test_html('full_1')
 
-def test_full_1_ne():
-  run_test_ne('full_1')
-
 def test_full_2():
   run_test('full_2')
 
 def test_full_2_html():
   run_test_html('full_2')
 
 def test_full_3():
   run_test('full_3')
 
 def test_full_3_html():
   run_test_html('full_3')
 
+def test_full_4():
+  run_test('full_4')
+
 def test_encounter_1():
   run_test('encounter_1')
 
 def test_simple_1():
   run_test('simple_1')
 
 def test_scope_1():
@@ -138,17 +126,14 @@
 
 def test_amendment_1():
   run_test('amendment_1')
 
 def test_eligibility_criteria_1():
   run_test('eligibility_criteria_1')
 
-def test_simple_1_ne():
-  run_test_ne('simple_1')
-
 def test_simple_1_html():
   run_test_html('simple_1')
 
 def test_config_1():
   run_test('config_1')
 
 def test_config_2():
@@ -159,29 +144,20 @@
 
 def test_address_comma():
   run_test('address')
 
 def test_complex_1():
   run_test('complex_1')
 
-def test_complex_1_ne():
-  run_test_ne('complex_1')
-
 def test_arms_epochs_1():
   run_test('arms_epochs')
 
-def test_arms_epochs_1_ne():
-  run_test_ne('arms_epochs')
-
 def test_cycles_1():
   run_test('cycles_1')
 
-def test_cycles_1_ne():
-  run_test_ne('cycles_1')
-
 def test_multiple_column_names():
   run_test('multiple_column_names')
 
 def test_invalid_section_levels():
   run_test('invalid_section_levels')
 
 def test_new_field_names():
```

### Comparing `usdm-0.48.0/tests/test_iso_3166.py` & `usdm-0.49.0/tests/test_iso_3166.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from usdm_excel.iso_3166 import ISO3166
 
-def test_code(mocker):
-    mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+
+def test_code(mocker, globals):
+    mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
     mock_id.side_effect=['Code_1', 'Code_2', 'Code_3']
-    item = ISO3166()
+    item = ISO3166(globals)
     code = item.code("GB")
     assert code.id == "Code_1"
     assert code.code == "GBR"
     assert code.codeSystem == "ISO 3166 1 alpha3"
     assert code.codeSystemVersion == "2020-08"
     assert code.decode == "United Kingdom of Great Britain and Northern Ireland"
     code = item.code("GBR")
@@ -19,18 +20,18 @@
     code = item.code("XXX")
     assert code.id == "Code_3"
     assert code.code == "DNK"
     assert code.codeSystem == "ISO 3166 1 alpha3"
     assert code.codeSystemVersion == "2020-08"
     assert code.decode == "Denmark"
 
-def test_region_code(mocker):
-    mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+def test_region_code(mocker, globals):
+    mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
     mock_id.side_effect=['Code_1', 'Code_2', 'Code_3', 'Code_4']
-    item = ISO3166()
+    item = ISO3166(globals)
     code = item.region_code("Americas")
     assert code.id == "Code_1"
     assert code.code == "019"
     assert code.codeSystem == "ISO 3166 1 alpha3"
     assert code.codeSystemVersion == "2020-08"
     assert code.decode == "Americas"
     code = item.region_code("South America")
```

### Comparing `usdm-0.48.0/tests/test_iso_8601_duration.py` & `usdm-0.49.0/tests/test_iso_8601_duration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from usdm_excel.iso_8601_duration import ISO8601Duration
 
-def test_encode(mocker):
+def test_encode(mocker, globals):
   item = ISO8601Duration()
   assert item.encode("1", "y") == "P1Y"
   assert item.encode("2", "yeaR") == "P2Y"
   assert item.encode("2", "years") == "P2Y"
   assert item.encode("3", "yrs") == "P3Y"
   assert item.encode("3", "yr") == "P3Y"
   assert item.encode("1", "MTHS") == "P1M"
```

### Comparing `usdm-0.48.0/tests/test_option_manager.py` & `usdm-0.49.0/tests/test_option_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from usdm_excel.option_manager import *
 
-def test_create():
-  object = OptionManager()
-  assert len(object.items.keys()) == 0
-  assert object.items == {}
-
-def test_set():
-  option_manager.items = {}
-  option_manager.set('fred', 'value')
-  assert len(option_manager.items.keys()) == 1
-  assert option_manager.items['fred'] == 'value'
-
-def test_get():
-  option_manager.items = {}
-  option_manager.items['fred'] = 'value'
-  assert option_manager.get('fred') == 'value'
-
-def test_clear():
-  option_manager.items = {}
-  option_manager.items['fred'] = 'value'
-  assert len(option_manager.items.keys()) == 1
-  option_manager.clear()
-  assert len(option_manager.items.keys()) == 0
-
-def test_options():
-  option_manager.set(Options.EMPTY_NONE, EmptyNoneOption.NONE)
-  assert option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.NONE.value
-  option_manager.set(Options.EMPTY_NONE, EmptyNoneOption.EMPTY)
-  assert option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value
-  option_manager.set(Options.USDM_VERSION, 2)
-  assert option_manager.get(Options.USDM_VERSION) == '2'
-  option_manager.set(Options.USDM_VERSION, 3)
-  assert option_manager.get(Options.USDM_VERSION) == '3'
-  # option_manager.set(Options.ROOT, RootOption.API_COMPLIANT)
-  # assert option_manager.get(Options.ROOT) == RootOption.API_COMPLIANT.value
-  # option_manager.set(Options.DESCRIPTION, 'Some text')
-  # assert option_manager.get(Options.DESCRIPTION) == 'Some text'
+
+def test_create(globals):
+  object = OptionManager(globals)
+  assert len(object._items.keys()) == 0
+  assert object._items == {}
+
+def test_set(globals):
+  globals.option_manager._items = {}
+  globals.option_manager.set('fred', 'value')
+  assert len(globals.option_manager._items.keys()) == 1
+  assert globals.option_manager._items['fred'] == 'value'
+
+def test_get(globals):
+  globals.option_manager._items = {}
+  globals.option_manager._items['fred'] = 'value'
+  assert globals.option_manager.get('fred') == 'value'
+
+def test_clear(globals):
+  globals.option_manager._items = {}
+  globals.option_manager._items['fred'] = 'value'
+  assert len(globals.option_manager._items.keys()) == 1
+  globals.option_manager.clear()
+  assert len(globals.option_manager._items.keys()) == 0
+
+def test_options(globals):
+  globals.option_manager.set(Options.EMPTY_NONE, EmptyNoneOption.NONE)
+  assert globals.option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.NONE.value
+  globals.option_manager.set(Options.EMPTY_NONE, EmptyNoneOption.EMPTY)
+  assert globals.option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value
+  globals.option_manager.set(Options.USDM_VERSION, 2)
+  assert globals.option_manager.get(Options.USDM_VERSION) == '2'
+  globals.option_manager.set(Options.USDM_VERSION, 3)
+  assert globals.option_manager.get(Options.USDM_VERSION) == '3'
+  # globals.option_manager.set(Options.ROOT, RootOption.API_COMPLIANT)
+  # assert globals.option_manager.get(Options.ROOT) == RootOption.API_COMPLIANT.value
+  # globals.option_manager.set(Options.DESCRIPTION, 'Some text')
+  # assert globals.option_manager.get(Options.DESCRIPTION) == 'Some text'
```

### Comparing `usdm-0.48.0/tests/test_quantity_type.py` & `usdm-0.49.0/tests/test_quantity_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,63 @@
+from tests.test_factory import Factory
 from usdm_excel.quantity_type import QuantityType
 
-def test_quantity_type(mocker):
+def test_quantity_type(mocker, globals):
   test_data = [
     ('15 days', "15", 'days', 'C25301', '15 days'),
     ('1%', "1", '%', 'C25613', '1%'),
     ('  10    %', "10", '%', 'C25613', '10    %'),
   ]
   for index, test in enumerate(test_data):
-    item = QuantityType(test[0])
+    item = QuantityType(test[0], globals)
     assert(item.value) == test[1]
     assert(item.units) == test[2]
     assert(item.units_code.code) == test[3]
     assert(item.errors) == [] 
     assert(item.empty) == False
     assert(item.label) == test[4]
 
-def test_quantity_type_empty(mocker):
+def test_quantity_type_empty(mocker, globals):
   test_data = [
     ('15 days', "15", 'days', 'C25301', False, '15 days'),
     ('', None, None, None, True, ''),
   ]
   for index, test in enumerate(test_data):
-    item = QuantityType(test[0], allow_empty=True)
+    item = QuantityType(test[0], globals, allow_empty=True)
     assert(item.value) == test[1]
     assert(item.units) == test[2]
     if test[3]:
       assert(item.units_code.code) == test[3]
     else:
       assert(item.units_code) == test[3]
     assert(item.errors) == [] 
     assert(item.empty) == test[4]
     assert(item.label) == test[5]
 
-def test_quantity_type_no_units(mocker):
+def test_quantity_type_no_units(mocker, globals):
   test_data = [
     (' 15 ', "15", None, None, False, '15'),
     (' 15 C ', "15", 'C', 'C42559', False, '15 C')
   ]
   for index, test in enumerate(test_data):
     #print(f"TEST {test}")
-    item = QuantityType(test[0], allow_missing_units=True)
+    item = QuantityType(test[0], globals, allow_missing_units=True)
     assert(item.value) == test[1]
     assert(item.units) == test[2]
     if test[3]:
       assert(item.units_code.code) == test[3]
     else:
       assert(item.units_code) == test[3]
     assert(item.errors) == [] 
     assert(item.empty) == test[4]
     assert(item.label) == test[5]
 
-def test_range_type_error(mocker):
+def test_range_type_error(mocker, globals):
   test_data = [
     (' Days', False, False, "Could not decode the quantity value ' Days'"),
     ('1', False, False, "Could not decode the quantity value, possible typographical errors '1'"),
     ('abc', False, False, "Could not decode the quantity value 'abc'"),
     ('10 slugs', False, False, "Unable to set the units code for the quantity '10 slugs'")
   ]
   for index, test in enumerate(test_data):
-    item = QuantityType(test[0], allow_missing_units=test[1], allow_empty=test[2])
+    item = QuantityType(test[0], globals, allow_missing_units=test[1], allow_empty=test[2])
     assert item.errors == [test[3]]
```

### Comparing `usdm-0.48.0/tests/test_range_type.py` & `usdm-0.49.0/tests/test_range_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
+from tests.test_factory import Factory
 from usdm_excel.range_type import RangeType
 
-def test_range_type(mocker):
+def test_range_type(mocker, globals):
   test_data = [
     ('1..1 Days', "1", "1", '1..1 Days', 'Days', 'C25301'),
     (' -1..1 days', "-1", "1", '-1..1 days', 'days', 'C25301'),
     ('5 .. 10 weeks ', "5", "10", '5 .. 10 weeks', 'weeks', 'C29844'),
   ]
   for index, test in enumerate(test_data):
-    item = RangeType(test[0])
+    item = RangeType(test[0], globals)
     assert(item.lower) == test[1]
     assert(item.upper) == test[2]
     assert(item.label) == test[3]
     assert(item.units) == test[4]
     assert(item.units_code.code) == test[5]
     assert(item.errors) == [] 
 
-def test_range_type_error(mocker):
+def test_range_type_error(mocker, globals):
   test_data = [
     ('1.. Days',"Could not decode the range value, possible typographical errors '1.. Days'"),
     ('-1.1 days',"Could not decode the range value, possible typographical errors '-1.1 days'"),
     ('-1 .. 1',"Could not decode the range value, possible typographical errors '-1 .. 1'"),
     (' .. 1 Weeks',"Could not decode the range value ' .. 1 Weeks'"),
     ('1 .. 10 slugs',"Unable to set the units code for the range '1 .. 10 slugs'")
   ]
   for index, test in enumerate(test_data):
-    item = RangeType(test[0])
+    item = RangeType(test[0], globals)
     assert item.errors == [test[1]]
```

### Comparing `usdm-0.48.0/tests/test_study_design_activity_sheet.py` & `usdm-0.49.0/tests/test_study_design_activity_sheet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 import pytest
 import pandas as pd
-
-xfail = pytest.mark.xfail
-
 from usdm_excel.study_design_activity_sheet.study_design_activity_sheet import StudyDesignActivitySheet
-from usdm_excel.cross_ref import cross_references
 from usdm_model.code import Code
+from tests.test_factory import Factory
+
+xfail = pytest.mark.xfail
 
-def test_create(mocker):
+def test_create(mocker, globals):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['ActivityId_1', 'ActivityId_2', 'ActivityId_3']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['Activity 1', 'Activity One', '', ''], ['Activity 2', 'Activity Two', 'T', 'Condition 2'], ['Activity 3', 'Activity Three', 'F', '']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['activityName', 'activityDescription', 'activityIsConditional', 'activityIsConditionalReason'])
-  activities = StudyDesignActivitySheet("")
+  activities = StudyDesignActivitySheet("", globals)
   assert len(activities.items) == 3
   assert activities.items[0].id == 'ActivityId_1'
   assert activities.items[0].name == 'Activity 1'
   assert activities.items[0].description == 'Activity One'
-#  assert activities.items[0].isConditional == False
-#  assert activities.items[0].isConditionalReason == ''
   assert activities.items[1].id == 'ActivityId_2'
   assert activities.items[1].description == 'Activity Two'
-#  assert activities.items[1].isConditional == True
-#  assert activities.items[1].isConditionalReason == 'Condition 2'
   assert activities.items[2].id == 'ActivityId_3'
-#  assert activities.items[2].isConditional == False
   
-def test_create_empty(mocker):
+def test_create_empty(mocker, globals):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['studyActivityName', 'studyActivityDescription', 'studyActivityType'])
-  activities = StudyDesignActivitySheet("")
+  activities = StudyDesignActivitySheet("", globals)
   assert len(activities.items) == 0
```

### Comparing `usdm-0.48.0/tests/test_study_design_arm_sheet.py` & `usdm-0.49.0/tests/test_study_design_arm_sheet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,95 +1,94 @@
 import pytest
 import pandas as pd
-
-xfail = pytest.mark.xfail
-
 from usdm_excel.study_design_arm_sheet.study_design_arm_sheet import StudyDesignArmSheet
-from usdm_excel.cross_ref import cross_references
 from usdm_model.code import Code
 
-def test_create(mocker):
-  cross_references.clear()
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+
+xfail = pytest.mark.xfail
+
+def test_create(mocker, globals):
+  globals.cross_references.clear()
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['ArmId_1', 'ArmId_2', 'ArmId_3']
   expected_1 = Code(id='Code1', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label1")
   expected_2 = Code(id='Code2', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label2")
   expected_3 = Code(id='Code3', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label3")
   expected_4 = Code(id='Code4', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label4")
   expected_5 = Code(id='Code5', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label5")
   expected_6 = Code(id='Code6', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label6")
   mock_code = mocker.patch("usdm_excel.cdisc_ct.CDISCCT.code_for_attribute")
   mock_code.side_effect=[expected_1, expected_2, expected_3, expected_4, expected_5, expected_6]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['Arm 1', 'Arm One', 'C12345', 'Subject', 'C99999'], ['Arm 2', 'Arm Two', 'C12345', 'BYOD', 'C99999'], ['Arm 3', 'Arm Three', 'C12345', 'ePRO', 'C99999']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['studyArmName', 'studyArmDescription', 'studyArmType', 'studyArmDataOriginDescription', 'studyArmDataOriginType'])
-  arms = StudyDesignArmSheet("")
+  arms = StudyDesignArmSheet("", globals)
   assert len(arms.items) == 3
   assert arms.items[0].id == 'ArmId_1'
   assert arms.items[0].name == 'Arm 1'
   assert arms.items[0].label == ''
   assert arms.items[0].dataOriginDescription == 'Subject'
   assert arms.items[0].dataOriginType == expected_2
   assert arms.items[1].id == 'ArmId_2'
   assert arms.items[1].description == 'Arm Two'
   assert arms.items[2].id == 'ArmId_3'
   assert arms.items[2].type == expected_5
   assert arms.items[2].dataOriginDescription == 'ePRO'
   
-def test_create_with_name_and_label(mocker):
-  cross_references.clear()
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+def test_create_with_name_and_label(mocker, globals):
+  globals.cross_references.clear()
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['ArmId_1', 'ArmId_2', 'ArmId_3']
   expected_1 = Code(id='Code1', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label1")
   expected_2 = Code(id='Code2', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label2")
   expected_3 = Code(id='Code3', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label3")
   expected_4 = Code(id='Code4', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label4")
   expected_5 = Code(id='Code5', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label5")
   expected_6 = Code(id='Code6', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label6")
   mock_code = mocker.patch("usdm_excel.cdisc_ct.CDISCCT.code_for_attribute")
   mock_code.side_effect=[expected_1, expected_2, expected_3, expected_4, expected_5, expected_6]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['Arm 1', 'Arm One', 'Arm 1', 'C12345', 'Subject', 'C99999'], ['Arm 2', 'Arm Two', 'Arm 2', 'C12345', 'BYOD', 'C99999'], ['Arm 3', 'Arm Three', 'Arm Tre', 'C12345', 'ePRO', 'C99999']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['name', 'description', 'label', 'type', 'studyArmDataOriginDescription', 'dataOriginType'])
-  arms = StudyDesignArmSheet("")
+  arms = StudyDesignArmSheet("", globals)
   assert len(arms.items) == 3
   assert arms.items[0].id == 'ArmId_1'
   assert arms.items[0].name == 'Arm 1'
   assert arms.items[0].description == 'Arm One'
   assert arms.items[0].label == 'Arm 1'
   assert arms.items[0].dataOriginDescription == 'Subject'
   assert arms.items[0].dataOriginType == expected_2
   assert arms.items[1].id == 'ArmId_2'
   assert arms.items[1].description == 'Arm Two'
   assert arms.items[2].id == 'ArmId_3'
   assert arms.items[2].type == expected_5
   assert arms.items[2].dataOriginDescription == 'ePRO'
   
-def test_create_empty(mocker):
-  cross_references.clear()
+def test_create_empty(mocker, globals):
+  globals.cross_references.clear()
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['studyArmName', 'studyArmDescription', 'studyArmType'])
-  arms = StudyDesignArmSheet("")
+  arms = StudyDesignArmSheet("", globals)
   assert len(arms.items) == 0
 
-def test_read_cell_by_name_error(mocker):
-  cross_references.clear()
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+def test_read_cell_by_name_error(mocker, globals):
+  globals.cross_references.clear()
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['Arm 1', 'Arm One']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['studyArmName', 'studyArmDescription'])
-  arms = StudyDesignArmSheet("")
+  arms = StudyDesignArmSheet("", globals)
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "studyDesignArms"
   assert mock_error.call_args[0][1] == None
   assert mock_error.call_args[0][2] == None
-  assert mock_error.call_args[0][3] == "Exception 'Failed to detect column(s) 'studyArmType, type' in sheet' raised reading sheet."
+  assert mock_error.call_args[0][3] == "Exception. Error [Failed to detect column(s) 'studyArmType, type' in sheet] while reading sheet 'studyDesignArms'. See log for additional details."
```

### Comparing `usdm-0.48.0/tests/test_study_design_conditions_sheet.py` & `usdm-0.49.0/tests/test_study_design_dictionary_sheet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,107 +1,78 @@
 import pytest
 import pandas as pd
+from usdm_excel.study_design_dictionary_sheet.study_design_dictionary_sheet import StudyDesignDictionarySheet
+from usdm_model.api_base_model import ApiBaseModelWithId
 
-xfail = pytest.mark.xfail
 
-from usdm_excel.study_design_conditions_sheet.study_design_conditions_sheet import StudyDesignConditionSheet
-from usdm_excel.cross_ref import cross_references
-from usdm_model.api_base_model import ApiBaseModelWithId
+xfail = pytest.mark.xfail
 
-def test_create(mocker):
+def test_create(mocker, globals):
   mock_cross_ref = mocker.patch("usdm_excel.cross_ref.CrossRef.get")
   mock_cross_ref.side_effect=[
-    ApiBaseModelWithId(id="X1"), ApiBaseModelWithId(id="X2"), ApiBaseModelWithId(id="X3"), ApiBaseModelWithId(id="X4"), ApiBaseModelWithId(id="X5"),
-    ApiBaseModelWithId(id="X6"), ApiBaseModelWithId(id="X7"), ApiBaseModelWithId(id="X8"), ApiBaseModelWithId(id="X9"), ApiBaseModelWithId(id="X10")
+    ApiBaseModelWithId(id="1"), ApiBaseModelWithId(id="2"), ApiBaseModelWithId(id="3"), ApiBaseModelWithId(id="4"), ApiBaseModelWithId(id="5")
   ]
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
-  mock_id.side_effect=['Cond_1', 'Cond_2', 'Cond_3', 'Cond_4', 'Cond_5']
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
+  mock_id.side_effect=['DictionaryId_1', 'MapId_1', 'MapId_2', 'DictionaryId_2', 'MapId_3', 'DictionaryId_3', 'MapId_4', 'MapId_5', 'MapId_6']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
-    ['Id 1', 'Description One',   'Label One',   'Condition 1', 'Context 1', 'Applies 1'], 
-    ['Id 2', 'Description Two',   'Label Two',   'Condition 2', 'Context 2', 'Applies 2'], 
-    ['Id 3', 'Description Three', 'Label Three', 'Condition 3', 'Context 3', 'Applies 3'], 
-    ['id 4', 'Description Four',  'Label Four',  'Condition 4', 'Context 4, context 5', 'Applies 4'], 
-    ['Id 5', 'Description Five',  'Label Five',  'Condition 5', '',          'Applies 5']
+    ['Dictionary 1', 'Dictionary One',   'Label One',   'Key 1', ApiBaseModelWithId, 'Id 1', 'Attribute 1', ''], 
+    ['',             '',                 '',            'Key 2', ApiBaseModelWithId, 'Id 2', 'Attribute 2', ''], 
+    ['Dictionary 2', 'Dictionary Two',   'Label Two',   'Key 3', ApiBaseModelWithId, 'Id 3', 'Attribute 3', ''], 
+    ['Dictionary 3', 'Dictionary Three', 'Label Three', 'Key 4', ApiBaseModelWithId, 'Id 4', 'Attribute 4', ''], 
+    ['',             '',                 '',            'Key 5', ApiBaseModelWithId, 'Id 5', 'Attribute 5', ''],
+    ['',             '',                 '',            'Key 6', ''                , '',     '',            'Hello!']
  ]
   mock_read = mocker.patch("pandas.read_excel")
-  mock_read.return_value = pd.DataFrame(data, columns=['name', 'description', 'label', 'text', 'context', 'appliesTo'])
-  items = StudyDesignConditionSheet("")
-  assert len(items.items) == 5
-  assert items.items[0].id == 'Cond_1'
-  assert items.items[0].name == 'Id 1'
-  assert items.items[0].description == 'Description One'
-  assert items.items[0].label == 'Label One'
-  assert items.items[0].contextIds == ['X1']
-  assert items.items[0].appliesToIds == ['X2']
-  assert items.items[3].contextIds == ['X7', 'X8']
-  assert items.items[4].contextIds == []
-  assert items.items[4].appliesToIds == ['X10']
+  mock_read.return_value = pd.DataFrame(data, columns=['name', 'description', 'label', 'key', 'class', 'xref', 'attribute', 'value'])
+  dictionaries = StudyDesignDictionarySheet("", globals)
+  assert len(dictionaries.items) == 3
+  assert dictionaries.items[0].id == 'DictionaryId_1'
+  assert dictionaries.items[0].name == 'Dictionary 1'
+  assert dictionaries.items[0].description == 'Dictionary One'
+  assert dictionaries.items[0].label == 'Label One'
+  assert dictionaries.items[0].parameterMaps[1].tag == 'Key 2'
+  assert dictionaries.items[0].parameterMaps[1].reference == '<usdm:ref klass="ApiBaseModelWithId" id="2" attribute="Attribute 2"></usdm:ref>'
+  assert [x.tag for x in dictionaries.items[1].parameterMaps] == ['Key 3']
+  assert [x.tag for x in dictionaries.items[2].parameterMaps] == ['Key 4', 'Key 5', 'Key 6']
+  assert dictionaries.items[2].parameterMaps[2].reference == "<div>Hello!</div>"
   
-def test_create_empty(mocker):
+def test_create_empty(mocker, globals):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
-  mock_read.return_value = pd.DataFrame(data, columns=['name', 'description', 'label', 'text', 'context', 'appliesTo'])
-  items = StudyDesignConditionSheet("")
-  assert len(items.items) == 0
-
-def test_missing_reference(mocker):
-  
-  call_parameters = []
-  
-  def my_add(sheet, row, column, message, level=10):
-    call_parameters.append((sheet, row, column, message, level))
-    return None
-
-  cross_references.clear()
-  mock_cross_ref = mocker.patch("usdm_excel.cross_ref.CrossRef.get")
-  mock_cross_ref.side_effect=[ApiBaseModelWithId(id="X1"), ApiBaseModelWithId(id="X2")]
-  mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
-  mock_present.side_effect=[True]
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add", side_effect=my_add)
-  mocked_open = mocker.mock_open(read_data="File")
-  mocker.patch("builtins.open", mocked_open)
-  data = [
-    ['Id 1', 'Description One',  'Condtition 1', 'Label One', 'Context 1', '']
-  ]
-  mock_read = mocker.patch("pandas.read_excel")
-  mock_read.return_value = pd.DataFrame(data, columns=['name', 'description', 'label', 'text', 'context', 'appliesTo'])
-  items = StudyDesignConditionSheet("")
-  mock_error.assert_called()
-  assert call_parameters == [
-    ("studyDesignConditions", 1, 6, "No condition references found for '', at least one required", 10)
-  ]
+  mock_read.return_value = pd.DataFrame(data, columns=['name', 'description', 'label', 'key', 'class', 'xref', 'attribute'])
+  dictionaries = StudyDesignDictionarySheet("", globals)
+  assert len(dictionaries.items) == 0
 
-def test_read_cell_by_name_error(mocker):
+def test_read_cell_by_name_error(mocker, globals):
   
   call_parameters = []
   
   def my_add(sheet, row, column, message, level=10):
     call_parameters.append((sheet, row, column, message, level))
     return None
 
-  cross_references.clear()
-  mock_cross_ref = mocker.patch("usdm_excel.cross_ref.CrossRef.get")
-  mock_cross_ref.side_effect=[ApiBaseModelWithId(id="X1"), ApiBaseModelWithId(id="X2")]
+  globals.cross_references.clear()
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add", side_effect=my_add)
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add", side_effect=my_add)
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
-    ['Id 1', 'Description One',   'Label One', 'Context 1', 'Applies 1']
-  ]
+    ['Dictionary 1', 'Dictionary One',   'Label One',   'Key 1', 'Klass 1', 'Attribute 1']
+ ]
   mock_read = mocker.patch("pandas.read_excel")
-  mock_read.return_value = pd.DataFrame(data, columns=['name', 'description', 'label', 'context', 'appliesTo'])
-  items = StudyDesignConditionSheet("")
+  mock_read.return_value = pd.DataFrame(data, columns=['name', 'description', 'label', 'key', 'class', 'attribute'])
+  dictionaries = StudyDesignDictionarySheet("", globals)
   mock_error.assert_called()
   assert call_parameters == [
-    ("studyDesignConditions", 1, -1, "Error 'Failed to detect column(s) 'text' in sheet' reading cell 'text'", 10)
+    ("dictionaries", 1, -1, "Error 'Failed to detect column(s) 'xref' in sheet' reading cell 'xref'", 40),
+    ('dictionaries', 1, 6, "Failed to translate reference path 'Attribute 1', could not find start instance 'Klass 1', ''", 40)
   ]
```

### Comparing `usdm-0.48.0/tests/test_study_design_content_sheet.py` & `usdm-0.49.0/tests/test_study_design_content_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import pytest
 import pandas as pd
-
 from usdm_excel.base_sheet import BaseSheet
+from usdm_excel.study_design_content_sheet.study_design_content_sheet import StudyDesignContentSheet
+from usdm_excel.option_manager import Options, EmptyNoneOption
+from tests.test_factory import Factory
 
 xfail = pytest.mark.xfail
 
-from usdm_excel.study_design_content_sheet.study_design_content_sheet import StudyDesignContentSheet
+def test_create(mocker, globals):
+  globals.option_manager.set(Options.EMPTY_NONE, EmptyNoneOption.EMPTY)
 
-def test_create(mocker):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Content_1', 'Content_2', 'Content_3', 'Content_4', 'Content_5', 'Content_6', 'Content_7', 'Content_8']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     ['1',     '',         'Section 1',     'Text 1'], 
     ['1.1',   'SET NAME', 'Section 1.1',   'Text 1.1'], 
     ['1.2',   '',         'Section 1.2',   'Text 1.2'], 
     ['1.2.1', '',         'Section 1.2.1', 'Text 1.2.1'], 
     ['2',     '',         'Section 2',     'Text 2'], 
     ['2.1',   '',         'Section 2.1',   'Text 2.1'], 
     ['3',     '',         'Section 3',     'Text 3'], 
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['sectionNumber', 'name', 'sectionTitle', 'text'])
-  content = StudyDesignContentSheet("")
+  content = StudyDesignContentSheet("", globals)
   assert len(content.items) == 8
   assert content.items[0].name == 'ROOT'
   assert content.items[0].previousId == ''
   assert content.items[0].nextId == 'Content_2'  
   assert content.items[1].id == 'Content_2'
   assert content.items[1].name == 'SECTION 1'
   assert content.items[1].sectionNumber == '1'
@@ -46,33 +48,33 @@
   assert content.items[3].nextId == 'Content_5'  
   assert content.items[4].name == 'SECTION 1.2.1'
   assert content.items[5].name == 'SECTION 2'
   assert content.items[6].name == 'SECTION 2.1'
   assert content.items[7].id == 'Content_8'
   assert content.items[7].name == 'SECTION 3'
 
-def test_create_training_dot(mocker):
+def test_create_training_dot(mocker, globals):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Content_1', 'Content_2', 'Content_3', 'Content_4', 'Content_5', 'Content_6', 'Content_7', 'Content_8']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     ['1',     '',         'Section 1',     'Text 1'], 
     ['1.1',   'SET NAME', 'Section 1.1',   'Text 1.1'], 
     ['1.2',   '',         'Section 1.2',   'Text 1.2'], 
     ['1.2.1', '',         'Section 1.2.1', 'Text 1.2.1.'], 
     ['2',     '',         'Section 2',     'Text 2'], 
     ['2.1',   '',         'Section 2.1',   'Text 2.1.'], 
     ['3',     '',         'Section 3',     'Text 3'], 
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['sectionNumber', 'name', 'sectionTitle', 'text'])
-  content = StudyDesignContentSheet("")
+  content = StudyDesignContentSheet("", globals)
   assert len(content.items) == 8
   assert content.items[0].name == 'ROOT'
   assert content.items[1].id == 'Content_2'
   assert content.items[1].name == 'SECTION 1'
   assert content.items[1].sectionNumber == '1'
   assert content.items[1].sectionTitle == 'Section 1'
   assert content.items[1].text == '<div>Text 1</div>'
@@ -81,33 +83,33 @@
   assert content.items[3].name == 'SECTION 1.2'
   assert content.items[4].name == 'SECTION 1.2.1'
   assert content.items[5].name == 'SECTION 2'
   assert content.items[6].name == 'SECTION 2.1'
   assert content.items[7].id == 'Content_8'
   assert content.items[7].name == 'SECTION 3'
 
-def test_create_4_levels(mocker):
+def test_create_4_levels(mocker, globals):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Content_1', 'Content_2', 'Content_3', 'Content_4', 'Content_5', 'Content_6', 'Content_7', 'Content_8']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     ['1',       '',         'Section 1',       'Text 1'], 
     ['1.1',     'SET NAME', 'Section 1.1',     'Text 1.1'], 
     ['1.2',     '',         'Section 1.2',     'Text 1.2'], 
     ['1.2.1',   '',         'Section 1.2.1',   'Text 1.2.1'], 
     ['1.2.1.1', '',         'Section 1.2.1.1', 'Text 1.2.1.1'], 
     ['2',       '',         'Section 2',       'Text 2'], 
     ['3',       '',         'Section 3',       'Text 3'], 
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['sectionNumber', 'name', 'sectionTitle', 'text'])
-  content = StudyDesignContentSheet("")
+  content = StudyDesignContentSheet("", globals)
   assert len(content.items) == 8
   assert content.items[0].name == 'ROOT'
   assert content.items[4].id == 'Content_5'
   assert content.items[4].name == 'SECTION 1.2.1'
   assert content.items[4].sectionNumber == '1.2.1'
   assert content.items[4].sectionTitle == 'Section 1.2.1'
   assert content.items[4].text == '<div>Text 1.2.1</div>'
@@ -115,91 +117,91 @@
   assert content.items[5].id == 'Content_6'
   assert content.items[5].name == 'SECTION 1.2.1.1'
   assert content.items[5].sectionNumber == '1.2.1.1'
   assert content.items[5].sectionTitle == 'Section 1.2.1.1'
   assert content.items[5].text == '<div>Text 1.2.1.1</div>'
   assert content.items[5].childIds == []
 
-def test_create_standard_section(mocker):
+def test_create_standard_section(mocker, globals):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Content_1', 'Content_2', 'Content_3', 'Content_4', 'Content_5', 'Content_6', 'Content_7', 'Content_8']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     ['1',       '',         'Section 1',       'Text 1'], 
     ['1.1',     'SET NAME', 'Section 1.1',     'Text 1.1'], 
     ['1.2',     '',         'Section 1.2',     '<usdm:section name="m11-title">'], 
     ['1.2.1',   '',         'Section 1.2.1',   '<div><usdm:section name="m11-title"></div>'], 
     ['2',       '',         'Section 2',       'Text 2'], 
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['sectionNumber', 'name', 'sectionTitle', 'text'])
-  content = StudyDesignContentSheet("")
+  content = StudyDesignContentSheet("", globals)
   assert len(content.items) == 6
   assert content.items[0].text == ''
   assert content.items[1].text == '<div>Text 1</div>'
   assert content.items[2].text == '<div>Text 1.1</div>'
   assert content.items[3].text == '<div><usdm:section name="m11-title"></div>'
   assert content.items[4].text == '<div><usdm:section name="m11-title"></div>'
   assert content.items[5].text == '<div>Text 2</div>'
 
-def test_create_invalid_levels(mocker):
+def test_create_invalid_levels(mocker, globals):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Content_1', 'Content_2', 'Content_3', 'Content_4', 'Content_5', 'Content_6', 'Content_7', 'Content_8']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     ['1',         '',         'Section 1',       'Text 1'], 
     ['1.1',       'SET NAME', 'Section 1.1',     'Text 1.1'], 
     ['1.2',       '',         'Section 1.2',     'Text 1.2'], 
     ['1.2.1',     '',         'Section 1.2.1',   'Text 1.2.1'], 
     ['1.2.1.1.4', '',         'Section 1.2.1.1', 'Text 1.2.1.1'], 
     ['2',         '',         'Section 2',       'Text 2'], 
     ['3',         '',         'Section 3',       'Text 3'], 
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['sectionNumber', 'name', 'sectionTitle', 'text'])
-  StudyDesignContentSheet("")
+  StudyDesignContentSheet("", globals)
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "studyDesignContent"
   assert mock_error.call_args[0][1] == None
   assert mock_error.call_args[0][2] == None
-  assert mock_error.call_args[0][3] == "Exception '' raised reading sheet."
+  assert mock_error.call_args[0][3] == "Exception. Error [] while reading sheet 'studyDesignContent'. See log for additional details."
 
-def test_create_empty(mocker):
+def test_create_empty(mocker, globals):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['sectionNumber', 'name', 'sectionTitle', 'text'])
-  content = StudyDesignContentSheet("")
+  content = StudyDesignContentSheet("", globals)
   assert len(content.items) == 1
 
-def test_read_cell_by_name_error(mocker):
+def test_read_cell_by_name_error(mocker, globals):
   
   call_parameters = []
   
   def my_add(sheet, row, column, message, level=10):
     call_parameters.append((sheet, row, column, message, level))
     return None
 
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add", side_effect=my_add)
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add", side_effect=my_add)
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['1', 'Section 1', 'Text 1']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['sectionNumber', 'name', 'text'])
-  content = StudyDesignContentSheet("")
+  content = StudyDesignContentSheet("", globals)
   mock_error.assert_called()
   assert call_parameters == [
-    ('studyDesignContent', 1, -1, "Error 'Failed to detect column(s) 'sectionTitle' in sheet' reading cell 'sectionTitle'", 10)
+    ('studyDesignContent', 1, -1, "Error 'Failed to detect column(s) 'sectionTitle' in sheet' reading cell 'sectionTitle'", 40)
   ]
```

### Comparing `usdm-0.48.0/tests/test_study_design_eligibility_criteria_sheet.py` & `usdm-0.49.0/tests/test_study_design_eligibility_criteria_sheet.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,70 @@
 import pytest
 import pandas as pd
-
-xfail = pytest.mark.xfail
-
 from usdm_excel.study_design_eligibility_criteria_sheet.study_design_eligibility_criteria_sheet import StudyDesignEligibilityCriteriaSheet
 from usdm_model.code import Code
 
-def test_create(mocker):
+
+xfail = pytest.mark.xfail
+def test_create(mocker, globals):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Code_1', 'EligibilityId_1', 'Code_2', 'EligibilityId_2', 'Code_3', 'EligibilityId_3']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     ['Inclusion', '01', 'INC01', 'The study age criterion', 'Age critierion', 'Subjects should be between 18 and 45 years old', "dictionary"], 
     ['Inclusion', '02', 'INC01', 'The study abc criterion',   'ABC critierion', 'Subjects should have ABC', "dictionary"], 
     ['Exclusion', '01', 'EXC01', 'Exclude those with all fingers',   'Fingers critierion', 'Subjects should not have all fingers', "dictionary"], 
  ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['category', 'identifier', 'name', 'description', 'label', 'text', 'dictionary'])
-  items = StudyDesignEligibilityCriteriaSheet("")
+  items = StudyDesignEligibilityCriteriaSheet("", globals)
   assert len(items.items) == 3
   assert items.items[0].id == 'EligibilityId_1'
   assert items.items[0].category.decode == 'Inclusion Criteria'
   assert items.items[0].identifier == '01'
   assert items.items[0].name == 'INC01'
   assert items.items[0].description == 'The study age criterion'
   assert items.items[0].label == 'Age critierion'
   assert items.items[0].text == 'Subjects should be between 18 and 45 years old'
   assert items.items[1].category.decode == 'Inclusion Criteria'
   assert items.items[2].category.decode == 'Exclusion Criteria'
   
-def test_create_empty(mocker):
+def test_create_empty(mocker, globals):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['category', 'identifier', 'name', 'description', 'label', 'text', 'dictionary'])
-  items = StudyDesignEligibilityCriteriaSheet("")
+  items = StudyDesignEligibilityCriteriaSheet("", globals)
   assert len(items.items) == 0
 
-def test_read_cell_by_name_error(mocker):
-  
+def test_read_cell_by_name_error(mocker, globals):
+  globals.cross_references.clear()
   call_parameters = []
   
   def my_add(sheet, row, column, message, level=10):
     call_parameters.append((sheet, row, column, message, level))
     return None
 
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add", side_effect=my_add)
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add", side_effect=my_add)
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     ['Inclusion', '01', 'The study age criterion', 'Age critierion', 'Subjects should be between 18 and 45 years old', "dictionary"]
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['category', 'identifier', 'name', 'label', 'text', 'dictionary'])
-  items = StudyDesignEligibilityCriteriaSheet("")
+  items = StudyDesignEligibilityCriteriaSheet("", globals)
   mock_error.assert_called()
   assert call_parameters == [
-    ('studyDesignEligibilityCriteria', 1, -1, "Error 'Failed to detect column(s) 'description' in sheet' reading cell 'description'", 10),
+    ('studyDesignEligibilityCriteria', 1, -1, "Error 'Failed to detect column(s) 'description' in sheet' reading cell 'description'", 40),
     ('studyDesignEligibilityCriteria', 1, 5, "Dictionary 'dictionary' not found", 30),
-    ('studyDesignEligibilityCriteria', None, None, "Unable to find dictionary with name 'dictionary'", 10)
+    ('studyDesignEligibilityCriteria', None, None, "Unable to find dictionary with name 'dictionary'", 40)
   ]
```

### Comparing `usdm-0.48.0/tests/test_study_design_encounter_sheet.py` & `usdm-0.49.0/tests/test_study_design_encounter_sheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pytest
 import pandas as pd
-
-xfail = pytest.mark.xfail
-
 from usdm_excel.study_design_encounter_sheet.study_design_encounter_sheet import StudyDesignEncounterSheet
 from usdm_model.code import Code
 
-def test_create(mocker):
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+
+xfail = pytest.mark.xfail
+
+def test_create(mocker, globals):
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['RuleId_1', 'EncounterId_1', 'RuleId_2', 'EncounterId_2', 'EncounterId_3']
   codes = []
   for index in range(1,10):
     codes.append(Code(id=f'Code{index}', code='code', codeSystem='codesys', codeSystemVersion='3', decode=f"label{index}"))
   mock_code = mocker.patch("usdm_excel.cdisc_ct.CDISCCT.code_for_attribute")
   mock_code.side_effect = codes
   mocked_open = mocker.mock_open(read_data="File")
@@ -19,25 +19,25 @@
   data = [
     ['E1', 'Encounter 1', 'Encounter One', 'visit', 'CLINIC', 'in Person', 'start rule', '' ], 
     ['E2', 'Encounter 2', 'Encounter Two', 'visit', 'CLINIC', 'in Person', '', 'end rule'], 
     ['E3', 'Encounter 3', 'Encounter Three', 'visit', 'HOME', 'TELEPHONE CALL', '', '']
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['xref', 'encounterName', 'encounterDescription', 'encounterType', 'encounterEnvironmentalSetting', 'encounterContactModes', 'transitionStartRule',	'transitionEndRule'])
-  encounters = StudyDesignEncounterSheet("")
+  encounters = StudyDesignEncounterSheet("", globals)
   assert len(encounters.items) == 3
   assert encounters.items[0].id == 'EncounterId_1'
   assert encounters.items[0].name == 'Encounter 1'
   assert encounters.items[1].id == 'EncounterId_2'
   assert encounters.items[1].description == 'Encounter Two'
   assert encounters.items[2].id == 'EncounterId_3'
   assert encounters.items[2].type == codes[6]
   
-def test_create_with_label(mocker):
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+def test_create_with_label(mocker, globals):
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['RuleId_1', 'EncounterId_1', 'RuleId_2', 'EncounterId_2', 'EncounterId_3']
   codes = []
   for index in range(1,10):
     codes.append(Code(id=f'Code{index}', code='code', codeSystem='codesys', codeSystemVersion='3', decode=f"label{index}"))
   mock_code = mocker.patch("usdm_excel.cdisc_ct.CDISCCT.code_for_attribute")
   mock_code.side_effect = codes
   mocked_open = mocker.mock_open(read_data="File")
@@ -45,41 +45,41 @@
   data = [
     ['E1', 'Encounter 1', 'Encounter One', '', 'visit', 'CLINIC', 'in Person', 'start rule', '' ], 
     ['E2', 'Encounter 2', 'Encounter Two', 'Label 2', 'visit', 'CLINIC', 'in Person', '', 'end rule'], 
     ['E3', 'Encounter 3', 'Encounter Three', 'Label 3', 'visit', 'HOME', 'TELEPHONE CALL', '', '']
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['xref', 'name', 'description', 'label', 'type', 'encounterEnvironmentalSetting', 'encounterContactModes', 'transitionStartRule',	'transitionEndRule'])
-  encounters = StudyDesignEncounterSheet("")
+  encounters = StudyDesignEncounterSheet("", globals)
   assert len(encounters.items) == 3
   assert encounters.items[0].id == 'EncounterId_1'
   assert encounters.items[0].name == 'Encounter 1'
   assert encounters.items[0].label == ''
   assert encounters.items[1].id == 'EncounterId_2'
   assert encounters.items[1].description == 'Encounter Two'
   assert encounters.items[2].id == 'EncounterId_3'
   assert encounters.items[2].type == codes[6]
   assert encounters.items[2].label == 'Label 3'
 
-def test_create_empty(mocker):
+def test_create_empty(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['xref', 'encounterName', 'encounterDescription', 'encounterType', 'encounterEnvironmentalSetting', 'encounterContactModes', 'transitionStartRule',	'transitionEndRule'])
-  encounters = StudyDesignEncounterSheet("")
+  encounters = StudyDesignEncounterSheet("", globals)
   assert len(encounters.items) == 0
 
-def test_read_cell_by_name_error(mocker):
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+def test_read_cell_by_name_error(mocker, globals):
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['E1', 'Encounter 1', 'Encounter One', 'CLINIC', 'in Person', 'start rule', '' ]]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['xref', 'encounterName', 'encounterDescription', 'encounterEnvironmentalSetting', 'encounterContactModes', 'transitionStartRule',	'transitionEndRule'])
-  encounters = StudyDesignEncounterSheet("")
+  encounters = StudyDesignEncounterSheet("", globals)
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "studyDesignEncounters"
   assert mock_error.call_args[0][1] == None
   assert mock_error.call_args[0][2] == None
-  assert mock_error.call_args[0][3] == "Exception 'Failed to detect column(s) 'encounterType, type' in sheet' raised reading sheet."
+  assert mock_error.call_args[0][3] == "Exception. Error [Failed to detect column(s) 'encounterType, type' in sheet] while reading sheet 'studyDesignEncounters'. See log for additional details."
```

### Comparing `usdm-0.48.0/tests/test_study_design_epoch_sheet.py` & `usdm-0.49.0/tests/test_study_design_epoch_sheet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 import pytest
 import pandas as pd
-
-xfail = pytest.mark.xfail
-
 from usdm_excel.study_design_epoch_sheet.study_design_epoch_sheet import StudyDesignEpochSheet
 from usdm_model.code import Code
 
-def test_create(mocker):
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+
+xfail = pytest.mark.xfail
+
+def test_create(mocker, globals):
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['EpochId_1', 'EpochId_2', 'EpochId_3']
   expected_1 = Code(id='Code1', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label1")
   expected_2 = Code(id='Code2', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label2")
   expected_3 = Code(id='Code3', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label3")
   mock_code = mocker.patch("usdm_excel.cdisc_ct.CDISCCT.code_for_attribute")
   mock_code.side_effect=[expected_1, expected_2, expected_3]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['Epoch 1', 'Epoch One', 'C12345'], ['Epoch 2', 'Epoch Two', 'C12345'], ['Epoch 3', 'Epoch Three', 'C12345']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['studyEpochName', 'studyEpochDescription', 'studyEpochType'])
-  epochs = StudyDesignEpochSheet("")
+  epochs = StudyDesignEpochSheet("", globals)
   assert len(epochs.items) == 3
   assert epochs.items[0].id == 'EpochId_1'
   assert epochs.items[0].name == 'Epoch 1'
   assert epochs.items[1].id == 'EpochId_2'
   assert epochs.items[1].description == 'Epoch Two'
   assert epochs.items[2].id == 'EpochId_3'
   assert epochs.items[2].type == expected_3
   
-def test_create_with_label(mocker):
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+def test_create_with_label(mocker, globals):
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['EpochId_1', 'EpochId_2', 'EpochId_3']
   expected_1 = Code(id='Code1', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label1")
   expected_2 = Code(id='Code2', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label2")
   expected_3 = Code(id='Code3', code='code', codeSystem='codesys', codeSystemVersion='3', decode="label3")
   mock_code = mocker.patch("usdm_excel.cdisc_ct.CDISCCT.code_for_attribute")
   mock_code.side_effect=[expected_1, expected_2, expected_3]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['Epoch 1', 'Epoch One', '1', 'C12345'], ['Epoch 2', 'Epoch Two', '2', 'C12345'], ['Epoch 3', 'Epoch Three', '', 'C12345']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['name', 'description', 'label', 'studyEpochType'])
-  epochs = StudyDesignEpochSheet("")
+  epochs = StudyDesignEpochSheet("", globals)
   assert len(epochs.items) == 3
   assert epochs.items[0].id == 'EpochId_1'
   assert epochs.items[0].name == 'Epoch 1'
   assert epochs.items[0].label == '1'
   assert epochs.items[1].id == 'EpochId_2'
   assert epochs.items[1].description == 'Epoch Two'
   assert epochs.items[2].id == 'EpochId_3'
   assert epochs.items[2].type == expected_3
   assert epochs.items[2].label == ''
   
-def test_create_empty(mocker):
+def test_create_empty(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['studyEpochName', 'studyEpochDescription', 'studyEpochType'])
-  epochs = StudyDesignEpochSheet("")
+  epochs = StudyDesignEpochSheet("", globals)
   assert len(epochs.items) == 0
 
-def test_read_cell_by_name_error(mocker):
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+def test_read_cell_by_name_error(mocker, globals):
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['Epoch 1', 'Epoch One']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['studyEpochName', 'studyEpochDescription'])
-  epochs = StudyDesignEpochSheet("")
+  epochs = StudyDesignEpochSheet("", globals)
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "studyDesignEpochs"
   assert mock_error.call_args[0][1] == None
   assert mock_error.call_args[0][2] == None
-  assert mock_error.call_args[0][3] == "Exception 'Failed to detect column(s) 'studyEpochType, type' in sheet' raised reading sheet."
+  assert mock_error.call_args[0][3] == "Exception. Error [Failed to detect column(s) 'studyEpochType, type' in sheet] while reading sheet 'studyDesignEpochs'. See log for additional details."
```

### Comparing `usdm-0.48.0/tests/test_study_design_indication_sheet.py` & `usdm-0.49.0/tests/test_study_design_indication_sheet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,57 @@
 import pytest
 import pandas as pd
-
-xfail = pytest.mark.xfail
-
 from usdm_excel.study_design_indication_sheet.study_design_indication_sheet import StudyDesignIndicationSheet
-from tests.test_utility import clear
 from usdm_model.code import Code
 
-def test_create(mocker):
-  clear()
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+
+xfail = pytest.mark.xfail
+
+def test_create(mocker, globals):
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Code_1', 'IndicationId_1', 'Code_2', 'IndicationId_2', 'Code_3', 'Code_4', 'IndicationId_3']
   expected_1 = Code(id='Code_1', code='X', codeSystem='SPONSOR', codeSystemVersion='None set', decode="Y")
   expected_2 = Code(id='Code_2', code='AAA', codeSystem='SPONSOR', codeSystemVersion='None set', decode="BBB")
   expected_3 = Code(id='Code_3', code='WWW', codeSystem='SPONSOR', codeSystemVersion='None set', decode="1234")
   expected_4 = Code(id='Code_4', code='EEE', codeSystem='SPONSOR', codeSystemVersion='None set', decode="3456")
   mock_code = mocker.patch("usdm_excel.cdisc_ct.CDISCCT.code_for_attribute")
   mock_code.side_effect=[expected_1, expected_2, expected_3, expected_4]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['Indication 1', 'Indication One', 'Label One', 'Sponsor:X=Y'], 
           ['Indication 2', 'Indication Two', '', 'SPONSOR: AAA=BBB'], 
           ['Indication 3', 'Indication Three', '', 'SPONSOR: WWW=1234, SPONSOR: EEE=3456']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['name', 'description', 'label', 'codes'])
-  Indications = StudyDesignIndicationSheet("")
+  Indications = StudyDesignIndicationSheet("", globals)
   assert len(Indications.items) == 3
   assert Indications.items[0].id == 'IndicationId_1'
   assert Indications.items[0].name == 'Indication 1'
   assert Indications.items[1].id == 'IndicationId_2'
   assert Indications.items[1].description == 'Indication Two'
   assert Indications.items[1].codes == [expected_2]
   assert Indications.items[2].id == 'IndicationId_3'
   assert Indications.items[2].codes == [expected_3, expected_4]
   
-def test_create_empty(mocker):
-  clear()
+def test_create_empty(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['studyIndicationName', 'studyIndicationDescription', 'studyIndicationType'])
-  Indications = StudyDesignIndicationSheet("")
+  Indications = StudyDesignIndicationSheet("", globals)
   assert len(Indications.items) == 0
 
-def test_read_cell_by_name_error(mocker):
-  clear()
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+def test_read_cell_by_name_error(mocker, globals):
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['Indication 1', 'Indication One']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['name', 'description'])
-  Indications = StudyDesignIndicationSheet("")
+  Indications = StudyDesignIndicationSheet("", globals)
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "studyDesignIndications"
   assert mock_error.call_args[0][1] == None
   assert mock_error.call_args[0][2] == None
-  assert mock_error.call_args[0][3] == "Exception ''codes'' raised reading sheet."
+  assert mock_error.call_args[0][3] == "Exception. Error [Failed to detect column(s) 'codes' in sheet] while reading sheet 'studyDesignIndications'. See log for additional details."
```

### Comparing `usdm-0.48.0/tests/test_study_design_intervention_sheet.py` & `usdm-0.49.0/tests/test_study_design_intervention_sheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import pytest
 import json
 import pandas as pd
-
-xfail = pytest.mark.xfail
-
 from usdm_excel.study_design_intervention_sheet.study_design_intervention_sheet import StudyDesignInterventionSheet
-from tests.test_utility import clear
 from usdm_model.code import Code
 
+
+xfail = pytest.mark.xfail
+
 SAVE = True
 COLUMNS = [ 'name', 'description', 'label', "codes", "role", "type", 
   "pharmacologicalClass", "productDesignation", "minimumResponseDuration", 'administrationName', 'administrationDescription', 
   'administrationLabel', "administrationRoute", "administrationDose", "administrationFrequency", 
   'administrationDurationDescription', 'administrationDurationWillVary', 'administrationDurationWillVaryReason', 'administrationDurationQuantity' ]
 
 def read_json(filename):
   with open(filename, 'r') as f:
     data = json.load(f)
   return data
 
 def dump_json(data):
   print(f"\n{json.dumps(data, indent=2)}")
 
-def test_create(mocker):
-  clear()
+def test_create(mocker, globals):
   expected = read_json(f"tests/integration_test_files/intervention/create.json")
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=[f"Id_{x}" for x in range(100)]
 
   mock_code = mocker.patch("usdm_excel.cdisc_ct.CDISCCT.code_for_attribute")
   mock_code.side_effect=[Code(id=f'Code_{x}', code='C12345', codeSystem='CDISC', codeSystemVersion='1', decode=f"INDEX{x}") for x in range(100)]
   
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
@@ -40,40 +38,38 @@
     [ 'Int 2', 'Int Desc 2',  'Int Label 2', 'SPONSOR: C=D',                'Placebo',                   'C12345', 'FDA: A=B',           'NIMP (AxMP)',          '3 Weeks',                'Admin 3',              'Admin Desc 3',           'Admin Label 1',    'C34567',          '100 mg',           'C65432',               'Dur desc 1',                     'False',                       '',                                  '12 C'                         ], 
     [ 'Int 3', 'Int Desc 3',  'Int Label 3', 'SPONSOR: E=F, SPONSOR: G=H',  'Rescue Medicine',           'C12345', 'FDA: A=B',           'IMP',                  '4 Years',                'Admin 4',              'Admin Desc 4',           'Admin Label 1',    'C34567',          '500 mg',           'C65432',               'Dur desc 1',                     'False',                       '',                                  '12 F'                         ], 
     [ '',      '',            '',            '',                            '',                          '',       '',                   '',                     '',                       'Admin 5',              'Admin Desc 5',           'Admin Label 1',    'C34567',          '1 mg',             'C65432',               'Dur desc 1',                     'False',                       '',                                  '15 in'                        ], 
   ]
 
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=COLUMNS)
-  interventions = StudyDesignInterventionSheet("")
+  interventions = StudyDesignInterventionSheet("", globals)
   #dump_json({'items': [json.loads(x.to_json()) for x in interventions.items]})
   for index, item in enumerate(interventions.items):
     result = json.loads(item.to_json())
     assert result == expected["items"][index]
   
-def test_create_empty(mocker):
-  clear()
+def test_create_empty(mocker, globals):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=COLUMNS)
-  interventions = StudyDesignInterventionSheet("")
+  interventions = StudyDesignInterventionSheet("", globals)
   assert len(interventions.items) == 0
 
-def test_read_cell_by_name_error(mocker):
-  clear()
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+def test_read_cell_by_name_error(mocker, globals):
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '']]
   mock_read = mocker.patch("pandas.read_excel")
   columns = COLUMNS
   columns = columns[0:-1]
   mock_read.return_value = pd.DataFrame(data, columns=columns)
-  interventions = StudyDesignInterventionSheet("")
+  interventions = StudyDesignInterventionSheet("", globals)
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "studyDesignInterventions"
   assert mock_error.call_args[0][1] == None
   assert mock_error.call_args[0][2] == None
-  assert mock_error.call_args[0][3] == "Exception 'Failed to detect column(s) 'administrationDurationQuantity' in sheet' raised reading sheet."
+  assert mock_error.call_args[0][3] == "Exception. Error [Failed to detect column(s) 'administrationDurationQuantity' in sheet] while reading sheet 'studyDesignInterventions'. See log for additional details."
```

### Comparing `usdm-0.48.0/tests/test_study_design_oe_sheet.py` & `usdm-0.49.0/tests/test_study_design_oe_sheet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pytest
 import pandas as pd
-
-xfail = pytest.mark.xfail
-
 from usdm_excel.study_design_objective_endpoint_sheet.study_design_objective_endpoint_sheet import StudyDesignObjectiveEndpointSheet
 from usdm_model.api_base_model import ApiBaseModelWithId
 
-def test_create(mocker):
+
+xfail = pytest.mark.xfail
+
+def test_create(mocker, globals):
   #mock_cross_ref = mocker.patch("usdm_excel.cross_ref.CrossRef.get")
   #mock_cross_ref.side_effect=[ApiBaseModelWithId(id="1"), ApiBaseModelWithId(id="2"), ApiBaseModelWithId(id="3"), ApiBaseModelWithId(id="4"), ApiBaseModelWithId(id="5")]
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=[
     'Code_1', 'Code_2', 'ObjId_1', 'EndId_1', 'Code_3', 'EndId_2', 
     'Code_4', 'Code_5', 'ObjId_2', 'EndId_3', 
     'Code_6', 'Code_7', 'ObjId_3', 'EndId_4', 'Code_8', 'EndId_5'
   ]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
@@ -27,15 +27,15 @@
     ['','', '', '', '',                                                        'End 5', 'End Desc 5', 'End Label 5', 'End Text 5', '', 'Secondary Endpoint']
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=[
     'objectiveName', 'objectiveDescription', 'objectiveLabel', 'objectiveText', 
     'objectiveLevel', 'endpointName', 'endpointDescription', 'endpointLabel', 'endpointText', 'endpointPurpose', 'endpointLevel']
   )
-  items = StudyDesignObjectiveEndpointSheet("")
+  items = StudyDesignObjectiveEndpointSheet("", globals)
   assert len(items.objectives) == 3
   assert items.objectives[0].id == 'ObjId_1'
   assert items.objectives[0].name == 'Obj 1'
   assert items.objectives[0].description == 'Obj Desc 1'
   assert items.objectives[0].label == 'Obj Label 1'
   assert items.objectives[0].endpoints[0].name == 'End 1'
   assert items.objectives[0].endpoints[1].name == 'End 2'
@@ -43,46 +43,46 @@
   assert items.objectives[1].name == 'Obj 2'
   assert items.objectives[1].endpoints[0].name == 'End 3'
   assert items.objectives[2].id == 'ObjId_3'
   assert items.objectives[2].name == 'Obj 3'
   assert items.objectives[2].endpoints[0].name == 'End 4'
   assert items.objectives[2].endpoints[1].name == 'End 5'
   
-def test_create_empty(mocker):
+def test_create_empty(mocker, globals):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=[
     'objectiveName', 'objectiveDescription', 'objectiveLabel', 'objectiveText', 
     'objectiveLevel', 'endpointName', 'endpointDescription', 'endpointLabel', 'endpointText', 'endpointPurpose', 'endpointLevel']
   )
-  items = StudyDesignObjectiveEndpointSheet("")
+  items = StudyDesignObjectiveEndpointSheet("", globals)
   assert len(items.objectives) == 0
 
-def test_read_cell_by_name_error(mocker):
+def test_read_cell_by_name_error(mocker, globals):
   
   call_parameters = []
   
   def my_add(sheet, row, column, message, level=10):
     call_parameters.append((sheet, row, column, message, level))
     return None
 
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add", side_effect=my_add)
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add", side_effect=my_add)
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     ['Obj 1','Obj Desc 1', 'Obj Label 1', 'Obj Text 1', 'Study Primary Objective', 'End 1', 'End Desc 1', 'End Label 1', 'End Text 1', 'Primary Endpoint']
  ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=[
     'objectiveName', 'objectiveDescription', 'objectiveLabel', 'objectiveText', 
     'objectiveLevel', 'endpointDescription', 'endpointLabel', 'endpointText', 'endpointPurpose', 'endpointLevel']
   )
-  items = StudyDesignObjectiveEndpointSheet("")
+  items = StudyDesignObjectiveEndpointSheet("", globals)
   mock_error.assert_called()
-  assert call_parameters[0] == ("studyDesignOE", 1, -1, "Error 'Failed to detect column(s) 'endpointXref, endpointName' in sheet' reading cell '['endpointXref', 'endpointName']'", 10)
+  assert call_parameters[0] == ("studyDesignOE", 1, -1, "Error 'Failed to detect column(s) 'endpointXref, endpointName' in sheet' reading cell '['endpointXref', 'endpointName']'", 40)
```

### Comparing `usdm-0.48.0/tests/test_study_design_sites_sheet.py` & `usdm-0.49.0/tests/test_study_design_sites_sheet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import pytest
 import pandas as pd
-
 from usdm_excel.study_design_sites_sheet.study_design_sites_sheet import StudyDesignSitesSheet
-from usdm_excel.cross_ref import cross_references
 from usdm_model.code import Code
 
-def test_create(mocker):
-  cross_references.clear()
+
+def test_create(mocker, globals):
+  globals.cross_references.clear()
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Site_1', 'Org_1', 'Addr_1', 'Id_1', 'Site_2', 'Org_2', 'Addr_2', 'Id_2', 'Site_3', 'Org_3', 'Addr_3', 'Id_3']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     [ 'CRO1', 'CRO One',   'Study Registry', 'DUNS', '111111111', 'line|district|city|state|postal_code|GBR',      'Site1', 'Site One', 'Big Site' ],
     [ 'CRO2', 'CRO Two',   'Study Registry', 'DUNS', '222222222', 'line2,district2,city2,state2,postal_code2,FRA', 'Site2', 'Site Two', 'Little Site'],
     [ 'CRO3', 'CRO Three', 'Study Registry', 'DUNS', '333333333', 'line3,district3,city3,state3,postal_code3,FR',  'Site3', 'Site Three', 'Middle Site']
@@ -23,15 +21,15 @@
   mock_json = mocker.patch("json.load")
   mock_json.return_value = {}
   expected_1 = Code(id='Code1', code='code', codeSystem='codesys', codeSystemVersion='3', decode="GBR")
   expected_2 = Code(id='Code2', code='code', codeSystem='codesys', codeSystemVersion='3', decode="FRA")
   expected_3 = Code(id='Code3', code='code', codeSystem='codesys', codeSystemVersion='3', decode="FRA")
   mock_code = mocker.patch("usdm_excel.iso_3166.ISO3166.code")
   mock_code.side_effect=[expected_1, expected_2, expected_3]
-  sites = StudyDesignSitesSheet("")
+  sites = StudyDesignSitesSheet("", globals)
   assert len(sites.organizations) == 3
   assert len(sites.sites) == 3
   assert sites.organizations[0].id == 'Id_1'
   assert sites.organizations[0].identifier == '111111111'
   assert sites.organizations[0].identifierScheme == 'DUNS'
   assert sites.organizations[0].legalAddress.city == 'city'
   assert sites.organizations[0].legalAddress.country.decode == 'GBR'
@@ -40,37 +38,37 @@
   assert sites.organizations[1].identifier == '222222222'
   assert sites.organizations[1].identifierScheme == 'DUNS'
   assert sites.organizations[1].legalAddress.city == 'city2'
   assert sites.organizations[2].id == 'Id_3'
   assert sites.organizations[2].identifier == '333333333'
   assert sites.organizations[2].manages[0].id == 'Site_3'
   
-def test_create_empty(mocker):
-  cross_references.clear()
+def test_create_empty(mocker, globals):
+  globals.cross_references.clear()
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['studyIdentifierName', 'studyIdentifierDescription', 'studyIdentifierType'])
-  sites = StudyDesignSitesSheet("")
+  sites = StudyDesignSitesSheet("", globals)
   assert len(sites.organizations) == 0
 
-def test_read_cell_by_name_error(mocker):
-  cross_references.clear()
+def test_read_cell_by_name_error(mocker, globals):
+  globals.cross_references.clear()
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     [ 'CRO1', 'CRO One', 'DUNS', '111111111', 'line|district|city|state|postal_code|GBR',      'Site1', 'Site One', 'Big Site' ],
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['name', 'label', 'identifierScheme', 'identifier', 'address', 'siteName', 'siteLabel', 'siteDescription'])
-  sites = StudyDesignSitesSheet("")
+  sites = StudyDesignSitesSheet("", globals)
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "studyDesignSites"
   assert mock_error.call_args[0][1] == None
   assert mock_error.call_args[0][2] == None
-  assert mock_error.call_args[0][3] == "Exception 'Failed to detect column(s) 'type' in sheet' raised reading sheet."
+  assert mock_error.call_args[0][3] == "Exception. Error [Failed to detect column(s) 'type' in sheet] while reading sheet 'studyDesignSites'. See log for additional details."
```

### Comparing `usdm-0.48.0/tests/test_study_design_timing_sheet.py` & `usdm-0.49.0/tests/test_study_design_timing_sheet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 import pandas as pd
-
 from usdm_excel.study_design_timing_sheet.study_design_timing_sheet import StudyDesignTimingSheet
 from usdm_excel.study_design_timing_sheet.window_type import WindowType
-from usdm_excel.errors.errors import error_manager 
 
-def test_create(mocker):
-  error_manager.clear()
+
+def test_create(mocker, globals):
+  globals.errors_and_logging.errors().clear()
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Range1', 'Code1', 'Code2', 'TimingId_1', 'Code3', 'Code4', 'TimingId_2', 'Code5', 'Code6', 'TimingId_3']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     ['Timing 1', 'Timing One', 'T1', 'After', 'X1', 'X2', '3 days', 'S2S', '-1..1 day'],
     ['Timing 2', 'Timing Two', 'T2', 'Before', 'X2', 'X3', '10 days', 'E2S', ''], 
     ['Timing 3', 'Timing Three', 'T3', 'Fixed', 'X4', 'X5', '3 days', 'e2e', '']
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['name', 'description', 'label', 'type', 'from', 'to', 'timingValue', 'toFrom', 'window'])
 
-  items = StudyDesignTimingSheet("")
-  #print(f"ERRORS: {[item.to_dict() for item in error_manager.items]}")
+  items = StudyDesignTimingSheet("", globals)
+  #print(f"ERRORS: {[item.to_dict() for item in globals.errors_and_logging.errors().items]}")
   #print(f"ITEMS: {items.items}")
-  assert len( error_manager.items) == 0
+  assert len( globals.errors_and_logging.errors().items) == 0
   assert len(items.items) == 3
   assert items.items[0].id == 'TimingId_1'
   assert items.items[0].name == 'Timing 1'
   assert items.items[0].description == 'Timing One'
   assert items.items[0].type.decode == 'After'
   assert items.items[1].id == 'TimingId_2'
   assert items.items[1].description == 'Timing Two'
   assert items.items[1].type.decode == 'Before'
   assert items.items[2].id == 'TimingId_3'
   assert items.items[2].type.decode == 'Fixed Reference'
 
-# def test_timepoint_type(mocker):
+# def test_timepoint_type(mocker, globals):
 #   mocked_open = mocker.mock_open(read_data="File")
 #   mocker.patch("builtins.open", mocked_open)
 #   mock_read = mocker.patch("pandas.read_excel")
 #   data = { 'col_1': [ 'A:', 'P: 2D ', 'P2:2D', 'C:', 'N3: 3 weeks', 'N: +2 days', 'P: -3 hrs' ] }
 #   mock_read.return_value = pd.DataFrame.from_dict(data)
 #   parent = BaseSheet("", "")
 #   test_data = [
@@ -54,55 +53,55 @@
 #   for index, test in enumerate(test_data):
 #     item = TimepointType(parent, test[0], test[1])
 #     assert(item.timing_type) == test[2]
 #     assert(item.relative_ref) == test[3]
 #     assert(item.description) == test[4]
 #     assert(item.value) == test[5]
 
-# def test_timepoint_type_error(mocker):
+# def test_timepoint_type_error(mocker, globals):
 #   mocked_open = mocker.mock_open(read_data="File")
 #   mocker.patch("builtins.open", mocked_open)
 #   mock_read = mocker.patch("pandas.read_excel")
 #   data = { 'col_1': [ 'A', 'P: 2 ', '', 'P2: 2 decades' ] }
 #   mock_read.return_value = pd.DataFrame.from_dict(data)
 #   parent = BaseSheet("", "Sheet X")
 #   test_data = [
 #     (0,0,"Could not decode the timing value, no ':' detected in 'A'"),
 #     (1,0,"Could not decode the duration value, no value and units found in '2'"),
 #     (2,0,"Could not decode the timing value, cell was empty"),
 #     (3,0,"Could not decode the duration value '2 decades'"),
 #   ]
 #   for index, test in enumerate(test_data):
-#     mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+#     mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
 #     item = TimepointType(parent, test[0], test[1])
 #     mock_error.assert_called()
 #     assert mock_error.call_args[0][0] == "Sheet X"
 #     assert mock_error.call_args[0][1] == test[0] + 1
 #     assert mock_error.call_args[0][2] == test[1] + 1
 #     assert mock_error.call_args[0][3] == test[2]
 
-def test_window_type(mocker):
+def test_window_type(mocker, globals):
   test_data = [
     ('1..1 Days', "P1D", "P1D", '1..1 Days'),
     (' -1..1 days', "P1D", "P1D", '-1..1 days'),
     ('-1 .. 1 weeks ', "P1W", "P1W", '-1 .. 1 weeks'),
     (None, None, None, ''),
   ]
   for index, test in enumerate(test_data):
-    error_manager.clear()
-    item = WindowType(test[0])
+    globals.errors_and_logging.errors().clear()
+    item = WindowType(test[0], globals)
     assert(item.lower) == test[1]
     assert(item.upper) == test[2]
     assert(item.label) == test[3]
     assert(item.errors) == [] 
 
-def test_window_type_error(mocker):
+def test_window_type_error(mocker, globals):
   test_data = [
     ('1.. Days',"Could not decode the range value, possible typographical errors '1.. Days'"),
     ('-1.1 days',"Could not decode the range value, possible typographical errors '-1.1 days'"),
     ('-1 .. 1',"Could not decode the range value, possible typographical errors '-1 .. 1'"),
     (' .. 1 Weeks',"Could not decode the range value '.. 1 Weeks'")
   ]
   for index, test in enumerate(test_data):
-    error_manager.clear()
-    item = WindowType(test[0])
+    globals.errors_and_logging.errors().clear()
+    item = WindowType(test[0], globals)
     assert item.errors == [test[1]]
```

### Comparing `usdm-0.48.0/tests/test_study_identifiers_sheet.py` & `usdm-0.49.0/tests/test_study_identifiers_sheet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import pytest
 import pandas as pd
-
 from usdm_excel.study_identifiers_sheet.study_identifiers_sheet import StudyIdentifiersSheet
-from usdm_excel.cross_ref import cross_references
 from usdm_model.code import Code
 
-def test_create(mocker):
-  cross_references.clear()
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+
+def test_create(mocker, globals):
+  globals.cross_references.clear()
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Code_1', 'Org_1', 'Addr_1', 'Id_1', 'Code_2', 'Org_2', 'Addr_2', 'Id_2', 'Code_3', 'Org_3', 'Addr_3', 'Id_3']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     [ 'USGOV', 'CT-GOV', 'ClinicalTrials.gov', 'Study Registry', 'NCT12345678', 'line|district|city|state|postal_code|GBR' ],
     [ 'USGOV2', 'CT-GOV2', 'ClinicalTrials2.gov', 'Study Registry', 'NCT12345679', 'line2,district2,city2,state2,postal_code2,FRA' ],
     [ 'USGOV3', 'CT-GOV3', 'ClinicalTrials3.gov', 'Study Registry', 'NCT123456710', 'line3,district3,city3,state3,postal_code3,FR' ]
@@ -21,103 +19,136 @@
   mock_json = mocker.patch("json.load")
   mock_json.return_value = {}
   expected_1 = Code(id='Code1', code='code', codeSystem='codesys', codeSystemVersion='3', decode="GBR")
   expected_2 = Code(id='Code2', code='code', codeSystem='codesys', codeSystemVersion='3', decode="FRA")
   expected_3 = Code(id='Code3', code='code', codeSystem='codesys', codeSystemVersion='3', decode="FRA")
   mock_code = mocker.patch("usdm_excel.iso_3166.ISO3166.code")
   mock_code.side_effect=[expected_1, expected_2, expected_3]
-  ids = StudyIdentifiersSheet("")
+  ids = StudyIdentifiersSheet("", globals)
+  assert len(ids.identifiers) == 3
+  assert ids.identifiers[0].id == 'Id_1'
+  assert ids.identifiers[0].studyIdentifier == 'NCT12345678'
+  assert ids.identifiers[0].studyIdentifierScope.name == 'ClinicalTrials.gov'
+  assert ids.identifiers[0].studyIdentifierScope.legalAddress.city == 'city'
+  assert ids.identifiers[1].id == 'Id_2'
+  assert ids.identifiers[1].studyIdentifier == 'NCT12345679'
+  assert ids.identifiers[1].studyIdentifierScope.name == 'ClinicalTrials2.gov'
+  assert ids.identifiers[1].studyIdentifierScope.legalAddress.city == 'city2'
+  assert ids.identifiers[2].id == 'Id_3'
+  assert ids.identifiers[2].studyIdentifier == 'NCT123456710'
+  
+def test_create_with_z(mocker, globals):
+  globals.cross_references.clear()
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
+  mock_id.side_effect=['Code_1', 'Org_1', 'Addr_1', 'Id_1', 'Code_2', 'Org_2', 'Addr_2', 'Id_2', 'Code_3', 'Org_3', 'Addr_3', 'Id_3']
+  mocked_open = mocker.mock_open(read_data="File")
+  mocker.patch("builtins.open", mocked_open)
+  data = [
+    [ 'USGOV', 'CT-GOV', 'ClinicalTrials.gov', 'Study Registry', 'NCT12345678', 'line|district|city|state|postal_code|GBR' ],
+    [ 'USGOV2', 'CT-GOV2', 'ClinicalTrials2.gov', 'Study Registry', 'NCT12345679', 'line2,district2,city2,state2,postal_code2,FRA' ],
+    [ 'USGOV3', 'CT-GOV3', 'ClinicalTrials3.gov', 'Study Registry', 'NCT123456710', 'line3,district3,city3,state3,postal_code3,FR' ]
+  ]
+  mock_read = mocker.patch("pandas.read_excel")
+  mock_read.return_value = pd.DataFrame(data, columns=['organizationIdentifierScheme', 'organizationIdentifier', 'organizationName', 'organizationType', 'studyIdentifier', 'organizationAddress'])
+  mock_json = mocker.patch("json.load")
+  mock_json.return_value = {}
+  expected_1 = Code(id='Code1', code='code', codeSystem='codesys', codeSystemVersion='3', decode="GBR")
+  expected_2 = Code(id='Code2', code='code', codeSystem='codesys', codeSystemVersion='3', decode="FRA")
+  expected_3 = Code(id='Code3', code='code', codeSystem='codesys', codeSystemVersion='3', decode="FRA")
+  mock_code = mocker.patch("usdm_excel.iso_3166.ISO3166.code")
+  mock_code.side_effect=[expected_1, expected_2, expected_3]
+  ids = StudyIdentifiersSheet("", globals)
   assert len(ids.identifiers) == 3
   assert ids.identifiers[0].id == 'Id_1'
   assert ids.identifiers[0].studyIdentifier == 'NCT12345678'
   assert ids.identifiers[0].studyIdentifierScope.name == 'ClinicalTrials.gov'
   assert ids.identifiers[0].studyIdentifierScope.legalAddress.city == 'city'
   assert ids.identifiers[1].id == 'Id_2'
   assert ids.identifiers[1].studyIdentifier == 'NCT12345679'
   assert ids.identifiers[1].studyIdentifierScope.name == 'ClinicalTrials2.gov'
   assert ids.identifiers[1].studyIdentifierScope.legalAddress.city == 'city2'
   assert ids.identifiers[2].id == 'Id_3'
   assert ids.identifiers[2].studyIdentifier == 'NCT123456710'
   
-def test_create_new_columns(mocker):
-  cross_references.clear()
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+def test_create_new_columns(mocker, globals):
+  globals.cross_references.clear()
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Code_1', 'Org_1', 'Addr_1', 'Id_1', 'Code_2', 'Org_2', 'Addr_2', 'Id_2', 'Code_3', 'Org_3', 'Addr_3', 'Id_3']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     [ 'USGOV', 'CT-GOV', 'ClinicalTrials.gov', 'CT.gov [1]', 'Study Registry', 'NCT12345678', 'line|district|city|state|postal_code|GBR' ],
     [ 'USGOV2', 'CT-GOV2', 'ClinicalTrials2.gov', '', 'Study Registry', 'NCT12345679', 'line2,district2,city2,state2,postal_code2,FRA' ],
     [ 'USGOV3', 'CT-GOV3', 'ClinicalTrials3.gov', 'CT.gov [3]', 'Study Registry', 'NCT123456710', 'line3,district3,city3,state3,postal_code3,FR' ]
   ]
   mock_read = mocker.patch("pandas.read_excel")
-  mock_read.return_value = pd.DataFrame(data, columns=['organisationIdentifierScheme', 'organisationIdentifier', 'name', 'label', 'type', 'studyIdentifier', 'organisationAddress'])
+  mock_read.return_value = pd.DataFrame(data, columns=['IdentifierScheme', 'organisationIdentifier', 'name', 'label', 'type', 'studyIdentifier', 'address'])
   mock_json = mocker.patch("json.load")
   mock_json.return_value = {}
   expected_1 = Code(id='Code1', code='code', codeSystem='codesys', codeSystemVersion='3', decode="GBR")
   expected_2 = Code(id='Code2', code='code', codeSystem='codesys', codeSystemVersion='3', decode="FRA")
   expected_3 = Code(id='Code3', code='code', codeSystem='codesys', codeSystemVersion='3', decode="FRA")
   mock_code = mocker.patch("usdm_excel.iso_3166.ISO3166.code")
   mock_code.side_effect=[expected_1, expected_2, expected_3]
-  ids = StudyIdentifiersSheet("")
+  ids = StudyIdentifiersSheet("", globals)
   assert len(ids.identifiers) == 3
   assert ids.identifiers[0].id == 'Id_1'
   assert ids.identifiers[0].studyIdentifier == 'NCT12345678'
   assert ids.identifiers[0].studyIdentifierScope.name == 'ClinicalTrials.gov'
   assert ids.identifiers[0].studyIdentifierScope.label == 'CT.gov [1]'
   assert ids.identifiers[0].studyIdentifierScope.legalAddress.city == 'city'
   assert ids.identifiers[1].id == 'Id_2'
   assert ids.identifiers[1].studyIdentifier == 'NCT12345679'
   assert ids.identifiers[1].studyIdentifierScope.name == 'ClinicalTrials2.gov'
   assert ids.identifiers[1].studyIdentifierScope.legalAddress.city == 'city2'
   assert ids.identifiers[1].studyIdentifierScope.label == ''
   assert ids.identifiers[2].id == 'Id_3'
   assert ids.identifiers[2].studyIdentifier == 'NCT123456710'
   
-def test_create_empty(mocker):
-  cross_references.clear()
+def test_create_empty(mocker, globals):
+  globals.cross_references.clear()
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['studyIdentifierName', 'studyIdentifierDescription', 'studyIdentifierType'])
-  ids = StudyIdentifiersSheet("")
+  ids = StudyIdentifiersSheet("", globals)
   assert len(ids.identifiers) == 0
 
-def test_read_cell_by_name_error(mocker):
-  cross_references.clear()
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
+def test_read_cell_by_name_error(mocker, globals):
+  globals.cross_references.clear()
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['Id 1', 'Id One']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['studyIdentifierName', 'studyIdentifierDescription'])
-  ids = StudyIdentifiersSheet("")
+  ids = StudyIdentifiersSheet("", globals)
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "studyIdentifiers"
   assert mock_error.call_args[0][1] == None
   assert mock_error.call_args[0][2] == None
-  assert mock_error.call_args[0][3] == "Exception 'Failed to detect column(s) 'organisationType, type' in sheet' raised reading sheet."
+  assert mock_error.call_args[0][3] == "Exception. Error [Failed to detect column(s) 'organisationType, organizationType, type' in sheet] while reading sheet 'studyIdentifiers'. See log for additional details."
   
-def test_address_error(mocker):
-  cross_references.clear()
-  mock_error = mocker.patch("usdm_excel.errors.errors.Errors.add")
-  mock_id = mocker.patch("usdm_excel.id_manager.build_id")
+def test_address_error(mocker, globals):
+  globals.cross_references.clear()
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
+  mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Code_1', 'Org_1', 'Addr_1', 'Id_1']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [
     [ 'USGOV', 'CT-GOV', 'ClinicalTrials.gov', 'Study Registry', 'NCT12345678', 'line|city|district|state|GBR' ],
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['organisationIdentifierScheme', 'organisationIdentifier', 'organisationName', 'organisationType', 'studyIdentifier', 'organisationAddress'])
   mock_json = mocker.patch("json.load")
   mock_json.return_value = {}
   expected_1 = Code(id='Code1', code='code', codeSystem='codesys', codeSystemVersion='3', decode="GBR")
   mock_code = mocker.patch("usdm_excel.iso_3166.ISO3166.code")
   mock_code.side_effect=[expected_1]
-  ids = StudyIdentifiersSheet("")
+  ids = StudyIdentifiersSheet("", globals)
   mock_error.assert_called()
   assert mock_error.call_args[0][0] == "studyIdentifiers"
   assert mock_error.call_args[0][1] == 1
   assert mock_error.call_args[0][2] == 6
-  assert mock_error.call_args[0][3] == "Address does not contain the required fields (line, district, city, state, postal code and country code) using '|' separator characters, only 5 found"
+  assert mock_error.call_args[0][3] == "Address 'line|city|district|state|GBR' does not contain the required fields (first line, district, city, state, postal code and country code) using '|' separator characters, only 5 found"
```

### Comparing `usdm-0.48.0/tests/test_study_sheet.py` & `usdm-0.49.0/tests/test_study_sheet.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 xfail = pytest.mark.xfail
 
 from usdm_excel.study_sheet.study_sheet import StudySheet
 from usdm_excel.base_sheet import BaseSheet
 
 @xfail
-def test_create(mocker):
+def test_create(mocker, globals):
   assert 0
   # mocked_open = mocker.mock_open(read_data="File")
   # mocker.patch("builtins.open", mocked_open)
   # mock_read = mocker.patch("pandas.read_excel")
   # data = { 
   #   'col_1': 
   #     [ 'studyTitle', 'studyVersion', 'studyType', 'studyPhase', 'studyAcronym', 'studyRationale',
```

