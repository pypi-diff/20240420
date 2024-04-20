# Comparing `tmp/omni-api-0.5.2.tar.gz` & `tmp/omni-api-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omni-api-0.5.2.tar", last modified: Wed Apr 10 13:01:34 2024, max compression
+gzip compressed data, was "dist/omni-api-0.5.3.tar", last modified: Sat Apr 20 08:15:27 2024, max compression
```

## Comparing `omni-api-0.5.2.tar` & `omni-api-0.5.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:01:34.000000 omni-api-0.5.2/
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-10 13:01:34.000000 omni-api-0.5.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3434 2024-04-10 13:01:29.000000 omni-api-0.5.2/README.md
--rw-r--r--   0 root         (0) root         (0)     2429 2024-04-10 13:01:29.000000 omni-api-0.5.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:01:34.000000 omni-api-0.5.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:01:34.000000 omni-api-0.5.2/src/omni_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-10 13:01:34.000000 omni-api-0.5.2/src/omni_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1220 2024-04-10 13:01:34.000000 omni-api-0.5.2/src/omni_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 13:01:34.000000 omni-api-0.5.2/src/omni_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 13:01:31.000000 omni-api-0.5.2/src/omni_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-10 13:01:34.000000 omni-api-0.5.2/src/omni_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     4960 2024-04-10 13:01:34.000000 omni-api-0.5.2/src/omni_api.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:01:34.000000 omni-api-0.5.2/src/omni/
--rw-r--r--   0 root         (0) root         (0)     3832 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/invoice.py
--rw-r--r--   0 root         (0) root         (0)     1889 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/util.py
--rw-r--r--   0 root         (0) root         (0)     2223 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/consignment_out.py
--rw-r--r--   0 root         (0) root         (0)     3959 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/export.py
--rw-r--r--   0 root         (0) root         (0)     1482 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/sub_product.py
--rw-r--r--   0 root         (0) root         (0)     1500 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/return_.py
--rw-r--r--   0 root         (0) root         (0)     3832 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/receipt.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/stock_adjustment.py
--rw-r--r--   0 root         (0) root         (0)     1636 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/consignment_slip.py
--rw-r--r--   0 root         (0) root         (0)     1720 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/document.py
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/inventory_line.py
--rw-r--r--   0 root         (0) root         (0)     1304 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/sale_order.py
--rw-r--r--   0 root         (0) root         (0)     2443 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/signed_document.py
--rw-r--r--   0 root         (0) root         (0)     1273 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/sale_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1453 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/store.py
--rw-r--r--   0 root         (0) root         (0)     1894 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/customer.py
--rw-r--r--   0 root         (0) root         (0)     9954 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/base.py
--rw-r--r--   0 root         (0) root         (0)     1863 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/errors.py
--rw-r--r--   0 root         (0) root         (0)     3178 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4056 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/entity.py
--rw-r--r--   0 root         (0) root         (0)     2081 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/saft_pt.py
--rw-r--r--   0 root         (0) root         (0)     2294 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/media.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/product.py
--rw-r--r--   0 root         (0) root         (0)     1640 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/transfer.py
--rw-r--r--   0 root         (0) root         (0)     1260 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/web.py
--rw-r--r--   0 root         (0) root         (0)     1208 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/user.py
--rw-r--r--   0 root         (0) root         (0)     1311 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/identifiable.py
--rw-r--r--   0 root         (0) root         (0)     3425 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/sale.py
--rw-r--r--   0 root         (0) root         (0)     1691 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/supplier.py
--rw-r--r--   0 root         (0) root         (0)     2056 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/merchandise.py
--rw-r--r--   0 root         (0) root         (0)     1207 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/status.py
--rw-r--r--   0 root         (0) root         (0)     2188 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/employee.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:01:34.000000 omni-api-0.5.2/src/omni/models/
--rw-r--r--   0 root         (0) root         (0)     1227 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/models/line.py
--rw-r--r--   0 root         (0) root         (0)     1103 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/models/customer.py
--rw-r--r--   0 root         (0) root         (0)     1183 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/models/base.py
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1101 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/models/entity.py
--rw-r--r--   0 root         (0) root         (0)     1123 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/models/operation.py
--rw-r--r--   0 root         (0) root         (0)     1178 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/models/sale.py
--rw-r--r--   0 root         (0) root         (0)     1133 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/models/merchandise.py
--rw-r--r--   0 root         (0) root         (0)     2190 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/system_company.py
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/money_sale_slip.py
--rw-r--r--   0 root         (0) root         (0)     1596 2024-04-10 13:01:29.000000 omni-api-0.5.2/src/omni/credit_note.py
--rw-r--r--   0 root         (0) root         (0)     4960 2024-04-10 13:01:34.000000 omni-api-0.5.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:15:27.000000 omni-api-0.5.3/
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-04-20 08:15:22.000000 omni-api-0.5.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2024-04-20 08:15:22.000000 omni-api-0.5.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-20 08:15:27.000000 omni-api-0.5.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4960 2024-04-20 08:15:27.000000 omni-api-0.5.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:15:27.000000 omni-api-0.5.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:15:27.000000 omni-api-0.5.3/src/omni/
+-rw-r--r--   0 root         (0) root         (0)     3832 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/inventory_line.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/product.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/sub_product.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/identifiable.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/money_sale_slip.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/saft_pt.py
+-rw-r--r--   0 root         (0) root         (0)     9954 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/base.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/customer.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/supplier.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/transfer.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/status.py
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/signed_document.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/sale_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4056 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/entity.py
+-rw-r--r--   0 root         (0) root         (0)     1260 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/web.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/consignment_slip.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/store.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/stock_adjustment.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/sale_order.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/export.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/merchandise.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/sale.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/task.py
+-rw-r--r--   0 root         (0) root         (0)     3832 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/receipt.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/user.py
+-rw-r--r--   0 root         (0) root         (0)     1720 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/document.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/util.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/employee.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/system_company.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/consignment_out.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/credit_note.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/return_.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/media.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:15:27.000000 omni-api-0.5.3/src/omni/models/
+-rw-r--r--   0 root         (0) root         (0)     1183 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/models/base.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/models/customer.py
+-rw-r--r--   0 root         (0) root         (0)     1101 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/models/entity.py
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/models/merchandise.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/models/sale.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/models/operation.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-04-20 08:15:22.000000 omni-api-0.5.3/src/omni/models/line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:15:27.000000 omni-api-0.5.3/src/omni_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 08:15:27.000000 omni-api-0.5.3/src/omni_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-04-20 08:15:27.000000 omni-api-0.5.3/src/omni_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-20 08:15:27.000000 omni-api-0.5.3/src/omni_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4960 2024-04-20 08:15:27.000000 omni-api-0.5.3/src/omni_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-20 08:15:27.000000 omni-api-0.5.3/src/omni_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 08:15:24.000000 omni-api-0.5.3/src/omni_api.egg-info/not-zip-safe
```

### Comparing `omni-api-0.5.2/README.md` & `omni-api-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/setup.py` & `omni-api-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
     name="omni-api",
