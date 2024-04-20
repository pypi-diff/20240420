# Comparing `tmp/spotPython-0.9.8.tar.gz` & `tmp/spotPython-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotPython-0.9.8.tar", last modified: Thu Jan  4 18:32:34 2024, max compression
+gzip compressed data, was "spotPython-0.9.9.tar", last modified: Thu Jan  4 22:34:29 2024, max compression
```

## Comparing `spotPython-0.9.8.tar` & `spotPython-0.9.9.tar`

### file list

```diff
@@ -1,245 +1,245 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.274811 spotPython-0.9.8/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.237946 spotPython-0.9.8/.github/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.241528 spotPython-0.9.8/.github/workflows/
--rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.9.8/.github/workflows/test.yml
--rw-r--r--   0 bartz      (501) staff       (20)    18201 2023-11-15 20:09:20.000000 spotPython-0.9.8/.gitignore
--rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 22:04:43.000000 spotPython-0.9.8/.nojekyll
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.247017 spotPython-0.9.8/Figures.d/
--rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.9.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.9.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.9.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.9.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.9.8/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.9.8/LICENSE.txt
--rw-r--r--   0 bartz      (501) staff       (20)      143 2023-11-13 20:43:59.000000 spotPython-0.9.8/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     8333 2024-01-04 18:32:34.274513 spotPython-0.9.8/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     6808 2023-06-08 16:18:46.000000 spotPython-0.9.8/README.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.247721 spotPython-0.9.8/docs/
--rw-r--r--   0 bartz      (501) staff       (20)    46499 2022-10-31 16:48:05.000000 spotPython-0.9.8/docs/about.md
--rw-r--r--   0 bartz      (501) staff       (20)       49 2023-07-12 23:09:54.000000 spotPython-0.9.8/docs/download.md
--rw-r--r--   0 bartz      (501) staff       (20)      802 2023-07-16 08:32:11.000000 spotPython-0.9.8/docs/examples.md
--rw-r--r--   0 bartz      (501) staff       (20)      947 2022-10-31 16:48:05.000000 spotPython-0.9.8/docs/gen_ref_pages.py
--rw-r--r--   0 bartz      (501) staff       (20)      350 2023-07-14 22:03:54.000000 spotPython-0.9.8/docs/hyperparameter-tuning-cookbook.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.247990 spotPython-0.9.8/docs/images/
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2022-10-31 16:48:05.000000 spotPython-0.9.8/docs/images/favicon.png
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2022-10-31 16:48:05.000000 spotPython-0.9.8/docs/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)      392 2023-07-15 18:25:23.000000 spotPython-0.9.8/docs/index.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.248316 spotPython-0.9.8/img/
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2023-07-13 05:52:18.000000 spotPython-0.9.8/img/favicon.png
--rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-27 21:03:27.000000 spotPython-0.9.8/img/spotLogo.png
--rwxr-xr-x   0 bartz      (501) staff       (20)      146 2023-11-13 16:20:28.000000 spotPython-0.9.8/makeSpot.sh
--rw-r--r--   0 bartz      (501) staff       (20)     2036 2023-12-05 21:02:30.000000 spotPython-0.9.8/mkdocs.yml
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.249595 spotPython-0.9.8/notebooks/
--rw-r--r--   0 bartz      (501) staff       (20)    77906 2024-01-04 11:08:23.000000 spotPython-0.9.8/notebooks/00_spotPython_tests.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    64826 2023-07-15 20:49:26.000000 spotPython-0.9.8/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   953521 2023-11-07 20:56:34.000000 spotPython-0.9.8/notebooks/31_spot_lightning_csv.ipynb
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.238438 spotPython-0.9.8/notebooks/data/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.250004 spotPython-0.9.8/notebooks/data/spotPython/
--rw-r--r--   0 bartz      (501) staff       (20)     2323 2023-11-07 20:50:14.000000 spotPython-0.9.8/notebooks/data/spotPython/data.csv
--rw-r--r--   0 bartz      (501) staff       (20)     7422 2023-11-09 20:35:06.000000 spotPython-0.9.8/notebooks/data/spotPython/data.pkl
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.250331 spotPython-0.9.8/notebooks/data/torch/
--rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.9.8/notebooks/data/torch/model_spot_trained.pt
--rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.9.8/notebooks/data.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.256448 spotPython-0.9.8/notebooks/figures/
--rw-r--r--   0 bartz      (501) staff       (20)   114797 2023-06-07 17:28:19.000000 spotPython-0.9.8/notebooks/figures/12-torch_p040025_1min_5init_2023-06-07_19-09-30_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)   117891 2023-06-08 12:22:25.000000 spotPython-0.9.8/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    35435 2023-06-08 12:22:25.000000 spotPython-0.9.8/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    41877 2023-06-08 12:22:25.000000 spotPython-0.9.8/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   117933 2023-06-07 11:49:47.000000 spotPython-0.9.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    29392 2023-06-07 11:04:53.000000 spotPython-0.9.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   770688 2023-06-07 11:10:20.000000 spotPython-0.9.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_01.png
--rw-r--r--   0 bartz      (501) staff       (20)   305679 2023-06-07 11:11:28.000000 spotPython-0.9.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_02.png
--rw-r--r--   0 bartz      (501) staff       (20)    34252 2023-06-24 19:48:27.000000 spotPython-0.9.8/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    44029 2023-06-24 19:48:27.000000 spotPython-0.9.8/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   121376 2023-05-28 06:32:18.000000 spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png
--rw-r--r--   0 bartz      (501) staff       (20)   116976 2023-06-07 05:09:22.000000 spotPython-0.9.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_contour_0_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    28703 2023-06-06 21:13:57.000000 spotPython-0.9.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)   161701 2023-06-07 06:30:18.000000 spotPython-0.9.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_parallel.png
--rw-r--r--   0 bartz      (501) staff       (20)    41471 2023-06-06 21:13:56.000000 spotPython-0.9.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.9.8/notebooks/figures/spotModel.graffle
--rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.9.8/notebooks/figures/spotModel.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.9.8/notebooks/figures/spotModel.png
--rw-r--r--   0 bartz      (501) staff       (20)   434803 2023-06-07 06:48:45.000000 spotPython-0.9.8/notebooks/figures/tensorboard_0.png
--rw-r--r--   0 bartz      (501) staff       (20)   145933 2023-06-07 06:46:35.000000 spotPython-0.9.8/notebooks/figures/tensorboard_1.png
--rw-r--r--   0 bartz      (501) staff       (20)   751199 2023-06-07 06:51:03.000000 spotPython-0.9.8/notebooks/figures/tensorboard_hdparams.png
--rw-r--r--   0 bartz      (501) staff       (20)  2025087 2023-06-07 06:53:15.000000 spotPython-0.9.8/notebooks/figures/tensorboard_parallel.png
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.258190 spotPython-0.9.8/notebooks/hyperdict/
--rw-r--r--   0 bartz      (501) staff       (20)     6159 2023-11-13 19:20:26.000000 spotPython-0.9.8/notebooks/hyperdict/user_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)   141639 2024-01-04 18:10:44.000000 spotPython-0.9.8/notebooks/testKriging.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     1699 2024-01-04 18:28:26.000000 spotPython-0.9.8/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2024-01-04 18:32:34.274846 spotPython-0.9.8/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.238756 spotPython-0.9.8/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.240077 spotPython-0.9.8/src/spotPython/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.259364 spotPython-0.9.8/src/spotPython/budget/
--rw-r--r--   0 bartz      (501) staff       (20)     7954 2024-01-01 14:25:15.000000 spotPython-0.9.8/src/spotPython/budget/ocba.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.259721 spotPython-0.9.8/src/spotPython/build/
--rw-r--r--   0 bartz      (501) staff       (20)    56929 2024-01-04 12:53:06.000000 spotPython-0.9.8/src/spotPython/build/kriging.py
--rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.9.8/src/spotPython/build/surrogates.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.261473 spotPython-0.9.8/src/spotPython/data/
--rw-r--r--   0 bartz      (501) staff       (20)    23267 2023-07-17 19:56:10.000000 spotPython-0.9.8/src/spotPython/data/base.py
--rw-r--r--   0 bartz      (501) staff       (20)     5255 2024-01-01 16:07:12.000000 spotPython-0.9.8/src/spotPython/data/csvdataset.py
--rw-r--r--   0 bartz      (501) staff       (20)     2323 2023-11-07 20:50:14.000000 spotPython-0.9.8/src/spotPython/data/data.csv
--rw-r--r--   0 bartz      (501) staff       (20)     7422 2023-11-09 20:35:06.000000 spotPython-0.9.8/src/spotPython/data/data.pkl
--rw-r--r--   0 bartz      (501) staff       (20)     4290 2024-01-01 16:07:25.000000 spotPython-0.9.8/src/spotPython/data/diabetes.py
--rw-r--r--   0 bartz      (501) staff       (20)     4882 2024-01-01 16:27:22.000000 spotPython-0.9.8/src/spotPython/data/lightcrossvalidationdatamodule.py
--rw-r--r--   0 bartz      (501) staff       (20)     6739 2023-11-13 16:20:28.000000 spotPython-0.9.8/src/spotPython/data/lightdatamodule.py
--rw-r--r--   0 bartz      (501) staff       (20)     1659 2023-06-25 16:06:47.000000 spotPython-0.9.8/src/spotPython/data/mnistdatamodule.py
--rw-r--r--   0 bartz      (501) staff       (20)     8280 2024-01-01 20:17:50.000000 spotPython-0.9.8/src/spotPython/data/pkldataset.py
--rw-r--r--   0 bartz      (501) staff       (20)     1472 2024-01-01 16:10:26.000000 spotPython-0.9.8/src/spotPython/data/torchdata.py
--rw-r--r--   0 bartz      (501) staff       (20)     2912 2023-07-17 20:14:22.000000 spotPython-0.9.8/src/spotPython/data/vbdp.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.261833 spotPython-0.9.8/src/spotPython/design/
--rw-r--r--   0 bartz      (501) staff       (20)     1223 2023-07-17 22:31:41.000000 spotPython-0.9.8/src/spotPython/design/designs.py
--rw-r--r--   0 bartz      (501) staff       (20)     1299 2023-07-23 21:35:33.000000 spotPython-0.9.8/src/spotPython/design/factorial.py
--rw-r--r--   0 bartz      (501) staff       (20)     2227 2023-07-23 21:36:02.000000 spotPython-0.9.8/src/spotPython/design/spacefilling.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.262495 spotPython-0.9.8/src/spotPython/fun/
--rw-r--r--   0 bartz      (501) staff       (20)     6556 2024-01-04 11:08:59.000000 spotPython-0.9.8/src/spotPython/fun/hyperlight.py
--rw-r--r--   0 bartz      (501) staff       (20)     5722 2024-01-01 16:12:32.000000 spotPython-0.9.8/src/spotPython/fun/hypersklearn.py
--rw-r--r--   0 bartz      (501) staff       (20)     7437 2024-01-01 16:12:52.000000 spotPython-0.9.8/src/spotPython/fun/hypertorch.py
--rw-r--r--   0 bartz      (501) staff       (20)    24148 2023-12-20 22:01:40.000000 spotPython-0.9.8/src/spotPython/fun/objectivefunctions.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.263296 spotPython-0.9.8/src/spotPython/hyperdict/
--rw-r--r--   0 bartz      (501) staff       (20)     8746 2023-11-13 20:54:18.000000 spotPython-0.9.8/src/spotPython/hyperdict/light_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)     2099 2023-11-15 21:51:13.000000 spotPython-0.9.8/src/spotPython/hyperdict/light_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-30 15:26:52.000000 spotPython-0.9.8/src/spotPython/hyperdict/sklearn_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)     1570 2023-11-15 23:29:54.000000 spotPython-0.9.8/src/spotPython/hyperdict/sklearn_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)     9208 2023-06-06 20:04:52.000000 spotPython-0.9.8/src/spotPython/hyperdict/torch_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)     1555 2023-11-15 23:30:01.000000 spotPython-0.9.8/src/spotPython/hyperdict/torch_hyper_dict.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.263750 spotPython-0.9.8/src/spotPython/hyperparameters/
--rw-r--r--   0 bartz      (501) staff       (20)     4859 2024-01-01 16:13:48.000000 spotPython-0.9.8/src/spotPython/hyperparameters/categorical.py
--rw-r--r--   0 bartz      (501) staff       (20)     7235 2024-01-01 16:13:59.000000 spotPython-0.9.8/src/spotPython/hyperparameters/optimizer.py
--rw-r--r--   0 bartz      (501) staff       (20)    41783 2024-01-04 18:30:03.000000 spotPython-0.9.8/src/spotPython/hyperparameters/values.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.264404 spotPython-0.9.8/src/spotPython/light/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.264571 spotPython-0.9.8/src/spotPython/light/cifar10/
--rw-r--r--   0 bartz      (501) staff       (20)     4057 2023-07-25 19:34:11.000000 spotPython-0.9.8/src/spotPython/light/cifar10/cifar10datamodule.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.264698 spotPython-0.9.8/src/spotPython/light/classification/
--rw-r--r--   0 bartz      (501) staff       (20)    12296 2024-01-01 16:27:22.000000 spotPython-0.9.8/src/spotPython/light/classification/netlightbasemapk.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.265096 spotPython-0.9.8/src/spotPython/light/cnn/
--rw-r--r--   0 bartz      (501) staff       (20)     4662 2023-11-15 20:43:10.000000 spotPython-0.9.8/src/spotPython/light/cnn/googlenet.py
--rw-r--r--   0 bartz      (501) staff       (20)     3241 2023-11-15 20:42:50.000000 spotPython-0.9.8/src/spotPython/light/cnn/inceptionblock.py
--rw-r--r--   0 bartz      (501) staff       (20)     4252 2023-11-15 22:13:20.000000 spotPython-0.9.8/src/spotPython/light/cnn/netcnnbase.py
--rw-r--r--   0 bartz      (501) staff       (20)     3877 2023-11-15 20:42:50.000000 spotPython-0.9.8/src/spotPython/light/cvmodel.py
--rw-r--r--   0 bartz      (501) staff       (20)     5546 2023-07-17 21:54:43.000000 spotPython-0.9.8/src/spotPython/light/litmodel.py
--rw-r--r--   0 bartz      (501) staff       (20)     1833 2023-11-15 22:40:59.000000 spotPython-0.9.8/src/spotPython/light/loadmodel.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.265263 spotPython-0.9.8/src/spotPython/light/regression/
--rw-r--r--   0 bartz      (501) staff       (20)    11553 2023-11-15 11:27:59.000000 spotPython-0.9.8/src/spotPython/light/regression/netlightregression.py
--rw-r--r--   0 bartz      (501) staff       (20)     4585 2023-11-15 21:38:42.000000 spotPython-0.9.8/src/spotPython/light/testmodel.py
--rw-r--r--   0 bartz      (501) staff       (20)     6014 2023-11-15 20:42:50.000000 spotPython-0.9.8/src/spotPython/light/trainmodel.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.265546 spotPython-0.9.8/src/spotPython/plot/
--rw-r--r--   0 bartz      (501) staff       (20)     1708 2023-07-23 21:37:57.000000 spotPython-0.9.8/src/spotPython/plot/contour.py
--rw-r--r--   0 bartz      (501) staff       (20)     9643 2023-11-05 19:41:15.000000 spotPython-0.9.8/src/spotPython/plot/validation.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.265710 spotPython-0.9.8/src/spotPython/sklearn/
--rw-r--r--   0 bartz      (501) staff       (20)     3794 2023-08-08 18:43:24.000000 spotPython-0.9.8/src/spotPython/sklearn/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.265827 spotPython-0.9.8/src/spotPython/spot/
--rw-r--r--   0 bartz      (501) staff       (20)    71927 2024-01-04 18:30:03.000000 spotPython-0.9.8/src/spotPython/spot/spot.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.267015 spotPython-0.9.8/src/spotPython/torch/
--rw-r--r--   0 bartz      (501) staff       (20)     1018 2023-06-23 13:29:53.000000 spotPython-0.9.8/src/spotPython/torch/activation.py
--rw-r--r--   0 bartz      (501) staff       (20)      517 2023-05-31 19:01:06.000000 spotPython-0.9.8/src/spotPython/torch/dataframedataset.py
--rw-r--r--   0 bartz      (501) staff       (20)      692 2023-06-27 22:26:23.000000 spotPython-0.9.8/src/spotPython/torch/initialization.py
--rw-r--r--   0 bartz      (501) staff       (20)     5191 2023-07-24 17:15:21.000000 spotPython-0.9.8/src/spotPython/torch/mapk.py
--rw-r--r--   0 bartz      (501) staff       (20)     1012 2023-05-27 19:17:19.000000 spotPython-0.9.8/src/spotPython/torch/netcifar10.py
--rw-r--r--   0 bartz      (501) staff       (20)      425 2023-05-27 19:21:33.000000 spotPython-0.9.8/src/spotPython/torch/netcore.py
--rw-r--r--   0 bartz      (501) staff       (20)      803 2023-05-27 19:17:19.000000 spotPython-0.9.8/src/spotPython/torch/netfashionMNIST.py
--rw-r--r--   0 bartz      (501) staff       (20)     1071 2023-06-06 19:59:34.000000 spotPython-0.9.8/src/spotPython/torch/netregression.py
--rw-r--r--   0 bartz      (501) staff       (20)     1565 2023-06-01 18:55:33.000000 spotPython-0.9.8/src/spotPython/torch/netvbdp.py
--rw-r--r--   0 bartz      (501) staff       (20)    14987 2023-06-20 05:35:32.000000 spotPython-0.9.8/src/spotPython/torch/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.268624 spotPython-0.9.8/src/spotPython/utils/
--rw-r--r--   0 bartz      (501) staff       (20)     2124 2023-12-29 16:37:32.000000 spotPython-0.9.8/src/spotPython/utils/aggregate.py
--rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.9.8/src/spotPython/utils/classes.py
--rw-r--r--   0 bartz      (501) staff       (20)     1783 2024-01-01 16:19:22.000000 spotPython-0.9.8/src/spotPython/utils/compare.py
--rw-r--r--   0 bartz      (501) staff       (20)     3831 2024-01-01 16:27:22.000000 spotPython-0.9.8/src/spotPython/utils/convert.py
--rw-r--r--   0 bartz      (501) staff       (20)      630 2024-01-01 16:27:22.000000 spotPython-0.9.8/src/spotPython/utils/device.py
--rw-r--r--   0 bartz      (501) staff       (20)    14604 2024-01-01 16:27:22.000000 spotPython-0.9.8/src/spotPython/utils/eda.py
--rw-r--r--   0 bartz      (501) staff       (20)     3314 2024-01-01 16:27:22.000000 spotPython-0.9.8/src/spotPython/utils/file.py
--rw-r--r--   0 bartz      (501) staff       (20)     6291 2024-01-04 18:32:23.000000 spotPython-0.9.8/src/spotPython/utils/init.py
--rw-r--r--   0 bartz      (501) staff       (20)     4834 2024-01-01 16:27:22.000000 spotPython-0.9.8/src/spotPython/utils/metrics.py
--rw-r--r--   0 bartz      (501) staff       (20)      912 2023-06-01 22:37:01.000000 spotPython-0.9.8/src/spotPython/utils/progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1381 2023-07-23 21:38:50.000000 spotPython-0.9.8/src/spotPython/utils/repair.py
--rw-r--r--   0 bartz      (501) staff       (20)      683 2023-11-15 19:12:17.000000 spotPython-0.9.8/src/spotPython/utils/tensorboard.py
--rw-r--r--   0 bartz      (501) staff       (20)    12686 2024-01-01 16:27:22.000000 spotPython-0.9.8/src/spotPython/utils/transform.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.274083 spotPython-0.9.8/src/spotPython.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     8333 2024-01-04 18:32:34.000000 spotPython-0.9.8/src/spotPython.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     9395 2024-01-04 18:32:34.000000 spotPython-0.9.8/src/spotPython.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2024-01-04 18:32:34.000000 spotPython-0.9.8/src/spotPython.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)      350 2024-01-04 18:32:34.000000 spotPython-0.9.8/src/spotPython.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)       11 2024-01-04 18:32:34.000000 spotPython-0.9.8/src/spotPython.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 18:32:34.273891 spotPython-0.9.8/test/
--rw-r--r--   0 bartz      (501) staff       (20)      744 2023-11-15 21:55:41.000000 spotPython-0.9.8/test/test_add_core_model_to_fun_control.py
--rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.9.8/test/test_aggregate_mean_var.py
--rw-r--r--   0 bartz      (501) staff       (20)      913 2023-12-06 22:05:45.000000 spotPython-0.9.8/test/test_branin.py
--rw-r--r--   0 bartz      (501) staff       (20)     4567 2023-12-29 16:21:01.000000 spotPython-0.9.8/test/test_build_Psi.py
--rw-r--r--   0 bartz      (501) staff       (20)     4532 2023-12-29 16:21:35.000000 spotPython-0.9.8/test/test_build_U.py
--rw-r--r--   0 bartz      (501) staff       (20)      806 2023-12-28 10:38:39.000000 spotPython-0.9.8/test/test_build_psi_vec.py
--rw-r--r--   0 bartz      (501) staff       (20)     1087 2023-11-15 21:55:41.000000 spotPython-0.9.8/test/test_check_X_shape.py
--rw-r--r--   0 bartz      (501) staff       (20)      516 2024-01-01 15:41:45.000000 spotPython-0.9.8/test/test_chg.py
--rw-r--r--   0 bartz      (501) staff       (20)      900 2023-11-10 14:45:12.000000 spotPython-0.9.8/test/test_csvdataset.py
--rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.9.8/test/test_evaluate_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.9.8/test/test_evaluate_new_solutions.py
--rw-r--r--   0 bartz      (501) staff       (20)    10396 2023-12-29 16:26:25.000000 spotPython-0.9.8/test/test_extract_from_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)      795 2023-12-31 13:33:23.000000 spotPython-0.9.8/test/test_fit_surrogate.py
--rw-r--r--   0 bartz      (501) staff       (20)      737 2023-10-31 15:30:29.000000 spotPython-0.9.8/test/test_fun_control_init.py
--rw-r--r--   0 bartz      (501) staff       (20)     2332 2024-01-03 21:17:18.000000 spotPython-0.9.8/test/test_generate_design.py
--rw-r--r--   0 bartz      (501) staff       (20)     1178 2024-01-02 22:13:10.000000 spotPython-0.9.8/test/test_get_new_X0.py
--rw-r--r--   0 bartz      (501) staff       (20)     1507 2023-11-14 19:22:31.000000 spotPython-0.9.8/test/test_get_var_name.py
--rw-r--r--   0 bartz      (501) staff       (20)     1257 2023-11-15 21:55:41.000000 spotPython-0.9.8/test/test_hyper_light_fun.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.9.8/test/test_infill.py
--rw-r--r--   0 bartz      (501) staff       (20)     3470 2023-12-31 11:25:29.000000 spotPython-0.9.8/test/test_initialize_design.py
--rw-r--r--   0 bartz      (501) staff       (20)      481 2024-01-01 15:40:32.000000 spotPython-0.9.8/test/test_is_any.py
--rw-r--r--   0 bartz      (501) staff       (20)     8755 2023-12-30 09:19:22.000000 spotPython-0.9.8/test/test_kriging.py
--rw-r--r--   0 bartz      (501) staff       (20)     1185 2023-11-12 22:54:45.000000 spotPython-0.9.8/test/test_lightdatamodule.py
--rw-r--r--   0 bartz      (501) staff       (20)     2299 2023-12-29 19:29:10.000000 spotPython-0.9.8/test/test_nat_to_cod.py
--rw-r--r--   0 bartz      (501) staff       (20)     1440 2023-11-15 21:55:41.000000 spotPython-0.9.8/test/test_net_light_regression_class.py
--rw-r--r--   0 bartz      (501) staff       (20)     2152 2024-01-03 18:05:00.000000 spotPython-0.9.8/test/test_ocba.py
--rw-r--r--   0 bartz      (501) staff       (20)     1989 2023-11-15 21:55:41.000000 spotPython-0.9.8/test/test_optimizer_handler.py
--rw-r--r--   0 bartz      (501) staff       (20)      900 2023-11-12 15:19:14.000000 spotPython-0.9.8/test/test_pkldataset.py
--rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.9.8/test/test_repair_non_numeric.py
--rw-r--r--   0 bartz      (501) staff       (20)      506 2023-12-31 18:16:20.000000 spotPython-0.9.8/test/test_selectNew().py
--rw-r--r--   0 bartz      (501) staff       (20)     1337 2024-01-02 10:36:40.000000 spotPython-0.9.8/test/test_set_data_module.py
--rw-r--r--   0 bartz      (501) staff       (20)     4904 2023-12-29 16:24:39.000000 spotPython-0.9.8/test/test_set_de_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.9.8/test/test_show_progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1107 2024-01-01 15:59:04.000000 spotPython-0.9.8/test/test_suggest_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1374 2023-11-15 21:55:41.000000 spotPython-0.9.8/test/test_testmodel.py
--rw-r--r--   0 bartz      (501) staff       (20)      996 2024-01-03 21:45:15.000000 spotPython-0.9.8/test/test_to_red.py
--rw-r--r--   0 bartz      (501) staff       (20)     1365 2023-11-15 21:55:41.000000 spotPython-0.9.8/test/test_trainmodel.py
--rw-r--r--   0 bartz      (501) staff       (20)     3568 2024-01-02 22:13:10.000000 spotPython-0.9.8/test/test_update_design.py
--rw-r--r--   0 bartz      (501) staff       (20)     3524 2024-01-03 21:08:41.000000 spotPython-0.9.8/test/test_update_stats.py
--rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.9.8/test/test_update_surrogate.py
--rw-r--r--   0 bartz      (501) staff       (20)     2300 2024-01-04 18:30:03.000000 spotPython-0.9.8/test/test_values.py
--rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 10:19:58.000000 spotPython-0.9.8/tox.ini
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.150528 spotPython-0.9.9/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.116933 spotPython-0.9.9/.github/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.120537 spotPython-0.9.9/.github/workflows/
+-rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.9.9/.github/workflows/test.yml
+-rw-r--r--   0 bartz      (501) staff       (20)    18201 2023-11-15 20:09:20.000000 spotPython-0.9.9/.gitignore
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 22:04:43.000000 spotPython-0.9.9/.nojekyll
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.125990 spotPython-0.9.9/Figures.d/
+-rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.9.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.9.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.9.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.9.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.9.9/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.9.9/LICENSE.txt
+-rw-r--r--   0 bartz      (501) staff       (20)      143 2023-11-13 20:43:59.000000 spotPython-0.9.9/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     8333 2024-01-04 22:34:29.150255 spotPython-0.9.9/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     6808 2023-06-08 16:18:46.000000 spotPython-0.9.9/README.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.126771 spotPython-0.9.9/docs/
+-rw-r--r--   0 bartz      (501) staff       (20)    46499 2022-10-31 16:48:05.000000 spotPython-0.9.9/docs/about.md
+-rw-r--r--   0 bartz      (501) staff       (20)       49 2023-07-12 23:09:54.000000 spotPython-0.9.9/docs/download.md
+-rw-r--r--   0 bartz      (501) staff       (20)      802 2023-07-16 08:32:11.000000 spotPython-0.9.9/docs/examples.md
+-rw-r--r--   0 bartz      (501) staff       (20)      947 2022-10-31 16:48:05.000000 spotPython-0.9.9/docs/gen_ref_pages.py
+-rw-r--r--   0 bartz      (501) staff       (20)      350 2023-07-14 22:03:54.000000 spotPython-0.9.9/docs/hyperparameter-tuning-cookbook.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.127098 spotPython-0.9.9/docs/images/
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2022-10-31 16:48:05.000000 spotPython-0.9.9/docs/images/favicon.png
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2022-10-31 16:48:05.000000 spotPython-0.9.9/docs/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)      392 2023-07-15 18:25:23.000000 spotPython-0.9.9/docs/index.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.127464 spotPython-0.9.9/img/
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2023-07-13 05:52:18.000000 spotPython-0.9.9/img/favicon.png
+-rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-27 21:03:27.000000 spotPython-0.9.9/img/spotLogo.png
+-rwxr-xr-x   0 bartz      (501) staff       (20)      146 2023-11-13 16:20:28.000000 spotPython-0.9.9/makeSpot.sh
+-rw-r--r--   0 bartz      (501) staff       (20)     2036 2023-12-05 21:02:30.000000 spotPython-0.9.9/mkdocs.yml
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.128684 spotPython-0.9.9/notebooks/
+-rw-r--r--   0 bartz      (501) staff       (20)    77906 2024-01-04 11:08:23.000000 spotPython-0.9.9/notebooks/00_spotPython_tests.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    64826 2023-07-15 20:49:26.000000 spotPython-0.9.9/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   953521 2023-11-07 20:56:34.000000 spotPython-0.9.9/notebooks/31_spot_lightning_csv.ipynb
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.117561 spotPython-0.9.9/notebooks/data/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.128976 spotPython-0.9.9/notebooks/data/spotPython/
+-rw-r--r--   0 bartz      (501) staff       (20)     2323 2023-11-07 20:50:14.000000 spotPython-0.9.9/notebooks/data/spotPython/data.csv
+-rw-r--r--   0 bartz      (501) staff       (20)     7422 2023-11-09 20:35:06.000000 spotPython-0.9.9/notebooks/data/spotPython/data.pkl
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.129089 spotPython-0.9.9/notebooks/data/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.9.9/notebooks/data/torch/model_spot_trained.pt
+-rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.9.9/notebooks/data.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.134823 spotPython-0.9.9/notebooks/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)   114797 2023-06-07 17:28:19.000000 spotPython-0.9.9/notebooks/figures/12-torch_p040025_1min_5init_2023-06-07_19-09-30_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)   117891 2023-06-08 12:22:25.000000 spotPython-0.9.9/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    35435 2023-06-08 12:22:25.000000 spotPython-0.9.9/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    41877 2023-06-08 12:22:25.000000 spotPython-0.9.9/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   117933 2023-06-07 11:49:47.000000 spotPython-0.9.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    29392 2023-06-07 11:04:53.000000 spotPython-0.9.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   770688 2023-06-07 11:10:20.000000 spotPython-0.9.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_01.png
+-rw-r--r--   0 bartz      (501) staff       (20)   305679 2023-06-07 11:11:28.000000 spotPython-0.9.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_02.png
+-rw-r--r--   0 bartz      (501) staff       (20)    34252 2023-06-24 19:48:27.000000 spotPython-0.9.9/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    44029 2023-06-24 19:48:27.000000 spotPython-0.9.9/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   121376 2023-05-28 06:32:18.000000 spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png
+-rw-r--r--   0 bartz      (501) staff       (20)   116976 2023-06-07 05:09:22.000000 spotPython-0.9.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    28703 2023-06-06 21:13:57.000000 spotPython-0.9.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)   161701 2023-06-07 06:30:18.000000 spotPython-0.9.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_parallel.png
+-rw-r--r--   0 bartz      (501) staff       (20)    41471 2023-06-06 21:13:56.000000 spotPython-0.9.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.9.9/notebooks/figures/spotModel.graffle
+-rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.9.9/notebooks/figures/spotModel.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.9.9/notebooks/figures/spotModel.png
+-rw-r--r--   0 bartz      (501) staff       (20)   434803 2023-06-07 06:48:45.000000 spotPython-0.9.9/notebooks/figures/tensorboard_0.png
+-rw-r--r--   0 bartz      (501) staff       (20)   145933 2023-06-07 06:46:35.000000 spotPython-0.9.9/notebooks/figures/tensorboard_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)   751199 2023-06-07 06:51:03.000000 spotPython-0.9.9/notebooks/figures/tensorboard_hdparams.png
+-rw-r--r--   0 bartz      (501) staff       (20)  2025087 2023-06-07 06:53:15.000000 spotPython-0.9.9/notebooks/figures/tensorboard_parallel.png
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.135864 spotPython-0.9.9/notebooks/hyperdict/
+-rw-r--r--   0 bartz      (501) staff       (20)     6159 2023-11-13 19:20:26.000000 spotPython-0.9.9/notebooks/hyperdict/user_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)   141639 2024-01-04 18:10:44.000000 spotPython-0.9.9/notebooks/testKriging.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     1699 2024-01-04 21:29:19.000000 spotPython-0.9.9/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2024-01-04 22:34:29.150576 spotPython-0.9.9/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.117918 spotPython-0.9.9/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.119042 spotPython-0.9.9/src/spotPython/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.136642 spotPython-0.9.9/src/spotPython/budget/
+-rw-r--r--   0 bartz      (501) staff       (20)     7954 2024-01-01 14:25:15.000000 spotPython-0.9.9/src/spotPython/budget/ocba.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.136888 spotPython-0.9.9/src/spotPython/build/
+-rw-r--r--   0 bartz      (501) staff       (20)    56929 2024-01-04 12:53:06.000000 spotPython-0.9.9/src/spotPython/build/kriging.py
+-rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.9.9/src/spotPython/build/surrogates.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.138162 spotPython-0.9.9/src/spotPython/data/
+-rw-r--r--   0 bartz      (501) staff       (20)    23267 2023-07-17 19:56:10.000000 spotPython-0.9.9/src/spotPython/data/base.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5255 2024-01-01 16:07:12.000000 spotPython-0.9.9/src/spotPython/data/csvdataset.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2323 2023-11-07 20:50:14.000000 spotPython-0.9.9/src/spotPython/data/data.csv
+-rw-r--r--   0 bartz      (501) staff       (20)     7422 2023-11-09 20:35:06.000000 spotPython-0.9.9/src/spotPython/data/data.pkl
+-rw-r--r--   0 bartz      (501) staff       (20)     4290 2024-01-01 16:07:25.000000 spotPython-0.9.9/src/spotPython/data/diabetes.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4882 2024-01-01 16:27:22.000000 spotPython-0.9.9/src/spotPython/data/lightcrossvalidationdatamodule.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6739 2023-11-13 16:20:28.000000 spotPython-0.9.9/src/spotPython/data/lightdatamodule.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1659 2023-06-25 16:06:47.000000 spotPython-0.9.9/src/spotPython/data/mnistdatamodule.py
+-rw-r--r--   0 bartz      (501) staff       (20)     8280 2024-01-01 20:17:50.000000 spotPython-0.9.9/src/spotPython/data/pkldataset.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1472 2024-01-01 16:10:26.000000 spotPython-0.9.9/src/spotPython/data/torchdata.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2912 2023-07-17 20:14:22.000000 spotPython-0.9.9/src/spotPython/data/vbdp.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.138490 spotPython-0.9.9/src/spotPython/design/
+-rw-r--r--   0 bartz      (501) staff       (20)     1223 2023-07-17 22:31:41.000000 spotPython-0.9.9/src/spotPython/design/designs.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1299 2023-07-23 21:35:33.000000 spotPython-0.9.9/src/spotPython/design/factorial.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2227 2023-07-23 21:36:02.000000 spotPython-0.9.9/src/spotPython/design/spacefilling.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.138930 spotPython-0.9.9/src/spotPython/fun/
+-rw-r--r--   0 bartz      (501) staff       (20)     6556 2024-01-04 11:08:59.000000 spotPython-0.9.9/src/spotPython/fun/hyperlight.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5722 2024-01-01 16:12:32.000000 spotPython-0.9.9/src/spotPython/fun/hypersklearn.py
+-rw-r--r--   0 bartz      (501) staff       (20)     7437 2024-01-01 16:12:52.000000 spotPython-0.9.9/src/spotPython/fun/hypertorch.py
+-rw-r--r--   0 bartz      (501) staff       (20)    24148 2023-12-20 22:01:40.000000 spotPython-0.9.9/src/spotPython/fun/objectivefunctions.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.139703 spotPython-0.9.9/src/spotPython/hyperdict/
+-rw-r--r--   0 bartz      (501) staff       (20)     2550 2024-01-04 21:28:15.000000 spotPython-0.9.9/src/spotPython/hyperdict/light_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)     2099 2023-11-15 21:51:13.000000 spotPython-0.9.9/src/spotPython/hyperdict/light_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-30 15:26:52.000000 spotPython-0.9.9/src/spotPython/hyperdict/sklearn_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)     1570 2023-11-15 23:29:54.000000 spotPython-0.9.9/src/spotPython/hyperdict/sklearn_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)     9208 2023-06-06 20:04:52.000000 spotPython-0.9.9/src/spotPython/hyperdict/torch_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)     1555 2023-11-15 23:30:01.000000 spotPython-0.9.9/src/spotPython/hyperdict/torch_hyper_dict.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.140024 spotPython-0.9.9/src/spotPython/hyperparameters/
+-rw-r--r--   0 bartz      (501) staff       (20)     4859 2024-01-01 16:13:48.000000 spotPython-0.9.9/src/spotPython/hyperparameters/categorical.py
+-rw-r--r--   0 bartz      (501) staff       (20)     7235 2024-01-01 16:13:59.000000 spotPython-0.9.9/src/spotPython/hyperparameters/optimizer.py
+-rw-r--r--   0 bartz      (501) staff       (20)    41806 2024-01-04 22:29:41.000000 spotPython-0.9.9/src/spotPython/hyperparameters/values.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.140574 spotPython-0.9.9/src/spotPython/light/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.140683 spotPython-0.9.9/src/spotPython/light/cifar10/
+-rw-r--r--   0 bartz      (501) staff       (20)     4057 2023-07-25 19:34:11.000000 spotPython-0.9.9/src/spotPython/light/cifar10/cifar10datamodule.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.140796 spotPython-0.9.9/src/spotPython/light/classification/
+-rw-r--r--   0 bartz      (501) staff       (20)    12296 2024-01-01 16:27:22.000000 spotPython-0.9.9/src/spotPython/light/classification/netlightbasemapk.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.141171 spotPython-0.9.9/src/spotPython/light/cnn/
+-rw-r--r--   0 bartz      (501) staff       (20)     4662 2023-11-15 20:43:10.000000 spotPython-0.9.9/src/spotPython/light/cnn/googlenet.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3241 2023-11-15 20:42:50.000000 spotPython-0.9.9/src/spotPython/light/cnn/inceptionblock.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4252 2023-11-15 22:13:20.000000 spotPython-0.9.9/src/spotPython/light/cnn/netcnnbase.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3877 2023-11-15 20:42:50.000000 spotPython-0.9.9/src/spotPython/light/cvmodel.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5546 2023-07-17 21:54:43.000000 spotPython-0.9.9/src/spotPython/light/litmodel.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1833 2023-11-15 22:40:59.000000 spotPython-0.9.9/src/spotPython/light/loadmodel.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.141284 spotPython-0.9.9/src/spotPython/light/regression/
+-rw-r--r--   0 bartz      (501) staff       (20)    11553 2023-11-15 11:27:59.000000 spotPython-0.9.9/src/spotPython/light/regression/netlightregression.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4585 2023-11-15 21:38:42.000000 spotPython-0.9.9/src/spotPython/light/testmodel.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6014 2023-11-15 20:42:50.000000 spotPython-0.9.9/src/spotPython/light/trainmodel.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.141553 spotPython-0.9.9/src/spotPython/plot/
+-rw-r--r--   0 bartz      (501) staff       (20)     1708 2023-07-23 21:37:57.000000 spotPython-0.9.9/src/spotPython/plot/contour.py
+-rw-r--r--   0 bartz      (501) staff       (20)     9643 2023-11-05 19:41:15.000000 spotPython-0.9.9/src/spotPython/plot/validation.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.141731 spotPython-0.9.9/src/spotPython/sklearn/
+-rw-r--r--   0 bartz      (501) staff       (20)     3794 2023-08-08 18:43:24.000000 spotPython-0.9.9/src/spotPython/sklearn/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.141842 spotPython-0.9.9/src/spotPython/spot/
+-rw-r--r--   0 bartz      (501) staff       (20)    71931 2024-01-04 22:26:20.000000 spotPython-0.9.9/src/spotPython/spot/spot.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.142968 spotPython-0.9.9/src/spotPython/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)     1018 2023-06-23 13:29:53.000000 spotPython-0.9.9/src/spotPython/torch/activation.py
+-rw-r--r--   0 bartz      (501) staff       (20)      517 2023-05-31 19:01:06.000000 spotPython-0.9.9/src/spotPython/torch/dataframedataset.py
+-rw-r--r--   0 bartz      (501) staff       (20)      692 2023-06-27 22:26:23.000000 spotPython-0.9.9/src/spotPython/torch/initialization.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5191 2023-07-24 17:15:21.000000 spotPython-0.9.9/src/spotPython/torch/mapk.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1012 2023-05-27 19:17:19.000000 spotPython-0.9.9/src/spotPython/torch/netcifar10.py
+-rw-r--r--   0 bartz      (501) staff       (20)      425 2023-05-27 19:21:33.000000 spotPython-0.9.9/src/spotPython/torch/netcore.py
+-rw-r--r--   0 bartz      (501) staff       (20)      803 2023-05-27 19:17:19.000000 spotPython-0.9.9/src/spotPython/torch/netfashionMNIST.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1071 2023-06-06 19:59:34.000000 spotPython-0.9.9/src/spotPython/torch/netregression.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1565 2023-06-01 18:55:33.000000 spotPython-0.9.9/src/spotPython/torch/netvbdp.py
+-rw-r--r--   0 bartz      (501) staff       (20)    14987 2023-06-20 05:35:32.000000 spotPython-0.9.9/src/spotPython/torch/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.144583 spotPython-0.9.9/src/spotPython/utils/
+-rw-r--r--   0 bartz      (501) staff       (20)     2124 2023-12-29 16:37:32.000000 spotPython-0.9.9/src/spotPython/utils/aggregate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.9.9/src/spotPython/utils/classes.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1783 2024-01-01 16:19:22.000000 spotPython-0.9.9/src/spotPython/utils/compare.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3831 2024-01-01 16:27:22.000000 spotPython-0.9.9/src/spotPython/utils/convert.py
+-rw-r--r--   0 bartz      (501) staff       (20)      630 2024-01-01 16:27:22.000000 spotPython-0.9.9/src/spotPython/utils/device.py
+-rw-r--r--   0 bartz      (501) staff       (20)    14604 2024-01-01 16:27:22.000000 spotPython-0.9.9/src/spotPython/utils/eda.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3314 2024-01-01 16:27:22.000000 spotPython-0.9.9/src/spotPython/utils/file.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6291 2024-01-04 18:32:23.000000 spotPython-0.9.9/src/spotPython/utils/init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4834 2024-01-01 16:27:22.000000 spotPython-0.9.9/src/spotPython/utils/metrics.py
+-rw-r--r--   0 bartz      (501) staff       (20)      912 2023-06-01 22:37:01.000000 spotPython-0.9.9/src/spotPython/utils/progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1381 2023-07-23 21:38:50.000000 spotPython-0.9.9/src/spotPython/utils/repair.py
+-rw-r--r--   0 bartz      (501) staff       (20)      683 2023-11-15 19:12:17.000000 spotPython-0.9.9/src/spotPython/utils/tensorboard.py
+-rw-r--r--   0 bartz      (501) staff       (20)    12686 2024-01-01 16:27:22.000000 spotPython-0.9.9/src/spotPython/utils/transform.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.149775 spotPython-0.9.9/src/spotPython.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     8333 2024-01-04 22:34:29.000000 spotPython-0.9.9/src/spotPython.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     9395 2024-01-04 22:34:29.000000 spotPython-0.9.9/src/spotPython.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2024-01-04 22:34:29.000000 spotPython-0.9.9/src/spotPython.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)      350 2024-01-04 22:34:29.000000 spotPython-0.9.9/src/spotPython.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       11 2024-01-04 22:34:29.000000 spotPython-0.9.9/src/spotPython.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-01-04 22:34:29.149592 spotPython-0.9.9/test/
+-rw-r--r--   0 bartz      (501) staff       (20)      744 2023-11-15 21:55:41.000000 spotPython-0.9.9/test/test_add_core_model_to_fun_control.py
+-rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.9.9/test/test_aggregate_mean_var.py
+-rw-r--r--   0 bartz      (501) staff       (20)      913 2023-12-06 22:05:45.000000 spotPython-0.9.9/test/test_branin.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4567 2023-12-29 16:21:01.000000 spotPython-0.9.9/test/test_build_Psi.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4532 2023-12-29 16:21:35.000000 spotPython-0.9.9/test/test_build_U.py
+-rw-r--r--   0 bartz      (501) staff       (20)      806 2023-12-28 10:38:39.000000 spotPython-0.9.9/test/test_build_psi_vec.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1087 2023-11-15 21:55:41.000000 spotPython-0.9.9/test/test_check_X_shape.py
+-rw-r--r--   0 bartz      (501) staff       (20)      516 2024-01-01 15:41:45.000000 spotPython-0.9.9/test/test_chg.py
+-rw-r--r--   0 bartz      (501) staff       (20)      900 2023-11-10 14:45:12.000000 spotPython-0.9.9/test/test_csvdataset.py
+-rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.9.9/test/test_evaluate_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.9.9/test/test_evaluate_new_solutions.py
+-rw-r--r--   0 bartz      (501) staff       (20)    10396 2023-12-29 16:26:25.000000 spotPython-0.9.9/test/test_extract_from_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)      795 2023-12-31 13:33:23.000000 spotPython-0.9.9/test/test_fit_surrogate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      737 2023-10-31 15:30:29.000000 spotPython-0.9.9/test/test_fun_control_init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2332 2024-01-03 21:17:18.000000 spotPython-0.9.9/test/test_generate_design.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1178 2024-01-02 22:13:10.000000 spotPython-0.9.9/test/test_get_new_X0.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1507 2023-11-14 19:22:31.000000 spotPython-0.9.9/test/test_get_var_name.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1257 2023-11-15 21:55:41.000000 spotPython-0.9.9/test/test_hyper_light_fun.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.9.9/test/test_infill.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3470 2023-12-31 11:25:29.000000 spotPython-0.9.9/test/test_initialize_design.py
+-rw-r--r--   0 bartz      (501) staff       (20)      481 2024-01-01 15:40:32.000000 spotPython-0.9.9/test/test_is_any.py
+-rw-r--r--   0 bartz      (501) staff       (20)     8755 2023-12-30 09:19:22.000000 spotPython-0.9.9/test/test_kriging.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1185 2023-11-12 22:54:45.000000 spotPython-0.9.9/test/test_lightdatamodule.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2299 2023-12-29 19:29:10.000000 spotPython-0.9.9/test/test_nat_to_cod.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1440 2023-11-15 21:55:41.000000 spotPython-0.9.9/test/test_net_light_regression_class.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2152 2024-01-03 18:05:00.000000 spotPython-0.9.9/test/test_ocba.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1989 2023-11-15 21:55:41.000000 spotPython-0.9.9/test/test_optimizer_handler.py
+-rw-r--r--   0 bartz      (501) staff       (20)      900 2023-11-12 15:19:14.000000 spotPython-0.9.9/test/test_pkldataset.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.9.9/test/test_repair_non_numeric.py
+-rw-r--r--   0 bartz      (501) staff       (20)      506 2023-12-31 18:16:20.000000 spotPython-0.9.9/test/test_selectNew().py
+-rw-r--r--   0 bartz      (501) staff       (20)     1337 2024-01-02 10:36:40.000000 spotPython-0.9.9/test/test_set_data_module.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4904 2023-12-29 16:24:39.000000 spotPython-0.9.9/test/test_set_de_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.9.9/test/test_show_progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1107 2024-01-01 15:59:04.000000 spotPython-0.9.9/test/test_suggest_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1374 2023-11-15 21:55:41.000000 spotPython-0.9.9/test/test_testmodel.py
+-rw-r--r--   0 bartz      (501) staff       (20)      996 2024-01-03 21:45:15.000000 spotPython-0.9.9/test/test_to_red.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1365 2023-11-15 21:55:41.000000 spotPython-0.9.9/test/test_trainmodel.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3568 2024-01-02 22:13:10.000000 spotPython-0.9.9/test/test_update_design.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3524 2024-01-03 21:08:41.000000 spotPython-0.9.9/test/test_update_stats.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.9.9/test/test_update_surrogate.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2449 2024-01-04 22:34:15.000000 spotPython-0.9.9/test/test_values.py
+-rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 10:19:58.000000 spotPython-0.9.9/tox.ini
```

### Comparing `spotPython-0.9.8/.github/workflows/test.yml` & `spotPython-0.9.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/.gitignore` & `spotPython-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf` & `spotPython-0.9.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf` & `spotPython-0.9.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf` & `spotPython-0.9.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf` & `spotPython-0.9.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf` & `spotPython-0.9.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf` & `spotPython-0.9.9/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/LICENSE.txt` & `spotPython-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/PKG-INFO` & `spotPython-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.9.8
+Version: 0.9.9
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.9.8/README.md` & `spotPython-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/docs/about.md` & `spotPython-0.9.9/docs/about.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/docs/examples.md` & `spotPython-0.9.9/docs/examples.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/docs/gen_ref_pages.py` & `spotPython-0.9.9/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/docs/images/favicon.png` & `spotPython-0.9.9/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/docs/images/spotlogo.png` & `spotPython-0.9.9/docs/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/img/favicon.png` & `spotPython-0.9.9/img/favicon.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/img/spotLogo.png` & `spotPython-0.9.9/img/spotLogo.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/mkdocs.yml` & `spotPython-0.9.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/00_spotPython_tests.ipynb` & `spotPython-0.9.9/notebooks/00_spotPython_tests.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb` & `spotPython-0.9.9/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/31_spot_lightning_csv.ipynb` & `spotPython-0.9.9/notebooks/31_spot_lightning_csv.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/data/spotPython/data.csv` & `spotPython-0.9.9/notebooks/data/spotPython/data.csv`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/data/spotPython/data.pkl` & `spotPython-0.9.9/notebooks/data/spotPython/data.pkl`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/data/torch/model_spot_trained.pt` & `spotPython-0.9.9/notebooks/data/torch/model_spot_trained.pt`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/12-torch_p040025_1min_5init_2023-06-07_19-09-30_contour_0_1.png` & `spotPython-0.9.9/notebooks/figures/12-torch_p040025_1min_5init_2023-06-07_19-09-30_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_contour_0_1.png` & `spotPython-0.9.9/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_importance.png` & `spotPython-0.9.9/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_progress.png` & `spotPython-0.9.9/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_contour_0_1.png` & `spotPython-0.9.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_progress.png` & `spotPython-0.9.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_01.png` & `spotPython-0.9.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_01.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_02.png` & `spotPython-0.9.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_02.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_importance.png` & `spotPython-0.9.9/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_progress.png` & `spotPython-0.9.9/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png` & `spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png` & `spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png` & `spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png` & `spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png` & `spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png` & `spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png` & `spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png` & `spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png` & `spotPython-0.9.9/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_contour_0_3.png` & `spotPython-0.9.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_contour_0_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_importance.png` & `spotPython-0.9.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_parallel.png` & `spotPython-0.9.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_progress.png` & `spotPython-0.9.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/spotModel.graffle` & `spotPython-0.9.9/notebooks/figures/spotModel.graffle`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/spotModel.pdf` & `spotPython-0.9.9/notebooks/figures/spotModel.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/spotModel.png` & `spotPython-0.9.9/notebooks/figures/spotModel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/tensorboard_0.png` & `spotPython-0.9.9/notebooks/figures/tensorboard_0.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/tensorboard_1.png` & `spotPython-0.9.9/notebooks/figures/tensorboard_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/tensorboard_hdparams.png` & `spotPython-0.9.9/notebooks/figures/tensorboard_hdparams.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/figures/tensorboard_parallel.png` & `spotPython-0.9.9/notebooks/figures/tensorboard_parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/hyperdict/user_hyper_dict.json` & `spotPython-0.9.9/notebooks/hyperdict/user_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/notebooks/testKriging.ipynb` & `spotPython-0.9.9/notebooks/testKriging.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/pyproject.toml` & `spotPython-0.9.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "setuptools_scm[toml]"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotPython"
-version = "0.9.8"
+version = "0.9.9"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotPython - Sequential Parameter Optimization in Python"
 readme = "README.md"
 license = { text="AGPL-3.0-or-later" }
 requires-python = ">=3.10"
