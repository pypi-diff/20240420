# Comparing `tmp/mns-scheduler-1.0.2.9.tar.gz` & `tmp/mns-scheduler-1.0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.2.9.tar", last modified: Thu Apr 18 15:09:51 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.3.0.tar", last modified: Sat Apr 20 14:08:35 2024, max compression
```

## Comparing `mns-scheduler-1.0.2.9.tar` & `mns-scheduler-1.0.3.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.267449 mns-scheduler-1.0.2.9/
--rw-rw-rw-   0        0        0       62 2024-04-18 15:09:51.267449 mns-scheduler-1.0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.239524 mns-scheduler-1.0.2.9/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.9/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.242515 mns-scheduler-1.0.2.9/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.9/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.2.9/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.243513 mns-scheduler-1.0.2.9/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.9/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20332 2024-04-18 14:12:36.000000 mns-scheduler-1.0.2.9/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.243513 mns-scheduler-1.0.2.9/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.244510 mns-scheduler-1.0.2.9/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.246505 mns-scheduler-1.0.2.9/mns_scheduler/concept/em/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/em/__init__.py
--rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.246505 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.247502 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/app/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.248499 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0    10238 2024-04-13 05:32:34.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     1662 2024-04-15 02:52:26.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.250494 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/symbol/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8757 2024-04-16 06:53:57.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.251491 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/web/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/web/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-13 05:23:41.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.252489 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/wen_cai/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.253486 mns-scheduler-1.0.2.9/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.2.9/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.254484 mns-scheduler-1.0.2.9/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.254484 mns-scheduler-1.0.2.9/mns_scheduler/ipo/
--rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.2.9/mns_scheduler/ipo/__init__.py
--rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.2.9/mns_scheduler/ipo/auto_ipo_buy_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.255481 mns-scheduler-1.0.2.9/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.256478 mns-scheduler-1.0.2.9/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.2.9/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7988 2024-04-18 13:32:07.000000 mns-scheduler-1.0.2.9/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.257475 mns-scheduler-1.0.2.9/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.2.9/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.257475 mns-scheduler-1.0.2.9/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.258473 mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.258473 mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     8016 2024-04-02 13:03:08.000000 mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.259470 mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.260467 mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0     7527 2024-04-02 14:49:34.000000 mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.261464 mns-scheduler-1.0.2.9/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.9/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.2.9/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.262462 mns-scheduler-1.0.2.9/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.2.9/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.265454 mns-scheduler-1.0.2.9/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.2.9/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.2.9/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.2.9/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.9/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7534 2024-04-16 13:51:28.000000 mns-scheduler-1.0.2.9/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.266452 mns-scheduler-1.0.2.9/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.9/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    13768 2024-04-16 14:08:50.000000 mns-scheduler-1.0.2.9/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.2.9/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:09:51.266452 mns-scheduler-1.0.2.9/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-04-18 15:09:51.000000 mns-scheduler-1.0.2.9/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3014 2024-04-18 15:09:51.000000 mns-scheduler-1.0.2.9/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 15:09:51.000000 mns-scheduler-1.0.2.9/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-18 15:09:51.000000 mns-scheduler-1.0.2.9/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 15:09:51.267449 mns-scheduler-1.0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-04-18 15:09:49.000000 mns-scheduler-1.0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.558014 mns-scheduler-1.0.3.0/
+-rw-rw-rw-   0        0        0       62 2024-04-20 14:08:35.558014 mns-scheduler-1.0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.523912 mns-scheduler-1.0.3.0/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.0/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.526877 mns-scheduler-1.0.3.0/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.0/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.3.0/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.528900 mns-scheduler-1.0.3.0/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.0/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20332 2024-04-18 14:12:36.000000 mns-scheduler-1.0.3.0/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.528900 mns-scheduler-1.0.3.0/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.529896 mns-scheduler-1.0.3.0/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.532081 mns-scheduler-1.0.3.0/mns_scheduler/concept/em/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/em/__init__.py
+-rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.533080 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.534078 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/app/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.535075 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0    10238 2024-04-13 05:32:34.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     1662 2024-04-15 02:52:26.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.537069 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/symbol/__init__.py
+-rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8757 2024-04-16 06:53:57.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.538067 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/web/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/web/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-13 05:23:41.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.539065 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/wen_cai/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.541059 mns-scheduler-1.0.3.0/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.3.0/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.542056 mns-scheduler-1.0.3.0/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.543054 mns-scheduler-1.0.3.0/mns_scheduler/ipo/
+-rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.3.0/mns_scheduler/ipo/__init__.py
+-rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.3.0/mns_scheduler/ipo/auto_ipo_buy_api.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.543054 mns-scheduler-1.0.3.0/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.545048 mns-scheduler-1.0.3.0/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.3.0/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7988 2024-04-18 13:32:07.000000 mns-scheduler-1.0.3.0/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.546045 mns-scheduler-1.0.3.0/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.3.0/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.546045 mns-scheduler-1.0.3.0/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.547043 mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.547043 mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     8016 2024-04-02 13:03:08.000000 mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.549038 mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.550035 mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-20 14:08:05.000000 mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.551033 mns-scheduler-1.0.3.0/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.0/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.3.0/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.552030 mns-scheduler-1.0.3.0/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.3.0/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.556019 mns-scheduler-1.0.3.0/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.3.0/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.3.0/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.3.0/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.0/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7534 2024-04-16 13:51:28.000000 mns-scheduler-1.0.3.0/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.557016 mns-scheduler-1.0.3.0/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.0/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    13768 2024-04-16 14:08:50.000000 mns-scheduler-1.0.3.0/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.3.0/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:08:35.558014 mns-scheduler-1.0.3.0/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-04-20 14:08:35.000000 mns-scheduler-1.0.3.0/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3014 2024-04-20 14:08:35.000000 mns-scheduler-1.0.3.0/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 14:08:35.000000 mns-scheduler-1.0.3.0/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-20 14:08:35.000000 mns-scheduler-1.0.3.0/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 14:08:35.558014 mns-scheduler-1.0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-04-20 14:08:05.000000 mns-scheduler-1.0.3.0/setup.py
```

### Comparing `mns-scheduler-1.0.2.9/README.md` & `mns-scheduler-1.0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.3.0/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.3.0/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.3.0/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py` & `mns-scheduler-1.0.3.0/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/concept/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.3.0/mns_scheduler/concept/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/concept/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.3.0/mns_scheduler/concept/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/concept/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.3.0/mns_scheduler/concept/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py` & `mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py` & `mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.3.0/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.3.0/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.3.0/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.3.0/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.3.0/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.3.0/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.3.0/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.3.0/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -76,14 +76,17 @@
     # 更新一级和二级之间的关联关系
     # 找出新增精选指数
     sync_best_choose_first_index.sync_best_choose_index()
     logger.info("同步开票啦精选概念指数完成")
     # 同步精选概念股票组成
     multi_thread_sync_kpl_best_choose_detail()
     logger.info("同步开票啦精选概念股票组成完成")
