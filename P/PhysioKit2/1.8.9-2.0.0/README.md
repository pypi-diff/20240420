# Comparing `tmp/PhysioKit2-1.8.9.tar.gz` & `tmp/physiokit2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PhysioKit2-1.8.9.tar", last modified: Sat Apr  6 23:37:13 2024, max compression
+gzip compressed data, was "physiokit2-2.0.0.tar", last modified: Sat Apr 20 13:58:39 2024, max compression
```

## Comparing `PhysioKit2-1.8.9.tar` & `physiokit2-2.0.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.407923 PhysioKit2-1.8.9/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1084 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/LICENSE
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    14082 2024-04-06 23:37:13.407472 PhysioKit2-1.8.9/PKG-INFO
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    13352 2024-04-06 23:33:15.000000 PhysioKit2-1.8.9/README.md
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)       38 2024-04-06 23:37:13.407976 PhysioKit2-1.8.9/setup.cfg
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1878 2024-04-06 23:36:24.000000 PhysioKit2-1.8.9/setup.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.388281 PhysioKit2-1.8.9/src/
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.392673 PhysioKit2-1.8.9/src/PhysioKit2/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/__init__.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.394081 PhysioKit2-1.8.9/src/PhysioKit2/analysis_helper/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/analysis_helper/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    33222 2024-04-06 16:59:36.000000 PhysioKit2-1.8.9/src/PhysioKit2/analysis_helper/process_signals.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.394492 PhysioKit2-1.8.9/src/PhysioKit2/analysis_helper/sample_data/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/analysis_helper/sample_data/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/analysis_helper/sample_data/download data from PhysioKit GitHub repo page.txt
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.394755 PhysioKit2-1.8.9/src/PhysioKit2/analysis_helper/utils/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/analysis_helper/utils/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3203 2023-10-21 20:33:26.000000 PhysioKit2-1.8.9/src/PhysioKit2/analysis_helper/utils/load_data.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.395154 PhysioKit2-1.8.9/src/PhysioKit2/configs/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/configs/__init__.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.396293 PhysioKit2-1.8.9/src/PhysioKit2/configs/arm_due/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/configs/arm_due/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      365 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/configs/arm_due/sw_config.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      374 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/configs/arm_due/sw_config_client.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      375 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/configs/arm_due/sw_config_server.json
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.397342 PhysioKit2-1.8.9/src/PhysioKit2/configs/avr_default/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/configs/avr_default/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      364 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/configs/avr_default/sw_config.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      369 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/configs/avr_default/sw_config_client.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      369 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/configs/avr_default/sw_config_server.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1109 2023-10-24 18:51:21.000000 PhysioKit2-1.8.9/src/PhysioKit2/configs/exp_config_phys.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    22491 2023-10-21 22:16:23.000000 PhysioKit2-1.8.9/src/PhysioKit2/form.ui
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    19094 2023-10-21 22:16:23.000000 PhysioKit2-1.8.9/src/PhysioKit2/form_ui.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.398599 PhysioKit2-1.8.9/src/PhysioKit2/images/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/images/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    42512 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/images/banner.png
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3095 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/images/color_bar.png
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    91499 2023-10-23 00:50:14.000000 PhysioKit2-1.8.9/src/PhysioKit2/images/sq_indication.png
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    35148 2024-04-06 16:59:36.000000 PhysioKit2-1.8.9/src/PhysioKit2/main.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/register_dummy.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.400349 PhysioKit2-1.8.9/src/PhysioKit2/sqa/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/sqa/__init__.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.402739 PhysioKit2-1.8.9/src/PhysioKit2/sqa/ckpt/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)   484328 2024-04-05 12:35:26.000000 PhysioKit2-1.8.9/src/PhysioKit2/sqa/ckpt/SQAPhysMD.pth
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/sqa/ckpt/__init__.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.403448 PhysioKit2-1.8.9/src/PhysioKit2/sqa/config/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      616 2024-04-06 17:04:06.000000 PhysioKit2-1.8.9/src/PhysioKit2/sqa/config/SQAPhysMD.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/sqa/config/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3860 2024-04-06 16:59:36.000000 PhysioKit2-1.8.9/src/PhysioKit2/sqa/inference.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     5734 2024-04-06 16:59:36.000000 PhysioKit2-1.8.9/src/PhysioKit2/sqa/inference_thread.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.404167 PhysioKit2-1.8.9/src/PhysioKit2/sqa/model/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    13247 2024-04-06 16:59:36.000000 PhysioKit2-1.8.9/src/PhysioKit2/sqa/model/SQAPhysMD.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/sqa/model/__init__.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.406920 PhysioKit2-1.8.9/src/PhysioKit2/utils/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/utils/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     8235 2024-04-06 16:54:52.000000 PhysioKit2-1.8.9/src/PhysioKit2/utils/acquisition.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    10939 2023-12-01 13:56:18.000000 PhysioKit2-1.8.9/src/PhysioKit2/utils/biofeedback.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      384 2023-11-01 02:26:11.000000 PhysioKit2-1.8.9/src/PhysioKit2/utils/config.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1877 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/utils/data_processing_lib.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3999 2023-12-01 00:17:10.000000 PhysioKit2-1.8.9/src/PhysioKit2/utils/external_sync.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     5682 2023-12-01 13:54:03.000000 PhysioKit2-1.8.9/src/PhysioKit2/utils/file_ops.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     2186 2023-10-21 17:57:29.000000 PhysioKit2-1.8.9/src/PhysioKit2/utils/load_data.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 23:37:13.407168 PhysioKit2-1.8.9/src/PhysioKit2.egg-info/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    14082 2024-04-06 23:37:13.000000 PhysioKit2-1.8.9/src/PhysioKit2.egg-info/PKG-INFO
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1971 2024-04-06 23:37:13.000000 PhysioKit2-1.8.9/src/PhysioKit2.egg-info/SOURCES.txt
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        1 2024-04-06 23:37:13.000000 PhysioKit2-1.8.9/src/PhysioKit2.egg-info/dependency_links.txt
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      119 2024-04-06 23:37:13.000000 PhysioKit2-1.8.9/src/PhysioKit2.egg-info/entry_points.txt
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      139 2024-04-06 23:37:13.000000 PhysioKit2-1.8.9/src/PhysioKit2.egg-info/requires.txt
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)       11 2024-04-06 23:37:13.000000 PhysioKit2-1.8.9/src/PhysioKit2.egg-info/top_level.txt
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.208469 physiokit2-2.0.0/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1084 2023-10-21 17:57:29.000000 physiokit2-2.0.0/LICENSE
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    14500 2024-04-20 13:58:39.208187 physiokit2-2.0.0/PKG-INFO
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    13771 2024-04-20 13:57:44.000000 physiokit2-2.0.0/README.md
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)       38 2024-04-20 13:58:39.208509 physiokit2-2.0.0/setup.cfg
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1878 2024-04-20 13:22:49.000000 physiokit2-2.0.0/setup.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.191543 physiokit2-2.0.0/src/
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.194443 physiokit2-2.0.0/src/PhysioKit2/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/__init__.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.195402 physiokit2-2.0.0/src/PhysioKit2/analysis_helper/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/analysis_helper/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    33222 2024-04-06 16:59:36.000000 physiokit2-2.0.0/src/PhysioKit2/analysis_helper/process_signals.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.195683 physiokit2-2.0.0/src/PhysioKit2/analysis_helper/sample_data/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/analysis_helper/sample_data/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/analysis_helper/sample_data/download data from PhysioKit GitHub repo page.txt
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.195850 physiokit2-2.0.0/src/PhysioKit2/analysis_helper/utils/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/analysis_helper/utils/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3203 2023-10-21 20:33:26.000000 physiokit2-2.0.0/src/PhysioKit2/analysis_helper/utils/load_data.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.196192 physiokit2-2.0.0/src/PhysioKit2/configs/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/configs/__init__.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.196918 physiokit2-2.0.0/src/PhysioKit2/configs/arm_due/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/configs/arm_due/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      365 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/configs/arm_due/sw_config.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      374 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/configs/arm_due/sw_config_client.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      375 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/configs/arm_due/sw_config_server.json
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.197552 physiokit2-2.0.0/src/PhysioKit2/configs/avr_default/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/configs/avr_default/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      364 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/configs/avr_default/sw_config.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      369 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/configs/avr_default/sw_config_client.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      369 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/configs/avr_default/sw_config_server.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1109 2023-10-24 18:51:21.000000 physiokit2-2.0.0/src/PhysioKit2/configs/exp_config_phys.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    22491 2023-10-21 22:16:23.000000 physiokit2-2.0.0/src/PhysioKit2/form.ui
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    19094 2023-10-21 22:16:23.000000 physiokit2-2.0.0/src/PhysioKit2/form_ui.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.198495 physiokit2-2.0.0/src/PhysioKit2/images/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/images/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    42512 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/images/banner.png
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3095 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/images/color_bar.png
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    91499 2023-10-23 00:50:14.000000 physiokit2-2.0.0/src/PhysioKit2/images/sq_indication.png
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    35148 2024-04-06 16:59:36.000000 physiokit2-2.0.0/src/PhysioKit2/main.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/register_dummy.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.199492 physiokit2-2.0.0/src/PhysioKit2/sqa/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/sqa/__init__.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.202225 physiokit2-2.0.0/src/PhysioKit2/sqa/ckpt/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)  1064611 2024-04-20 13:19:48.000000 physiokit2-2.0.0/src/PhysioKit2/sqa/ckpt/SQAPhysMD.pth
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/sqa/ckpt/__init__.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.203917 physiokit2-2.0.0/src/PhysioKit2/sqa/config/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      616 2024-04-06 17:04:06.000000 physiokit2-2.0.0/src/PhysioKit2/sqa/config/SQAPhysMD.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/sqa/config/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3860 2024-04-06 16:59:36.000000 physiokit2-2.0.0/src/PhysioKit2/sqa/inference.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     5734 2024-04-06 16:59:36.000000 physiokit2-2.0.0/src/PhysioKit2/sqa/inference_thread.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.205387 physiokit2-2.0.0/src/PhysioKit2/sqa/model/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    13247 2024-04-06 16:59:36.000000 physiokit2-2.0.0/src/PhysioKit2/sqa/model/SQAPhysMD.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/sqa/model/__init__.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.207794 physiokit2-2.0.0/src/PhysioKit2/utils/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/utils/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     8235 2024-04-06 16:54:52.000000 physiokit2-2.0.0/src/PhysioKit2/utils/acquisition.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    10939 2023-12-01 13:56:18.000000 physiokit2-2.0.0/src/PhysioKit2/utils/biofeedback.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      384 2023-11-01 02:26:11.000000 physiokit2-2.0.0/src/PhysioKit2/utils/config.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1877 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/utils/data_processing_lib.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3999 2023-12-01 00:17:10.000000 physiokit2-2.0.0/src/PhysioKit2/utils/external_sync.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     5682 2023-12-01 13:54:03.000000 physiokit2-2.0.0/src/PhysioKit2/utils/file_ops.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     2186 2023-10-21 17:57:29.000000 physiokit2-2.0.0/src/PhysioKit2/utils/load_data.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-20 13:58:39.207978 physiokit2-2.0.0/src/PhysioKit2.egg-info/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    14500 2024-04-20 13:58:39.000000 physiokit2-2.0.0/src/PhysioKit2.egg-info/PKG-INFO
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1971 2024-04-20 13:58:39.000000 physiokit2-2.0.0/src/PhysioKit2.egg-info/SOURCES.txt
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        1 2024-04-20 13:58:39.000000 physiokit2-2.0.0/src/PhysioKit2.egg-info/dependency_links.txt
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      119 2024-04-20 13:58:39.000000 physiokit2-2.0.0/src/PhysioKit2.egg-info/entry_points.txt
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      139 2024-04-20 13:58:39.000000 physiokit2-2.0.0/src/PhysioKit2.egg-info/requires.txt
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)       11 2024-04-20 13:58:39.000000 physiokit2-2.0.0/src/PhysioKit2.egg-info/top_level.txt
```

### Comparing `PhysioKit2-1.8.9/LICENSE` & `physiokit2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/PKG-INFO` & `physiokit2-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PhysioKit2
-Version: 1.8.9
+Version: 2.0.0
 Summary: PhysioKit: An Open-Source, Low-Cost Physiological Computing Toolkit for Single- and Multi-User Studies
 Home-page: https://github.com/PhysiologicAILab/PhysioKit
 Author: ['Jitesh Joshi', 'Katherine wang', 'Youngjun Cho']
 Author-email: youngjun.cho@ucl.ac.uk
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,94 +21,99 @@
 Requires-Dist: torch
 Requires-Dist: setuptools
 Requires-Dist: requests
 
 # **Overview of PhysioKit**
 
 Authors: Jitesh Joshi, Katherine Wang, and Youngjun Cho <br>
