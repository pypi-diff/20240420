# Comparing `tmp/gdshoplib-2.4.9.tar.gz` & `tmp/gdshoplib-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdshoplib-2.4.9.tar", max compression
+gzip compressed data, was "gdshoplib-2.5.0.tar", max compression
```

## Comparing `gdshoplib-2.4.9.tar` & `gdshoplib-2.5.0.tar`

### file list

```diff
@@ -1,99 +1,103 @@
--rw-r--r--   0        0        0     2004 2023-10-24 20:30:30.973793 gdshoplib-2.4.9/README.md
--rw-r--r--   0        0        0     6148 2023-11-25 14:34:09.996559 gdshoplib-2.4.9/gdshoplib/.DS_Store
--rw-r--r--   0        0        0      210 2023-10-24 20:30:30.974587 gdshoplib-2.4.9/gdshoplib/__init__.py
--rw-r--r--   0        0        0       80 2023-10-24 20:30:30.974687 gdshoplib-2.4.9/gdshoplib/__main__.py
--rw-r--r--   0        0        0      117 2023-10-24 20:30:30.974862 gdshoplib-2.4.9/gdshoplib/activities/notion.py
--rw-r--r--   0        0        0        0 2023-10-24 20:30:30.974957 gdshoplib-2.4.9/gdshoplib/apps/__init__.py
--rw-r--r--   0        0        0     3001 2023-10-24 20:30:30.975212 gdshoplib-2.4.9/gdshoplib/apps/crm/cart.py
--rw-r--r--   0        0        0      292 2023-10-24 20:30:30.975323 gdshoplib-2.4.9/gdshoplib/apps/crm/dialog.py
--rw-r--r--   0        0        0     3768 2023-12-07 22:25:11.824801 gdshoplib-2.4.9/gdshoplib/apps/crm/on_request.py
--rw-r--r--   0        0        0    13286 2023-12-06 14:08:29.796695 gdshoplib-2.4.9/gdshoplib/apps/crm/orders.py
--rw-r--r--   0        0        0      674 2023-10-24 20:30:30.975839 gdshoplib-2.4.9/gdshoplib/apps/crm/stats.py
--rw-r--r--   0        0        0      315 2023-10-24 20:30:30.976032 gdshoplib-2.4.9/gdshoplib/apps/delivery/delivery.py
--rw-r--r--   0        0        0        0 2023-10-24 20:30:30.976172 gdshoplib-2.4.9/gdshoplib/apps/finance/__init__.py
--rw-r--r--   0        0        0      206 2023-10-24 20:30:30.976338 gdshoplib-2.4.9/gdshoplib/apps/finance/storage.py
--rw-r--r--   0        0        0        0 2023-10-24 20:30:30.976443 gdshoplib-2.4.9/gdshoplib/apps/marketing/__init__.py
--rw-r--r--   0        0        0      163 2023-10-24 20:30:30.976598 gdshoplib-2.4.9/gdshoplib/apps/payments/payments.py
--rw-r--r--   0        0        0      378 2023-10-24 20:30:30.976762 gdshoplib-2.4.9/gdshoplib/apps/platforms/README.md
--rw-r--r--   0        0        0      665 2023-10-24 20:30:30.976877 gdshoplib-2.4.9/gdshoplib/apps/platforms/__init__.py
--rw-r--r--   0        0        0     1742 2023-12-06 13:25:16.514598 gdshoplib-2.4.9/gdshoplib/apps/platforms/avito.py
--rw-r--r--   0        0        0      113 2023-10-24 20:30:30.977195 gdshoplib-2.4.9/gdshoplib/apps/platforms/base.py
--rw-r--r--   0        0        0      152 2023-10-24 20:30:30.977350 gdshoplib-2.4.9/gdshoplib/apps/platforms/instagram.py
--rw-r--r--   0        0        0       95 2023-10-24 20:30:30.977522 gdshoplib-2.4.9/gdshoplib/apps/platforms/ok.py
--rw-r--r--   0        0        0      467 2023-10-24 20:30:30.977649 gdshoplib-2.4.9/gdshoplib/apps/platforms/sm.py
--rw-r--r--   0        0        0       95 2023-10-24 20:30:30.977762 gdshoplib-2.4.9/gdshoplib/apps/platforms/tg.py
--rw-r--r--   0        0        0      908 2023-10-24 20:30:30.977942 gdshoplib-2.4.9/gdshoplib/apps/platforms/ula.py
--rw-r--r--   0        0        0      967 2023-11-25 14:34:10.148798 gdshoplib-2.4.9/gdshoplib/apps/platforms/vk.py
--rw-r--r--   0        0        0     3996 2023-12-07 22:38:04.344686 gdshoplib-2.4.9/gdshoplib/apps/platforms/yam.py
--rw-r--r--   0        0        0      187 2023-10-24 20:30:30.978653 gdshoplib-2.4.9/gdshoplib/apps/products/README.md
--rw-r--r--   0        0        0        0 2023-10-24 20:30:30.978734 gdshoplib-2.4.9/gdshoplib/apps/products/__init__.py
--rw-r--r--   0        0        0     1931 2023-10-24 20:30:30.978875 gdshoplib-2.4.9/gdshoplib/apps/products/description.py
--rw-r--r--   0        0        0     6150 2023-11-25 14:35:58.485555 gdshoplib-2.4.9/gdshoplib/apps/products/media.py
--rw-r--r--   0        0        0     1828 2023-11-25 14:35:43.176963 gdshoplib-2.4.9/gdshoplib/apps/products/price.py
--rw-r--r--   0        0        0     5687 2023-10-24 20:30:30.979697 gdshoplib-2.4.9/gdshoplib/apps/products/product.py
--rw-r--r--   0        0        0     6283 2023-10-24 20:30:30.980010 gdshoplib-2.4.9/gdshoplib/apps/uploader/uploader.py
--rw-r--r--   0        0        0      654 2023-11-25 14:34:09.998108 gdshoplib-2.4.9/gdshoplib/cli/application.py
--rw-r--r--   0        0        0      243 2023-10-24 20:30:30.980554 gdshoplib-2.4.9/gdshoplib/cli/crm/application.py
--rw-r--r--   0        0        0     1270 2023-11-30 20:25:08.735149 gdshoplib-2.4.9/gdshoplib/cli/crm/order.py
--rw-r--r--   0        0        0      357 2023-10-24 20:30:30.980813 gdshoplib-2.4.9/gdshoplib/cli/crm/stats.py
--rw-r--r--   0        0        0      162 2023-10-24 20:30:30.980995 gdshoplib-2.4.9/gdshoplib/cli/finance/application.py
--rw-r--r--   0        0        0      383 2023-10-24 20:30:30.981138 gdshoplib-2.4.9/gdshoplib/cli/finance/store.py
--rw-r--r--   0        0        0      734 2023-10-24 20:30:30.981385 gdshoplib-2.4.9/gdshoplib/cli/product/application.py
--rw-r--r--   0        0        0     2239 2023-10-24 20:30:30.981566 gdshoplib-2.4.9/gdshoplib/cli/product/barcode_cli.py
--rw-r--r--   0        0        0     5613 2023-10-24 20:30:30.981722 gdshoplib-2.4.9/gdshoplib/cli/product/cache.py
--rw-r--r--   0        0        0     1963 2023-10-24 20:30:30.981845 gdshoplib-2.4.9/gdshoplib/cli/product/controle.py
--rw-r--r--   0        0        0     1854 2023-12-15 20:16:22.695375 gdshoplib-2.4.9/gdshoplib/cli/product/description.py
--rw-r--r--   0        0        0      672 2023-10-24 20:30:30.982110 gdshoplib-2.4.9/gdshoplib/cli/product/feed.py
--rw-r--r--   0        0        0     3181 2023-12-20 19:02:49.370643 gdshoplib-2.4.9/gdshoplib/cli/product/media.py
--rw-r--r--   0        0        0     2300 2023-11-25 14:36:10.016321 gdshoplib-2.4.9/gdshoplib/cli/product/price.py
--rw-r--r--   0        0        0      238 2023-10-24 20:30:30.982705 gdshoplib-2.4.9/gdshoplib/cli/service/application.py
--rw-r--r--   0        0        0      458 2023-10-24 20:30:30.982924 gdshoplib-2.4.9/gdshoplib/cli/service/avito.py
--rw-r--r--   0        0        0     1070 2023-10-24 20:30:30.983141 gdshoplib-2.4.9/gdshoplib/cli/service/vk.py
--rw-r--r--   0        0        0      156 2023-11-25 14:34:09.998673 gdshoplib-2.4.9/gdshoplib/cli/stock/application.py
--rw-r--r--   0        0        0     2605 2023-11-25 14:34:09.998845 gdshoplib-2.4.9/gdshoplib/cli/stock/cart.py
--rw-r--r--   0        0        0      962 2023-10-24 20:30:30.983373 gdshoplib-2.4.9/gdshoplib/cli/temporal/application.py
--rw-r--r--   0        0        0     1345 2023-10-24 20:30:30.983622 gdshoplib-2.4.9/gdshoplib/core/ecosystem.py
--rw-r--r--   0        0        0     3794 2023-10-24 20:30:30.983893 gdshoplib-2.4.9/gdshoplib/core/settings.py
--rw-r--r--   0        0        0        0 2023-10-24 20:30:30.984018 gdshoplib-2.4.9/gdshoplib/packages/__init__.py
--rw-r--r--   0        0        0     1320 2023-10-24 20:30:30.984163 gdshoplib-2.4.9/gdshoplib/packages/barcode_pack.py
--rw-r--r--   0        0        0     3829 2023-10-24 20:30:30.984294 gdshoplib-2.4.9/gdshoplib/packages/cache.py
--rw-r--r--   0        0        0     4204 2023-12-05 22:27:24.856929 gdshoplib-2.4.9/gdshoplib/packages/feed.py
--rw-r--r--   0        0        0      774 2023-10-24 20:30:30.984613 gdshoplib-2.4.9/gdshoplib/packages/lang.py
--rw-r--r--   0        0        0      148 2023-10-24 20:30:30.984727 gdshoplib-2.4.9/gdshoplib/packages/marker.py
--rw-r--r--   0        0        0     2362 2023-10-24 20:30:30.984864 gdshoplib-2.4.9/gdshoplib/packages/renderer.py
--rw-r--r--   0        0        0     3869 2023-10-24 20:30:30.985009 gdshoplib-2.4.9/gdshoplib/packages/s3.py
--rw-r--r--   0        0        0     1986 2023-10-24 20:30:30.985195 gdshoplib-2.4.9/gdshoplib/packages/s3v2.py
--rw-r--r--   0        0        0        0 2023-10-24 20:30:30.985383 gdshoplib-2.4.9/gdshoplib/services/__init__.py
--rw-r--r--   0        0        0     3746 2023-10-24 20:30:30.985657 gdshoplib-2.4.9/gdshoplib/services/avito/avito.py
--rw-r--r--   0        0        0        0 2023-10-24 20:30:30.985836 gdshoplib-2.4.9/gdshoplib/services/cdek/cdek.py
--rw-r--r--   0        0        0     1709 2023-12-07 22:34:23.560068 gdshoplib-2.4.9/gdshoplib/services/gdshop/gdshop.py
--rw-r--r--   0        0        0     2821 2023-10-24 20:30:30.986215 gdshoplib-2.4.9/gdshoplib/services/notion/README.md
--rw-r--r--   0        0        0       50 2023-10-24 20:30:30.986411 gdshoplib-2.4.9/gdshoplib/services/notion/__init__.py
--rw-r--r--   0        0        0     1931 2023-10-24 20:30:30.986609 gdshoplib-2.4.9/gdshoplib/services/notion/base.py
--rw-r--r--   0        0        0      655 2023-10-24 20:30:30.986815 gdshoplib-2.4.9/gdshoplib/services/notion/block.py
--rw-r--r--   0        0        0     1174 2023-10-24 20:30:30.986950 gdshoplib-2.4.9/gdshoplib/services/notion/database.py
--rw-r--r--   0        0        0     1948 2023-11-25 14:34:10.149338 gdshoplib-2.4.9/gdshoplib/services/notion/manager.py
--rw-r--r--   0        0        0     2531 2023-10-24 20:30:30.987387 gdshoplib-2.4.9/gdshoplib/services/notion/models/props.py
--rw-r--r--   0        0        0     4027 2023-10-24 20:30:30.987558 gdshoplib-2.4.9/gdshoplib/services/notion/notion.py
--rw-r--r--   0        0        0    10492 2023-12-05 23:57:54.805354 gdshoplib-2.4.9/gdshoplib/services/notion/page.py
--rw-r--r--   0        0        0     2893 2023-10-24 20:30:30.987876 gdshoplib-2.4.9/gdshoplib/services/vk/market.py
--rw-r--r--   0        0        0     1825 2023-10-24 20:30:30.988026 gdshoplib-2.4.9/gdshoplib/services/vk/media.py
--rw-r--r--   0        0        0      986 2023-10-24 20:30:30.988126 gdshoplib-2.4.9/gdshoplib/services/vk/page.py
--rw-r--r--   0        0        0     2596 2023-10-24 20:30:30.988269 gdshoplib-2.4.9/gdshoplib/services/vk/stats.py
--rw-r--r--   0        0        0     2880 2023-10-24 20:30:30.988407 gdshoplib-2.4.9/gdshoplib/services/vk/stories.py
--rw-r--r--   0        0        0     2433 2023-10-24 20:30:30.988538 gdshoplib-2.4.9/gdshoplib/services/vk/vk.py
--rw-r--r--   0        0        0      104 2023-10-24 20:30:30.988713 gdshoplib-2.4.9/gdshoplib/services/ym/ym.py
--rw-r--r--   0        0        0     6148 2023-11-25 14:34:10.000140 gdshoplib-2.4.9/gdshoplib/templates/.DS_Store
--rw-r--r--   0        0        0   501468 2023-11-25 14:35:43.179225 gdshoplib-2.4.9/gdshoplib/templates/BungeeSpice-Regular.ttf
--rw-r--r--   0        0        0      792 2023-10-24 20:41:14.538116 gdshoplib-2.4.9/gdshoplib/templates/basic.txt
--rw-r--r--   0        0        0   430782 2023-11-25 14:34:10.014007 gdshoplib-2.4.9/gdshoplib/templates/bg.png
--rw-r--r--   0        0        0      508 2023-11-25 14:34:10.015089 gdshoplib-2.4.9/gdshoplib/templates/cart.html
--rw-r--r--   0        0        0      618 2023-12-05 18:32:28.311857 gdshoplib-2.4.9/gdshoplib/templates/instagram.txt
--rw-r--r--   0        0        0    26636 2023-11-25 14:34:10.015501 gdshoplib-2.4.9/gdshoplib/templates/name.png
--rw-r--r--   0        0        0      972 2023-11-25 15:07:05.179627 gdshoplib-2.4.9/gdshoplib/templates/qr.png
--rw-r--r--   0        0        0      661 2023-11-25 15:07:05.203175 gdshoplib-2.4.9/gdshoplib/templates/stock_cart.html
--rw-r--r--   0        0        0      854 2023-10-24 20:30:30.989246 gdshoplib-2.4.9/gdshoplib/templates/vk.txt
--rw-r--r--   0        0        0      572 2023-12-05 20:29:02.034240 gdshoplib-2.4.9/gdshoplib/templates/yam.txt
--rw-r--r--   0        0        0      470 2023-10-24 20:30:30.989416 gdshoplib-2.4.9/gdshoplib/workflows/notion.py
--rw-r--r--   0        0        0     1673 2023-12-20 19:03:01.263284 gdshoplib-2.4.9/pyproject.toml
--rw-r--r--   0        0        0     3902 1970-01-01 00:00:00.000000 gdshoplib-2.4.9/PKG-INFO
+-rw-r--r--   0        0        0     2004 2023-10-24 20:30:30.973793 gdshoplib-2.5.0/README.md
+-rw-r--r--   0        0        0     6148 2023-11-25 14:34:09.996559 gdshoplib-2.5.0/gdshoplib/.DS_Store
+-rw-r--r--   0        0        0      210 2023-10-24 20:30:30.974587 gdshoplib-2.5.0/gdshoplib/__init__.py
+-rw-r--r--   0        0        0       80 2023-10-24 20:30:30.974687 gdshoplib-2.5.0/gdshoplib/__main__.py
+-rw-r--r--   0        0        0      117 2023-10-24 20:30:30.974862 gdshoplib-2.5.0/gdshoplib/activities/notion.py
+-rw-r--r--   0        0        0        0 2023-10-24 20:30:30.974957 gdshoplib-2.5.0/gdshoplib/apps/__init__.py
+-rw-r--r--   0        0        0     3001 2023-10-24 20:30:30.975212 gdshoplib-2.5.0/gdshoplib/apps/crm/cart.py
+-rw-r--r--   0        0        0      292 2023-10-24 20:30:30.975323 gdshoplib-2.5.0/gdshoplib/apps/crm/dialog.py
+-rw-r--r--   0        0        0     3768 2023-12-07 22:25:11.824801 gdshoplib-2.5.0/gdshoplib/apps/crm/on_request.py
+-rw-r--r--   0        0        0    13286 2024-04-20 00:51:19.823887 gdshoplib-2.5.0/gdshoplib/apps/crm/orders.py
+-rw-r--r--   0        0        0      674 2023-10-24 20:30:30.975839 gdshoplib-2.5.0/gdshoplib/apps/crm/stats.py
+-rw-r--r--   0        0        0      315 2023-10-24 20:30:30.976032 gdshoplib-2.5.0/gdshoplib/apps/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2023-10-24 20:30:30.976172 gdshoplib-2.5.0/gdshoplib/apps/finance/__init__.py
+-rw-r--r--   0        0        0      206 2023-10-24 20:30:30.976338 gdshoplib-2.5.0/gdshoplib/apps/finance/storage.py
+-rw-r--r--   0        0        0        0 2023-10-24 20:30:30.976443 gdshoplib-2.5.0/gdshoplib/apps/marketing/__init__.py
+-rw-r--r--   0        0        0      163 2023-10-24 20:30:30.976598 gdshoplib-2.5.0/gdshoplib/apps/payments/payments.py
+-rw-r--r--   0        0        0      378 2023-10-24 20:30:30.976762 gdshoplib-2.5.0/gdshoplib/apps/platforms/README.md
+-rw-r--r--   0        0        0      775 2024-04-20 00:51:19.702763 gdshoplib-2.5.0/gdshoplib/apps/platforms/__init__.py
+-rw-r--r--   0        0        0     1829 2023-12-21 12:28:31.379758 gdshoplib-2.5.0/gdshoplib/apps/platforms/avito.py
+-rw-r--r--   0        0        0      113 2023-10-24 20:30:30.977195 gdshoplib-2.5.0/gdshoplib/apps/platforms/base.py
+-rw-r--r--   0        0        0      152 2023-10-24 20:30:30.977350 gdshoplib-2.5.0/gdshoplib/apps/platforms/instagram.py
+-rw-r--r--   0        0        0       95 2023-10-24 20:30:30.977522 gdshoplib-2.5.0/gdshoplib/apps/platforms/ok.py
+-rw-r--r--   0        0        0      467 2023-10-24 20:30:30.977649 gdshoplib-2.5.0/gdshoplib/apps/platforms/sm.py
+-rw-r--r--   0        0        0       95 2023-10-24 20:30:30.977762 gdshoplib-2.5.0/gdshoplib/apps/platforms/tg.py
+-rw-r--r--   0        0        0      908 2023-10-24 20:30:30.977942 gdshoplib-2.5.0/gdshoplib/apps/platforms/ula.py
+-rw-r--r--   0        0        0      967 2023-11-25 14:34:10.148798 gdshoplib-2.5.0/gdshoplib/apps/platforms/vk.py
+-rw-r--r--   0        0        0     3039 2024-04-19 21:56:04.819623 gdshoplib-2.5.0/gdshoplib/apps/platforms/web.py
+-rw-r--r--   0        0        0     3996 2023-12-22 23:20:10.423873 gdshoplib-2.5.0/gdshoplib/apps/platforms/yam.py
+-rw-r--r--   0        0        0     3475 2023-12-23 02:25:41.564212 gdshoplib-2.5.0/gdshoplib/apps/platforms/yamb.py
+-rw-r--r--   0        0        0      187 2023-10-24 20:30:30.978653 gdshoplib-2.5.0/gdshoplib/apps/products/README.md
+-rw-r--r--   0        0        0        0 2023-10-24 20:30:30.978734 gdshoplib-2.5.0/gdshoplib/apps/products/__init__.py
+-rw-r--r--   0        0        0     1931 2023-10-24 20:30:30.978875 gdshoplib-2.5.0/gdshoplib/apps/products/description.py
+-rw-r--r--   0        0        0     6150 2023-11-25 14:35:58.485555 gdshoplib-2.5.0/gdshoplib/apps/products/media.py
+-rw-r--r--   0        0        0     1828 2023-11-25 14:35:43.176963 gdshoplib-2.5.0/gdshoplib/apps/products/price.py
+-rw-r--r--   0        0        0     5672 2023-12-21 17:50:54.782020 gdshoplib-2.5.0/gdshoplib/apps/products/product.py
+-rw-r--r--   0        0        0     6283 2023-10-24 20:30:30.980010 gdshoplib-2.5.0/gdshoplib/apps/uploader/uploader.py
+-rw-r--r--   0        0        0      654 2023-11-25 14:34:09.998108 gdshoplib-2.5.0/gdshoplib/cli/application.py
+-rw-r--r--   0        0        0      243 2023-10-24 20:30:30.980554 gdshoplib-2.5.0/gdshoplib/cli/crm/application.py
+-rw-r--r--   0        0        0     1270 2023-11-30 20:25:08.735149 gdshoplib-2.5.0/gdshoplib/cli/crm/order.py
+-rw-r--r--   0        0        0      357 2023-10-24 20:30:30.980813 gdshoplib-2.5.0/gdshoplib/cli/crm/stats.py
+-rw-r--r--   0        0        0      162 2023-10-24 20:30:30.980995 gdshoplib-2.5.0/gdshoplib/cli/finance/application.py
+-rw-r--r--   0        0        0      383 2023-10-24 20:30:30.981138 gdshoplib-2.5.0/gdshoplib/cli/finance/store.py
+-rw-r--r--   0        0        0      734 2023-10-24 20:30:30.981385 gdshoplib-2.5.0/gdshoplib/cli/product/application.py
+-rw-r--r--   0        0        0     2239 2023-10-24 20:30:30.981566 gdshoplib-2.5.0/gdshoplib/cli/product/barcode_cli.py
+-rw-r--r--   0        0        0     5753 2024-03-18 21:11:11.044728 gdshoplib-2.5.0/gdshoplib/cli/product/cache.py
+-rw-r--r--   0        0        0     1963 2023-10-24 20:30:30.981845 gdshoplib-2.5.0/gdshoplib/cli/product/controle.py
+-rw-r--r--   0        0        0     1854 2023-12-15 20:16:22.695375 gdshoplib-2.5.0/gdshoplib/cli/product/description.py
+-rw-r--r--   0        0        0      672 2023-10-24 20:30:30.982110 gdshoplib-2.5.0/gdshoplib/cli/product/feed.py
+-rw-r--r--   0        0        0     3182 2024-01-29 20:33:16.765265 gdshoplib-2.5.0/gdshoplib/cli/product/media.py
+-rw-r--r--   0        0        0     2300 2023-11-25 14:36:10.016321 gdshoplib-2.5.0/gdshoplib/cli/product/price.py
+-rw-r--r--   0        0        0      238 2023-10-24 20:30:30.982705 gdshoplib-2.5.0/gdshoplib/cli/service/application.py
+-rw-r--r--   0        0        0      458 2023-10-24 20:30:30.982924 gdshoplib-2.5.0/gdshoplib/cli/service/avito.py
+-rw-r--r--   0        0        0     1070 2023-10-24 20:30:30.983141 gdshoplib-2.5.0/gdshoplib/cli/service/vk.py
+-rw-r--r--   0        0        0      156 2023-11-25 14:34:09.998673 gdshoplib-2.5.0/gdshoplib/cli/stock/application.py
+-rw-r--r--   0        0        0     2605 2023-11-25 14:34:09.998845 gdshoplib-2.5.0/gdshoplib/cli/stock/cart.py
+-rw-r--r--   0        0        0      962 2023-10-24 20:30:30.983373 gdshoplib-2.5.0/gdshoplib/cli/temporal/application.py
+-rw-r--r--   0        0        0     1345 2023-10-24 20:30:30.983622 gdshoplib-2.5.0/gdshoplib/core/ecosystem.py
+-rw-r--r--   0        0        0     3794 2023-10-24 20:30:30.983893 gdshoplib-2.5.0/gdshoplib/core/settings.py
+-rw-r--r--   0        0        0        0 2023-10-24 20:30:30.984018 gdshoplib-2.5.0/gdshoplib/packages/__init__.py
+-rw-r--r--   0        0        0     1320 2023-10-24 20:30:30.984163 gdshoplib-2.5.0/gdshoplib/packages/barcode_pack.py
+-rw-r--r--   0        0        0     3829 2023-10-24 20:30:30.984294 gdshoplib-2.5.0/gdshoplib/packages/cache.py
+-rw-r--r--   0        0        0     4204 2023-12-05 22:27:24.856929 gdshoplib-2.5.0/gdshoplib/packages/feed.py
+-rw-r--r--   0        0        0      774 2023-10-24 20:30:30.984613 gdshoplib-2.5.0/gdshoplib/packages/lang.py
+-rw-r--r--   0        0        0      148 2023-10-24 20:30:30.984727 gdshoplib-2.5.0/gdshoplib/packages/marker.py
+-rw-r--r--   0        0        0     2362 2023-10-24 20:30:30.984864 gdshoplib-2.5.0/gdshoplib/packages/renderer.py
+-rw-r--r--   0        0        0     3869 2023-10-24 20:30:30.985009 gdshoplib-2.5.0/gdshoplib/packages/s3.py
+-rw-r--r--   0        0        0     1986 2023-10-24 20:30:30.985195 gdshoplib-2.5.0/gdshoplib/packages/s3v2.py
+-rw-r--r--   0        0        0        0 2023-10-24 20:30:30.985383 gdshoplib-2.5.0/gdshoplib/services/__init__.py
+-rw-r--r--   0        0        0     3746 2023-10-24 20:30:30.985657 gdshoplib-2.5.0/gdshoplib/services/avito/avito.py
+-rw-r--r--   0        0        0        0 2023-10-24 20:30:30.985836 gdshoplib-2.5.0/gdshoplib/services/cdek/cdek.py
+-rw-r--r--   0        0        0     1709 2023-12-07 22:34:23.560068 gdshoplib-2.5.0/gdshoplib/services/gdshop/gdshop.py
+-rw-r--r--   0        0        0     2821 2023-10-24 20:30:30.986215 gdshoplib-2.5.0/gdshoplib/services/notion/README.md
+-rw-r--r--   0        0        0       50 2023-10-24 20:30:30.986411 gdshoplib-2.5.0/gdshoplib/services/notion/__init__.py
+-rw-r--r--   0        0        0     1931 2023-10-24 20:30:30.986609 gdshoplib-2.5.0/gdshoplib/services/notion/base.py
+-rw-r--r--   0        0        0      655 2023-10-24 20:30:30.986815 gdshoplib-2.5.0/gdshoplib/services/notion/block.py
+-rw-r--r--   0        0        0     1174 2023-10-24 20:30:30.986950 gdshoplib-2.5.0/gdshoplib/services/notion/database.py
+-rw-r--r--   0        0        0     1948 2023-11-25 14:34:10.149338 gdshoplib-2.5.0/gdshoplib/services/notion/manager.py
+-rw-r--r--   0        0        0     2531 2023-10-24 20:30:30.987387 gdshoplib-2.5.0/gdshoplib/services/notion/models/props.py
+-rw-r--r--   0        0        0     4027 2023-10-24 20:30:30.987558 gdshoplib-2.5.0/gdshoplib/services/notion/notion.py
+-rw-r--r--   0        0        0    10492 2023-12-05 23:57:54.805354 gdshoplib-2.5.0/gdshoplib/services/notion/page.py
+-rw-r--r--   0        0        0     2893 2023-10-24 20:30:30.987876 gdshoplib-2.5.0/gdshoplib/services/vk/market.py
+-rw-r--r--   0        0        0     1825 2023-10-24 20:30:30.988026 gdshoplib-2.5.0/gdshoplib/services/vk/media.py
+-rw-r--r--   0        0        0      986 2023-10-24 20:30:30.988126 gdshoplib-2.5.0/gdshoplib/services/vk/page.py
+-rw-r--r--   0        0        0     2596 2023-10-24 20:30:30.988269 gdshoplib-2.5.0/gdshoplib/services/vk/stats.py
+-rw-r--r--   0        0        0     2880 2023-10-24 20:30:30.988407 gdshoplib-2.5.0/gdshoplib/services/vk/stories.py
+-rw-r--r--   0        0        0     2433 2023-10-24 20:30:30.988538 gdshoplib-2.5.0/gdshoplib/services/vk/vk.py
+-rw-r--r--   0        0        0      104 2023-10-24 20:30:30.988713 gdshoplib-2.5.0/gdshoplib/services/ym/ym.py
+-rw-r--r--   0        0        0     6148 2023-11-25 14:34:10.000140 gdshoplib-2.5.0/gdshoplib/templates/.DS_Store
+-rw-r--r--   0        0        0   501468 2023-11-25 14:35:43.179225 gdshoplib-2.5.0/gdshoplib/templates/BungeeSpice-Regular.ttf
+-rw-r--r--   0        0        0     1325 2024-01-31 05:42:21.611071 gdshoplib-2.5.0/gdshoplib/templates/avito.txt
+-rw-r--r--   0        0        0      792 2023-10-24 20:41:14.538116 gdshoplib-2.5.0/gdshoplib/templates/basic.txt
+-rw-r--r--   0        0        0   430782 2023-11-25 14:34:10.014007 gdshoplib-2.5.0/gdshoplib/templates/bg.png
+-rw-r--r--   0        0        0      508 2023-11-25 14:34:10.015089 gdshoplib-2.5.0/gdshoplib/templates/cart.html
+-rw-r--r--   0        0        0      618 2023-12-05 18:32:28.311857 gdshoplib-2.5.0/gdshoplib/templates/instagram.txt
+-rw-r--r--   0        0        0    26636 2023-11-25 14:34:10.015501 gdshoplib-2.5.0/gdshoplib/templates/name.png
+-rw-r--r--   0        0        0      972 2023-11-25 15:07:05.179627 gdshoplib-2.5.0/gdshoplib/templates/qr.png
+-rw-r--r--   0        0        0      661 2023-11-25 15:07:05.203175 gdshoplib-2.5.0/gdshoplib/templates/stock_cart.html
+-rw-r--r--   0        0        0      901 2024-01-30 12:27:40.339785 gdshoplib-2.5.0/gdshoplib/templates/vk.txt
+-rw-r--r--   0        0        0      502 2023-12-22 23:16:00.483442 gdshoplib-2.5.0/gdshoplib/templates/yam.txt
+-rw-r--r--   0        0        0      502 2023-12-22 23:16:06.121440 gdshoplib-2.5.0/gdshoplib/templates/yamb.txt
+-rw-r--r--   0        0        0      470 2023-10-24 20:30:30.989416 gdshoplib-2.5.0/gdshoplib/workflows/notion.py
+-rw-r--r--   0        0        0     1673 2024-04-20 00:14:31.874623 gdshoplib-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3902 1970-01-01 00:00:00.000000 gdshoplib-2.5.0/PKG-INFO
```

### Comparing `gdshoplib-2.4.9/README.md` & `gdshoplib-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/.DS_Store` & `gdshoplib-2.5.0/gdshoplib/.DS_Store`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/crm/cart.py` & `gdshoplib-2.5.0/gdshoplib/apps/crm/cart.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/crm/on_request.py` & `gdshoplib-2.5.0/gdshoplib/apps/crm/on_request.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/crm/orders.py` & `gdshoplib-2.5.0/gdshoplib/apps/crm/orders.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/crm/stats.py` & `gdshoplib-2.5.0/gdshoplib/apps/crm/stats.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/platforms/__init__.py` & `gdshoplib-2.5.0/gdshoplib/apps/platforms/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from .base import Platform
 from .instagram import InstagramManager
 from .ok import OkManager
 from .sm import SberMarketManager
 from .tg import TgManager
 from .ula import UlaManager
 from .vk import VKManager
+from .web import WebManager
 from .yam import YandexMarketManager
+from .yamb import YandexBussinesManager
 
 
 def search_platform(key):
     for platform_class in Platform.__subclasses__():
         if platform_class.KEY.lower() == key.lower():
             return platform_class
 
@@ -19,11 +21,12 @@
     "AvitoManager",
     "InstagramManager",
     "OkManager",
     "TgManager",
     "UlaManager",
     "VKManager",
     "YandexMarketManager",
-    "SberMarketManager",
+    "YandexBussinesManager" "SberMarketManager",
+    "WebManager",
     "Platform",
     "search_platform",
 )
```

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/platforms/avito.py` & `gdshoplib-2.5.0/gdshoplib/apps/platforms/avito.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from gdshoplib.apps.platforms.base import Platform
 from gdshoplib.packages.feed import Feed
 
 
 class AvitoManager(Platform, Feed):
     KEY = "AVITO"