```

### Comparing `spotPython-0.9.8/src/spotPython/budget/ocba.py` & `spotPython-0.9.9/src/spotPython/budget/ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/build/kriging.py` & `spotPython-0.9.9/src/spotPython/build/kriging.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/data/base.py` & `spotPython-0.9.9/src/spotPython/data/base.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/data/csvdataset.py` & `spotPython-0.9.9/src/spotPython/data/csvdataset.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/data/data.csv` & `spotPython-0.9.9/src/spotPython/data/data.csv`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/data/data.pkl` & `spotPython-0.9.9/src/spotPython/data/data.pkl`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/data/diabetes.py` & `spotPython-0.9.9/src/spotPython/data/diabetes.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/data/lightcrossvalidationdatamodule.py` & `spotPython-0.9.9/src/spotPython/data/lightcrossvalidationdatamodule.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/data/lightdatamodule.py` & `spotPython-0.9.9/src/spotPython/data/lightdatamodule.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/data/mnistdatamodule.py` & `spotPython-0.9.9/src/spotPython/data/mnistdatamodule.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/data/pkldataset.py` & `spotPython-0.9.9/src/spotPython/data/pkldataset.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/data/torchdata.py` & `spotPython-0.9.9/src/spotPython/data/torchdata.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/data/vbdp.py` & `spotPython-0.9.9/src/spotPython/data/vbdp.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/design/designs.py` & `spotPython-0.9.9/src/spotPython/design/designs.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/design/factorial.py` & `spotPython-0.9.9/src/spotPython/design/factorial.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/design/spacefilling.py` & `spotPython-0.9.9/src/spotPython/design/spacefilling.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/fun/hyperlight.py` & `spotPython-0.9.9/src/spotPython/fun/hyperlight.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/fun/hypersklearn.py` & `spotPython-0.9.9/src/spotPython/fun/hypersklearn.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/fun/hypertorch.py` & `spotPython-0.9.9/src/spotPython/fun/hypertorch.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/fun/objectivefunctions.py` & `spotPython-0.9.9/src/spotPython/fun/objectivefunctions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/hyperdict/light_hyper_dict.py` & `spotPython-0.9.9/src/spotPython/hyperdict/light_hyper_dict.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/hyperdict/sklearn_hyper_dict.json` & `spotPython-0.9.9/src/spotPython/hyperdict/sklearn_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/hyperdict/sklearn_hyper_dict.py` & `spotPython-0.9.9/src/spotPython/hyperdict/sklearn_hyper_dict.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/hyperdict/torch_hyper_dict.json` & `spotPython-0.9.9/src/spotPython/hyperdict/torch_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/hyperdict/torch_hyper_dict.py` & `spotPython-0.9.9/src/spotPython/hyperdict/torch_hyper_dict.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/hyperparameters/categorical.py` & `spotPython-0.9.9/src/spotPython/hyperparameters/categorical.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/hyperparameters/optimizer.py` & `spotPython-0.9.9/src/spotPython/hyperparameters/optimizer.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/hyperparameters/values.py` & `spotPython-0.9.9/src/spotPython/hyperparameters/values.py`

 * *Files 2% similar despite different names*

```diff
@@ -1018,70 +1018,70 @@
     Returns:
         (object):
             model object.
     """
     return fun_control["core_model"](**config, **kwargs)
 
 
-def set_control_key_value(fun_control, key, value, replace=False) -> None:
+def set_control_key_value(control_dict, key, value, replace=False) -> None:
     """