+    # 更新开票啦空名字名称
+    update_null_name()
+    logger.info("更新开票啦空名字名称")
 
 
 # 更新一二级关系
 def update_best_choose_plate_relation():
     first_index_df = sync_best_choose_first_index.choose_field_choose_first_index()
     kpl_all_concept_df = kpl_concept_common_service_api.get_kpl_all_concept()
     for first_index_df_one in first_index_df.itertuples():
@@ -131,12 +134,55 @@
         first_index_df['plate_code'].isin(list(kpl_sub_concept_df_exist['plate_code']))]
     if data_frame_util.is_not_empty(kpl_sub_concept_df_change):
         update_query = {"plate_code": {"$in": list(kpl_sub_concept_df_change['plate_code'])}}
         new_values = {"$set": {"index_class": kpl_constant.FIRST_INDEX}}
         mongodb_util.update_many(update_query, new_values, db_name_constant.KPL_BEST_CHOOSE_INDEX)
 
 
+def update_null_name():
+    query = {"plate_name": ''}
+    kpl_best_choose_index_df = mongodb_util.find_query_data(db_name_constant.KPL_BEST_CHOOSE_INDEX, query)
+    if data_frame_util.is_empty(kpl_best_choose_index_df):
+        return
+    else:
+        kpl_best_choose_index_df_sub = kpl_best_choose_index_df.loc[
+            kpl_best_choose_index_df["index_class"] == kpl_constant.SUB_INDEX]
+        if data_frame_util.is_not_empty(kpl_best_choose_index_df_sub):
+            for sub_one in kpl_best_choose_index_df_sub.itertuples():
+                try:
+                    first_plate_code = sub_one.first_plate_code
+                    sub_plate_code = sub_one.plate_code
+                    kpl_best_choose_sub_index_detail = selection_plate_api.best_choose_sub_index(first_plate_code)
+                    sub_kpl_best_choose_sub_index_detail = kpl_best_choose_sub_index_detail.loc[
+                        kpl_best_choose_sub_index_detail['plate_code'] == sub_plate_code]
+                    if data_frame_util.is_not_empty(sub_kpl_best_choose_sub_index_detail):
+                        plate_name = list(sub_kpl_best_choose_sub_index_detail['plate_name'])[0]
+                        new_values = {"$set": {"plate_name": plate_name}}
+                        update_query = {"plate_code": sub_plate_code}
+                        mongodb_util.update_many(update_query, new_values, db_name_constant.KPL_BEST_CHOOSE_INDEX)
+                except BaseException as e:
+                    logger.error("更新板块kpl概念名称出现异常:{},{}", sub_plate_code, e)
+        kpl_best_choose_index_df_first = kpl_best_choose_index_df.loc[
+            kpl_best_choose_index_df["index_class"] == kpl_constant.FIRST_INDEX]
+        if data_frame_util.is_not_empty(kpl_best_choose_index_df_first):
+            for first_one in kpl_best_choose_index_df_sub.itertuples():
+                try:
+                    first_plate_code = first_one.plate_code
+                    first_index_df = sync_best_choose_first_index.choose_field_choose_first_index()
+                    first_index_df_one = first_index_df.loc[first_index_df['plate_code'] == first_plate_code]
+                    if data_frame_util.is_not_empty(first_index_df_one):
+                        plate_name = list(first_index_df_one['plate_name'])[0]
+                        new_values = {"$set": {"plate_name": plate_name}}
+                        update_query = {"plate_code": first_plate_code}
+                        mongodb_util.update_many(update_query, new_values, db_name_constant.KPL_BEST_CHOOSE_INDEX)
+                except BaseException as e:
+                    logger.error("更新板块kpl概念名称出现异常:{},{}", first_plate_code, e)
+
+    return kpl_best_choose_index_df
+
+
 if __name__ == '__main__':
+    update_null_name()
     update_best_choose_plate_relation()
 
     # 同步第一和第二级别精选指数
     sync_all_plate_info()
```

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.3.0/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.3.0/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.3.0/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.3.0/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.3.0/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.3.0/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.3.0/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.3.0/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.3.0/mns_scheduler/zz_task/data_sync_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.3.0/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.9/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.3.0/mns_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

