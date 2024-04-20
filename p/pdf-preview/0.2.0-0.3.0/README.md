# Comparing `tmp/pdf_preview-0.2.0.tar.gz` & `tmp/pdf_preview-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_preview-0.2.0.tar", max compression
+gzip compressed data, was "pdf_preview-0.3.0.tar", max compression
```

## Comparing `pdf_preview-0.2.0.tar` & `pdf_preview-0.3.0.tar`

### file list

```diff
@@ -1,411 +1,411 @@
--rw-r--r--   0        0        0       23 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/__init__.py
--rw-r--r--   0        0        0     2045 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/__main__.py
--rw-r--r--   0        0        0    21943 2024-03-03 06:45:47.000000 pdf_preview-0.2.0/pdf_preview/main_window.py
--rw-r--r--   0        0        0   756276 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/build/pdf.js
--rw-r--r--   0        0        0  1207855 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/build/pdf.js.map
--rw-r--r--   0        0        0  1707645 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/build/pdf.worker.js
--rw-r--r--   0        0        0  3133372 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/build/pdf.worker.js.map
--rw-r--r--   0        0        0    10351 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/LICENSE
--rw-r--r--   0        0        0     2404 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/78-EUC-H.bcmap
--rw-r--r--   0        0        0      173 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/78-EUC-V.bcmap
--rw-r--r--   0        0        0     2379 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/78-H.bcmap
--rw-r--r--   0        0        0     2398 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/78-RKSJ-H.bcmap
--rw-r--r--   0        0        0      173 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/78-RKSJ-V.bcmap
--rw-r--r--   0        0        0      169 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/78-V.bcmap
--rw-r--r--   0        0        0     2651 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/78ms-RKSJ-H.bcmap
--rw-r--r--   0        0        0      290 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/78ms-RKSJ-V.bcmap
--rw-r--r--   0        0        0      905 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/83pv-RKSJ-H.bcmap
--rw-r--r--   0        0        0      721 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/90ms-RKSJ-H.bcmap
--rw-r--r--   0        0        0      290 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/90ms-RKSJ-V.bcmap
--rw-r--r--   0        0        0      715 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/90msp-RKSJ-H.bcmap
--rw-r--r--   0        0        0      291 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/90msp-RKSJ-V.bcmap
--rw-r--r--   0        0        0      982 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/90pv-RKSJ-H.bcmap
--rw-r--r--   0        0        0      260 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/90pv-RKSJ-V.bcmap
--rw-r--r--   0        0        0     2419 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Add-H.bcmap
--rw-r--r--   0        0        0     2413 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Add-RKSJ-H.bcmap
--rw-r--r--   0        0        0      287 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Add-RKSJ-V.bcmap
--rw-r--r--   0        0        0      282 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Add-V.bcmap
--rw-r--r--   0        0        0      317 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-0.bcmap
--rw-r--r--   0        0        0      371 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-1.bcmap
--rw-r--r--   0        0        0      376 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-2.bcmap
--rw-r--r--   0        0        0      401 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-3.bcmap
--rw-r--r--   0        0        0      405 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-4.bcmap
--rw-r--r--   0        0        0      406 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-5.bcmap
--rw-r--r--   0        0        0      406 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-6.bcmap
--rw-r--r--   0        0        0    41193 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-UCS2.bcmap
--rw-r--r--   0        0        0      217 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-0.bcmap
--rw-r--r--   0        0        0      250 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-1.bcmap
--rw-r--r--   0        0        0      465 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-2.bcmap
--rw-r--r--   0        0        0      470 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-3.bcmap
--rw-r--r--   0        0        0      601 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-4.bcmap
--rw-r--r--   0        0        0      625 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-5.bcmap
--rw-r--r--   0        0        0    33974 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-UCS2.bcmap
--rw-r--r--   0        0        0      225 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-0.bcmap
--rw-r--r--   0        0        0      226 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-1.bcmap
--rw-r--r--   0        0        0      233 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-2.bcmap
--rw-r--r--   0        0        0      242 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-3.bcmap
--rw-r--r--   0        0        0      337 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-4.bcmap
--rw-r--r--   0        0        0      430 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-5.bcmap
--rw-r--r--   0        0        0      485 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-6.bcmap
--rw-r--r--   0        0        0    40951 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-UCS2.bcmap
--rw-r--r--   0        0        0      241 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Korea1-0.bcmap
--rw-r--r--   0        0        0      386 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Korea1-1.bcmap
--rw-r--r--   0        0        0      391 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Korea1-2.bcmap
--rw-r--r--   0        0        0    23293 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Korea1-UCS2.bcmap
--rw-r--r--   0        0        0     1086 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/B5-H.bcmap
--rw-r--r--   0        0        0      142 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/B5-V.bcmap
--rw-r--r--   0        0        0     1099 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/B5pc-H.bcmap
--rw-r--r--   0        0        0      144 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/B5pc-V.bcmap
--rw-r--r--   0        0        0     1780 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/CNS-EUC-H.bcmap
--rw-r--r--   0        0        0     1920 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/CNS-EUC-V.bcmap
--rw-r--r--   0        0        0      706 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/CNS1-H.bcmap
--rw-r--r--   0        0        0      143 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/CNS1-V.bcmap
--rw-r--r--   0        0        0      504 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/CNS2-H.bcmap
--rw-r--r--   0        0        0       93 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/CNS2-V.bcmap
--rw-r--r--   0        0        0     1125 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/ETen-B5-H.bcmap
--rw-r--r--   0        0        0      158 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/ETen-B5-V.bcmap
--rw-r--r--   0        0        0      101 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/ETenms-B5-H.bcmap
--rw-r--r--   0        0        0      172 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/ETenms-B5-V.bcmap
--rw-r--r--   0        0        0     4426 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/ETHK-B5-H.bcmap
--rw-r--r--   0        0        0      158 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/ETHK-B5-V.bcmap
--rw-r--r--   0        0        0      578 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/EUC-H.bcmap
--rw-r--r--   0        0        0      170 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/EUC-V.bcmap
--rw-r--r--   0        0        0     2536 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Ext-H.bcmap
--rw-r--r--   0        0        0     2542 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Ext-RKSJ-H.bcmap
--rw-r--r--   0        0        0      218 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Ext-RKSJ-V.bcmap
--rw-r--r--   0        0        0      215 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Ext-V.bcmap
--rw-r--r--   0        0        0      549 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GB-EUC-H.bcmap
--rw-r--r--   0        0        0      179 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GB-EUC-V.bcmap
--rw-r--r--   0        0        0      528 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GB-H.bcmap
--rw-r--r--   0        0        0      175 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GB-V.bcmap
--rw-r--r--   0        0        0    14692 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBK-EUC-H.bcmap
--rw-r--r--   0        0        0      180 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBK-EUC-V.bcmap
--rw-r--r--   0        0        0    19662 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBK2K-H.bcmap
--rw-r--r--   0        0        0      219 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBK2K-V.bcmap
--rw-r--r--   0        0        0    14686 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBKp-EUC-H.bcmap
--rw-r--r--   0        0        0      181 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBKp-EUC-V.bcmap
--rw-r--r--   0        0        0      557 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBpc-EUC-H.bcmap
--rw-r--r--   0        0        0      181 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBpc-EUC-V.bcmap
--rw-r--r--   0        0        0     7290 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBT-EUC-H.bcmap
--rw-r--r--   0        0        0      180 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBT-EUC-V.bcmap
--rw-r--r--   0        0        0     7269 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBT-H.bcmap
--rw-r--r--   0        0        0      176 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBT-V.bcmap
--rw-r--r--   0        0        0     7298 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBTpc-EUC-H.bcmap
--rw-r--r--   0        0        0      182 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBTpc-EUC-V.bcmap
--rw-r--r--   0        0        0      553 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/H.bcmap
--rw-r--r--   0        0        0      132 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Hankaku.bcmap
--rw-r--r--   0        0        0      124 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Hiragana.bcmap
--rw-r--r--   0        0        0     2654 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKdla-B5-H.bcmap
--rw-r--r--   0        0        0      148 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKdla-B5-V.bcmap
--rw-r--r--   0        0        0     2414 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKdlb-B5-H.bcmap
--rw-r--r--   0        0        0      148 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKdlb-B5-V.bcmap
--rw-r--r--   0        0        0     2292 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKgccs-B5-H.bcmap
--rw-r--r--   0        0        0      149 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKgccs-B5-V.bcmap
--rw-r--r--   0        0        0     1772 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKm314-B5-H.bcmap
--rw-r--r--   0        0        0      149 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKm314-B5-V.bcmap
--rw-r--r--   0        0        0     2171 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKm471-B5-H.bcmap
--rw-r--r--   0        0        0      149 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKm471-B5-V.bcmap
--rw-r--r--   0        0        0     4437 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKscs-B5-H.bcmap
--rw-r--r--   0        0        0      159 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKscs-B5-V.bcmap
--rw-r--r--   0        0        0      100 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Katakana.bcmap
--rw-r--r--   0        0        0     1848 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-EUC-H.bcmap
--rw-r--r--   0        0        0      164 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-EUC-V.bcmap
--rw-r--r--   0        0        0     1831 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-H.bcmap
--rw-r--r--   0        0        0    16791 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-Johab-H.bcmap
--rw-r--r--   0        0        0      166 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-Johab-V.bcmap
--rw-r--r--   0        0        0      160 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-V.bcmap
--rw-r--r--   0        0        0     2787 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSCms-UHC-H.bcmap
--rw-r--r--   0        0        0     2789 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSCms-UHC-HW-H.bcmap
--rw-r--r--   0        0        0      169 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSCms-UHC-HW-V.bcmap
--rw-r--r--   0        0        0      166 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSCms-UHC-V.bcmap
--rw-r--r--   0        0        0     2024 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSCpc-EUC-H.bcmap
--rw-r--r--   0        0        0      166 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSCpc-EUC-V.bcmap
--rw-r--r--   0        0        0     2116 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/LICENSE
--rw-r--r--   0        0        0     2765 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/NWP-H.bcmap
--rw-r--r--   0        0        0      252 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/NWP-V.bcmap
--rw-r--r--   0        0        0      534 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/RKSJ-H.bcmap
--rw-r--r--   0        0        0      170 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/RKSJ-V.bcmap
--rw-r--r--   0        0        0       96 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Roman.bcmap
--rw-r--r--   0        0        0    48280 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UCS2-H.bcmap
--rw-r--r--   0        0        0      156 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UCS2-V.bcmap
--rw-r--r--   0        0        0    50419 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF16-H.bcmap
--rw-r--r--   0        0        0      156 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF16-V.bcmap
--rw-r--r--   0        0        0    52679 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF32-H.bcmap
--rw-r--r--   0        0        0      160 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF32-V.bcmap
--rw-r--r--   0        0        0    53629 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF8-H.bcmap
--rw-r--r--   0        0        0      157 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF8-V.bcmap
--rw-r--r--   0        0        0    43366 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UCS2-H.bcmap
--rw-r--r--   0        0        0      193 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UCS2-V.bcmap
--rw-r--r--   0        0        0    44086 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF16-H.bcmap
--rw-r--r--   0        0        0      178 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF16-V.bcmap
--rw-r--r--   0        0        0    45738 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF32-H.bcmap
--rw-r--r--   0        0        0      182 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF32-V.bcmap
--rw-r--r--   0        0        0    46837 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF8-H.bcmap
--rw-r--r--   0        0        0      181 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF8-V.bcmap
--rw-r--r--   0        0        0    25439 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-H.bcmap
--rw-r--r--   0        0        0      119 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-HW-H.bcmap
--rw-r--r--   0        0        0      680 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-HW-V.bcmap
--rw-r--r--   0        0        0      664 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-V.bcmap
--rw-r--r--   0        0        0    39443 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF16-H.bcmap
--rw-r--r--   0        0        0      643 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF16-V.bcmap
--rw-r--r--   0        0        0    40539 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF32-H.bcmap
--rw-r--r--   0        0        0      677 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF32-V.bcmap
--rw-r--r--   0        0        0    41695 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF8-H.bcmap
--rw-r--r--   0        0        0      678 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF8-V.bcmap
--rw-r--r--   0        0        0    39534 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF16-H.bcmap
--rw-r--r--   0        0        0      647 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF16-V.bcmap
--rw-r--r--   0        0        0    40630 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF32-H.bcmap
--rw-r--r--   0        0        0      681 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF32-V.bcmap
--rw-r--r--   0        0        0    41779 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF8-H.bcmap
--rw-r--r--   0        0        0      682 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF8-V.bcmap
--rw-r--r--   0        0        0      705 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISPro-UCS2-HW-V.bcmap
--rw-r--r--   0        0        0      689 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISPro-UCS2-V.bcmap
--rw-r--r--   0        0        0      726 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISPro-UTF8-V.bcmap
--rw-r--r--   0        0        0    40517 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX0213-UTF32-H.bcmap
--rw-r--r--   0        0        0      684 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX0213-UTF32-V.bcmap
--rw-r--r--   0        0        0    40608 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX02132004-UTF32-H.bcmap
--rw-r--r--   0        0        0      688 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX02132004-UTF32-V.bcmap
--rw-r--r--   0        0        0    25783 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UCS2-H.bcmap
--rw-r--r--   0        0        0      178 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UCS2-V.bcmap
--rw-r--r--   0        0        0    26327 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF16-H.bcmap
--rw-r--r--   0        0        0      164 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF16-V.bcmap
--rw-r--r--   0        0        0    26451 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF32-H.bcmap
--rw-r--r--   0        0        0      168 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF32-V.bcmap
--rw-r--r--   0        0        0    27790 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF8-H.bcmap
--rw-r--r--   0        0        0      169 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF8-V.bcmap
--rw-r--r--   0        0        0      166 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/V.bcmap
--rw-r--r--   0        0        0      179 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/WP-Symbol.bcmap
--rw-r--r--   0        0        0  1016315 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/compressed.tracemonkey-pldi-09.pdf
--rw-r--r--   0        0        0    19722 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/debugger.js
--rw-r--r--   0        0        0      426 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-check.svg
--rw-r--r--   0        0        0      899 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-comment.svg
--rw-r--r--   0        0        0     2194 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-help.svg
--rw-r--r--   0        0        0      418 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-insert.svg
--rw-r--r--   0        0        0     1463 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-key.svg
--rw-r--r--   0        0        0      437 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-newparagraph.svg
--rw-r--r--   0        0        0      165 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-noicon.svg
--rw-r--r--   0        0        0     1083 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-note.svg
--rw-r--r--   0        0        0     1159 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-paragraph.svg
--rw-r--r--   0        0        0      199 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/findbarButton-next-rtl.png
--rw-r--r--   0        0        0      304 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/findbarButton-next-rtl@2x.png
--rw-r--r--   0        0        0      193 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/findbarButton-next.png
--rw-r--r--   0        0        0      296 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/findbarButton-next@2x.png
--rw-r--r--   0        0        0      193 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/findbarButton-previous-rtl.png
--rw-r--r--   0        0        0      296 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/findbarButton-previous-rtl@2x.png
--rw-r--r--   0        0        0      199 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/findbarButton-previous.png
--rw-r--r--   0        0        0      304 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/findbarButton-previous@2x.png
--rw-r--r--   0        0        0      326 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/grab.cur
--rw-r--r--   0        0        0      326 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/grabbing.cur
--rw-r--r--   0        0        0     2545 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/loading-icon.gif
--rw-r--r--   0        0        0     7402 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/loading-small.png
--rw-r--r--   0        0        0    16131 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/loading-small@2x.png
--rw-r--r--   0        0        0      403 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-documentProperties.png
--rw-r--r--   0        0        0      933 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-documentProperties@2x.png
--rw-r--r--   0        0        0      179 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-firstPage.png
--rw-r--r--   0        0        0      266 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-firstPage@2x.png
--rw-r--r--   0        0        0      301 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-handTool.png
--rw-r--r--   0        0        0      583 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-handTool@2x.png
--rw-r--r--   0        0        0      175 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-lastPage.png
--rw-r--r--   0        0        0      276 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-lastPage@2x.png
--rw-r--r--   0        0        0      360 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-rotateCcw.png
--rw-r--r--   0        0        0      731 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-rotateCcw@2x.png
--rw-r--r--   0        0        0      359 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-rotateCw.png
--rw-r--r--   0        0        0      714 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-rotateCw@2x.png
--rw-r--r--   0        0        0      218 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-scrollHorizontal.png
--rw-r--r--   0        0        0      332 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-scrollHorizontal@2x.png
--rw-r--r--   0        0        0      228 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-scrollVertical.png
--rw-r--r--   0        0        0      349 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-scrollVertical@2x.png
--rw-r--r--   0        0        0      297 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-scrollWrapped.png
--rw-r--r--   0        0        0      490 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-scrollWrapped@2x.png
--rw-r--r--   0        0        0      461 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-selectTool.png
--rw-r--r--   0        0        0     1067 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-selectTool@2x.png
--rw-r--r--   0        0        0      347 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadEven.png
--rw-r--r--   0        0        0      694 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadEven@2x.png
--rw-r--r--   0        0        0      179 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadNone.png
--rw-r--r--   0        0        0      261 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadNone@2x.png
--rw-r--r--   0        0        0      344 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadOdd.png
--rw-r--r--   0        0        0      621 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadOdd@2x.png
--rw-r--r--   0        0        0      290 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/shadow.png
--rw-r--r--   0        0        0     2417 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/texture.png
--rw-r--r--   0        0        0      174 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-bookmark.png
--rw-r--r--   0        0        0      260 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-bookmark@2x.png
--rw-r--r--   0        0        0      259 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-download.png
--rw-r--r--   0        0        0      425 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-download@2x.png
--rw-r--r--   0        0        0      107 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-menuArrows.png
--rw-r--r--   0        0        0      152 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-menuArrows@2x.png
--rw-r--r--   0        0        0      295 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-openFile.png
--rw-r--r--   0        0        0      550 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-openFile@2x.png
--rw-r--r--   0        0        0      242 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageDown-rtl.png
--rw-r--r--   0        0        0      398 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageDown-rtl@2x.png
--rw-r--r--   0        0        0      238 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageDown.png
--rw-r--r--   0        0        0      396 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageDown@2x.png
--rw-r--r--   0        0        0      245 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageUp-rtl.png
--rw-r--r--   0        0        0      405 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageUp-rtl@2x.png
--rw-r--r--   0        0        0      246 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageUp.png
--rw-r--r--   0        0        0      403 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageUp@2x.png
--rw-r--r--   0        0        0      321 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-presentationMode.png
--rw-r--r--   0        0        0      586 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-presentationMode@2x.png
--rw-r--r--   0        0        0      257 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-print.png
--rw-r--r--   0        0        0      464 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-print@2x.png
--rw-r--r--   0        0        0      309 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-search.png
--rw-r--r--   0        0        0      653 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-search@2x.png
--rw-r--r--   0        0        0      246 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-secondaryToolbarToggle-rtl.png
--rw-r--r--   0        0        0      456 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-secondaryToolbarToggle-rtl@2x.png
--rw-r--r--   0        0        0      243 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-secondaryToolbarToggle.png
--rw-r--r--   0        0        0      458 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-secondaryToolbarToggle@2x.png
--rw-r--r--   0        0        0      225 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-sidebarToggle-rtl.png
--rw-r--r--   0        0        0      344 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-sidebarToggle-rtl@2x.png
--rw-r--r--   0        0        0      225 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-sidebarToggle.png
--rw-r--r--   0        0        0      331 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-sidebarToggle@2x.png
--rw-r--r--   0        0        0      384 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewAttachments.png
--rw-r--r--   0        0        0      859 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewAttachments@2x.png
--rw-r--r--   0        0        0      177 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewOutline-rtl.png
--rw-r--r--   0        0        0      394 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewOutline-rtl@2x.png
--rw-r--r--   0        0        0      178 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewOutline.png
--rw-r--r--   0        0        0      331 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewOutline@2x.png
--rw-r--r--   0        0        0      185 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewThumbnail.png
--rw-r--r--   0        0        0      219 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewThumbnail@2x.png
--rw-r--r--   0        0        0      136 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-zoomIn.png
--rw-r--r--   0        0        0      160 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-zoomIn@2x.png
--rw-r--r--   0        0        0       88 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-zoomOut.png
--rw-r--r--   0        0        0      109 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-zoomOut@2x.png
--rw-r--r--   0        0        0      143 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/treeitem-collapsed-rtl.png
--rw-r--r--   0        0        0      167 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/treeitem-collapsed-rtl@2x.png
--rw-r--r--   0        0        0      128 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/treeitem-collapsed.png
--rw-r--r--   0        0        0      149 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/treeitem-collapsed@2x.png
--rw-r--r--   0        0        0      125 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/treeitem-expanded.png
--rw-r--r--   0        0        0      172 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/treeitem-expanded@2x.png
--rw-r--r--   0        0        0     9055 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ach/viewer.properties
--rw-r--r--   0        0        0     7911 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/af/viewer.properties
--rw-r--r--   0        0        0     5634 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ak/viewer.properties
--rw-r--r--   0        0        0     8269 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/an/viewer.properties
--rw-r--r--   0        0        0    13055 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ar/viewer.properties
--rw-r--r--   0        0        0    10143 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/as/viewer.properties
--rw-r--r--   0        0        0     9379 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ast/viewer.properties
--rw-r--r--   0        0        0    11748 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/az/viewer.properties
--rw-r--r--   0        0        0    14218 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/be/viewer.properties
--rw-r--r--   0        0        0    14401 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/bg/viewer.properties
--rw-r--r--   0        0        0    14592 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/bn-BD/viewer.properties
--rw-r--r--   0        0        0    16295 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/bn-IN/viewer.properties
--rw-r--r--   0        0        0    12044 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/br/viewer.properties
--rw-r--r--   0        0        0    10333 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/brx/viewer.properties
--rw-r--r--   0        0        0     9300 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/bs/viewer.properties
--rw-r--r--   0        0        0    11423 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ca/viewer.properties
--rw-r--r--   0        0        0    12120 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/cak/viewer.properties
--rw-r--r--   0        0        0    11558 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/crh/viewer.properties
--rw-r--r--   0        0        0    11830 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/cs/viewer.properties
--rw-r--r--   0        0        0     4966 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/csb/viewer.properties
--rw-r--r--   0        0        0    11475 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/cy/viewer.properties
--rw-r--r--   0        0        0    11426 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/da/viewer.properties
--rw-r--r--   0        0        0    12040 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/de/viewer.properties
--rw-r--r--   0        0        0    14732 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/el/viewer.properties
--rw-r--r--   0        0        0    11208 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/en-CA/viewer.properties
--rw-r--r--   0        0        0    11208 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/en-GB/viewer.properties
--rw-r--r--   0        0        0    11212 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/en-US/viewer.properties
--rw-r--r--   0        0        0     7147 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/en-ZA/viewer.properties
--rw-r--r--   0        0        0    11597 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/eo/viewer.properties
--rw-r--r--   0        0        0    11724 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/es-AR/viewer.properties
--rw-r--r--   0        0        0    11929 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/es-CL/viewer.properties
--rw-r--r--   0        0        0    11957 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/es-ES/viewer.properties
--rw-r--r--   0        0        0    11676 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/es-MX/viewer.properties
--rw-r--r--   0        0        0    11518 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/et/viewer.properties
--rw-r--r--   0        0        0    11813 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/eu/viewer.properties
--rw-r--r--   0        0        0    11908 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/fa/viewer.properties
--rw-r--r--   0        0        0    11204 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ff/viewer.properties
--rw-r--r--   0        0        0    11672 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/fi/viewer.properties
--rw-r--r--   0        0        0    12160 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/fr/viewer.properties
--rw-r--r--   0        0        0    11524 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/fy-NL/viewer.properties
--rw-r--r--   0        0        0     8400 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ga-IE/viewer.properties
--rw-r--r--   0        0        0    12038 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/gd/viewer.properties
--rw-r--r--   0        0        0    11827 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/gl/viewer.properties
--rw-r--r--   0        0        0    11835 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/gn/viewer.properties
--rw-r--r--   0        0        0    15686 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/gu-IN/viewer.properties
--rw-r--r--   0        0        0    12596 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/he/viewer.properties
--rw-r--r--   0        0        0    14265 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/hi-IN/viewer.properties
--rw-r--r--   0        0        0    11763 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/hr/viewer.properties
--rw-r--r--   0        0        0    11921 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/hsb/viewer.properties
--rw-r--r--   0        0        0     5309 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/hto/viewer.properties
--rw-r--r--   0        0        0    12115 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/hu/viewer.properties
--rw-r--r--   0        0        0    11156 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/hy-AM/viewer.properties
--rw-r--r--   0        0        0    11903 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ia/viewer.properties
--rw-r--r--   0        0        0    11573 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/id/viewer.properties
--rw-r--r--   0        0        0    11160 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/is/viewer.properties
--rw-r--r--   0        0        0     8068 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/it/viewer.properties
--rw-r--r--   0        0        0    12561 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ja/viewer.properties
--rw-r--r--   0        0        0    16502 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ka/viewer.properties
--rw-r--r--   0        0        0    11636 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/kab/viewer.properties
--rw-r--r--   0        0        0    14053 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/kk/viewer.properties
--rw-r--r--   0        0        0    12013 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/km/viewer.properties
--rw-r--r--   0        0        0    12304 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/kn/viewer.properties
--rw-r--r--   0        0        0    11902 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ko/viewer.properties
--rw-r--r--   0        0        0     9740 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/kok/viewer.properties
--rw-r--r--   0        0        0     8714 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ks/viewer.properties
--rw-r--r--   0        0        0     6471 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ku/viewer.properties
--rw-r--r--   0        0        0     4622 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/lg/viewer.properties
--rw-r--r--   0        0        0    11638 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/lij/viewer.properties
--rw-r--r--   0        0        0     8030 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/lo/viewer.properties
--rw-r--r--   0        0        0     5479 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/locale.properties
--rw-r--r--   0        0        0    11977 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/lt/viewer.properties
--rw-r--r--   0        0        0    10139 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ltg/viewer.properties
--rw-r--r--   0        0        0    11527 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/lv/viewer.properties
--rw-r--r--   0        0        0     9615 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/mai/viewer.properties
--rw-r--r--   0        0        0     3212 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/meh/viewer.properties
--rw-r--r--   0        0        0     7846 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/mk/viewer.properties
--rw-r--r--   0        0        0    13681 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ml/viewer.properties
--rw-r--r--   0        0        0     3639 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/mn/viewer.properties
--rw-r--r--   0        0        0    14314 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/mr/viewer.properties
--rw-r--r--   0        0        0    11313 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ms/viewer.properties
--rw-r--r--   0        0        0    12957 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/my/viewer.properties
--rw-r--r--   0        0        0    11298 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/nb-NO/viewer.properties
--rw-r--r--   0        0        0    11875 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ne-NP/viewer.properties
--rw-r--r--   0        0        0    11771 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/nl/viewer.properties
--rw-r--r--   0        0        0    11266 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/nn-NO/viewer.properties
--rw-r--r--   0        0        0     5740 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/nso/viewer.properties
--rw-r--r--   0        0        0     9965 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/oc/viewer.properties
--rw-r--r--   0        0        0    10564 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/or/viewer.properties
--rw-r--r--   0        0        0    13990 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/pa-IN/viewer.properties
--rw-r--r--   0        0        0    12085 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/pl/viewer.properties
--rw-r--r--   0        0        0    11873 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/pt-BR/viewer.properties
--rw-r--r--   0        0        0    11907 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/pt-PT/viewer.properties
--rw-r--r--   0        0        0    11912 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/rm/viewer.properties
--rw-r--r--   0        0        0    12063 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ro/viewer.properties
--rw-r--r--   0        0        0    14314 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ru/viewer.properties
--rw-r--r--   0        0        0     3569 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/rw/viewer.properties
--rw-r--r--   0        0        0     8567 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sah/viewer.properties
--rw-r--r--   0        0        0     8480 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sat/viewer.properties
--rw-r--r--   0        0        0    12191 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/si/viewer.properties
--rw-r--r--   0        0        0    12063 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sk/viewer.properties
--rw-r--r--   0        0        0    11569 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sl/viewer.properties
--rw-r--r--   0        0        0     7625 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/son/viewer.properties
--rw-r--r--   0        0        0    11559 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sq/viewer.properties
--rw-r--r--   0        0        0    12456 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sr/viewer.properties
--rw-r--r--   0        0        0    11319 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sv-SE/viewer.properties
--rw-r--r--   0        0        0     5396 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sw/viewer.properties
--rw-r--r--   0        0        0    13674 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ta/viewer.properties
--rw-r--r--   0        0        0     3572 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ta-LK/viewer.properties
--rw-r--r--   0        0        0    13758 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/te/viewer.properties
--rw-r--r--   0        0        0    15330 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/th/viewer.properties
--rw-r--r--   0        0        0    11305 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/tl/viewer.properties
--rw-r--r--   0        0        0     3713 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/tn/viewer.properties
--rw-r--r--   0        0        0    11694 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/tr/viewer.properties
--rw-r--r--   0        0        0     3288 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/tsz/viewer.properties
--rw-r--r--   0        0        0    14147 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/uk/viewer.properties
--rw-r--r--   0        0        0    10695 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ur/viewer.properties
--rw-r--r--   0        0        0     7509 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/uz/viewer.properties
--rw-r--r--   0        0        0    12223 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/vi/viewer.properties
--rw-r--r--   0        0        0     5037 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/wo/viewer.properties
--rw-r--r--   0        0        0     8376 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/xh/viewer.properties
--rw-r--r--   0        0        0     3786 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/zam/viewer.properties
--rw-r--r--   0        0        0    11148 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/zh-CN/viewer.properties
--rw-r--r--   0        0        0    11208 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/zh-TW/viewer.properties
--rw-r--r--   0        0        0     5803 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/zu/viewer.properties
--rw-r--r--   0        0        0  9316700 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/testtext2.pdf
--rw-r--r--   0        0        0    61862 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/viewer.css
--rw-r--r--   0        0        0    22080 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/viewer.html
--rw-r--r--   0        0        0   490689 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/viewer.js
--rw-r--r--   0        0        0   749301 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/viewer.js.map
--rw-r--r--   0        0        0     7309 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/saveAsPDF.py
--rw-r--r--   0        0        0      549 2024-03-03 05:43:33.000000 pdf_preview-0.2.0/pdf_preview/util.py
--rw-r--r--   0        0        0      578 2024-03-30 06:50:43.593259 pdf_preview-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      647 2024-03-03 07:12:58.000000 pdf_preview-0.2.0/README.rst
--rw-r--r--   0        0        0     1145 1970-01-01 00:00:00.000000 pdf_preview-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-20 17:07:08.957487 pdf_preview-0.3.0/pdf_preview/__init__.py
+-rw-r--r--   0        0        0     2045 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/__main__.py
+-rw-r--r--   0        0        0    21383 2024-04-20 17:04:25.584277 pdf_preview-0.3.0/pdf_preview/main_window.py
+-rw-r--r--   0        0        0   756276 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/build/pdf.js
+-rw-r--r--   0        0        0  1207855 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/build/pdf.js.map
+-rw-r--r--   0        0        0  1707645 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/build/pdf.worker.js
+-rw-r--r--   0        0        0  3133372 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/build/pdf.worker.js.map
+-rw-r--r--   0        0        0    10351 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/LICENSE
+-rw-r--r--   0        0        0     2404 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/78-EUC-H.bcmap
+-rw-r--r--   0        0        0      173 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/78-EUC-V.bcmap
+-rw-r--r--   0        0        0     2379 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/78-H.bcmap
+-rw-r--r--   0        0        0     2398 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/78-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      173 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/78-RKSJ-V.bcmap
+-rw-r--r--   0        0        0      169 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/78-V.bcmap
+-rw-r--r--   0        0        0     2651 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/78ms-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      290 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/78ms-RKSJ-V.bcmap
+-rw-r--r--   0        0        0      905 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/83pv-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      721 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/90ms-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      290 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/90ms-RKSJ-V.bcmap
+-rw-r--r--   0        0        0      715 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/90msp-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      291 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/90msp-RKSJ-V.bcmap
+-rw-r--r--   0        0        0      982 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/90pv-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      260 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/90pv-RKSJ-V.bcmap
+-rw-r--r--   0        0        0     2419 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Add-H.bcmap
+-rw-r--r--   0        0        0     2413 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Add-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      287 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Add-RKSJ-V.bcmap
+-rw-r--r--   0        0        0      282 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Add-V.bcmap
+-rw-r--r--   0        0        0      317 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-0.bcmap
+-rw-r--r--   0        0        0      371 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-1.bcmap
+-rw-r--r--   0        0        0      376 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-2.bcmap
+-rw-r--r--   0        0        0      401 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-3.bcmap
+-rw-r--r--   0        0        0      405 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-4.bcmap
+-rw-r--r--   0        0        0      406 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-5.bcmap
+-rw-r--r--   0        0        0      406 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-6.bcmap
+-rw-r--r--   0        0        0    41193 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-UCS2.bcmap
+-rw-r--r--   0        0        0      217 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-0.bcmap
+-rw-r--r--   0        0        0      250 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-1.bcmap
+-rw-r--r--   0        0        0      465 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-2.bcmap
+-rw-r--r--   0        0        0      470 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-3.bcmap
+-rw-r--r--   0        0        0      601 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-4.bcmap
+-rw-r--r--   0        0        0      625 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-5.bcmap
+-rw-r--r--   0        0        0    33974 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-UCS2.bcmap
+-rw-r--r--   0        0        0      225 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-0.bcmap
+-rw-r--r--   0        0        0      226 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-1.bcmap
+-rw-r--r--   0        0        0      233 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-2.bcmap
+-rw-r--r--   0        0        0      242 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-3.bcmap
+-rw-r--r--   0        0        0      337 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-4.bcmap
+-rw-r--r--   0        0        0      430 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-5.bcmap
+-rw-r--r--   0        0        0      485 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-6.bcmap
+-rw-r--r--   0        0        0    40951 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-UCS2.bcmap
+-rw-r--r--   0        0        0      241 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Korea1-0.bcmap
+-rw-r--r--   0        0        0      386 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Korea1-1.bcmap
+-rw-r--r--   0        0        0      391 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Korea1-2.bcmap
+-rw-r--r--   0        0        0    23293 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Korea1-UCS2.bcmap
+-rw-r--r--   0        0        0     1086 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/B5-H.bcmap
+-rw-r--r--   0        0        0      142 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/B5-V.bcmap
+-rw-r--r--   0        0        0     1099 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/B5pc-H.bcmap
+-rw-r--r--   0        0        0      144 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/B5pc-V.bcmap
+-rw-r--r--   0        0        0     1780 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/CNS-EUC-H.bcmap
+-rw-r--r--   0        0        0     1920 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/CNS-EUC-V.bcmap
+-rw-r--r--   0        0        0      706 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/CNS1-H.bcmap
+-rw-r--r--   0        0        0      143 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/CNS1-V.bcmap
+-rw-r--r--   0        0        0      504 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/CNS2-H.bcmap
+-rw-r--r--   0        0        0       93 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/CNS2-V.bcmap
+-rw-r--r--   0        0        0     1125 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/ETen-B5-H.bcmap
+-rw-r--r--   0        0        0      158 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/ETen-B5-V.bcmap
+-rw-r--r--   0        0        0      101 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/ETenms-B5-H.bcmap
+-rw-r--r--   0        0        0      172 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/ETenms-B5-V.bcmap
+-rw-r--r--   0        0        0     4426 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/ETHK-B5-H.bcmap
+-rw-r--r--   0        0        0      158 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/ETHK-B5-V.bcmap
+-rw-r--r--   0        0        0      578 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/EUC-H.bcmap
+-rw-r--r--   0        0        0      170 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/EUC-V.bcmap
+-rw-r--r--   0        0        0     2536 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Ext-H.bcmap
+-rw-r--r--   0        0        0     2542 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Ext-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      218 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Ext-RKSJ-V.bcmap
+-rw-r--r--   0        0        0      215 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Ext-V.bcmap
+-rw-r--r--   0        0        0      549 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GB-EUC-H.bcmap
+-rw-r--r--   0        0        0      179 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GB-EUC-V.bcmap
+-rw-r--r--   0        0        0      528 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GB-H.bcmap
+-rw-r--r--   0        0        0      175 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GB-V.bcmap
+-rw-r--r--   0        0        0    14692 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBK-EUC-H.bcmap
+-rw-r--r--   0        0        0      180 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBK-EUC-V.bcmap
+-rw-r--r--   0        0        0    19662 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBK2K-H.bcmap
+-rw-r--r--   0        0        0      219 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBK2K-V.bcmap
+-rw-r--r--   0        0        0    14686 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBKp-EUC-H.bcmap
+-rw-r--r--   0        0        0      181 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBKp-EUC-V.bcmap
+-rw-r--r--   0        0        0      557 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBpc-EUC-H.bcmap
+-rw-r--r--   0        0        0      181 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBpc-EUC-V.bcmap
+-rw-r--r--   0        0        0     7290 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBT-EUC-H.bcmap
+-rw-r--r--   0        0        0      180 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBT-EUC-V.bcmap
+-rw-r--r--   0        0        0     7269 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBT-H.bcmap
+-rw-r--r--   0        0        0      176 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBT-V.bcmap
+-rw-r--r--   0        0        0     7298 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBTpc-EUC-H.bcmap
+-rw-r--r--   0        0        0      182 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBTpc-EUC-V.bcmap
+-rw-r--r--   0        0        0      553 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/H.bcmap
+-rw-r--r--   0        0        0      132 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Hankaku.bcmap
+-rw-r--r--   0        0        0      124 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Hiragana.bcmap
+-rw-r--r--   0        0        0     2654 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKdla-B5-H.bcmap
+-rw-r--r--   0        0        0      148 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKdla-B5-V.bcmap
+-rw-r--r--   0        0        0     2414 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKdlb-B5-H.bcmap
+-rw-r--r--   0        0        0      148 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKdlb-B5-V.bcmap
+-rw-r--r--   0        0        0     2292 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKgccs-B5-H.bcmap
+-rw-r--r--   0        0        0      149 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKgccs-B5-V.bcmap
+-rw-r--r--   0        0        0     1772 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKm314-B5-H.bcmap
+-rw-r--r--   0        0        0      149 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKm314-B5-V.bcmap
+-rw-r--r--   0        0        0     2171 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKm471-B5-H.bcmap
+-rw-r--r--   0        0        0      149 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKm471-B5-V.bcmap
+-rw-r--r--   0        0        0     4437 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKscs-B5-H.bcmap
+-rw-r--r--   0        0        0      159 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKscs-B5-V.bcmap
+-rw-r--r--   0        0        0      100 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Katakana.bcmap
+-rw-r--r--   0        0        0     1848 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-EUC-H.bcmap
+-rw-r--r--   0        0        0      164 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-EUC-V.bcmap
+-rw-r--r--   0        0        0     1831 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-H.bcmap
+-rw-r--r--   0        0        0    16791 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-Johab-H.bcmap
+-rw-r--r--   0        0        0      166 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-Johab-V.bcmap
+-rw-r--r--   0        0        0      160 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-V.bcmap
+-rw-r--r--   0        0        0     2787 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSCms-UHC-H.bcmap
+-rw-r--r--   0        0        0     2789 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSCms-UHC-HW-H.bcmap
+-rw-r--r--   0        0        0      169 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSCms-UHC-HW-V.bcmap
+-rw-r--r--   0        0        0      166 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSCms-UHC-V.bcmap
+-rw-r--r--   0        0        0     2024 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSCpc-EUC-H.bcmap
+-rw-r--r--   0        0        0      166 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSCpc-EUC-V.bcmap
+-rw-r--r--   0        0        0     2116 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/LICENSE
+-rw-r--r--   0        0        0     2765 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/NWP-H.bcmap
+-rw-r--r--   0        0        0      252 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/NWP-V.bcmap
+-rw-r--r--   0        0        0      534 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/RKSJ-H.bcmap
+-rw-r--r--   0        0        0      170 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/RKSJ-V.bcmap
+-rw-r--r--   0        0        0       96 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Roman.bcmap
+-rw-r--r--   0        0        0    48280 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UCS2-H.bcmap
+-rw-r--r--   0        0        0      156 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UCS2-V.bcmap
+-rw-r--r--   0        0        0    50419 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF16-H.bcmap
+-rw-r--r--   0        0        0      156 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF16-V.bcmap
+-rw-r--r--   0        0        0    52679 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF32-H.bcmap
+-rw-r--r--   0        0        0      160 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF32-V.bcmap
+-rw-r--r--   0        0        0    53629 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF8-H.bcmap
+-rw-r--r--   0        0        0      157 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF8-V.bcmap
+-rw-r--r--   0        0        0    43366 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UCS2-H.bcmap
+-rw-r--r--   0        0        0      193 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UCS2-V.bcmap
+-rw-r--r--   0        0        0    44086 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF16-H.bcmap
+-rw-r--r--   0        0        0      178 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF16-V.bcmap
+-rw-r--r--   0        0        0    45738 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF32-H.bcmap
+-rw-r--r--   0        0        0      182 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF32-V.bcmap
+-rw-r--r--   0        0        0    46837 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF8-H.bcmap
+-rw-r--r--   0        0        0      181 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF8-V.bcmap
+-rw-r--r--   0        0        0    25439 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-H.bcmap
+-rw-r--r--   0        0        0      119 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-HW-H.bcmap
+-rw-r--r--   0        0        0      680 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-HW-V.bcmap
+-rw-r--r--   0        0        0      664 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-V.bcmap
+-rw-r--r--   0        0        0    39443 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF16-H.bcmap
+-rw-r--r--   0        0        0      643 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF16-V.bcmap
+-rw-r--r--   0        0        0    40539 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF32-H.bcmap
+-rw-r--r--   0        0        0      677 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF32-V.bcmap
+-rw-r--r--   0        0        0    41695 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF8-H.bcmap
+-rw-r--r--   0        0        0      678 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF8-V.bcmap
+-rw-r--r--   0        0        0    39534 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF16-H.bcmap
+-rw-r--r--   0        0        0      647 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF16-V.bcmap
+-rw-r--r--   0        0        0    40630 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF32-H.bcmap
+-rw-r--r--   0        0        0      681 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF32-V.bcmap
+-rw-r--r--   0        0        0    41779 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF8-H.bcmap
+-rw-r--r--   0        0        0      682 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF8-V.bcmap
+-rw-r--r--   0        0        0      705 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISPro-UCS2-HW-V.bcmap
+-rw-r--r--   0        0        0      689 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISPro-UCS2-V.bcmap
+-rw-r--r--   0        0        0      726 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISPro-UTF8-V.bcmap
+-rw-r--r--   0        0        0    40517 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX0213-UTF32-H.bcmap
+-rw-r--r--   0        0        0      684 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX0213-UTF32-V.bcmap
+-rw-r--r--   0        0        0    40608 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX02132004-UTF32-H.bcmap
+-rw-r--r--   0        0        0      688 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX02132004-UTF32-V.bcmap
+-rw-r--r--   0        0        0    25783 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UCS2-H.bcmap
+-rw-r--r--   0        0        0      178 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UCS2-V.bcmap
+-rw-r--r--   0        0        0    26327 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF16-H.bcmap
+-rw-r--r--   0        0        0      164 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF16-V.bcmap
+-rw-r--r--   0        0        0    26451 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF32-H.bcmap
+-rw-r--r--   0        0        0      168 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF32-V.bcmap
+-rw-r--r--   0        0        0    27790 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF8-H.bcmap
+-rw-r--r--   0        0        0      169 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF8-V.bcmap
+-rw-r--r--   0        0        0      166 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/V.bcmap
+-rw-r--r--   0        0        0      179 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/WP-Symbol.bcmap
+-rw-r--r--   0        0        0  1016315 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/compressed.tracemonkey-pldi-09.pdf
+-rw-r--r--   0        0        0    19722 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/debugger.js
+-rw-r--r--   0        0        0      426 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-check.svg
+-rw-r--r--   0        0        0      899 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-comment.svg
+-rw-r--r--   0        0        0     2194 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-help.svg
+-rw-r--r--   0        0        0      418 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-insert.svg
+-rw-r--r--   0        0        0     1463 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-key.svg
+-rw-r--r--   0        0        0      437 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-newparagraph.svg
+-rw-r--r--   0        0        0      165 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-noicon.svg
+-rw-r--r--   0        0        0     1083 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-note.svg
+-rw-r--r--   0        0        0     1159 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-paragraph.svg
+-rw-r--r--   0        0        0      199 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/findbarButton-next-rtl.png
+-rw-r--r--   0        0        0      304 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/findbarButton-next-rtl@2x.png
+-rw-r--r--   0        0        0      193 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/findbarButton-next.png
+-rw-r--r--   0        0        0      296 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/findbarButton-next@2x.png
+-rw-r--r--   0        0        0      193 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/findbarButton-previous-rtl.png
+-rw-r--r--   0        0        0      296 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/findbarButton-previous-rtl@2x.png
+-rw-r--r--   0        0        0      199 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/findbarButton-previous.png
+-rw-r--r--   0        0        0      304 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/findbarButton-previous@2x.png
+-rw-r--r--   0        0        0      326 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/grab.cur
+-rw-r--r--   0        0        0      326 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/grabbing.cur
+-rw-r--r--   0        0        0     2545 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/loading-icon.gif
+-rw-r--r--   0        0        0     7402 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/loading-small.png
+-rw-r--r--   0        0        0    16131 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/loading-small@2x.png
+-rw-r--r--   0        0        0      403 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-documentProperties.png
+-rw-r--r--   0        0        0      933 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-documentProperties@2x.png
+-rw-r--r--   0        0        0      179 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-firstPage.png
+-rw-r--r--   0        0        0      266 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-firstPage@2x.png
+-rw-r--r--   0        0        0      301 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-handTool.png
+-rw-r--r--   0        0        0      583 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-handTool@2x.png
+-rw-r--r--   0        0        0      175 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-lastPage.png
+-rw-r--r--   0        0        0      276 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-lastPage@2x.png
+-rw-r--r--   0        0        0      360 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-rotateCcw.png
+-rw-r--r--   0        0        0      731 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-rotateCcw@2x.png
+-rw-r--r--   0        0        0      359 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-rotateCw.png
+-rw-r--r--   0        0        0      714 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-rotateCw@2x.png
+-rw-r--r--   0        0        0      218 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-scrollHorizontal.png
+-rw-r--r--   0        0        0      332 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-scrollHorizontal@2x.png
+-rw-r--r--   0        0        0      228 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-scrollVertical.png
+-rw-r--r--   0        0        0      349 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-scrollVertical@2x.png
+-rw-r--r--   0        0        0      297 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-scrollWrapped.png
+-rw-r--r--   0        0        0      490 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-scrollWrapped@2x.png
+-rw-r--r--   0        0        0      461 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-selectTool.png
+-rw-r--r--   0        0        0     1067 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-selectTool@2x.png
+-rw-r--r--   0        0        0      347 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadEven.png
+-rw-r--r--   0        0        0      694 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadEven@2x.png
+-rw-r--r--   0        0        0      179 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadNone.png
+-rw-r--r--   0        0        0      261 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadNone@2x.png
+-rw-r--r--   0        0        0      344 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadOdd.png
+-rw-r--r--   0        0        0      621 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadOdd@2x.png
+-rw-r--r--   0        0        0      290 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/shadow.png
+-rw-r--r--   0        0        0     2417 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/texture.png
+-rw-r--r--   0        0        0      174 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-bookmark.png
+-rw-r--r--   0        0        0      260 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-bookmark@2x.png
+-rw-r--r--   0        0        0      259 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-download.png
+-rw-r--r--   0        0        0      425 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-download@2x.png
+-rw-r--r--   0        0        0      107 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-menuArrows.png
+-rw-r--r--   0        0        0      152 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-menuArrows@2x.png
+-rw-r--r--   0        0        0      295 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-openFile.png
+-rw-r--r--   0        0        0      550 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-openFile@2x.png
+-rw-r--r--   0        0        0      242 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageDown-rtl.png
+-rw-r--r--   0        0        0      398 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageDown-rtl@2x.png
+-rw-r--r--   0        0        0      238 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageDown.png
+-rw-r--r--   0        0        0      396 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageDown@2x.png
+-rw-r--r--   0        0        0      245 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageUp-rtl.png
+-rw-r--r--   0        0        0      405 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageUp-rtl@2x.png
+-rw-r--r--   0        0        0      246 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageUp.png
+-rw-r--r--   0        0        0      403 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-pageUp@2x.png
+-rw-r--r--   0        0        0      321 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-presentationMode.png
+-rw-r--r--   0        0        0      586 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-presentationMode@2x.png
+-rw-r--r--   0        0        0      257 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-print.png
+-rw-r--r--   0        0        0      464 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-print@2x.png
+-rw-r--r--   0        0        0      309 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-search.png
+-rw-r--r--   0        0        0      653 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-search@2x.png
+-rw-r--r--   0        0        0      246 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-secondaryToolbarToggle-rtl.png
+-rw-r--r--   0        0        0      456 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-secondaryToolbarToggle-rtl@2x.png
+-rw-r--r--   0        0        0      243 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-secondaryToolbarToggle.png
+-rw-r--r--   0        0        0      458 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-secondaryToolbarToggle@2x.png
+-rw-r--r--   0        0        0      225 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-sidebarToggle-rtl.png
+-rw-r--r--   0        0        0      344 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-sidebarToggle-rtl@2x.png
+-rw-r--r--   0        0        0      225 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-sidebarToggle.png
+-rw-r--r--   0        0        0      331 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-sidebarToggle@2x.png
+-rw-r--r--   0        0        0      384 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewAttachments.png
+-rw-r--r--   0        0        0      859 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewAttachments@2x.png
+-rw-r--r--   0        0        0      177 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewOutline-rtl.png
+-rw-r--r--   0        0        0      394 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewOutline-rtl@2x.png
+-rw-r--r--   0        0        0      178 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewOutline.png
+-rw-r--r--   0        0        0      331 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewOutline@2x.png
+-rw-r--r--   0        0        0      185 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewThumbnail.png
+-rw-r--r--   0        0        0      219 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewThumbnail@2x.png
+-rw-r--r--   0        0        0      136 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-zoomIn.png
+-rw-r--r--   0        0        0      160 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-zoomIn@2x.png
+-rw-r--r--   0        0        0       88 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-zoomOut.png
+-rw-r--r--   0        0        0      109 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-zoomOut@2x.png
+-rw-r--r--   0        0        0      143 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/treeitem-collapsed-rtl.png
+-rw-r--r--   0        0        0      167 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/treeitem-collapsed-rtl@2x.png
+-rw-r--r--   0        0        0      128 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/treeitem-collapsed.png
+-rw-r--r--   0        0        0      149 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/treeitem-collapsed@2x.png
+-rw-r--r--   0        0        0      125 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/treeitem-expanded.png
+-rw-r--r--   0        0        0      172 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/treeitem-expanded@2x.png
+-rw-r--r--   0        0        0     9055 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ach/viewer.properties
+-rw-r--r--   0        0        0     7911 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/af/viewer.properties
+-rw-r--r--   0        0        0     5634 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ak/viewer.properties
+-rw-r--r--   0        0        0     8269 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/an/viewer.properties
+-rw-r--r--   0        0        0    13055 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ar/viewer.properties
+-rw-r--r--   0        0        0    10143 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/as/viewer.properties
+-rw-r--r--   0        0        0     9379 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ast/viewer.properties
+-rw-r--r--   0        0        0    11748 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/az/viewer.properties
+-rw-r--r--   0        0        0    14218 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/be/viewer.properties
+-rw-r--r--   0        0        0    14401 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/bg/viewer.properties
+-rw-r--r--   0        0        0    14592 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/bn-BD/viewer.properties
+-rw-r--r--   0        0        0    16295 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/bn-IN/viewer.properties
+-rw-r--r--   0        0        0    12044 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/br/viewer.properties
+-rw-r--r--   0        0        0    10333 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/brx/viewer.properties
+-rw-r--r--   0        0        0     9300 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/bs/viewer.properties
+-rw-r--r--   0        0        0    11423 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ca/viewer.properties
+-rw-r--r--   0        0        0    12120 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/cak/viewer.properties
+-rw-r--r--   0        0        0    11558 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/crh/viewer.properties
+-rw-r--r--   0        0        0    11830 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/cs/viewer.properties
+-rw-r--r--   0        0        0     4966 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/csb/viewer.properties
+-rw-r--r--   0        0        0    11475 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/cy/viewer.properties
+-rw-r--r--   0        0        0    11426 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/da/viewer.properties
+-rw-r--r--   0        0        0    12040 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/de/viewer.properties
+-rw-r--r--   0        0        0    14732 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/el/viewer.properties
+-rw-r--r--   0        0        0    11208 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/en-CA/viewer.properties
+-rw-r--r--   0        0        0    11208 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/en-GB/viewer.properties
+-rw-r--r--   0        0        0    11212 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/en-US/viewer.properties
+-rw-r--r--   0        0        0     7147 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/en-ZA/viewer.properties
+-rw-r--r--   0        0        0    11597 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/eo/viewer.properties
+-rw-r--r--   0        0        0    11724 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/es-AR/viewer.properties
+-rw-r--r--   0        0        0    11929 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/es-CL/viewer.properties
+-rw-r--r--   0        0        0    11957 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/es-ES/viewer.properties
+-rw-r--r--   0        0        0    11676 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/es-MX/viewer.properties
+-rw-r--r--   0        0        0    11518 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/et/viewer.properties
+-rw-r--r--   0        0        0    11813 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/eu/viewer.properties
+-rw-r--r--   0        0        0    11908 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/fa/viewer.properties
+-rw-r--r--   0        0        0    11204 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ff/viewer.properties
+-rw-r--r--   0        0        0    11672 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/fi/viewer.properties
+-rw-r--r--   0        0        0    12160 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/fr/viewer.properties
+-rw-r--r--   0        0        0    11524 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/fy-NL/viewer.properties
+-rw-r--r--   0        0        0     8400 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ga-IE/viewer.properties
+-rw-r--r--   0        0        0    12038 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/gd/viewer.properties
+-rw-r--r--   0        0        0    11827 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/gl/viewer.properties
+-rw-r--r--   0        0        0    11835 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/gn/viewer.properties
+-rw-r--r--   0        0        0    15686 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/gu-IN/viewer.properties
+-rw-r--r--   0        0        0    12596 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/he/viewer.properties
+-rw-r--r--   0        0        0    14265 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/hi-IN/viewer.properties
+-rw-r--r--   0        0        0    11763 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/hr/viewer.properties
+-rw-r--r--   0        0        0    11921 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/hsb/viewer.properties
+-rw-r--r--   0        0        0     5309 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/hto/viewer.properties
+-rw-r--r--   0        0        0    12115 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/hu/viewer.properties
+-rw-r--r--   0        0        0    11156 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/hy-AM/viewer.properties
+-rw-r--r--   0        0        0    11903 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ia/viewer.properties
+-rw-r--r--   0        0        0    11573 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/id/viewer.properties
+-rw-r--r--   0        0        0    11160 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/is/viewer.properties
+-rw-r--r--   0        0        0     8068 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/it/viewer.properties
+-rw-r--r--   0        0        0    12561 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ja/viewer.properties
+-rw-r--r--   0        0        0    16502 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ka/viewer.properties
+-rw-r--r--   0        0        0    11636 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/kab/viewer.properties
+-rw-r--r--   0        0        0    14053 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/kk/viewer.properties
+-rw-r--r--   0        0        0    12013 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/km/viewer.properties
+-rw-r--r--   0        0        0    12304 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/kn/viewer.properties
+-rw-r--r--   0        0        0    11902 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ko/viewer.properties
+-rw-r--r--   0        0        0     9740 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/kok/viewer.properties
+-rw-r--r--   0        0        0     8714 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ks/viewer.properties
+-rw-r--r--   0        0        0     6471 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ku/viewer.properties
+-rw-r--r--   0        0        0     4622 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/lg/viewer.properties
+-rw-r--r--   0        0        0    11638 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/lij/viewer.properties
+-rw-r--r--   0        0        0     8030 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/lo/viewer.properties
+-rw-r--r--   0        0        0     5479 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/locale.properties
+-rw-r--r--   0        0        0    11977 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/lt/viewer.properties
+-rw-r--r--   0        0        0    10139 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ltg/viewer.properties
+-rw-r--r--   0        0        0    11527 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/lv/viewer.properties
+-rw-r--r--   0        0        0     9615 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/mai/viewer.properties
+-rw-r--r--   0        0        0     3212 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/meh/viewer.properties
+-rw-r--r--   0        0        0     7846 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/mk/viewer.properties
+-rw-r--r--   0        0        0    13681 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ml/viewer.properties
+-rw-r--r--   0        0        0     3639 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/mn/viewer.properties
+-rw-r--r--   0        0        0    14314 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/mr/viewer.properties
+-rw-r--r--   0        0        0    11313 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ms/viewer.properties
+-rw-r--r--   0        0        0    12957 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/my/viewer.properties
+-rw-r--r--   0        0        0    11298 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/nb-NO/viewer.properties
+-rw-r--r--   0        0        0    11875 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ne-NP/viewer.properties
+-rw-r--r--   0        0        0    11771 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/nl/viewer.properties
+-rw-r--r--   0        0        0    11266 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/nn-NO/viewer.properties
+-rw-r--r--   0        0        0     5740 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/nso/viewer.properties
+-rw-r--r--   0        0        0     9965 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/oc/viewer.properties
+-rw-r--r--   0        0        0    10564 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/or/viewer.properties
+-rw-r--r--   0        0        0    13990 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/pa-IN/viewer.properties
+-rw-r--r--   0        0        0    12085 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/pl/viewer.properties
+-rw-r--r--   0        0        0    11873 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/pt-BR/viewer.properties
+-rw-r--r--   0        0        0    11907 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/pt-PT/viewer.properties
+-rw-r--r--   0        0        0    11912 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/rm/viewer.properties
+-rw-r--r--   0        0        0    12063 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ro/viewer.properties
+-rw-r--r--   0        0        0    14314 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ru/viewer.properties
+-rw-r--r--   0        0        0     3569 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/rw/viewer.properties
+-rw-r--r--   0        0        0     8567 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sah/viewer.properties
+-rw-r--r--   0        0        0     8480 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sat/viewer.properties
+-rw-r--r--   0        0        0    12191 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/si/viewer.properties
+-rw-r--r--   0        0        0    12063 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sk/viewer.properties
+-rw-r--r--   0        0        0    11569 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sl/viewer.properties
+-rw-r--r--   0        0        0     7625 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/son/viewer.properties
+-rw-r--r--   0        0        0    11559 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sq/viewer.properties
+-rw-r--r--   0        0        0    12456 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sr/viewer.properties
+-rw-r--r--   0        0        0    11319 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sv-SE/viewer.properties
+-rw-r--r--   0        0        0     5396 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sw/viewer.properties
+-rw-r--r--   0        0        0    13674 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ta/viewer.properties
+-rw-r--r--   0        0        0     3572 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ta-LK/viewer.properties
+-rw-r--r--   0        0        0    13758 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/te/viewer.properties
+-rw-r--r--   0        0        0    15330 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/th/viewer.properties
+-rw-r--r--   0        0        0    11305 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/tl/viewer.properties
+-rw-r--r--   0        0        0     3713 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/tn/viewer.properties
+-rw-r--r--   0        0        0    11694 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/tr/viewer.properties
+-rw-r--r--   0        0        0     3288 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/tsz/viewer.properties
+-rw-r--r--   0        0        0    14147 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/uk/viewer.properties
+-rw-r--r--   0        0        0    10695 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ur/viewer.properties
+-rw-r--r--   0        0        0     7509 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/uz/viewer.properties
+-rw-r--r--   0        0        0    12223 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/vi/viewer.properties
+-rw-r--r--   0        0        0     5037 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/wo/viewer.properties
+-rw-r--r--   0        0        0     8376 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/xh/viewer.properties
+-rw-r--r--   0        0        0     3786 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/zam/viewer.properties
+-rw-r--r--   0        0        0    11148 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/zh-CN/viewer.properties
+-rw-r--r--   0        0        0    11208 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/zh-TW/viewer.properties
+-rw-r--r--   0        0        0     5803 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/zu/viewer.properties
+-rw-r--r--   0        0        0  9316700 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/testtext2.pdf
+-rw-r--r--   0        0        0    61862 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/viewer.css
+-rw-r--r--   0        0        0    22080 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/viewer.html
+-rw-r--r--   0        0        0   490689 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/viewer.js
+-rw-r--r--   0        0        0   749301 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/viewer.js.map
+-rw-r--r--   0        0        0     7309 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/saveAsPDF.py
+-rw-r--r--   0        0        0      549 2024-03-03 05:43:33.000000 pdf_preview-0.3.0/pdf_preview/util.py
+-rw-r--r--   0        0        0      637 2024-04-20 17:06:01.316491 pdf_preview-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      647 2024-03-03 07:12:58.000000 pdf_preview-0.3.0/README.rst
+-rw-r--r--   0        0        0     1145 1970-01-01 00:00:00.000000 pdf_preview-0.3.0/PKG-INFO
```

### Comparing `pdf_preview-0.2.0/pdf_preview/__main__.py` & `pdf_preview-0.3.0/pdf_preview/__main__.py`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/main_window.py` & `pdf_preview-0.3.0/pdf_preview/main_window.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,22 +81,18 @@
 
     self.filepath(index) -> fullpath
     self.data(index, Qt.CheckStateRole) -> check state
     """
 
     updateCheckState = QtCore.Signal(str, int)
 
-    def __init__(self, parent=None, single_file_mode=None):
+    def __init__(self, parent=None):
         super(CheckableFileSystemModel, self).__init__(parent)
         self.file_order_widget: QtWidgets.QListWidget = None
-        self.single_file = single_file_mode
-        if self.single_file:
-            self.setNameFilters([self.single_file])
-        else:
-            self.setNameFilters(["*.xls", "*.xlsx", "*.xlsm", "*.doc", "*.docx", "*.pdf"])
+        self.setNameFilters(["*.xls", "*.xlsx", "*.xlsm", "*.doc", "*.docx"])
 
     def setBookListWidget(self, widget):
         """Book の一覧を保持する ListWidget を設定する"""
         self.file_order_widget = widget
 
     def checkState(self, index):
         if self.filePath(index) in self.check:
@@ -139,18 +135,17 @@
 class FileOrderWidget(QtWidgets.QListWidget):
     """選択したファイルの順番を変更するリスト
 
     signal: fileOrderChanged(list) list: 変更結果のファイルの一覧
     """
     fileOrderChanged = QtCore.Signal()
 
-    def __init__(self, parent, root, single_file):
+    def __init__(self, parent, root):
         super(FileOrderWidget, self).__init__(parent)
         self.root = root
-        self.single_file = single_file
         self.model().rowsInserted.connect(self.fileOrderChanged)
         self.model().rowsInserted.connect(self.addWatchPath)
         self.model().rowsRemoved.connect(self.fileOrderChanged)
         self.model().rowsMoved.connect(self.fileOrderChanged)
         # ファイル変更時にPDFを再作成する
         self.watcher = QtCore.QFileSystemWatcher()
         self.watcher.fileChanged.connect(self.on_file_changed)
@@ -202,18 +197,15 @@
                 LOGGER.debug("一覧に変更はないのですがファイルが更新されたようなのでPDFを作り直してもらいます。")
                 self.on_rows_changed()
 
     def addItem(self, filename):
         if isinstance(filename, str):
             item = QtWidgets.QListWidgetItem(filename)
             item.setIcon(self.iconProvider.icon(QtCore.QFileInfo(self.abspath(filename))))
-            if not self.single_file or self.single_file == filename:
-                item.setFlags(item.flags() | Qt.ItemIsEnabled)
-            else:
-                item.setFlags(item.flags() & ~Qt.ItemIsEnabled)
+            item.setFlags(item.flags() & ~Qt.ItemIsEnabled)
             self.addItem(item)
             super().addItem(item)
         else:
             super().addItem(filename)
 
     @Slot(str, int)
     def updateFileList(self, filename, value):
@@ -299,51 +291,39 @@
 
     PDF化対象のファイル選択、シート選択の状態は、中段のブック一覧の QListWidget に追加する
     QListWidgetItem とその data として保持します。ツリービューでは順番を変えられないので。
     """
     file_selection_changed = QtCore.Signal(list)
     sheet_selection_changed = QtCore.Signal(list, str, str, Qt.CheckState)
 
-    @Slot(str, str, Qt.CheckState)
-    def on_sheetSelectionUpdated(self, filename, sheet_name, state):
-        paths = [self.book_list.item(i).text() for i in range(self.book_list.count())]
-        self.sheet_selection_changed.emit(paths, filename, sheet_name, state)
-
-    def on_update_check_state(self, filename, value):
-        """ブック一覧を更新する"""
-        self.book_list.updateFileList(filename, value)
-
-    def on_currentItemChanged(self, newitem: QtWidgets.QListWidgetItem, olditem: QtWidgets.QListWidgetItem):
-        """シート一覧を初期化し、新しいブックのシート一覧を表示する"""
-        if newitem:
-            r_path = newitem.text()
-            root = self.model.rootPath()
-            self.sheet_list.setSheetList(root, r_path)
-
-    def __init__(self, parent, root, single_file):
+    def __init__(self, parent, root):
         super(LeftPane, self).__init__(parent)
         self.sheet_selected_dict = {}
 
+        #
         # ファイルのツリービュー
-        self.model = CheckableFileSystemModel(self, single_file)
+        #
+        self.model = CheckableFileSystemModel(self)
         self.tv = QTreeView(self)
         self.tv.setModel(self.model)
         self.tv.setRootIndex(self.model.setRootPath(root))
         self.tv.header().setStretchLastSection(False)  # 一番右のカラムをストレッチする→False
         self.tv.setColumnWidth(0, 200)
-        self.tv.resizeColumnToContents(1)
-        self.tv.resizeColumnToContents(2)
-        self.tv.resizeColumnToContents(3)
 
+        #
         # ファイル一覧のビュー
-        self.book_list = FileOrderWidget(self, root, single_file)
+        #
+        self.book_list = FileOrderWidget(self, root)
         self.book_list.setAcceptDrops(True)
         self.book_list.setDragEnabled(True)
         self.book_list.setDragDropMode(QAbstractItemView.DragDropMode.InternalMove)
+
+        #
         # Excel のシート一覧のビュー
+        #
         self.sheet_list = ExcelSheetsView()
 
         # ツリービューのチェックボックスはブック一覧のリスト内容と連動
         self.model.setBookListWidget(self.book_list)
 
         # 上段のチェックボックスの変更に合わせて中段のファイルの一覧を更新する
         self.model.updateCheckState.connect(self.on_update_check_state)
@@ -366,21 +346,36 @@
         lo.addWidget(s)
         self.setLayout(lo)
 
     def open_file(self, index):
         LOGGER.debug("ファイルを開きます:{}".format(index))
         QDesktopServices.openUrl(QUrl.fromLocalFile(self.model.filePath(index)))
 
+    @Slot(str, str, Qt.CheckState)
+    def on_sheetSelectionUpdated(self, filename, sheet_name, state):
+        paths = [self.book_list.item(i).text() for i in range(self.book_list.count())]
+        self.sheet_selection_changed.emit(paths, filename, sheet_name, state)
+
+    def on_update_check_state(self, filename, value):
+        """ブック一覧を更新する"""
+        self.book_list.updateFileList(filename, value)
+
+    def on_currentItemChanged(self, newitem: QtWidgets.QListWidgetItem, olditem: QtWidgets.QListWidgetItem):
+        """シート一覧を初期化し、新しいブックのシート一覧を表示する"""
+        if newitem:
+            r_path = newitem.text()
+            root = self.model.rootPath()
+            self.sheet_list.setSheetList(root, r_path)
+
     @Slot()
     def on_fileOrderChanged(self):
         LOGGER.debug("ファイル一覧が変更されました。有効なファイルは次の通りです。")
         paths = [self.book_list.item(i).text() for i in range(self.book_list.count()) if
                  not self.book_list.item(i).isHidden()]
         LOGGER.debug("{}".format(paths))
-        self.tv.resizeColumnToContents(0)
         self.file_selection_changed.emit(paths)
 
 
 class MainWindow(QMainWindow):
     def load_sheet_selection(self):
         """シート選択の状態を復元する"""
         try:
@@ -388,15 +383,15 @@
         except IOError:
             return
         try:
             self.left_pane.sheet_list.sheet_selection = json_data["sheets"]
             blocker = QtCore.QSignalBlocker(self.left_pane.book_list)
             for book_name in json_data["files"]:
                 self.left_pane.book_list.addItem(book_name)
-                self.left_pane.book_list.watcher.addPath(str(Path(self.source) / book_name))
+                self.left_pane.book_list.watcher.addPath(str(Path(self.source_dir) / book_name))
             del blocker
         except KeyError:
             pass
 
     def save_sheet_selection(self):
         """シート選択の状態をファイルに保存する
 
@@ -412,34 +407,31 @@
             item = self.left_pane.book_list.item(i)
             path = item.text()  # path(relative)
             json_data["files"].append(path)
         json_data["sheets"] = self.left_pane.sheet_list.sheet_selection
         LOGGER.debug("save setting: {}: {}".format(self.sheet_selection_filename, json_data))
         json.dump(json_data, open(self.sheet_selection_filename, "w"), indent=4, ensure_ascii=False)
 
-    def __init__(self, source):
+    def __init__(self, source_dir: str):
         """
 
         :param source: 対象のファイルまたはディレクトリ
         """
         super(MainWindow, self).__init__()
-        self.source = source
+        self.source_dir = source_dir
         # 対象がファイルの場合はファイルのあるディレクトリをツリーに表示する
-        if Path(source).is_file():
-            self.root = str(Path(source).parent)
-            self.single_file = Path(source).name
-        else:
-            self.root = source
-            self.single_file = None
+        if Path(source_dir).is_file():
+            self.source_dir = str(Path(source_dir).parent)
 
-        self.output_path = Path(self.source).absolute().with_suffix(".PDF")
-        self.sheet_selection_filename = Path(self.root) / "PDF.json"
+        # 出力先は対象ディレクトリの中。ディレクトリと同名で拡張子を変えたもの。
+        self.output_path = Path(self.source_dir) / Path(self.source_dir).with_suffix(".PDF").name
+        self.sheet_selection_filename = self.output_path.with_suffix(".PDF.json")
         self.setWindowTitle(str(self.output_path))
 
-        self.left_pane = LeftPane(self, self.root, self.single_file)
+        self.left_pane = LeftPane(self, self.source_dir)
         self.left_pane.model.updateCheckState.connect(self.save_sheet_selection)  # ツリーでチェックされたら保存
         self.left_pane.file_selection_changed.connect(self.convertToPdf)  # ファイル選択の変更
         self.left_pane.sheet_selection_changed.connect(self.on_sheet_selection_changed)  # シート選択の変更
         self.web = QWebEngineView()
         ## self.web.settings().setAttribute(QWebEngineSettings.PluginsEnabled, True)
         self.viewer_html = str(Path(__file__).parent / Path('pdfjs-dist/web/viewer.html'))
         LOGGER.debug(self.viewer_html)
@@ -476,17 +468,15 @@
 
     # ブックを並び替えたら（最初のブックを選択したときも含む）PDF変換してすべて結合
     def convertToPdf(self, book_names, recreate_file: list = None):
         if recreate_file is None:
             recreate_file = []
         LOGGER.debug("PDF作成:{}".format(book_names))
         self.save_sheet_selection()
-        if self.single_file:
-            book_names = [self.single_file]
-        p = ConvertThread(self.root, self.output_path, book_names, recreate_file,
+        p = ConvertThread(self.source_dir, self.output_path, book_names, recreate_file,
                           self.left_pane.sheet_list.sheet_selection)
         p.obj_connection.threadFinished.connect(self.reload)
         QtCore.QThreadPool.globalInstance().start(p)
 
 
 def main(source):
     LOGGER.debug("source:{}".format(source))
```

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/build/pdf.js` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/build/pdf.js`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/build/pdf.js.map` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/build/pdf.js.map`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/build/pdf.worker.js` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/build/pdf.worker.js`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/build/pdf.worker.js.map` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/build/pdf.worker.js.map`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/LICENSE` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/78-EUC-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/78-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/78-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/78-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/78-RKSJ-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/78-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/78ms-RKSJ-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/78ms-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/83pv-RKSJ-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/83pv-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/90ms-RKSJ-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/90ms-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/90msp-RKSJ-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/90msp-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/90pv-RKSJ-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/90pv-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Add-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Add-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Add-RKSJ-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Add-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-UCS2.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-CNS1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-4.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-4.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-5.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-5.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-UCS2.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-GB1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-UCS2.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Japan1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Korea1-UCS2.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Adobe-Korea1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/B5-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/B5pc-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/B5pc-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/CNS-EUC-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/CNS-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/CNS-EUC-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/CNS-EUC-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/CNS1-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/CNS1-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/ETen-B5-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/ETen-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/ETHK-B5-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/ETHK-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/EUC-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Ext-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Ext-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/Ext-RKSJ-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/Ext-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GB-EUC-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GB-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GB-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GB-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBK-EUC-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBK-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBK2K-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBK2K-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBKp-EUC-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBKp-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBpc-EUC-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBT-EUC-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBT-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBT-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBT-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/GBTpc-EUC-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/GBTpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKdla-B5-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKdla-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKdlb-B5-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKdlb-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKgccs-B5-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKgccs-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKm314-B5-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKm314-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKm471-B5-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKm471-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/HKscs-B5-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/HKscs-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-EUC-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-Johab-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSC-Johab-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSCms-UHC-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSCms-UHC-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSCms-UHC-HW-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSCms-UHC-HW-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/KSCpc-EUC-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/KSCpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/LICENSE` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/NWP-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/NWP-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/RKSJ-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UCS2-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF16-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF32-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF8-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniCNS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UCS2-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF16-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF32-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF8-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniGB-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-HW-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-HW-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UCS2-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF16-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF16-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF16-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF32-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF32-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF8-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF8-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF16-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF16-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF16-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF32-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF32-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF8-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF8-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJIS2004-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISPro-UCS2-HW-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISPro-UCS2-HW-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISPro-UCS2-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISPro-UCS2-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISPro-UTF8-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISPro-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX0213-UTF32-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX0213-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX0213-UTF32-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX0213-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX02132004-UTF32-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX02132004-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX02132004-UTF32-V.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniJISX02132004-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UCS2-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF16-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF32-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF8-H.bcmap` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/cmaps/UniKS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/compressed.tracemonkey-pldi-09.pdf` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/compressed.tracemonkey-pldi-09.pdf`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/debugger.js` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/debugger.js`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-comment.svg` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-comment.svg`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-help.svg` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-help.svg`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-key.svg` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-key.svg`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-note.svg` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-note.svg`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/annotation-paragraph.svg` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/annotation-paragraph.svg`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/loading-icon.gif` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/loading-icon.gif`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/loading-small.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/loading-small.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/loading-small@2x.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/loading-small@2x.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-documentProperties@2x.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-documentProperties@2x.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-handTool@2x.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-handTool@2x.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-rotateCcw@2x.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-rotateCcw@2x.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-rotateCw@2x.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-rotateCw@2x.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-selectTool@2x.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-selectTool@2x.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadEven@2x.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadEven@2x.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadOdd@2x.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/secondaryToolbarButton-spreadOdd@2x.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/texture.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/texture.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-openFile@2x.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-openFile@2x.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-presentationMode@2x.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-presentationMode@2x.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-search@2x.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-search@2x.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewAttachments@2x.png` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/images/toolbarButton-viewAttachments@2x.png`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ach/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ach/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/af/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/af/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ak/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ak/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/an/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/an/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ar/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ar/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/as/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/as/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ast/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ast/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/az/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/az/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/be/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/be/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/bg/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/bg/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/bn-BD/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/bn-BD/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/bn-IN/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/bn-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/br/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/br/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/brx/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/brx/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/bs/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/bs/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ca/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ca/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/cak/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/cak/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/crh/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/crh/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/cs/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/cs/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/csb/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/csb/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/cy/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/cy/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/da/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/da/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/de/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/de/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/el/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/el/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/en-CA/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/en-CA/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/en-GB/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/en-GB/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/en-US/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/en-US/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/en-ZA/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/en-ZA/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/eo/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/eo/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/es-AR/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/es-AR/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/es-CL/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/es-CL/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/es-ES/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/es-ES/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/es-MX/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/es-MX/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/et/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/et/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/eu/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/eu/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/fa/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/fa/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ff/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ff/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/fi/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/fi/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/fr/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/fr/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/fy-NL/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/fy-NL/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ga-IE/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ga-IE/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/gd/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/gd/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/gl/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/gl/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/gn/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/gn/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/gu-IN/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/gu-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/he/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/he/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/hi-IN/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/hi-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/hr/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/hr/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/hsb/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/hsb/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/hto/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/hto/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/hu/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/hu/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/hy-AM/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/hy-AM/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ia/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ia/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/id/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/id/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/is/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/is/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/it/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/it/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ja/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ja/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ka/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ka/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/kab/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/kab/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/kk/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/kk/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/km/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/km/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/kn/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/kn/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ko/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ko/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/kok/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/kok/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ks/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ks/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ku/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ku/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/lg/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/lg/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/lij/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/lij/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/lo/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/lo/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/locale.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/locale.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/lt/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/lt/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ltg/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ltg/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/lv/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/lv/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/mai/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/mai/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/meh/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/meh/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/mk/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/mk/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ml/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ml/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/mn/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/mn/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/mr/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/mr/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ms/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ms/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/my/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/my/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/nb-NO/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/nb-NO/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ne-NP/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ne-NP/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/nl/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/nl/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/nn-NO/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/nn-NO/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/nso/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/nso/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/oc/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/oc/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/or/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/or/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/pa-IN/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/pa-IN/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/pl/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/pl/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/pt-BR/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/pt-BR/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/pt-PT/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/pt-PT/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/rm/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/rm/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ro/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ro/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ru/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ru/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/rw/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/rw/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sah/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sah/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sat/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sat/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/si/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/si/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sk/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sk/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sl/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sl/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/son/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/son/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sq/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sq/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sr/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sr/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sv-SE/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sv-SE/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/sw/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/sw/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ta/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ta/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ta-LK/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ta-LK/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/te/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/te/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/th/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/th/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/tl/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/tl/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/tn/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/tn/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/tr/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/tr/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/tsz/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/tsz/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/uk/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/uk/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/ur/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/ur/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/uz/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/uz/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/vi/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/vi/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/wo/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/wo/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/xh/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/xh/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/zam/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/zam/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/zh-CN/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/zh-CN/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/zh-TW/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/zh-TW/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/locale/zu/viewer.properties` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/locale/zu/viewer.properties`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/testtext2.pdf` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/testtext2.pdf`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/viewer.css` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/viewer.css`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/viewer.html` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/viewer.html`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/viewer.js` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/viewer.js`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/pdfjs-dist/web/viewer.js.map` & `pdf_preview-0.3.0/pdf_preview/pdfjs-dist/web/viewer.js.map`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/saveAsPDF.py` & `pdf_preview-0.3.0/pdf_preview/saveAsPDF.py`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pdf_preview/util.py` & `pdf_preview-0.3.0/pdf_preview/util.py`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/pyproject.toml` & `pdf_preview-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [tool.poetry]
 name = "pdf-preview"
-version = "0.2.0"
+version = "0.3.0"
 description = "PDF Previewer for Excel / Word document."
 authors = ["kkzk <shohachi.kakizaki@gmail.com>"]
 homepage = "https://github.com/kkzk/pdf-preview"
 readme = "README.rst"
 packages = [{include = "pdf_preview", from = "."}]
 
 [tool.poetry.dependencies]
 python = ">=3.12,<3.13"
 pyside6 = "^6.6.2"
 pypdf = "^4.0.2"
 pywin32 = "^306"
 openpyxl = "^3.1.2"
 
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.1.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 pdf-preview = "pdf_preview.__main__:main"
```

### Comparing `pdf_preview-0.2.0/README.rst` & `pdf_preview-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pdf_preview-0.2.0/PKG-INFO` & `pdf_preview-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-preview
-Version: 0.2.0
+Version: 0.3.0
 Summary: PDF Previewer for Excel / Word document.
 Home-page: https://github.com/kkzk/pdf-preview
 Author: kkzk
 Author-email: shohachi.kakizaki@gmail.com
 Requires-Python: >=3.12,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
```