-    This function sets the key value pair in the fun_control dictionary.
+    This function sets the key value pair in the control_dict dictionary.
 
     Args:
-        fun_control (dict):
-            fun_control dictionary
+        control_dict (dict):
+            control_dict dictionary
         key (str): key
         value (Any): value
         replace (bool): replace value if key already exists. Default is False.
 
     Returns:
         None.
 
     Attributes:
         key (str): key
         value (Any): value
 
     Examples:
         >>> from spotPython.utils.init import fun_control_init
             from spotPython.hyperparameters.values import set_control_key_value
-            fun_control = fun_control_init()
-            set_control_key_value(fun_control=fun_control,
+            control_dict = fun_control_init()
+            set_control_key_value(control_dict=control_dict,
                           key="key",
                           value="value")
-            fun_control["key"]
+            control_dict["key"]
 
     """
     if replace:
-        fun_control.update({key: value})
+        control_dict.update({key: value})
     else:
-        if key not in fun_control.keys():
-            fun_control.update({key: value})
+        if key not in control_dict.keys():
+            control_dict.update({key: value})
 
 
-def get_control_key_value(fun_control=None, key=None) -> Any:
+def get_control_key_value(control_dict=None, key=None) -> Any:
     """
-    This function gets the key value pair from the fun_control dictionary.
+    This function gets the key value pair from the control_dict dictionary.
     If the key does not exist, return None.
-    If the fun_control dictionary is None, return None.
+    If the control_dict dictionary is None, return None.
 
     Args:
-        fun_control (dict):
-            fun_control dictionary
+        control_dict (dict):
+            control_dict dictionary
         key (str): key
 
     Returns:
         value (Any):
             value
 
     Examples:
         >>> from spotPython.utils.init import fun_control_init
             from spotPython.hyperparameters.values import get_control_key_value
-            fun_control = fun_control_init()
-            get_control_key_value(fun_control=fun_control,
+            control_dict = fun_control_init()
+            get_control_key_value(control_dict=control_dict,
                             key="key")
             "value"
     """
-    # check if key exists in fun_control:
-    if fun_control is None or key not in fun_control.keys():
+    # check if key exists in control_dict:
+    if control_dict is None or key not in control_dict.keys():
         return None
     else:
-        return fun_control[key]
+        return control_dict[key]
```

### Comparing `spotPython-0.9.8/src/spotPython/light/cifar10/cifar10datamodule.py` & `spotPython-0.9.9/src/spotPython/light/cifar10/cifar10datamodule.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/light/classification/netlightbasemapk.py` & `spotPython-0.9.9/src/spotPython/light/classification/netlightbasemapk.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/light/cnn/googlenet.py` & `spotPython-0.9.9/src/spotPython/light/cnn/googlenet.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/light/cnn/inceptionblock.py` & `spotPython-0.9.9/src/spotPython/light/cnn/inceptionblock.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/light/cnn/netcnnbase.py` & `spotPython-0.9.9/src/spotPython/light/cnn/netcnnbase.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/light/cvmodel.py` & `spotPython-0.9.9/src/spotPython/light/cvmodel.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/light/litmodel.py` & `spotPython-0.9.9/src/spotPython/light/litmodel.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/light/loadmodel.py` & `spotPython-0.9.9/src/spotPython/light/loadmodel.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/light/regression/netlightregression.py` & `spotPython-0.9.9/src/spotPython/light/regression/netlightregression.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/light/testmodel.py` & `spotPython-0.9.9/src/spotPython/light/testmodel.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/light/trainmodel.py` & `spotPython-0.9.9/src/spotPython/light/trainmodel.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/plot/contour.py` & `spotPython-0.9.9/src/spotPython/plot/contour.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/plot/validation.py` & `spotPython-0.9.9/src/spotPython/plot/validation.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/sklearn/traintest.py` & `spotPython-0.9.9/src/spotPython/sklearn/traintest.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/spot/spot.py` & `spotPython-0.9.9/src/spotPython/spot/spot.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,16 +236,16 @@
         self.fun_control = fun_control
 
         # set fun_control["sigma"] to sigma if "sigma" is not in fun_control dictionary
         # If no fun_control is provided, the fun_control dictionary is initialized with the
         # key "sigma" and the value sigma amd the key "seed" and the value seed.
         # This is a mimimum requirement for the fun_control dictionary to call
         # objective functions from the spotPython.fun.objectivefunctions module.
-        set_control_key_value(fun_control=self.fun_control, key="sigma", value=sigma)
-        set_control_key_value(fun_control=self.fun_control, key="seed", value=seed)
+        set_control_key_value(control_dict=self.fun_control, key="sigma", value=sigma)
+        set_control_key_value(control_dict=self.fun_control, key="seed", value=seed)
         # Random number generator:
         self.rng = default_rng(self.fun_control["seed"])
 
         # 2. lower attribute updates:
         # -----------------------
         # if lower is in the fun_control dictionary, use the value of the key "lower" as the lower bound
         # else use the lower bound lower
@@ -396,16 +396,16 @@
         Args:
             self (object): the object whose attribute is to be set
             attribute (str): the attribute to set
             value (Any): the value to set the attribute to
             dict (dict): the dictionary to check for the key
         """
         setattr(self, attribute, value)
-        if get_control_key_value(fun_control=dict, key=attribute) is not None:
-            setattr(self, attribute, get_control_key_value(fun_control=dict, key=attribute))
+        if get_control_key_value(control_dict=dict, key=attribute) is not None:
+            setattr(self, attribute, get_control_key_value(control_dict=dict, key=attribute))
 
     def get_spot_attributes_as_df(self) -> pd.DataFrame:
         """Get all attributes of the spot object as a pandas dataframe.
 
         Returns:
             (pandas.DataFrame): dataframe with all attributes of the spot object.
```

### Comparing `spotPython-0.9.8/src/spotPython/torch/activation.py` & `spotPython-0.9.9/src/spotPython/torch/activation.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/torch/dataframedataset.py` & `spotPython-0.9.9/src/spotPython/torch/dataframedataset.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/torch/initialization.py` & `spotPython-0.9.9/src/spotPython/torch/initialization.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/torch/mapk.py` & `spotPython-0.9.9/src/spotPython/torch/mapk.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/torch/netcifar10.py` & `spotPython-0.9.9/src/spotPython/torch/netcifar10.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/torch/netfashionMNIST.py` & `spotPython-0.9.9/src/spotPython/torch/netfashionMNIST.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/torch/netregression.py` & `spotPython-0.9.9/src/spotPython/torch/netregression.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/torch/netvbdp.py` & `spotPython-0.9.9/src/spotPython/torch/netvbdp.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/torch/traintest.py` & `spotPython-0.9.9/src/spotPython/torch/traintest.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/utils/aggregate.py` & `spotPython-0.9.9/src/spotPython/utils/aggregate.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/utils/compare.py` & `spotPython-0.9.9/src/spotPython/utils/compare.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/utils/convert.py` & `spotPython-0.9.9/src/spotPython/utils/convert.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/utils/device.py` & `spotPython-0.9.9/src/spotPython/utils/device.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/utils/eda.py` & `spotPython-0.9.9/src/spotPython/utils/eda.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/utils/file.py` & `spotPython-0.9.9/src/spotPython/utils/file.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/utils/init.py` & `spotPython-0.9.9/src/spotPython/utils/init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/utils/metrics.py` & `spotPython-0.9.9/src/spotPython/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/utils/progress.py` & `spotPython-0.9.9/src/spotPython/utils/progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/utils/repair.py` & `spotPython-0.9.9/src/spotPython/utils/repair.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/utils/tensorboard.py` & `spotPython-0.9.9/src/spotPython/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython/utils/transform.py` & `spotPython-0.9.9/src/spotPython/utils/transform.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/src/spotPython.egg-info/PKG-INFO` & `spotPython-0.9.9/src/spotPython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.9.8
+Version: 0.9.9
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.9.8/src/spotPython.egg-info/SOURCES.txt` & `spotPython-0.9.9/src/spotPython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_add_core_model_to_fun_control.py` & `spotPython-0.9.9/test/test_add_core_model_to_fun_control.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_aggregate_mean_var.py` & `spotPython-0.9.9/test/test_aggregate_mean_var.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_branin.py` & `spotPython-0.9.9/test/test_branin.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_build_Psi.py` & `spotPython-0.9.9/test/test_build_Psi.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_build_U.py` & `spotPython-0.9.9/test/test_build_U.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_build_psi_vec.py` & `spotPython-0.9.9/test/test_build_psi_vec.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_check_X_shape.py` & `spotPython-0.9.9/test/test_check_X_shape.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_chg.py` & `spotPython-0.9.9/test/test_chg.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_csvdataset.py` & `spotPython-0.9.9/test/test_csvdataset.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_evaluate_new_X.py` & `spotPython-0.9.9/test/test_evaluate_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_evaluate_new_solutions.py` & `spotPython-0.9.9/test/test_evaluate_new_solutions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_extract_from_bounds.py` & `spotPython-0.9.9/test/test_extract_from_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_fit_surrogate.py` & `spotPython-0.9.9/test/test_fit_surrogate.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_fun_control_init.py` & `spotPython-0.9.9/test/test_fun_control_init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_generate_design.py` & `spotPython-0.9.9/test/test_generate_design.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_get_new_X0.py` & `spotPython-0.9.9/test/test_get_new_X0.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_get_var_name.py` & `spotPython-0.9.9/test/test_get_var_name.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_hyper_light_fun.py` & `spotPython-0.9.9/test/test_hyper_light_fun.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_infill.py` & `spotPython-0.9.9/test/test_infill.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_initialize_design.py` & `spotPython-0.9.9/test/test_initialize_design.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_kriging.py` & `spotPython-0.9.9/test/test_kriging.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_lightdatamodule.py` & `spotPython-0.9.9/test/test_lightdatamodule.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_nat_to_cod.py` & `spotPython-0.9.9/test/test_nat_to_cod.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_net_light_regression_class.py` & `spotPython-0.9.9/test/test_net_light_regression_class.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_ocba.py` & `spotPython-0.9.9/test/test_ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_optimizer_handler.py` & `spotPython-0.9.9/test/test_optimizer_handler.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_pkldataset.py` & `spotPython-0.9.9/test/test_pkldataset.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_repair_non_numeric.py` & `spotPython-0.9.9/test/test_repair_non_numeric.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_set_data_module.py` & `spotPython-0.9.9/test/test_set_data_module.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_set_de_bounds.py` & `spotPython-0.9.9/test/test_set_de_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_show_progress.py` & `spotPython-0.9.9/test/test_show_progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_suggest_new_X.py` & `spotPython-0.9.9/test/test_suggest_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_testmodel.py` & `spotPython-0.9.9/test/test_testmodel.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_to_red.py` & `spotPython-0.9.9/test/test_to_red.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_trainmodel.py` & `spotPython-0.9.9/test/test_trainmodel.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_update_design.py` & `spotPython-0.9.9/test/test_update_design.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_update_stats.py` & `spotPython-0.9.9/test/test_update_stats.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_update_surrogate.py` & `spotPython-0.9.9/test/test_update_surrogate.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.9.8/test/test_values.py` & `spotPython-0.9.9/test/test_values.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,35 +29,35 @@
         get_bound_values(fun_control, "invalid", as_list=True)
 
 
 def test_set_control_key_value():
     fun_control = fun_control_init()
 
     # Test when key is not in fun_control and replace is False
-    set_control_key_value(fun_control, "key1", "value1")
+    set_control_key_value(control_dict=fun_control, key="key1", value="value1")
     assert fun_control["key1"] == "value1"
 
     # Test when key is in fun_control and replace is False
-    set_control_key_value(fun_control, "key1", "value2")
+    set_control_key_value(control_dict=fun_control, key="key1", value="value2")
     assert fun_control["key1"] == "value1"
 
     # Test when key is in fun_control and replace is True
-    set_control_key_value(fun_control, "key1", "value2", replace=True)
+    set_control_key_value(control_dict=fun_control, key="key1", value="value2", replace=True)
     assert fun_control["key1"] == "value2"
 
     # Test when key is not in fun_control and replace is True
-    set_control_key_value(fun_control, "key2", "value3", replace=True)
+    set_control_key_value(control_dict=fun_control, key="key2", value="value3", replace=True)
     assert fun_control["key2"] == "value3"
 
 def test_get_control_key_value():
     fun_control = fun_control_init()
 
     # Test when key is not in fun_control
-    assert get_control_key_value(fun_control, "key1") is None
+    assert get_control_key_value(control_dict=fun_control, key="key1") is None
 
     # Test when fun_control is None
     assert get_control_key_value() is None
 
     # Test when key is in fun_control
-    set_control_key_value(fun_control, "key1", "value1")
-    assert get_control_key_value(fun_control, "key1") == "value1"
+    set_control_key_value(control_dict=fun_control, key="key1", value="value1")
+    assert get_control_key_value(control_dict=fun_control, key="key1") == "value1"
```