-    version="0.5.2",
+    version="0.5.3",
     author="Hive Solutions Lda.",
     author_email="development@hive.pt",
     description="Omni API Client",
     license="Apache License, Version 2.0",
     keywords="omni api",
     url="http://omni-api.hive.pt",
     zip_safe=False,
```

### Comparing `omni-api-0.5.2/src/omni_api.egg-info/SOURCES.txt` & `omni-api-0.5.3/src/omni_api.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 src/omni/signed_document.py
 src/omni/status.py
 src/omni/stock_adjustment.py
 src/omni/store.py
 src/omni/sub_product.py
 src/omni/supplier.py
 src/omni/system_company.py
+src/omni/task.py
 src/omni/transfer.py
 src/omni/user.py
 src/omni/util.py
 src/omni/web.py
 src/omni/models/__init__.py
 src/omni/models/base.py
 src/omni/models/customer.py
```

### Comparing `omni-api-0.5.2/src/omni_api.egg-info/PKG-INFO` & `omni-api-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-api
-Version: 0.5.2
+Version: 0.5.3
 Summary: Omni API Client
 Home-page: http://omni-api.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Omni API](http://omni-api.hive.pt)
```

### Comparing `omni-api-0.5.2/src/omni/invoice.py` & `omni-api-0.5.3/src/omni/invoice.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/util.py` & `omni-api-0.5.3/src/omni/util.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/consignment_out.py` & `omni-api-0.5.3/src/omni/consignment_out.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/export.py` & `omni-api-0.5.3/src/omni/export.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/sub_product.py` & `omni-api-0.5.3/src/omni/sub_product.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/return_.py` & `omni-api-0.5.3/src/omni/return_.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/receipt.py` & `omni-api-0.5.3/src/omni/receipt.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/stock_adjustment.py` & `omni-api-0.5.3/src/omni/stock_adjustment.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/consignment_slip.py` & `omni-api-0.5.3/src/omni/consignment_slip.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/document.py` & `omni-api-0.5.3/src/omni/document.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/inventory_line.py` & `omni-api-0.5.3/src/omni/inventory_line.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/sale_order.py` & `omni-api-0.5.3/src/omni/sale_order.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/signed_document.py` & `omni-api-0.5.3/src/omni/signed_document.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/sale_snapshot.py` & `omni-api-0.5.3/src/omni/sale_snapshot.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/store.py` & `omni-api-0.5.3/src/omni/store.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/customer.py` & `omni-api-0.5.3/src/omni/customer.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/base.py` & `omni-api-0.5.3/src/omni/base.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/errors.py` & `omni-api-0.5.3/src/omni/errors.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/__init__.py` & `omni-api-0.5.3/src/omni/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,24 +76,25 @@
 from .invoice import InvoiceAPI
 from .media import MediaAPI
 from .merchandise import MerchandiseAPI
 from .money_sale_slip import MoneySaleSlipAPI
 from .product import ProductAPI
 from .receipt import ReceiptAPI
 from .return_ import ReturnAPI