+    DESCRIPTION_TEMPLATE = "avito.txt"
 
     def get_root(self):
         root = etree.Element("Ads")
         objectify.deannotate(root, cleanup_namespaces=True, xsi_nil=True)
         root.attrib["target"] = "Avito"
         root.attrib["formatVersion"] = "3"
         return root
@@ -20,14 +21,15 @@
         appt.Title = product.name
         appt.Category = self.feed_settings.AVITO_CATEGORY
         appt.ListingFee = "Package"
         appt.AdStatus = "Free"
         appt.ContactMethod = "По телефону и в сообщениях"
         appt.Condition = "Новое"
         appt.Description = product.description.render(self)
+        appt.Delivery = "Свой курьер"
         appt.Address = self.feed_settings.ADDRESS
         appt.Price = product.price.now
         appt.ManagerName = self.feed_settings.MANAGER_NAME
         appt.ContactPhone = self.feed_settings.PHONE
         appt.Stock = product.quantity
 
         images = objectify.Element("Images")
```

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/platforms/ula.py` & `gdshoplib-2.5.0/gdshoplib/apps/platforms/ula.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/platforms/vk.py` & `gdshoplib-2.5.0/gdshoplib/apps/platforms/vk.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/platforms/yam.py` & `gdshoplib-2.5.0/gdshoplib/apps/platforms/yam.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/products/description.py` & `gdshoplib-2.5.0/gdshoplib/apps/products/description.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/products/media.py` & `gdshoplib-2.5.0/gdshoplib/apps/products/media.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/products/price.py` & `gdshoplib-2.5.0/gdshoplib/apps/products/price.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/products/product.py` & `gdshoplib-2.5.0/gdshoplib/apps/products/product.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
         return result
 
     @property
     def tags(self):
         result = []
         for tag in self.split(self.tags_field):
-            result.append(re.sub(r"[\W\s]", "", tag).lower())
+            result.append(tag.strip().lower())
         return result
 
     @property
     def specifications(self):
         result = []
         for spec in self.split(self.specifications_field):
             result.append(spec.capitalize())
```