-Contact: Physiological Computing and Artificial Intelligence lab @ GDIH - WHO Collaboration Centre for Assistive Technology, UCL Computer Science  (<youngjun.cho@ucl.ac.uk>)
+Contact: Computational Physiology and Intelligence group @ GDIH - WHO Collaboration Centre for Assistive Technology, UCL Computer Science  (<youngjun.cho@ucl.ac.uk>)
 
 PhysioKit is a novel physiological computing toolkit which is open-source, accessible and affordable. HCI hobbyists and practitioners can easily access physiological sensing channels that help monitor our physiological signatures and vital signs including heart rate, heart rate variability, breathing rate, electrodermal activities. The toolkit works with a low-cost micro-controller such as Arduino. Currently, it supports acquiring EDA, Resp and PPG using any low-cost Arduino board.
 
 PhysioKit consists of (i) a sensor and hardware layer that can be configured in a modular manner along with research needs, (ii) a software application layer that enables real-time data collection, streaming and visualization for both single and multi-user experiments. This also supports basic visual biofeedback configurations and multi-signal synchronization for co-located or remote multi-user settings.
 
 Below figure shows architecture of PhysioKit:
-<p align="left">
-<img src="images/architecture.png" alt="Architecture of PhysioKit" width="1024"/>
-</p>
+
+![Architecture of PhysioKit](https://github.com/PhysiologicAILab/PhysioKit/blob/main/images/architecture.png|width=1024)
 
 ## **Installation**
 
 Pre-requisite: Python >= 3.8
 
 It is recommended to create separate Python virtual environment, which can be achieved using venv/ anaconda/ miniconda as follows. After creating the environment, activate the same.
 
 Using venv:
 
+Creating virtual environment using venv (recommended for Windows users) -- To be executed once.
 
-    Creating virtual environment using venv (recommended for Windows users) -- To be executed once.
-``` bash
-        cd ~
-        mkdir envs
-        cd envs
-        python -m venv phys .
+```bash
+    cd ~
+    mkdir envs
+    cd envs
+    python -m venv phys .
 ```
-    Activating "phys" environment -- To be executed everytime after opening new terminal/ Powershell window.
+
+Activating "phys" environment -- To be executed everytime after opening new terminal/ Powershell window.
+
 ``` bash
-        ~/envs/phys/Scripts/Activate.ps1
+    ~/envs/phys/Scripts/Activate.ps1
 ```
 
 Using conda:
 
-    Creating virtual environment using conda -- To be done once
+Creating virtual environment using conda -- To be done once
+
 ``` bash
-        conda create -n phys
+    conda create -n phys
 ```
-    Activating "phys" environment -- To be executed everytime after opening new terminal/ Powershell window.
+
+Activating "phys" environment -- To be executed everytime after opening new terminal/ Powershell window.
+
 ``` bash
-        conda activate phys
+    conda activate phys
 ```
 
 You can then use [PyPI package](https://pypi.org/project/PhysioKit2/) to install PhysioKit, using the below mentioned command:
 
 ``` bash
-pip install PhysioKit2
+    pip install PhysioKit2
 ```
 
 To update the currently installed package:
 
 ``` bash
-pip install --upgrade PhysioKit2
+    pip install --upgrade PhysioKit2
 ```
 
 ## **Building wheel (.whl) package from source**
+
 Requires 'build' package that can be installed using pip with following command:
 
 ``` bash
-pip install build
+    pip install build
 ```
 
 Clone the PhysioKit repository from GitHub and 'cd' to the clonned repo:
 
 ``` bash
-git clone https://github.com/PhysiologicAILab/PhysioKit.git
-cd PhysioKit
+    git clone https://github.com/PhysiologicAILab/PhysioKit.git
+    cd PhysioKit
 ```
 
 Make the changes to the repo as required to serve your objectives.
-In setup.py, change the version - for your tracking purpose, e.g. 1.8.0 and then build the wheel package:
+In setup.py, change the version - for your tracking purpose, e.g. 2.0.0 and then build the wheel package:
 
 ``` bash
-python -m build 
+    python -m build 
 ```
 
 Install the package that has been built:
 
 ``` bash
-python -m pip install .\dist\PhysioKit2-1.8.0-py3-none-any.whl
+    python -m pip install .\dist\PhysioKit2-2.0.0-py3-none-any.whl
 ```
 
 ## **Usage Instructions**
 
 ### **Step-1: Upload program on the Arduino board**
 
 Connect the Arduino board that you want to use. For this step, the sensors need not be connected.
@@ -138,61 +143,83 @@
 
 If the study protocol requires acquisition for indefinitely long duration with manual stop, then *timed_acquisition* can be specified as *False*, otherwise in every other scenario, this is to be set as *true*. If this is specified as *true*, it is required to specify the acquisition duration (in seconds) separately for each experimental condition.
 
 Using the *datapath* field, we can specify the path at which the acquired data with get stored.
 
 Lastly, as the interface supports marking of asynchronous events, the description about the type of events along with *event_code* can be specified.
 
+```json
+{
+    "exp":
+    {
         "study_name": "PhysioKit_Validation",
         "conditions": ["baseline", "mathEasy", "mathDifficult", "movement"],
         "channels": ["EDA", "Resp", "PPG Finger", "PPG Ear"],
         "channel_types": ["eda", "resp", "ppg", "ppg"],
         "timed_acquisition": true,
+        "assess_signal_quality": true,
         "max_time_seconds": [180, 180, 180, 180],
         "datapath": "data",
         "event_codes":{
             "0": "event_1",
             "1": "event_2"
         }
 
+    },
+    "biofeedback":
+    {
+        "enabled": false,
+        "ch_index": 3,
+        "metric": "HRV_MeanNN",
+        "window": 10,
+        "step": 1,
+        "modulation_threshold": 2,
+        "mapping": "linear_increase",
+        "type": "visual",
+        "visual_feedback": {
+            "shape": "circle",
+            "varying_parameter": "size"
+        }
+    }
+}
+```
+
 ### **Step-4: Launch the PhysioKit Interface**
 
 Before launching the interface, ensure that the Arduino board is connected to the computer using USB connection or through Bluetooth connection. At this step, sensors are required to be appropriately connected to the analog channels of Arduino board.
 
 To launch the interface, run the following command in the terminal:
 
 ``` bash
-physiokit --config <path of config file>
-see example below 
-physiokit --config configs/avr_default/sw_config.json
+    physiokit --config <path of config file>
+    see example below 
+    physiokit --config configs/avr_default/sw_config.json
 ```
 
 This shall open user interface, basic functioning of which is shown in this demo. Please note that if secondary screen is connected, the interface uses it to adjust its resolution, however it may have to be moved to the secondary screen if it got launched on the primary.
 
-<p align="left">
-    <img src="images/PhysioKitDemo.gif" alt="Demo of PhysioKit" width="1024"/>
-</p>
+![Demo of PhysioKit](https://github.com/PhysiologicAILab/PhysioKit/blob/main/images/PhysioKitDemo.gif|width=1024)
 
 A brief description of each step is mentioned below:
 
-> **Step-4a: Connect with the Serial Port**: Select the serial / com-port where Arduino board is connected. Observe the *Info* displayed at the bottom of the interface in the status bar. On successful connection, the *Info* bar shall display the port details along with the baudrate.
+* **Step-4a: Connect with the Serial Port**: Select the serial / com-port where Arduino board is connected. Observe the *Info* displayed at the bottom of the interface in the status bar. On successful connection, the *Info* bar shall display the port details along with the baudrate.
 
-> **Step-4b: Browse and select appropriate Experiment Configuration file**: Using the interface, browse the *Experiment Configuration File* as updated in [Step-3](#step-3-update-experiment-configurartion-file). On successful loading of the config file, the interface shall start displaying he plotting area with the specified number of channels. Please note if the number of channels are more than 4, the interface will only show real-time plotting of first four physiological signals as specified in the configuration file.
+* **Step-4b: Browse and select appropriate Experiment Configuration file**: Using the interface, browse the *Experiment Configuration File* as updated in [Step-3](#step-3-update-experiment-configuration-file). On successful loading of the config file, the interface shall start displaying he plotting area with the specified number of channels. Please note if the number of channels are more than 4, the interface will only show real-time plotting of first four physiological signals as specified in the configuration file.
 
-> **Step-4c: Specify Participant ID**: This allows specifying the participant ID in user preferred manner. The ID specified here will be used for storing the data in organized manner.
+* **Step-4c: Specify Participant ID**: This allows specifying the participant ID in user preferred manner. The ID specified here will be used for storing the data in organized manner.
 
-> **Step-4d: Select Experiment Condition**: This part of the interface shows a list of conditions as specified in the *Experiment Configuration File* in [Step-3](#step-3-update-experiment-configurartion-file). Each condition listed can be selected with a mouse click. Experimental condition will also be used in naming the file while storing acquired physiological signals.
+* **Step-4d: Select Experiment Condition**: This part of the interface shows a list of conditions as specified in the *Experiment Configuration File* in [Step-3](#step-3-update-experiment-configuration-file). Each condition listed can be selected with a mouse click. Experimental condition will also be used in naming the file while storing acquired physiological signals.
 
-> **Step-4e: Start Live Acquisition**: In this step, real-time plots can be seen in the plotting area of the interface. Signals are not yet being recorded and the objective at this step is to visually inspect the physiological signals and verify if good quality signals are being acquired.
+* **Step-4e: Start Live Acquisition**: In this step, real-time plots can be seen in the plotting area of the interface. Signals are not yet being recorded and the objective at this step is to visually inspect the physiological signals and verify if good quality signals are being acquired.
 
-> **Step-4f: Start Recording**: Having verified the signals with real-time plotting feature, recording can be started with a manual trigger. In case of multi-user settings, all the client computers are required to remain ready for recording the data before the recording starts at the server computer. Pressing *Record Data* on client computer makes it ready to wait for a trigger from the connected server. The recording of the data on all the computers can be started synchronously with a manual trigger at server computer.
+* **Step-4f: Start Recording**: Having verified the signals with real-time plotting feature, recording can be started with a manual trigger. In case of multi-user settings, all the client computers are required to remain ready for recording the data before the recording starts at the server computer. Pressing *Record Data* on client computer makes it ready to wait for a trigger from the connected server. The recording of the data on all the computers can be started synchronously with a manual trigger at server computer.
 
-> **Step-4g: Marking the Events**: While the recording of physiological signals is in progress, interface allows marking events by pressing *Start Marking* button. Before pressing this, one can choose the relevant *Event Code* from the list which will show the *Event Codes* as specified in [Step-3](#step-3-update-experiment-configurartion-file). The same button then can be pressed to stop marking of the event. These marking information will be stored along with the data samples in CSV file - with the corresponding *Event-Code*.
+* **Step-4g: Marking the Events**: While the recording of physiological signals is in progress, interface allows marking events by pressing *Start Marking* button. Before pressing this, one can choose the relevant *Event Code* from the list which will show the *Event Codes* as specified in [Step-3](#step-3-update-experiment-configuration-file). The same button then can be pressed to stop marking of the event. These marking information will be stored along with the data samples in CSV file - with the corresponding *Event-Code*.
 
-> **Step-4h: Stopping to Record**: If the *timed_acquisition* field specified in the [Step-3](#step-3-update-experiment-configurartion-file) is set to *true*, the recording will stop after the specified time, and pressing *Stop Recording* will interrupt the planned acquisition. This can be used only in exception cases in which experiment is to be terminated abruptly. However, if the *timed_acquisition* field is set to *false*, then *Stop Recording* is required to be pressed manually to end the acquisition.
+* **Step-4h: Stopping to Record**: If the *timed_acquisition* field specified in the [Step-3](#step-3-update-experiment-configuration-file) is set to *true*, the recording will stop after the specified time, and pressing *Stop Recording* will interrupt the planned acquisition. This can be used only in exception cases in which experiment is to be terminated abruptly. However, if the *timed_acquisition* field is set to *false*, then *Stop Recording* is required to be pressed manually to end the acquisition.
 
 ---
 
 ### **Data Analysis**
 
 Data analysis is supported by the *analysis_helper* folder. To extract features and export in spreadsheet, please refer to the README provided within the folder.
 In addition, Jupyter notebooks *phys_analysis_eda.ipynb*, *phys_analysis_ppg.ipynb*, and *phys_analysis_resp.ipynb* are provided to illustrate basic analysis steps. This includes pre-processing as well as feature extraction for EDA, PPG and Resp signals respectively.
@@ -205,31 +232,31 @@
 
 ---
 
 ### **Citation**
 
 If you find our [paper](https://www.mdpi.com/1424-8220/23/19/8244) or this toolkit useful for your research, please cite our following works.
 
-```
+```text
 @article{joshi2023physiokit,
     title={PhysioKit: An Open-Source, Low-Cost Physiological Computing Toolkit for Single-and Multi-User Studies},
     author={Joshi, Jitesh and Wang, Katherine and Cho, Youngjun},
     journal={Sensors},
     publisher={MDPI},
     volume={23},
     number={19},
     article-number={8244},
     year={2023},
     url={https://www.mdpi.com/1424-8220/23/19/8244}
     issn={1424-8220},
     doi={10.3390/s23198244}
 }
 
-@article{joshi2024imaging,
-    title={Imaging Blood Volume Pulse Dataset: RGB-Thermal Remote Photoplethysmography Dataset with High-Resolution Signal-Quality Labels},
+@article{joshi2024ibvp,
+    title={iBVP Dataset: RGB-Thermal rPPG Dataset with High Resolution Signal Quality Labels},
     author={Joshi, Jitesh and Cho, Youngjun},
     journal={Electronics},
     publisher={MDPI},
     volume={13},
     year={2024},
     number={7},
     article-number={1334},
```

### Comparing `PhysioKit2-1.8.9/README.md` & `physiokit2-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,90 +1,95 @@
 # **Overview of PhysioKit**
 
 Authors: Jitesh Joshi, Katherine Wang, and Youngjun Cho <br>
-Contact: Physiological Computing and Artificial Intelligence lab @ GDIH - WHO Collaboration Centre for Assistive Technology, UCL Computer Science  (<youngjun.cho@ucl.ac.uk>)
+Contact: Computational Physiology and Intelligence group @ GDIH - WHO Collaboration Centre for Assistive Technology, UCL Computer Science  (<youngjun.cho@ucl.ac.uk>)
 
 PhysioKit is a novel physiological computing toolkit which is open-source, accessible and affordable. HCI hobbyists and practitioners can easily access physiological sensing channels that help monitor our physiological signatures and vital signs including heart rate, heart rate variability, breathing rate, electrodermal activities. The toolkit works with a low-cost micro-controller such as Arduino. Currently, it supports acquiring EDA, Resp and PPG using any low-cost Arduino board.
 
 PhysioKit consists of (i) a sensor and hardware layer that can be configured in a modular manner along with research needs, (ii) a software application layer that enables real-time data collection, streaming and visualization for both single and multi-user experiments. This also supports basic visual biofeedback configurations and multi-signal synchronization for co-located or remote multi-user settings.
 
 Below figure shows architecture of PhysioKit:
-<p align="left">
-<img src="images/architecture.png" alt="Architecture of PhysioKit" width="1024"/>
-</p>
+
+![Architecture of PhysioKit](https://github.com/PhysiologicAILab/PhysioKit/blob/main/images/architecture.png|width=1024)
 
 ## **Installation**
 
 Pre-requisite: Python >= 3.8
 
 It is recommended to create separate Python virtual environment, which can be achieved using venv/ anaconda/ miniconda as follows. After creating the environment, activate the same.
 
 Using venv:
 
+Creating virtual environment using venv (recommended for Windows users) -- To be executed once.
 
-    Creating virtual environment using venv (recommended for Windows users) -- To be executed once.
-``` bash
-        cd ~
-        mkdir envs
-        cd envs
-        python -m venv phys .
+```bash
+    cd ~
+    mkdir envs
+    cd envs
+    python -m venv phys .
 ```
-    Activating "phys" environment -- To be executed everytime after opening new terminal/ Powershell window.
+
+Activating "phys" environment -- To be executed everytime after opening new terminal/ Powershell window.
+
 ``` bash
-        ~/envs/phys/Scripts/Activate.ps1
+    ~/envs/phys/Scripts/Activate.ps1
 ```
 
 Using conda:
 
-    Creating virtual environment using conda -- To be done once
+Creating virtual environment using conda -- To be done once
+
 ``` bash
-        conda create -n phys
+    conda create -n phys
 ```
-    Activating "phys" environment -- To be executed everytime after opening new terminal/ Powershell window.
+
+Activating "phys" environment -- To be executed everytime after opening new terminal/ Powershell window.
+
 ``` bash
-        conda activate phys
+    conda activate phys
 ```
 
 You can then use [PyPI package](https://pypi.org/project/PhysioKit2/) to install PhysioKit, using the below mentioned command:
 
 ``` bash
-pip install PhysioKit2
+    pip install PhysioKit2
 ```
 
 To update the currently installed package:
 
 ``` bash
-pip install --upgrade PhysioKit2
+    pip install --upgrade PhysioKit2
 ```
 
 ## **Building wheel (.whl) package from source**
+
 Requires 'build' package that can be installed using pip with following command:
 
 ``` bash
-pip install build
+    pip install build
 ```
 
 Clone the PhysioKit repository from GitHub and 'cd' to the clonned repo:
 
 ``` bash
-git clone https://github.com/PhysiologicAILab/PhysioKit.git
-cd PhysioKit
+    git clone https://github.com/PhysiologicAILab/PhysioKit.git
+    cd PhysioKit
 ```
 
 Make the changes to the repo as required to serve your objectives.
-In setup.py, change the version - for your tracking purpose, e.g. 1.8.0 and then build the wheel package:
+In setup.py, change the version - for your tracking purpose, e.g. 2.0.0 and then build the wheel package:
 
 ``` bash
-python -m build 
+    python -m build 
 ```
 
 Install the package that has been built:
 
 ``` bash
-python -m pip install .\dist\PhysioKit2-1.8.0-py3-none-any.whl
+    python -m pip install .\dist\PhysioKit2-2.0.0-py3-none-any.whl
 ```
 
 ## **Usage Instructions**
 
 ### **Step-1: Upload program on the Arduino board**
 
 Connect the Arduino board that you want to use. For this step, the sensors need not be connected.
@@ -114,61 +119,83 @@
 
 If the study protocol requires acquisition for indefinitely long duration with manual stop, then *timed_acquisition* can be specified as *False*, otherwise in every other scenario, this is to be set as *true*. If this is specified as *true*, it is required to specify the acquisition duration (in seconds) separately for each experimental condition.
 
 Using the *datapath* field, we can specify the path at which the acquired data with get stored.
 
 Lastly, as the interface supports marking of asynchronous events, the description about the type of events along with *event_code* can be specified.
 
+```json
+{
+    "exp":
+    {
         "study_name": "PhysioKit_Validation",
         "conditions": ["baseline", "mathEasy", "mathDifficult", "movement"],
         "channels": ["EDA", "Resp", "PPG Finger", "PPG Ear"],
         "channel_types": ["eda", "resp", "ppg", "ppg"],
         "timed_acquisition": true,
+        "assess_signal_quality": true,
         "max_time_seconds": [180, 180, 180, 180],
         "datapath": "data",
         "event_codes":{
             "0": "event_1",
             "1": "event_2"
         }
 
+    },
+    "biofeedback":
+    {
+        "enabled": false,
+        "ch_index": 3,
+        "metric": "HRV_MeanNN",
+        "window": 10,
+        "step": 1,
+        "modulation_threshold": 2,
+        "mapping": "linear_increase",
+        "type": "visual",
+        "visual_feedback": {
+            "shape": "circle",
+            "varying_parameter": "size"
+        }
+    }
+}
+```
+
 ### **Step-4: Launch the PhysioKit Interface**
 
 Before launching the interface, ensure that the Arduino board is connected to the computer using USB connection or through Bluetooth connection. At this step, sensors are required to be appropriately connected to the analog channels of Arduino board.
 
 To launch the interface, run the following command in the terminal:
 
 ``` bash
-physiokit --config <path of config file>
-see example below 
-physiokit --config configs/avr_default/sw_config.json
+    physiokit --config <path of config file>
+    see example below 
+    physiokit --config configs/avr_default/sw_config.json
 ```
 
 This shall open user interface, basic functioning of which is shown in this demo. Please note that if secondary screen is connected, the interface uses it to adjust its resolution, however it may have to be moved to the secondary screen if it got launched on the primary.
 
-<p align="left">
-    <img src="images/PhysioKitDemo.gif" alt="Demo of PhysioKit" width="1024"/>
-</p>
+![Demo of PhysioKit](https://github.com/PhysiologicAILab/PhysioKit/blob/main/images/PhysioKitDemo.gif|width=1024)
 
 A brief description of each step is mentioned below:
 
-> **Step-4a: Connect with the Serial Port**: Select the serial / com-port where Arduino board is connected. Observe the *Info* displayed at the bottom of the interface in the status bar. On successful connection, the *Info* bar shall display the port details along with the baudrate.
+* **Step-4a: Connect with the Serial Port**: Select the serial / com-port where Arduino board is connected. Observe the *Info* displayed at the bottom of the interface in the status bar. On successful connection, the *Info* bar shall display the port details along with the baudrate.
 
-> **Step-4b: Browse and select appropriate Experiment Configuration file**: Using the interface, browse the *Experiment Configuration File* as updated in [Step-3](#step-3-update-experiment-configurartion-file). On successful loading of the config file, the interface shall start displaying he plotting area with the specified number of channels. Please note if the number of channels are more than 4, the interface will only show real-time plotting of first four physiological signals as specified in the configuration file.
+* **Step-4b: Browse and select appropriate Experiment Configuration file**: Using the interface, browse the *Experiment Configuration File* as updated in [Step-3](#step-3-update-experiment-configuration-file). On successful loading of the config file, the interface shall start displaying he plotting area with the specified number of channels. Please note if the number of channels are more than 4, the interface will only show real-time plotting of first four physiological signals as specified in the configuration file.
 
-> **Step-4c: Specify Participant ID**: This allows specifying the participant ID in user preferred manner. The ID specified here will be used for storing the data in organized manner.
+* **Step-4c: Specify Participant ID**: This allows specifying the participant ID in user preferred manner. The ID specified here will be used for storing the data in organized manner.
 
-> **Step-4d: Select Experiment Condition**: This part of the interface shows a list of conditions as specified in the *Experiment Configuration File* in [Step-3](#step-3-update-experiment-configurartion-file). Each condition listed can be selected with a mouse click. Experimental condition will also be used in naming the file while storing acquired physiological signals.
+* **Step-4d: Select Experiment Condition**: This part of the interface shows a list of conditions as specified in the *Experiment Configuration File* in [Step-3](#step-3-update-experiment-configuration-file). Each condition listed can be selected with a mouse click. Experimental condition will also be used in naming the file while storing acquired physiological signals.
 
-> **Step-4e: Start Live Acquisition**: In this step, real-time plots can be seen in the plotting area of the interface. Signals are not yet being recorded and the objective at this step is to visually inspect the physiological signals and verify if good quality signals are being acquired.
+* **Step-4e: Start Live Acquisition**: In this step, real-time plots can be seen in the plotting area of the interface. Signals are not yet being recorded and the objective at this step is to visually inspect the physiological signals and verify if good quality signals are being acquired.
 
-> **Step-4f: Start Recording**: Having verified the signals with real-time plotting feature, recording can be started with a manual trigger. In case of multi-user settings, all the client computers are required to remain ready for recording the data before the recording starts at the server computer. Pressing *Record Data* on client computer makes it ready to wait for a trigger from the connected server. The recording of the data on all the computers can be started synchronously with a manual trigger at server computer.
+* **Step-4f: Start Recording**: Having verified the signals with real-time plotting feature, recording can be started with a manual trigger. In case of multi-user settings, all the client computers are required to remain ready for recording the data before the recording starts at the server computer. Pressing *Record Data* on client computer makes it ready to wait for a trigger from the connected server. The recording of the data on all the computers can be started synchronously with a manual trigger at server computer.
 
-> **Step-4g: Marking the Events**: While the recording of physiological signals is in progress, interface allows marking events by pressing *Start Marking* button. Before pressing this, one can choose the relevant *Event Code* from the list which will show the *Event Codes* as specified in [Step-3](#step-3-update-experiment-configurartion-file). The same button then can be pressed to stop marking of the event. These marking information will be stored along with the data samples in CSV file - with the corresponding *Event-Code*.
+* **Step-4g: Marking the Events**: While the recording of physiological signals is in progress, interface allows marking events by pressing *Start Marking* button. Before pressing this, one can choose the relevant *Event Code* from the list which will show the *Event Codes* as specified in [Step-3](#step-3-update-experiment-configuration-file). The same button then can be pressed to stop marking of the event. These marking information will be stored along with the data samples in CSV file - with the corresponding *Event-Code*.
 
-> **Step-4h: Stopping to Record**: If the *timed_acquisition* field specified in the [Step-3](#step-3-update-experiment-configurartion-file) is set to *true*, the recording will stop after the specified time, and pressing *Stop Recording* will interrupt the planned acquisition. This can be used only in exception cases in which experiment is to be terminated abruptly. However, if the *timed_acquisition* field is set to *false*, then *Stop Recording* is required to be pressed manually to end the acquisition.
+* **Step-4h: Stopping to Record**: If the *timed_acquisition* field specified in the [Step-3](#step-3-update-experiment-configuration-file) is set to *true*, the recording will stop after the specified time, and pressing *Stop Recording* will interrupt the planned acquisition. This can be used only in exception cases in which experiment is to be terminated abruptly. However, if the *timed_acquisition* field is set to *false*, then *Stop Recording* is required to be pressed manually to end the acquisition.
 
 ---
 
 ### **Data Analysis**
 
 Data analysis is supported by the *analysis_helper* folder. To extract features and export in spreadsheet, please refer to the README provided within the folder.
 In addition, Jupyter notebooks *phys_analysis_eda.ipynb*, *phys_analysis_ppg.ipynb*, and *phys_analysis_resp.ipynb* are provided to illustrate basic analysis steps. This includes pre-processing as well as feature extraction for EDA, PPG and Resp signals respectively.
@@ -181,37 +208,37 @@
 
 ---
 
 ### **Citation**
 
 If you find our [paper](https://www.mdpi.com/1424-8220/23/19/8244) or this toolkit useful for your research, please cite our following works.
 
-```
+```text
 @article{joshi2023physiokit,
     title={PhysioKit: An Open-Source, Low-Cost Physiological Computing Toolkit for Single-and Multi-User Studies},
     author={Joshi, Jitesh and Wang, Katherine and Cho, Youngjun},
     journal={Sensors},
     publisher={MDPI},
     volume={23},
     number={19},
     article-number={8244},
     year={2023},
     url={https://www.mdpi.com/1424-8220/23/19/8244}
     issn={1424-8220},
     doi={10.3390/s23198244}
 }
 
-@article{joshi2024imaging,
-    title={Imaging Blood Volume Pulse Dataset: RGB-Thermal Remote Photoplethysmography Dataset with High-Resolution Signal-Quality Labels},
+@article{joshi2024ibvp,
+    title={iBVP Dataset: RGB-Thermal rPPG Dataset with High Resolution Signal Quality Labels},
     author={Joshi, Jitesh and Cho, Youngjun},
     journal={Electronics},
     publisher={MDPI},
     volume={13},
     year={2024},
     number={7},
     article-number={1334},
     url={https://www.mdpi.com/2079-9292/13/7/1334},
     issn={2079-9292},
     doi={10.3390/electronics13071334}
 }
 
-```
+```
```

### Comparing `PhysioKit2-1.8.9/setup.py` & `physiokit2-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='PhysioKit2',
-      version='1.8.9',
+      version='2.0.0',
       description="PhysioKit: An Open-Source, Low-Cost Physiological Computing Toolkit for Single- and Multi-User Studies",
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/PhysiologicAILab/PhysioKit',
       author=['Jitesh Joshi', 'Katherine wang', 'Youngjun Cho'],
       author_email='youngjun.cho@ucl.ac.uk',
       license='MIT',
```

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/analysis_helper/process_signals.py` & `physiokit2-2.0.0/src/PhysioKit2/analysis_helper/process_signals.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/analysis_helper/utils/load_data.py` & `physiokit2-2.0.0/src/PhysioKit2/analysis_helper/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/configs/exp_config_phys.json` & `physiokit2-2.0.0/src/PhysioKit2/configs/exp_config_phys.json`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/form.ui` & `physiokit2-2.0.0/src/PhysioKit2/form.ui`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/form_ui.py` & `physiokit2-2.0.0/src/PhysioKit2/form_ui.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/images/banner.png` & `physiokit2-2.0.0/src/PhysioKit2/images/banner.png`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/images/color_bar.png` & `physiokit2-2.0.0/src/PhysioKit2/images/color_bar.png`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/images/sq_indication.png` & `physiokit2-2.0.0/src/PhysioKit2/images/sq_indication.png`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/main.py` & `physiokit2-2.0.0/src/PhysioKit2/main.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/sqa/config/SQAPhysMD.json` & `physiokit2-2.0.0/src/PhysioKit2/sqa/config/SQAPhysMD.json`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/sqa/inference.py` & `physiokit2-2.0.0/src/PhysioKit2/sqa/inference.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/sqa/inference_thread.py` & `physiokit2-2.0.0/src/PhysioKit2/sqa/inference_thread.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/sqa/model/SQAPhysMD.py` & `physiokit2-2.0.0/src/PhysioKit2/sqa/model/SQAPhysMD.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/utils/acquisition.py` & `physiokit2-2.0.0/src/PhysioKit2/utils/acquisition.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/utils/biofeedback.py` & `physiokit2-2.0.0/src/PhysioKit2/utils/biofeedback.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/utils/data_processing_lib.py` & `physiokit2-2.0.0/src/PhysioKit2/utils/data_processing_lib.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/utils/external_sync.py` & `physiokit2-2.0.0/src/PhysioKit2/utils/external_sync.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/utils/file_ops.py` & `physiokit2-2.0.0/src/PhysioKit2/utils/file_ops.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2/utils/load_data.py` & `physiokit2-2.0.0/src/PhysioKit2/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2.egg-info/PKG-INFO` & `physiokit2-2.0.0/src/PhysioKit2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PhysioKit2
-Version: 1.8.9
+Version: 2.0.0
 Summary: PhysioKit: An Open-Source, Low-Cost Physiological Computing Toolkit for Single- and Multi-User Studies
 Home-page: https://github.com/PhysiologicAILab/PhysioKit
 Author: ['Jitesh Joshi', 'Katherine wang', 'Youngjun Cho']
 Author-email: youngjun.cho@ucl.ac.uk
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,94 +21,99 @@
 Requires-Dist: torch
 Requires-Dist: setuptools
 Requires-Dist: requests
 
 # **Overview of PhysioKit**
 
 Authors: Jitesh Joshi, Katherine Wang, and Youngjun Cho <br>
-Contact: Physiological Computing and Artificial Intelligence lab @ GDIH - WHO Collaboration Centre for Assistive Technology, UCL Computer Science  (<youngjun.cho@ucl.ac.uk>)
+Contact: Computational Physiology and Intelligence group @ GDIH - WHO Collaboration Centre for Assistive Technology, UCL Computer Science  (<youngjun.cho@ucl.ac.uk>)
 
 PhysioKit is a novel physiological computing toolkit which is open-source, accessible and affordable. HCI hobbyists and practitioners can easily access physiological sensing channels that help monitor our physiological signatures and vital signs including heart rate, heart rate variability, breathing rate, electrodermal activities. The toolkit works with a low-cost micro-controller such as Arduino. Currently, it supports acquiring EDA, Resp and PPG using any low-cost Arduino board.
 
 PhysioKit consists of (i) a sensor and hardware layer that can be configured in a modular manner along with research needs, (ii) a software application layer that enables real-time data collection, streaming and visualization for both single and multi-user experiments. This also supports basic visual biofeedback configurations and multi-signal synchronization for co-located or remote multi-user settings.
 
 Below figure shows architecture of PhysioKit:
-<p align="left">
-<img src="images/architecture.png" alt="Architecture of PhysioKit" width="1024"/>
-</p>
+
+![Architecture of PhysioKit](https://github.com/PhysiologicAILab/PhysioKit/blob/main/images/architecture.png|width=1024)
 
 ## **Installation**
 
 Pre-requisite: Python >= 3.8
 
 It is recommended to create separate Python virtual environment, which can be achieved using venv/ anaconda/ miniconda as follows. After creating the environment, activate the same.
 
 Using venv:
 
+Creating virtual environment using venv (recommended for Windows users) -- To be executed once.
 
-    Creating virtual environment using venv (recommended for Windows users) -- To be executed once.
-``` bash
-        cd ~
-        mkdir envs
-        cd envs
-        python -m venv phys .
+```bash
+    cd ~
+    mkdir envs
+    cd envs
+    python -m venv phys .
 ```
-    Activating "phys" environment -- To be executed everytime after opening new terminal/ Powershell window.
+
+Activating "phys" environment -- To be executed everytime after opening new terminal/ Powershell window.
+
 ``` bash
-        ~/envs/phys/Scripts/Activate.ps1
+    ~/envs/phys/Scripts/Activate.ps1
 ```
 
 Using conda:
 
-    Creating virtual environment using conda -- To be done once
+Creating virtual environment using conda -- To be done once
+
 ``` bash
-        conda create -n phys
+    conda create -n phys
 ```
-    Activating "phys" environment -- To be executed everytime after opening new terminal/ Powershell window.
+
+Activating "phys" environment -- To be executed everytime after opening new terminal/ Powershell window.
+
 ``` bash
-        conda activate phys
+    conda activate phys
 ```
 
 You can then use [PyPI package](https://pypi.org/project/PhysioKit2/) to install PhysioKit, using the below mentioned command:
 
 ``` bash
-pip install PhysioKit2
+    pip install PhysioKit2
 ```
 
 To update the currently installed package:
 
 ``` bash
-pip install --upgrade PhysioKit2
+    pip install --upgrade PhysioKit2
 ```
 
 ## **Building wheel (.whl) package from source**
+
 Requires 'build' package that can be installed using pip with following command:
 
 ``` bash
-pip install build
+    pip install build
 ```
 
 Clone the PhysioKit repository from GitHub and 'cd' to the clonned repo:
 
 ``` bash
-git clone https://github.com/PhysiologicAILab/PhysioKit.git
-cd PhysioKit
+    git clone https://github.com/PhysiologicAILab/PhysioKit.git
+    cd PhysioKit
 ```
 
 Make the changes to the repo as required to serve your objectives.
-In setup.py, change the version - for your tracking purpose, e.g. 1.8.0 and then build the wheel package:
+In setup.py, change the version - for your tracking purpose, e.g. 2.0.0 and then build the wheel package:
 
 ``` bash
-python -m build 
+    python -m build 
 ```
 
 Install the package that has been built:
 
 ``` bash
-python -m pip install .\dist\PhysioKit2-1.8.0-py3-none-any.whl
+    python -m pip install .\dist\PhysioKit2-2.0.0-py3-none-any.whl
 ```
 
 ## **Usage Instructions**
 
 ### **Step-1: Upload program on the Arduino board**
 
 Connect the Arduino board that you want to use. For this step, the sensors need not be connected.
@@ -138,61 +143,83 @@
 
 If the study protocol requires acquisition for indefinitely long duration with manual stop, then *timed_acquisition* can be specified as *False*, otherwise in every other scenario, this is to be set as *true*. If this is specified as *true*, it is required to specify the acquisition duration (in seconds) separately for each experimental condition.
 
 Using the *datapath* field, we can specify the path at which the acquired data with get stored.
 
 Lastly, as the interface supports marking of asynchronous events, the description about the type of events along with *event_code* can be specified.
 
+```json
+{
+    "exp":
+    {
         "study_name": "PhysioKit_Validation",
         "conditions": ["baseline", "mathEasy", "mathDifficult", "movement"],
         "channels": ["EDA", "Resp", "PPG Finger", "PPG Ear"],
         "channel_types": ["eda", "resp", "ppg", "ppg"],
         "timed_acquisition": true,
+        "assess_signal_quality": true,
         "max_time_seconds": [180, 180, 180, 180],
         "datapath": "data",
         "event_codes":{
             "0": "event_1",
             "1": "event_2"
         }
 
+    },
+    "biofeedback":
+    {
+        "enabled": false,
+        "ch_index": 3,
+        "metric": "HRV_MeanNN",
+        "window": 10,
+        "step": 1,
+        "modulation_threshold": 2,
+        "mapping": "linear_increase",
+        "type": "visual",
+        "visual_feedback": {
+            "shape": "circle",
+            "varying_parameter": "size"
+        }
+    }
+}
+```
+
 ### **Step-4: Launch the PhysioKit Interface**
 
 Before launching the interface, ensure that the Arduino board is connected to the computer using USB connection or through Bluetooth connection. At this step, sensors are required to be appropriately connected to the analog channels of Arduino board.
 
 To launch the interface, run the following command in the terminal:
 
 ``` bash
-physiokit --config <path of config file>
-see example below 
-physiokit --config configs/avr_default/sw_config.json
+    physiokit --config <path of config file>
+    see example below 
+    physiokit --config configs/avr_default/sw_config.json
 ```
 
 This shall open user interface, basic functioning of which is shown in this demo. Please note that if secondary screen is connected, the interface uses it to adjust its resolution, however it may have to be moved to the secondary screen if it got launched on the primary.
 
-<p align="left">
-    <img src="images/PhysioKitDemo.gif" alt="Demo of PhysioKit" width="1024"/>
-</p>
+![Demo of PhysioKit](https://github.com/PhysiologicAILab/PhysioKit/blob/main/images/PhysioKitDemo.gif|width=1024)
 
 A brief description of each step is mentioned below:
 
-> **Step-4a: Connect with the Serial Port**: Select the serial / com-port where Arduino board is connected. Observe the *Info* displayed at the bottom of the interface in the status bar. On successful connection, the *Info* bar shall display the port details along with the baudrate.
+* **Step-4a: Connect with the Serial Port**: Select the serial / com-port where Arduino board is connected. Observe the *Info* displayed at the bottom of the interface in the status bar. On successful connection, the *Info* bar shall display the port details along with the baudrate.
 
-> **Step-4b: Browse and select appropriate Experiment Configuration file**: Using the interface, browse the *Experiment Configuration File* as updated in [Step-3](#step-3-update-experiment-configurartion-file). On successful loading of the config file, the interface shall start displaying he plotting area with the specified number of channels. Please note if the number of channels are more than 4, the interface will only show real-time plotting of first four physiological signals as specified in the configuration file.
+* **Step-4b: Browse and select appropriate Experiment Configuration file**: Using the interface, browse the *Experiment Configuration File* as updated in [Step-3](#step-3-update-experiment-configuration-file). On successful loading of the config file, the interface shall start displaying he plotting area with the specified number of channels. Please note if the number of channels are more than 4, the interface will only show real-time plotting of first four physiological signals as specified in the configuration file.
 
-> **Step-4c: Specify Participant ID**: This allows specifying the participant ID in user preferred manner. The ID specified here will be used for storing the data in organized manner.
+* **Step-4c: Specify Participant ID**: This allows specifying the participant ID in user preferred manner. The ID specified here will be used for storing the data in organized manner.
 
-> **Step-4d: Select Experiment Condition**: This part of the interface shows a list of conditions as specified in the *Experiment Configuration File* in [Step-3](#step-3-update-experiment-configurartion-file). Each condition listed can be selected with a mouse click. Experimental condition will also be used in naming the file while storing acquired physiological signals.
+* **Step-4d: Select Experiment Condition**: This part of the interface shows a list of conditions as specified in the *Experiment Configuration File* in [Step-3](#step-3-update-experiment-configuration-file). Each condition listed can be selected with a mouse click. Experimental condition will also be used in naming the file while storing acquired physiological signals.
 
-> **Step-4e: Start Live Acquisition**: In this step, real-time plots can be seen in the plotting area of the interface. Signals are not yet being recorded and the objective at this step is to visually inspect the physiological signals and verify if good quality signals are being acquired.
+* **Step-4e: Start Live Acquisition**: In this step, real-time plots can be seen in the plotting area of the interface. Signals are not yet being recorded and the objective at this step is to visually inspect the physiological signals and verify if good quality signals are being acquired.
 
-> **Step-4f: Start Recording**: Having verified the signals with real-time plotting feature, recording can be started with a manual trigger. In case of multi-user settings, all the client computers are required to remain ready for recording the data before the recording starts at the server computer. Pressing *Record Data* on client computer makes it ready to wait for a trigger from the connected server. The recording of the data on all the computers can be started synchronously with a manual trigger at server computer.
+* **Step-4f: Start Recording**: Having verified the signals with real-time plotting feature, recording can be started with a manual trigger. In case of multi-user settings, all the client computers are required to remain ready for recording the data before the recording starts at the server computer. Pressing *Record Data* on client computer makes it ready to wait for a trigger from the connected server. The recording of the data on all the computers can be started synchronously with a manual trigger at server computer.
 
-> **Step-4g: Marking the Events**: While the recording of physiological signals is in progress, interface allows marking events by pressing *Start Marking* button. Before pressing this, one can choose the relevant *Event Code* from the list which will show the *Event Codes* as specified in [Step-3](#step-3-update-experiment-configurartion-file). The same button then can be pressed to stop marking of the event. These marking information will be stored along with the data samples in CSV file - with the corresponding *Event-Code*.
+* **Step-4g: Marking the Events**: While the recording of physiological signals is in progress, interface allows marking events by pressing *Start Marking* button. Before pressing this, one can choose the relevant *Event Code* from the list which will show the *Event Codes* as specified in [Step-3](#step-3-update-experiment-configuration-file). The same button then can be pressed to stop marking of the event. These marking information will be stored along with the data samples in CSV file - with the corresponding *Event-Code*.
 
-> **Step-4h: Stopping to Record**: If the *timed_acquisition* field specified in the [Step-3](#step-3-update-experiment-configurartion-file) is set to *true*, the recording will stop after the specified time, and pressing *Stop Recording* will interrupt the planned acquisition. This can be used only in exception cases in which experiment is to be terminated abruptly. However, if the *timed_acquisition* field is set to *false*, then *Stop Recording* is required to be pressed manually to end the acquisition.
+* **Step-4h: Stopping to Record**: If the *timed_acquisition* field specified in the [Step-3](#step-3-update-experiment-configuration-file) is set to *true*, the recording will stop after the specified time, and pressing *Stop Recording* will interrupt the planned acquisition. This can be used only in exception cases in which experiment is to be terminated abruptly. However, if the *timed_acquisition* field is set to *false*, then *Stop Recording* is required to be pressed manually to end the acquisition.
 
 ---
 
 ### **Data Analysis**
 
 Data analysis is supported by the *analysis_helper* folder. To extract features and export in spreadsheet, please refer to the README provided within the folder.
 In addition, Jupyter notebooks *phys_analysis_eda.ipynb*, *phys_analysis_ppg.ipynb*, and *phys_analysis_resp.ipynb* are provided to illustrate basic analysis steps. This includes pre-processing as well as feature extraction for EDA, PPG and Resp signals respectively.
@@ -205,31 +232,31 @@
 
 ---
 
 ### **Citation**
 
 If you find our [paper](https://www.mdpi.com/1424-8220/23/19/8244) or this toolkit useful for your research, please cite our following works.
 
-```
+```text
 @article{joshi2023physiokit,
     title={PhysioKit: An Open-Source, Low-Cost Physiological Computing Toolkit for Single-and Multi-User Studies},
     author={Joshi, Jitesh and Wang, Katherine and Cho, Youngjun},
     journal={Sensors},
     publisher={MDPI},
     volume={23},
     number={19},
     article-number={8244},
     year={2023},
     url={https://www.mdpi.com/1424-8220/23/19/8244}
     issn={1424-8220},
     doi={10.3390/s23198244}
 }
 
-@article{joshi2024imaging,
-    title={Imaging Blood Volume Pulse Dataset: RGB-Thermal Remote Photoplethysmography Dataset with High-Resolution Signal-Quality Labels},
+@article{joshi2024ibvp,
+    title={iBVP Dataset: RGB-Thermal rPPG Dataset with High Resolution Signal Quality Labels},
     author={Joshi, Jitesh and Cho, Youngjun},
     journal={Electronics},
     publisher={MDPI},
     volume={13},
     year={2024},
     number={7},
     article-number={1334},
```

### Comparing `PhysioKit2-1.8.9/src/PhysioKit2.egg-info/SOURCES.txt` & `physiokit2-2.0.0/src/PhysioKit2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