-from .saft_pt import SaftPtAPI, SaftPtReport, SaftPtReportPayload
+from .saft_pt import SaftPtAPI, SaftPtReport, SaftPtReportDelta, SaftPtReportPayload
 from .sale_order import SaleOrderAPI
 from .sale_snapshot import SaleSnapshotAPI
 from .sale import SaleAPI
 from .signed_document import SignedDocumentAPI
 from .status import StatusAPI
 from .stock_adjustment import StockAdjustmentAPI
 from .store import StoreAPI
 from .sub_product import SubProductAPI
 from .supplier import SupplierAPI
 from .system_company import SystemCompanyAPI
+from .task import TaskState, Task, TaskDelta
 from .transfer import TransferAPI
 from .user import UserAPI
 from .util import format_places, filter_args
 from .web import WebAPI
 
 from .export import export as export_do
```

### Comparing `omni-api-0.5.2/src/omni/entity.py` & `omni-api-0.5.3/src/omni/entity.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/saft_pt.py` & `omni-api-0.5.3/src/omni/saft_pt.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,13 +56,17 @@
 
     def file_decompressed_saft_pt(self, object_id):
         url = self.base_url + "omni/saft_pt/%d/file_decompressed" % object_id
         contents = self.get(url)
         return contents
 
 
-class SaftPtReport(object):
+class SaftPtReport(dict):
     pass
 
 
-class SaftPtReportPayload(object):
+class SaftPtReportDelta(dict):
+    pass
+
+
+class SaftPtReportPayload(dict):
     pass
```

### Comparing `omni-api-0.5.2/src/omni/media.py` & `omni-api-0.5.3/src/omni/media.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/product.py` & `omni-api-0.5.3/src/omni/product.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/transfer.py` & `omni-api-0.5.3/src/omni/transfer.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/web.py` & `omni-api-0.5.3/src/omni/web.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/user.py` & `omni-api-0.5.3/src/omni/user.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/identifiable.py` & `omni-api-0.5.3/src/omni/identifiable.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/sale.py` & `omni-api-0.5.3/src/omni/sale.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/supplier.py` & `omni-api-0.5.3/src/omni/supplier.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/merchandise.py` & `omni-api-0.5.3/src/omni/merchandise.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/status.py` & `omni-api-0.5.3/src/omni/status.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/employee.py` & `omni-api-0.5.3/src/omni/employee.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/models/line.py` & `omni-api-0.5.3/src/omni/models/line.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/models/customer.py` & `omni-api-0.5.3/src/omni/models/customer.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/models/base.py` & `omni-api-0.5.3/src/omni/models/base.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/models/__init__.py` & `omni-api-0.5.3/src/omni/models/__init__.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/models/entity.py` & `omni-api-0.5.3/src/omni/models/entity.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/models/operation.py` & `omni-api-0.5.3/src/omni/models/operation.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/models/sale.py` & `omni-api-0.5.3/src/omni/models/sale.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/models/merchandise.py` & `omni-api-0.5.3/src/omni/models/merchandise.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/system_company.py` & `omni-api-0.5.3/src/omni/system_company.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/money_sale_slip.py` & `omni-api-0.5.3/src/omni/money_sale_slip.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/src/omni/credit_note.py` & `omni-api-0.5.3/src/omni/credit_note.py`

 * *Files identical despite different names*

### Comparing `omni-api-0.5.2/PKG-INFO` & `omni-api-0.5.3/src/omni_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-api
-Version: 0.5.2
+Version: 0.5.3
 Summary: Omni API Client
 Home-page: http://omni-api.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Omni API](http://omni-api.hive.pt)
```