### Comparing `gdshoplib-2.4.9/gdshoplib/apps/uploader/uploader.py` & `gdshoplib-2.5.0/gdshoplib/apps/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/cli/application.py` & `gdshoplib-2.5.0/gdshoplib/cli/application.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/cli/crm/order.py` & `gdshoplib-2.5.0/gdshoplib/cli/crm/order.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/cli/product/application.py` & `gdshoplib-2.5.0/gdshoplib/cli/product/application.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/cli/product/barcode_cli.py` & `gdshoplib-2.5.0/gdshoplib/cli/product/barcode_cli.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/cli/product/cache.py` & `gdshoplib-2.5.0/gdshoplib/cli/product/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,22 +26,26 @@
 @app.command()
 def listen(topic: List[str]):
     for message in KeyDBCache().subscribe(topic):
         print(message)
 
 
 @app.command()
-def upload(page_id: Optional[str] = typer.Option(None), infinity: bool = True):
+def upload(page_id: Optional[str] = typer.Option(None), infinity: bool = False):
     uploader = Uploader(NotionSettings().KAFKA_TOPIC)
     notion = Notion()
 
     last_edited = None
     new_time = None
     while True:
-        _itarator = notion.search()
+        _itarator = filter(
+            lambda x: x["parent"].get("database_id")
+            == "2d1707fb-877d-4d83-8ae6-3c3d00ff5091",
+            notion.search(),
+        )
 
         if page_id:
             _itarator = [Notion().get_page(page_id)]
 
         for page in _itarator:
             page_last_edited = datetime.strptime(
                 page["last_edited_time"].split(".")[0], "%Y-%m-%dT%H:%M:%S"
```

### Comparing `gdshoplib-2.4.9/gdshoplib/cli/product/controle.py` & `gdshoplib-2.5.0/gdshoplib/cli/product/controle.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/cli/product/description.py` & `gdshoplib-2.5.0/gdshoplib/cli/product/description.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/cli/product/feed.py` & `gdshoplib-2.5.0/gdshoplib/cli/product/feed.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/cli/product/media.py` & `gdshoplib-2.5.0/gdshoplib/cli/product/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 @app.command()
 def warm(
     single: bool = typer.Option(False),
     with_badges: bool = typer.Option(False),
     loop_iteration: Optional[int] = typer.Option(None),
     sku: Optional[str] = typer.Option(None),
-    all: bool = typer.Option(False)
+    all: bool = typer.Option(False),
 ):
     while True:
         gen = Product.query(filter=dict(status_publication="Публикация"))
 
         if sku:
             warm_product_media(Product.get(sku).id, with_badges)
             return
```

### Comparing `gdshoplib-2.4.9/gdshoplib/cli/product/price.py` & `gdshoplib-2.5.0/gdshoplib/cli/product/price.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/cli/service/vk.py` & `gdshoplib-2.5.0/gdshoplib/cli/service/vk.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/cli/stock/cart.py` & `gdshoplib-2.5.0/gdshoplib/cli/stock/cart.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/cli/temporal/application.py` & `gdshoplib-2.5.0/gdshoplib/cli/temporal/application.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/core/ecosystem.py` & `gdshoplib-2.5.0/gdshoplib/core/ecosystem.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/core/settings.py` & `gdshoplib-2.5.0/gdshoplib/core/settings.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/packages/barcode_pack.py` & `gdshoplib-2.5.0/gdshoplib/packages/barcode_pack.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/packages/cache.py` & `gdshoplib-2.5.0/gdshoplib/packages/cache.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/packages/feed.py` & `gdshoplib-2.5.0/gdshoplib/packages/feed.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/packages/lang.py` & `gdshoplib-2.5.0/gdshoplib/packages/lang.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/packages/renderer.py` & `gdshoplib-2.5.0/gdshoplib/packages/renderer.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/packages/s3.py` & `gdshoplib-2.5.0/gdshoplib/packages/s3.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/packages/s3v2.py` & `gdshoplib-2.5.0/gdshoplib/packages/s3v2.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/avito/avito.py` & `gdshoplib-2.5.0/gdshoplib/services/avito/avito.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/gdshop/gdshop.py` & `gdshoplib-2.5.0/gdshoplib/services/gdshop/gdshop.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/notion/README.md` & `gdshoplib-2.5.0/gdshoplib/services/notion/README.md`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/notion/base.py` & `gdshoplib-2.5.0/gdshoplib/services/notion/base.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/notion/block.py` & `gdshoplib-2.5.0/gdshoplib/services/notion/block.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/notion/database.py` & `gdshoplib-2.5.0/gdshoplib/services/notion/database.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/notion/manager.py` & `gdshoplib-2.5.0/gdshoplib/services/notion/manager.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/notion/models/props.py` & `gdshoplib-2.5.0/gdshoplib/services/notion/models/props.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/notion/notion.py` & `gdshoplib-2.5.0/gdshoplib/services/notion/notion.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/notion/page.py` & `gdshoplib-2.5.0/gdshoplib/services/notion/page.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/vk/market.py` & `gdshoplib-2.5.0/gdshoplib/services/vk/market.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/vk/media.py` & `gdshoplib-2.5.0/gdshoplib/services/vk/media.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/vk/page.py` & `gdshoplib-2.5.0/gdshoplib/services/vk/page.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/vk/stats.py` & `gdshoplib-2.5.0/gdshoplib/services/vk/stats.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/vk/stories.py` & `gdshoplib-2.5.0/gdshoplib/services/vk/stories.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/services/vk/vk.py` & `gdshoplib-2.5.0/gdshoplib/services/vk/vk.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/templates/.DS_Store` & `gdshoplib-2.5.0/gdshoplib/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/templates/BungeeSpice-Regular.ttf` & `gdshoplib-2.5.0/gdshoplib/templates/BungeeSpice-Regular.ttf`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/templates/basic.txt` & `gdshoplib-2.5.0/gdshoplib/templates/basic.txt`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/templates/bg.png` & `gdshoplib-2.5.0/gdshoplib/templates/bg.png`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/templates/instagram.txt` & `gdshoplib-2.5.0/gdshoplib/templates/instagram.txt`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/templates/name.png` & `gdshoplib-2.5.0/gdshoplib/templates/name.png`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/templates/qr.png` & `gdshoplib-2.5.0/gdshoplib/templates/qr.png`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/templates/stock_cart.html` & `gdshoplib-2.5.0/gdshoplib/templates/stock_cart.html`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.4.9/gdshoplib/templates/vk.txt` & `gdshoplib-2.5.0/gdshoplib/templates/vk.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-{% if product.quantity == 0 %}📦 Под заказ 📦
-{% endif %}{{ product.name }}
+{{ product.name }}
+{% if product.quantity == 0 %}📦 Под заказ 📦{% else %} ✅ <strong>В наличии</strong>{%endif%}
 
 {% if product.brand %}Бренд: {{product.brand.title}}{% endif %}{% if product.collection %}
 Коллекция: {{product.collection}}{% endif %}{% if product.size %}
 Размер: {{product.size}}{% endif %}{% if product.color %}
 Цвет: {{product.color}}{% endif %}
 
 {% if product.short_description %}{{product.short_description}}{% endif %}
```

### Comparing `gdshoplib-2.4.9/pyproject.toml` & `gdshoplib-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gdshoplib"
-version = "2.4.9"
+version = "2.5.0"
 description = ""
 authors = ["Nikolay Baryshnikov <root@k0d.ru>"]
 packages=[
     { include = "gdshoplib" },
 ]
 license="MIT"
 readme="README.md"
```

### Comparing `gdshoplib-2.4.9/PKG-INFO` & `gdshoplib-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdshoplib
-Version: 2.4.9
+Version: 2.5.0
 Summary: 
 Home-page: https://github.com/p141592
 License: MIT
 Author: Nikolay Baryshnikov
 Author-email: root@k0d.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

