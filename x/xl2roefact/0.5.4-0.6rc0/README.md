# Comparing `tmp/xl2roefact-0.5.4.tar.gz` & `tmp/xl2roefact-0.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xl2roefact-0.5.4.tar", last modified: Sat Apr  6 17:45:42 2024, max compression
+gzip compressed data, was "xl2roefact-0.6rc0.tar", last modified: Sat Apr 20 01:23:45 2024, max compression
```

## Comparing `xl2roefact-0.5.4.tar` & `xl2roefact-0.6rc0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0    35149 2024-04-06 17:45:09.666372 xl2roefact-0.5.4/LICENSE
--rw-r--r--   0        0        0    18286 2024-04-06 17:45:09.666372 xl2roefact-0.5.4/README.md
--rw-r--r--   0        0        0     3284 2024-04-06 17:45:42.462232 xl2roefact-0.5.4/pyproject.toml
--rw-r--r--   0        0        0        1 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/.gitkeep
--rw-r--r--   0        0        0    18903 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/Fact_Petrom_11017969.json
--rw-r--r--   0        0        0   268862 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/Fact_Petrom_11017969.xlsx
--rw-r--r--   0        0        0    15740 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/Fact_Petrom_11017969.xml
--rw-r--r--   0        0        0      986 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/_test_results.txt
--rw-r--r--   0        0        0    20914 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/fact_RENF1004.json
--rw-r--r--   0        0        0    16332 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/tests/fact_RENF1004.xlsx
--rw-r--r--   0        0        0      567 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/__init__.py
--rw-r--r--   0        0        0      626 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/__main__.py
--rw-r--r--   0        0        0     1492 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/__version__.py
--rw-r--r--   0        0        0     7875 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/app_cli.py
--rw-r--r--   0        0        0      727 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/chkisld.py
--rw-r--r--   0        0        0      584 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/chkxml.py
--rw-r--r--   0        0        0     8246 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/config_settings.py
--rw-r--r--   0        0        0     1808 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/data/README_app_config_rules.md
--rw-r--r--   0        0        0        1 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/data/__init__.py
--rw-r--r--   0        0        0     6867 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/data/app_settings.yml
--rw-r--r--   0        0        0      600 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/ldxml.py
--rw-r--r--   0        0        0    10480 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/libutils.py
--rw-r--r--   0        0        0    69307 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/rdinv.py
--rw-r--r--   0        0        0      612 2024-04-06 17:45:10.082370 xl2roefact-0.5.4/xl2roefact/wrxml.py
--rw-r--r--   0        0        0    60832 1970-01-01 00:00:00.000000 xl2roefact-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-20 01:23:19.951218 xl2roefact-0.6rc0/LICENSE
+-rw-r--r--   0        0        0    18602 2024-04-20 01:23:19.951218 xl2roefact-0.6rc0/README.md
+-rw-r--r--   0        0        0     3364 2024-04-20 01:23:45.699419 xl2roefact-0.6rc0/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/.gitkeep
+-rw-r--r--   0        0        0    21622 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.json
+-rw-r--r--   0        0        0   268862 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.xlsx
+-rw-r--r--   0        0        0    15740 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.xml
+-rw-r--r--   0        0        0      986 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/_test_results.txt
+-rw-r--r--   0        0        0    24084 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/fact_RENF1004.json
+-rw-r--r--   0        0        0    16332 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/fact_RENF1004.xlsx
+-rw-r--r--   0        0        0     1531 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/todosXML.md
+-rw-r--r--   0        0        0      567 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/__init__.py
+-rw-r--r--   0        0        0      626 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/__main__.py
+-rw-r--r--   0        0        0     1500 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/__version__.py
+-rw-r--r--   0        0        0     7913 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/app_cli.py
+-rw-r--r--   0        0        0      727 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/chkisld.py
+-rw-r--r--   0        0        0      584 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/chkxml.py
+-rw-r--r--   0        0        0     8915 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/config_settings.py
+-rw-r--r--   0        0        0     1808 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/data/README_app_config_rules.md
+-rw-r--r--   0        0        0        1 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/data/__init__.py
+-rw-r--r--   0        0        0     7134 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/data/app_settings.yml
+-rw-r--r--   0        0        0      600 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/ldxml.py
+-rw-r--r--   0        0        0    10480 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/libutils.py
+-rw-r--r--   0        0        0    71476 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/rdinv.py
+-rw-r--r--   0        0        0     1319 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/sys_settings.py
+-rw-r--r--   0        0        0      612 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/wrxml.py
+-rw-r--r--   0        0        0    61200 1970-01-01 00:00:00.000000 xl2roefact-0.6rc0/PKG-INFO
```

### Comparing `xl2roefact-0.5.4/LICENSE` & `xl2roefact-0.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.4/README.md` & `xl2roefact-0.6rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 
 Legaturi externe utile:
 
 * [**Web Site**](https://invoicetoroefact.renware.eu/). (*Pentru acces corect la toate referintele din acest document vizitati site-ul dedicat acestui sistem.*)
 * [Pachet *PyPi*](https://pypi.org/project/xl2roefact/)
 * [Surse *GitHub*](https://github.com/petre-renware/api_to_roefact/)
 * [Vedere de ansamblu pachet biblioteca Python](./doc/README_xl2roefact_library.md)
-* [Referinta *API*](./doc/810.05a-xl2roefact_DLD_specs.md)
-
+* [Referinta *API*](https://invoicetoroefact.renware.eu/xl2roefact/doc/wrapper_810.05a-xl2roefact_DLD_specs.html)
+<!--Refrence to source doc. If used like that, then must be resolved with an external tool before generating a complete README.html doc. The `mkdoxs` is able to do that but in `PyPi` published version will be unusable
+(./doc/810.05a-xl2roefact_DLD_specs.md)
+-->
 
 
 ## Facilitati
 
 ![Static Badge](https://img.shields.io/badge/MSI_installer-YES-darkgreen)
 ![Static Badge](https://img.shields.io/badge/standlone_EXE-YES-darkgreen)
 ![Static Badge](https://img.shields.io/badge/script_Python3-YES-darkgreen)
```

### Comparing `xl2roefact-0.5.4/pyproject.toml` & `xl2roefact-0.6rc0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -31,43 +31,48 @@
     "pywin32-ctypes~=0.2",
     "rich~=13.7",
     "setuptools~=69.0",
     "shellingham~=1.5",
     "six~=1.16",
     "time-machine~=2.13",
     "tomli~=2.0",
+    "click~=8.1",
+    "typer~=0.9",
     "typing-extensions~=4.9",
     "tzdata~=2023.4",
     "userpath~=1.9",
     "wheel~=0.42",
     "msgpack>=1.0.8",
     "pyyaml>=6.0.1",
 ]
 readme = "README.md"
-requires-python = ">=3.10,<3.11"
+requires-python = "<3.12,>=3.9"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Operating System :: OS Independent",
     "Topic :: Office/Business :: Financial",
 ]
-version = "0.5.4"
+version = "0.6rc0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://invoicetoroefact.renware.eu"
 PDF-Documentation = "https://invoicetoroefact.renware.eu/pdfs/print_page.html/print_page.pdf"
 PyPi-Package = "https://pypi.org/project/xl2roefact/"
 GitHub = "https://github.com/petre-renware/api_to_roefact"
 
+[project.scripts]
+xl2roefact = "xl2roefact.app_cli:main"
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
@@ -84,14 +89,17 @@
 
 [tool.pdm.scripts.build_wheel]
 shell = "pdm build --no-clean"
 
 [tool.pdm.scripts.build_msi]
 shell = "python setup.py bdist_msi"
 
+[tool.pdm.scripts.build_appimage]
+shell = "python setup.py bdist_appimage"
+
 [tool.pdm.scripts.build_sexe]
 cmd = [
     "pyinstaller",
     "--distpath=dist_sexe/",
     "--name=xl2roefact",
     "--log-level=WARN",
     "--onefile",
@@ -118,26 +126,21 @@
 
 [tool.pdm.scripts.pypi_publish]
 shell = "git checkout -b pypi-publish; git push --force"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "build~=1.0",
-    "click~=8.1",
-    "typer~=0.9",
     "pydoc-markdown~=4.8",
     "cx-Freeze~=6.15",
     "cx-Logging~=3.1",
     "pyinstaller>=4.10",
     "pyinstaller-hooks-contrib~=2023.12",
 ]
 
-[tool.hatch.metadata]
-allow-direct-references = true
-
 [tool.distutils.build_exe]
 excludes = [
     "tkinter",
     "unittest",
 ]
 zip_include_packages = [
     "encodings",
```

### Comparing `xl2roefact-0.5.4/tests/Fact_Petrom_11017969.json` & `xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9216376336819044%*

 * *Differences: {"'Invoice'": "{'cac_AccountingSupplierParty': {'cac_Party': {'cac_PartyLegalEntity': "*

 * *              "{'cbc_CompanyID': 'RO1590082', 'cbc_RegistrationName': 'OMV Petrom S.A.'}, "*

 * *              "'cac_Contact': {'RegCom': None, 'Bank': 'Comerciala Romana', 'IBAN': None}, "*

 * *              "'cac_PartyTaxScheme': {'cbc_CompanyID': 'RO1590082'}}}, 'cbc_DueDate': "*

 * *              "'2023-11-16', 'cbc_Note': 'proccesed @2024-04-18T04:10:02.798583+00:00 with "*

 * *              "xl2roefact', 'cac_PaymentMeans': OrderedDic […]*

```diff
@@ -22,40 +22,43 @@
                     "cbc_StreetName": "Coralilor Nr. 22"
                 }
             }
         },
         "cac_AccountingSupplierParty": {
             "cac_Party": {
                 "cac_Contact": {
-                    "Bank": "...",
-                    "IBAN": "...",
-                    "RegCom": "...",
+                    "Bank": "Comerciala Romana",
+                    "IBAN": null,
+                    "RegCom": null,
                     "cbc_ElectronicMail": null,
                     "cbc_Telephone": null
                 },
                 "cac_PartyLegalEntity": {
-                    "cbc_CompanyID": "...",
-                    "cbc_RegistrationName": "..."
+                    "cbc_CompanyID": "RO1590082",
+                    "cbc_RegistrationName": "OMV Petrom S.A."
                 },
                 "cac_PartyTaxScheme": {
                     "cac_TaxScheme": {
                         "cbc_ID": "VAT"
                     },
-                    "cbc_CompanyID": "..."
+                    "cbc_CompanyID": "RO1590082"
                 },
                 "cac_PostalAddress": {
                     "cac_Country": {
                         "cbc_IdentificationCode": "RO"
                     },
                     "cbc_CityName": "",
                     "cbc_PostalZone": "Postal 013329",
                     "cbc_StreetName": "Coralilor Nr. 22"
                 }
             }
         },
+        "cac_Delivery": {
+            "cbc_ActualDeliveryDate": "2023-10-17"
+        },
         "cac_InvoiceLine": [
             {
                 "LineVatAmount": 8123.66,
                 "cac_Item": {
                     "cac_ClassifiedTaxCategory": {
                         "cac_TaxScheme": {
                             "cbc_ID": "VAT"
@@ -116,14 +119,17 @@
         ],
         "cac_LegalMonetaryTotal": {
             "cbc_LineExtensionAmount": 43611.0,
             "cbc_PayableAmount": 51734.0,
             "cbc_TaxExclusiveAmount": 43611.0,
             "cbc_TaxInclusiveAmount": 51734.0
         },
+        "cac_PaymentMeans": {
+            "cbc_PaymentMeansCode": 1
+        },
         "cac_TaxTotal": {
             "cac_TaxSubtotal": [
                 {
                     "cac_TaxCategory": {
                         "ID": "S",
                         "cac_ClassifiedTaxCategory": {
                             "cac_TaxScheme": {
@@ -161,16 +167,19 @@
                     "cbc_TaxAmount": 0.0,
                     "cbc_TaxableAmount": 855.12
                 }
             ],
             "cbc_TaxAmount": 8123.66
         },
         "cbc_DocumentCurrencyCode": "RON",
+        "cbc_DueDate": "2023-11-16",
         "cbc_ID": "11017969",
-        "cbc_IssueDate": "2023-10-17"
+        "cbc_IssueDate": "2023-10-17",
+        "cbc_Note": "proccesed @2024-04-18T04:10:02.798583+00:00 with xl2roefact",
+        "cbc_TaxPointDate": "2023-11-25"
     },
     "excel_original_data": {
         "invoice_footer_area": {
             "end_cell": [
                 49,
                 8
             ],
@@ -280,14 +289,23 @@
                     "location": [
                         null,
                         null
                     ],
                     "value": null
                 }
             },
+            "due_date": {
+                "label_location": null,
+                "label_value": null,
+                "location": [
+                    null,
+                    null
+                ],
+                "value": "2023-11-16"
+            },
             "end_cell": [
                 28,
                 8
             ],
             "invoice_number": {
                 "label_location": [
                     10,
@@ -314,56 +332,102 @@
             },
             "start_cell": [
                 1,
                 1
             ],
             "supplier_area": {
                 "CUI": {
-                    "label_location": null,
-                    "label_value": null,
-                    "location": "external file (PartyLegalEntity -> CompanyID)",
-                    "value": "..."
+                    "label_location": [
+                        10,
+                        2
+                    ],
+                    "label_value": "C.U.I. RO1590082",
+                    "location": [
+                        10,
+                        2
+                    ],
+                    "value": "RO1590082"
                 },
                 "IBAN": {
-                    "location": "external file (Contact -> IBAN)",
-                    "value": "..."
+                    "label_location": null,
+                    "label_value": null,
+                    "location": [
+                        null,
+                        null
+                    ],
+                    "value": null
                 },
                 "PostalAddress": {
                     "cac_Country": {
                         "cbc_IdentificationCode": "RO"
                     },
-                    "cbc_CityName": "...",
-                    "cbc_PostalZone": "...",
-                    "cbc_StreetName": "..."
+                    "cbc_CityName": "",
+                    "cbc_PostalZone": "Postal 013329",
+                    "cbc_StreetName": "Coralilor Nr. 22"
                 },
                 "RegistrationName": {
-                    "label_location": null,
-                    "label_value": null,
-                    "location": "external file (PartyLegalEntity -> CompanyID)",
-                    "value": "..."
+                    "label_location": "n/a",
+                    "label_value": "n/a",
+                    "location": [
+                        8,
+                        2
+                    ],
+                    "value": "OMV Petrom S.A."
                 },
                 "area_info": {
-                    "location": "external file",
-                    "value": "/home/petre/api_to_roefact/xl2roefact/xl2roefact/data/owner.yml"
+                    "location": [
+                        [
+                            8,
+                            2
+                        ],
+                        [
+                            18,
+                            3
+                        ]
+                    ],
+                    "value": "OMV Petrom S.A."
                 },
                 "bank": {
-                    "location": "external file (Contact -> Bank)",
-                    "value": "..."
+                    "label_location": [
+                        16,
+                        2
+                    ],
+                    "label_value": "Banca Comerciala Romana",
+                    "location": [
+                        16,
+                        2
+                    ],
+                    "value": "Comerciala Romana"
                 },
                 "email": {
-                    "location": "external file (Contact -> ElectronicMail)",
+                    "label_location": null,
+                    "label_value": null,
+                    "location": [
+                        null,
+                        null
+                    ],
                     "value": null
                 },
                 "phone": {
-                    "location": "external file (Contact -> Telephone)",
+                    "label_location": null,
+                    "label_value": null,
+                    "location": [
+                        null,
+                        null
+                    ],
                     "value": null
                 },
                 "reg_com": {
-                    "location": "external file (PartyLegalEntity -> CompanyID)",
-                    "value": "..."
+                    "label_location": null,
+                    "label_value": null,
+                    "location": [
+                        null,
+                        null
+                    ],
+                    "value": null
                 }
             }
         },
         "invoice_items_area": {
             "data": [
                 [
                     "Inlocuit conducta PSI coloana C2 DAV.",
@@ -420,15 +484,15 @@
         "invoice_max_rows": 49,
         "invoice_worksheet": "Factura(Invoice)",
         "items_table_start_cell": [
             29,
             1
         ],
         "items_table_start_marker": "No. crt.",
-        "last_processing_time": "2024-04-04T08:23:19.821130+00:00",
+        "last_processing_time": "2024-04-18T04:10:02.798215+00:00",
         "map_JSONkeys_XMLtags": [
             [
                 "cac_InvoiceLine",
                 "cac:InvoiceLine"
             ],
             [
                 "cac_Item",
@@ -483,14 +547,18 @@
                 "cbc:DocumentCurrencyCode"
             ],
             [
                 "cbc_IssueDate",
                 "cbc:IssueDate"
             ],
             [
+                "cbc_DueDate",
+                "cbc:DueDate"
+            ],
+            [
                 "cac_AccountingCustomerParty",
                 "cac:AccountingCustomerParty"
             ],
             [
                 "cac_Party",
                 "cac:Party"
             ],
@@ -601,11 +669,47 @@
             [
                 "cac_AccountingSupplierParty",
                 "cac:AccountingSupplierParty"
             ],
             [
                 "cac_PartyTaxScheme",
                 "cac:PartyTaxScheme"
+            ],
+            [
+                "cbc_DueDate",
+                "cbc:DueDate"
+            ],
+            [
+                "cbc_InvoiceTypeCode",
+                "cbc:InvoiceTypeCode"
+            ],
+            [
+                "cbc_Note",
+                "cbc:Note"
+            ],
+            [
+                "cbc_TaxPointDate",
+                "cbc:TaxPointDate"
+            ],
+            [
+                "cac_Delivery",
+                "cac:Delivery"
+            ],
+            [
+                "cbc_ActualDeliveryDate",
+                "cbc:ActualDeliveryDate"
+            ],
+            [
+                "cac_PaymentMeans",
+                "cac:PaymentMeans"
+            ],
+            [
+                "cbc_PaymentMeansCode",
+                "cbc:PaymentMeansCode"
+            ],
+            [
+                "cbc_TaxPointDate",
+                "cbc:TaxPointDate"
             ]
         ]
     }
 }
```

### Comparing `xl2roefact-0.5.4/tests/Fact_Petrom_11017969.xlsx` & `xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.xlsx`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.4/tests/Fact_Petrom_11017969.xml` & `xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.xml`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.4/tests/_test_results.txt` & `xl2roefact-0.6rc0/tests/_test_results.txt`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.4/tests/fact_RENF1004.json` & `xl2roefact-0.6rc0/tests/fact_RENF1004.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9215333928224553%*

 * *Differences: {"'Invoice'": "{'cac_AccountingSupplierParty': {'cac_Party': {'cac_PartyLegalEntity': "*

 * *              "{'cbc_CompanyID': '42561459', 'cbc_RegistrationName': 'REN-CONSULTING SOFT ACTIVITY "*

 * *              "SRL'}, 'cac_Contact': {'cbc_Telephone': '0744-68.48.76', 'cbc_ElectronicMail': "*

 * *              "'renware.systems@gmail.com', 'RegCom': 'J40/5662/2020', 'Bank': 'Banca "*

 * *              "Transilvania', 'IBAN': 'RO29 BTRL RONC RT05 5704 8601'}, 'cac_PartyTaxScheme': "*

 * *              "{'cbc_CompanyID': '42561459' […]*

```diff
@@ -22,40 +22,43 @@
                     "cbc_StreetName": ""
                 }
             }
         },
         "cac_AccountingSupplierParty": {
             "cac_Party": {
                 "cac_Contact": {
-                    "Bank": "...",
-                    "IBAN": "...",
-                    "RegCom": "...",
-                    "cbc_ElectronicMail": null,
-                    "cbc_Telephone": null
+                    "Bank": "Banca Transilvania",
+                    "IBAN": "RO29 BTRL RONC RT05 5704 8601",
+                    "RegCom": "J40/5662/2020",
+                    "cbc_ElectronicMail": "renware.systems@gmail.com",
+                    "cbc_Telephone": "0744-68.48.76"
                 },
                 "cac_PartyLegalEntity": {
-                    "cbc_CompanyID": "...",
-                    "cbc_RegistrationName": "..."
+                    "cbc_CompanyID": "42561459",
+                    "cbc_RegistrationName": "REN-CONSULTING SOFT ACTIVITY SRL"
                 },
                 "cac_PartyTaxScheme": {
                     "cac_TaxScheme": {
                         "cbc_ID": "VAT"
                     },
-                    "cbc_CompanyID": "..."
+                    "cbc_CompanyID": "42561459"
                 },
                 "cac_PostalAddress": {
                     "cac_Country": {
                         "cbc_IdentificationCode": "RO"
                     },
                     "cbc_CityName": "Bucure\u015fti Sectorul 1, Strada: BUZE\u015eTI, Nr. 71, Etaj 7 si 8, tara: Romania",
                     "cbc_PostalZone": "",
                     "cbc_StreetName": ""
                 }
             }
         },
+        "cac_Delivery": {
+            "cbc_ActualDeliveryDate": "2023-08-28"
+        },
         "cac_InvoiceLine": [
             {
                 "LineVatAmount": 7389.15,
                 "cac_Item": {
                     "cac_ClassifiedTaxCategory": {
                         "cac_TaxScheme": {
                             "cbc_ID": "VAT"
@@ -156,14 +159,17 @@
         ],
         "cac_LegalMonetaryTotal": {
             "cbc_LineExtensionAmount": 39001.0,
             "cbc_PayableAmount": 46390.0,
             "cbc_TaxExclusiveAmount": 39001.0,
             "cbc_TaxInclusiveAmount": 46390.0
         },
+        "cac_PaymentMeans": {
+            "cbc_PaymentMeansCode": 1
+        },
         "cac_TaxTotal": {
             "cac_TaxSubtotal": [
                 {
                     "cac_TaxCategory": {
                         "ID": "S",
                         "cac_ClassifiedTaxCategory": {
                             "cac_TaxScheme": {
@@ -188,16 +194,19 @@
                     "cbc_TaxAmount": null,
                     "cbc_TaxableAmount": null
                 }
             ],
             "cbc_TaxAmount": 7389.15
         },
         "cbc_DocumentCurrencyCode": "RON",
+        "cbc_DueDate": "2023-09-27",
         "cbc_ID": "RENF-1004",
-        "cbc_IssueDate": "2023-08-28"
+        "cbc_IssueDate": "2023-08-28",
+        "cbc_Note": "proccesed @2024-04-18T04:10:02.876896+00:00 with xl2roefact",
+        "cbc_TaxPointDate": "2023-09-25"
     },
     "excel_original_data": {
         "invoice_footer_area": {
             "end_cell": [
                 31,
                 9
             ],
@@ -319,14 +328,23 @@
                     "location": [
                         10,
                         6
                     ],
                     "value": "J40/11864/06.07.2005"
                 }
             },
+            "due_date": {
+                "label_location": null,
+                "label_value": null,
+                "location": [
+                    null,
+                    null
+                ],
+                "value": "2023-09-27"
+            },
             "end_cell": [
                 19,
                 9
             ],
             "invoice_number": {
                 "label_location": [
                     5,
@@ -353,56 +371,114 @@
             },
             "start_cell": [
                 1,
                 1
             ],
             "supplier_area": {
                 "CUI": {
-                    "label_location": null,
-                    "label_value": null,
-                    "location": "external file (PartyLegalEntity -> CompanyID)",
-                    "value": "..."
+                    "label_location": [
+                        11,
+                        2
+                    ],
+                    "label_value": "CIF:",
+                    "location": [
+                        11,
+                        3
+                    ],
+                    "value": "42561459"
                 },
                 "IBAN": {
-                    "location": "external file (Contact -> IBAN)",
-                    "value": "..."
+                    "label_location": [
+                        17,
+                        2
+                    ],
+                    "label_value": "Cont:",
+                    "location": [
+                        17,
+                        3
+                    ],
+                    "value": "RO29 BTRL RONC RT05 5704 8601"
                 },
                 "PostalAddress": {
                     "cac_Country": {
                         "cbc_IdentificationCode": "RO"
                     },
-                    "cbc_CityName": "...",
-                    "cbc_PostalZone": "...",
-                    "cbc_StreetName": "..."
+                    "cbc_CityName": "",
+                    "cbc_PostalZone": "",
+                    "cbc_StreetName": "Nicolae Titulescu, nr 81-87, Bucure\u015fti, Sector 1"
                 },
                 "RegistrationName": {
-                    "label_location": null,
-                    "label_value": null,
-                    "location": "external file (PartyLegalEntity -> CompanyID)",
-                    "value": "..."
+                    "label_location": "n/a",
+                    "label_value": "n/a",
+                    "location": [
+                        9,
+                        2
+                    ],
+                    "value": "REN-CONSULTING SOFT ACTIVITY SRL"
                 },
                 "area_info": {
-                    "location": "external file",
-                    "value": "/home/petre/api_to_roefact/xl2roefact/xl2roefact/data/owner.yml"
+                    "location": [
+                        [
+                            8,
+                            2
+                        ],
+                        [
+                            17,
+                            3
+                        ]
+                    ],
+                    "value": "Furnizor"
                 },
                 "bank": {
-                    "location": "external file (Contact -> Bank)",
-                    "value": "..."
+                    "label_location": [
+                        16,
+                        2
+                    ],
+                    "label_value": "Banca:",
+                    "location": [
+                        16,
+                        3
+                    ],
+                    "value": "Banca Transilvania"
                 },
                 "email": {
-                    "location": "external file (Contact -> ElectronicMail)",
-                    "value": null
+                    "label_location": [
+                        14,
+                        2
+                    ],
+                    "label_value": "Email:",
+                    "location": [
+                        14,
+                        3
+                    ],
+                    "value": "renware.systems@gmail.com"
                 },
                 "phone": {
-                    "location": "external file (Contact -> Telephone)",
-                    "value": null
+                    "label_location": [
+                        15,
+                        2
+                    ],
+                    "label_value": "Tel:",
+                    "location": [
+                        15,
+                        3
+                    ],
+                    "value": "0744-68.48.76"
                 },
                 "reg_com": {
-                    "location": "external file (PartyLegalEntity -> CompanyID)",
-                    "value": "..."
+                    "label_location": [
+                        10,
+                        2
+                    ],
+                    "label_value": "Reg. com.: ",
+                    "location": [
+                        10,
+                        3
+                    ],
+                    "value": "J40/5662/2020"
                 }
             }
         },
         "invoice_items_area": {
             "data": [
                 [
                     "Elaborare documentatie tehnica aplicatie NEXGEN.AI",
@@ -483,15 +559,15 @@
         "invoice_max_rows": 31,
         "invoice_worksheet": "FACTURA FINALA",
         "items_table_start_cell": [
             20,
             1
         ],
         "items_table_start_marker": "#",
-        "last_processing_time": "2024-04-04T08:23:19.886397+00:00",
+        "last_processing_time": "2024-04-18T04:10:02.876450+00:00",
         "map_JSONkeys_XMLtags": [
             [
                 "cac_InvoiceLine",
                 "cac:InvoiceLine"
             ],
             [
                 "cac_Item",
@@ -546,14 +622,18 @@
                 "cbc:DocumentCurrencyCode"
             ],
             [
                 "cbc_IssueDate",
                 "cbc:IssueDate"
             ],
             [
+                "cbc_DueDate",
+                "cbc:DueDate"
+            ],
+            [
                 "cac_AccountingCustomerParty",
                 "cac:AccountingCustomerParty"
             ],
             [
                 "cac_Party",
                 "cac:Party"
             ],
@@ -664,11 +744,47 @@
             [
                 "cac_AccountingSupplierParty",
                 "cac:AccountingSupplierParty"
             ],
             [
                 "cac_PartyTaxScheme",
                 "cac:PartyTaxScheme"
+            ],
+            [
+                "cbc_DueDate",
+                "cbc:DueDate"
+            ],
+            [
+                "cbc_InvoiceTypeCode",
+                "cbc:InvoiceTypeCode"
+            ],
+            [
+                "cbc_Note",
+                "cbc:Note"
+            ],
+            [
+                "cbc_TaxPointDate",
+                "cbc:TaxPointDate"
+            ],
+            [
+                "cac_Delivery",
+                "cac:Delivery"
+            ],
+            [
+                "cbc_ActualDeliveryDate",
+                "cbc:ActualDeliveryDate"
+            ],
+            [
+                "cac_PaymentMeans",
+                "cac:PaymentMeans"
+            ],
+            [
+                "cbc_PaymentMeansCode",
+                "cbc:PaymentMeansCode"
+            ],
+            [
+                "cbc_TaxPointDate",
+                "cbc:TaxPointDate"
             ]
         ]
     }
 }
```

### Comparing `xl2roefact-0.5.4/tests/fact_RENF1004.xlsx` & `xl2roefact-0.6rc0/tests/fact_RENF1004.xlsx`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.4/xl2roefact/__init__.py` & `xl2roefact-0.6rc0/xl2roefact/__init__.py`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.4/xl2roefact/__main__.py` & `xl2roefact-0.6rc0/xl2roefact/__main__.py`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.4/xl2roefact/__version__.py` & `xl2roefact-0.6rc0/xl2roefact/__version__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  #  #  ##    ##          #      # #  #     #  ##  # ##    ##   #  #
 ####   #  ######           ######## ####     ########  ######    ####
 ```
 """
 
 import packaging.utils
 
-__version__ = "0.5.4"  # prev release "0.5.3rc1"
+__version__ = "0.6rc0"  # current 0.6rc0, previous 0.5.4
 
 
 def normalized_version(
     raw_version: str = __version__
 ) -> str:
     """transform version string in canonical form.
```

### Comparing `xl2roefact-0.5.4/xl2roefact/app_cli.py` & `xl2roefact-0.6rc0/xl2roefact/app_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! /usr/bin/env python
+#! /usr/bin/env python3
 """app_cli: the command line application for all xl2roefact functionalities.
 
 Identification:
 
 * copyright: (c) 2023 RENWare Software Systems
 * author: Petre Iordanescu (petre.iordanescu@gmail.com)
 """
@@ -26,14 +26,15 @@
 from xl2roefact.libutils import hier_get_data_file
 import xl2roefact.config_settings as configs  # configuration elements to use with `settings` command
 from xl2roefact.rdinv import rdinv  # status #TODO: wip...
 from xl2roefact.wrxml import wrxml  # status #FIXME: not yet started
 from xl2roefact.chkxml import chkxml  # status #FIXME: not yet started
 from xl2roefact.ldxml import ldxml  # status #FIXME: not yet started
 from xl2roefact.chkisld import chkisld  # status #FIXME: not yet started
+from xl2roefact import sys_settings
 
 
 
 """ CLI builder section.
 """
 app_cli = typer.Typer(name="xl2roefact")
```

### Comparing `xl2roefact-0.5.4/xl2roefact/chkisld.py` & `xl2roefact-0.6rc0/xl2roefact/chkisld.py`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.4/xl2roefact/chkxml.py` & `xl2roefact-0.6rc0/xl2roefact/chkxml.py`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.4/xl2roefact/config_settings.py` & `xl2roefact-0.6rc0/xl2roefact/config_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Configuration and setting parameters.
 
 Regulile recomandate se gasessc in documentul (recommended rules are in document `xl2roefact/data/README_app_config_rules.md`)
 
 Public objects:
 
 * `rules_content`: contains the rules text (rendered)
-
-Info:
+
+Info:
 
 * copyright: (c) 2023 RENWare Software Systems
 * author: Petre Iordanescu (petre.iordanescu@gmail.com)
 """
 
 from pathlib import Path
 import os
@@ -48,14 +48,18 @@
 # aceste constante sunt utilizate ca si tara implicita pentru "parterii" facturilor in condtiile in care tarile "parterilor" nu sunt gasite
 # in mod explicit pe factura (in zona de adresa). Prin sintagma "partener" pe factura sa intelege oricare din cele doua parti implicate in
 # procesul de facturare, si anume: FURNIZORUL si CLIENTUL
 DEFAULT_CUSTOMER_COUNTRY: str = "RO"
 # ...and the corresponding one for supplier
 DEFAULT_SUPPLIER_COUNTRY: str = "RO"
 
+#--- scadenta implicita
+# scadenta implicita a facturii (in zile calendaristice) daca nu estrecuta in clar pe factura
+DEFAULT_DUE_DATE_DAYS: int = 30
+
 
 """---------------------------------------------------------------------------------------------------------------------------
 # NOTE: "pattern-uri" (sabloane) de identificare si regasire a datelor folositi de
 #   comanda `xl2json` reprezentind functionalitatea de extragere a datelor din Excel si exportul lor in formatul JSON (modulul `rdinv)
 ---------------------------------------------------------------------------------------------------------------------------"""
 
 # --- contine secventele de caractere care permit inceputul zonei (sub-tabelului) ce contine liniile facturii
@@ -175,14 +179,21 @@
 ]
 
 # --- numele legal al companiei furnizoare
 # pattern utilizat pentru regasirea numelui legal al furnizorului
 # NOTE se presupune a fi la inceputul zonei cu datele furnizorului, deci se ca cauta dupa acelasi pattern
 PATTERN_FOR_SUPPLIER_LEGAL_NAME = PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER
 
+# --- data scadentei
+# pattern utilizat pentru regasirea datei scadentei facturii
+PATTERN_FOR_DUE_DATE = [
+    "scad", "termen plat", "termen de plat"
+    "due da", "date due"
+]
+
 
 
 
 # ------- NOTE: the following code runs unconditionally at module import
 
 # section to read settings from external data file
 file_to_use = hier_get_data_file("app_settings.yml")
@@ -193,10 +204,13 @@
     print("***INFO: Application settings loaded from file.")
 # assign `python_object` to locals() environment...
 if python_object is not None:  # ...only if previous method has read something
     locals().update(python_object)
 else:  # if nothing or wrong read from previous method, settings applied will remain to values hard-coded in this module
     print("***INFO: Application settings loaded from application code (default settings).")
 
-
+# prepare `rules_content` public variable to be use as "mini help" by `settings -r` command of application
+rules_content = ""  # initialize with empty string to show nothing in case is a problem with file reading
+rules_file = hier_get_data_file("README_app_config_rules.md")
+rules_content = Markdown(rules_file.read_text())
```

### Comparing `xl2roefact-0.5.4/xl2roefact/data/README_app_config_rules.md` & `xl2roefact-0.6rc0/xl2roefact/data/README_app_config_rules.md`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.4/xl2roefact/data/app_settings.yml` & `xl2roefact-0.6rc0/xl2roefact/data/app_settings.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,27 @@
 # este utilizat de catre aplicatie in toate conditiile in care unitatea de masura unui produs sau serviciu (liniile facturii) nu este cunoscuta
 # unitatea de masura este considerta necunoscuta atunci cind este lasata 'blank' sau pur si simplu celula respectiva este goala
 DEFAULT_UNKNOWN_UOM: null
 
 # --- moneda implicita
 # este utilizat de catre aplicatie in toate conditiile in care pe factura nu este specifcata in clar o moneda
 # specifcarea monedei ca sau in titlurile coloanelor nu este luata in considerare (nu este garantat ca este moneda reala a facturii !)
-# --- TIPUL INFORMATIEI; ...
 DEFAULT_CURRENCY: "RON"
 
 # --- tara implicita
 # aceste constante sunt utilizate ca si tara implicita pentru "parterii" facturilor in condtiile in care tarile "parterilor" nu sunt gasite
 # in mod explicit pe factura (in zona de adresa). Prin sintagma "partener" pe factura sa intelege oricare din cele doua parti implicate in
 # procesul de facturare, si anume: FURNIZORUL si CLIENTUL
-# --- TIPUL INFORMATIEI; ...
 DEFAULT_CUSTOMER_COUNTRY: "RO"
 DEFAULT_SUPPLIER_COUNTRY: "RO"
 
+#--- scadenta implicita
+# scadenta implicita a facturii (in zile calendaristice) daca nu estrecuta in clar pe factura
+DEFAULT_DUE_DATE_DAYS: 30
+
 
 #---------------------------------------------------------------------------------------------------------------------------
 # NOTE: "pattern-uri" (sabloane) de identificare si regasire a datelor folositi de
 #   comanda `xl2json` reprezentind functionalitatea de extragere a datelor din Excel si exportul lor in formatul JSON (modulul `rdinv)
 #---------------------------------------------------------------------------------------------------------------------------
 
 # --- contine secventele de caractere care permit inceputul zonei (sub-tabelului) ce contine liniile facturii
@@ -166,8 +168,15 @@
 ]
 
 # --- numele legal al companiei furnizoare
 # pattern utilizat pentru regasirea numelui legal al furnizorului
 # NOTE se presupune a fi la inceputul zonei cu datele furnizorului, deci se ca cauta dupa acelasi pattern
 PATTERN_FOR_SUPPLIER_LEGAL_NAME: *patt_suppl_marker
 
+# --- data scadentei
+# pattern utilizat pentru regasirea datei scadentei facturii
+PATTERN_FOR_DUE_DATE: [
+    "scad", "termen plat", "termen de plat",
+    "due da", "date due",
+]
+
```

### Comparing `xl2roefact-0.5.4/xl2roefact/ldxml.py` & `xl2roefact-0.6rc0/xl2roefact/ldxml.py`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.4/xl2roefact/libutils.py` & `xl2roefact-0.6rc0/xl2roefact/libutils.py`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.4/xl2roefact/rdinv.py` & `xl2roefact-0.6rc0/xl2roefact/rdinv.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,1115 +1,1173 @@
-"""rdinv: modul de procesare a fisierului Excel ce contine factura si colectare a datelor aferente.
-
-Formatul acceptat fisier Excel este `XLSX`.
-
-Identification:
-
-* code-name: `rdinv`
-* copyright: (c) 2023 RENWare Software Systems
-* author: Petre Iordanescu (petre.iordanescu@gmail.com)
-
-Specifications:
-
-* document cerinte initiale: `110-SRE-api_to_roefact_requirements.md` section `Componenta xl2roefact`
-* INTRARI: fisier format XLSX ce contine factura emisa (cod: `f-XLSX`)
-* IESIRI: fisier format JSON imagine a datelor facturii (cod: `f-JSON`)
-"""
-
-import os, sys
-from datetime import datetime, timezone, tzinfo
-from rich import print
-import copy
-from rich.pretty import pprint
-from string import ascii_lowercase
-import json
-import yaml
-from typing import Callable, Any
-from functools import partial
-from pathlib import Path
-import pylightxl as xl
-import openpyxl as opnxl
-
-# local modules (part of package), application misc/general utilities
-from .libutils import isnumber
-from .libutils import find_str_in_list
-from .libutils import dict_sum_by_key
-from .libutils import invoice_taxes_summary
-from .libutils import hier_get_data_file
-from . import config_settings  # application configuration parameters
-
-__all__ = ["rdinv"]  # limit what symbols to be available when import all/full module as `from xl2roefact.rdinv import *`
-
-# local constants. Change them with caution only for a functional objective
-SYS_FILLED_EMPTY_CELL = "_sys_keep_cell"
-
-# imported constants (NOTE: some are subject to change values as reading Excel file - these will be declared as `global` in function that will change them)
-DEFAULT_VAT_PERCENT = config_settings.DEFAULT_VAT_PERCENT
-DEFAULT_UNKNOWN_ITEM_NAME = config_settings.DEFAULT_UNKNOWN_ITEM_NAME
-DEFAULT_UNKNOWN_UOM = config_settings.DEFAULT_UNKNOWN_UOM
-DEFAULT_CURRENCY = config_settings.DEFAULT_CURRENCY
-DEFAULT_CUSTOMER_COUNTRY = config_settings.DEFAULT_CUSTOMER_COUNTRY
-DEFAULT_SUPPLIER_COUNTRY = config_settings.DEFAULT_SUPPLIER_COUNTRY
-PATTERN_FOR_INVOICE_ITEMS_SUBTABLE_MARKER = config_settings.PATTERN_FOR_INVOICE_ITEMS_SUBTABLE_MARKER
-PATTERN_FOR_INVOICE_NUMBER_LABEL = config_settings.PATTERN_FOR_INVOICE_NUMBER_LABEL
-PATTERN_FOR_INVOICE_CURRENCY_LABEL = config_settings.PATTERN_FOR_INVOICE_CURRENCY_LABEL
-PATTERN_FOR_INVOICE_ISSUE_DATE_LABEL = config_settings.PATTERN_FOR_INVOICE_ISSUE_DATE_LABEL
-PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER = config_settings.PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER
-PATTERN_FOR_INVOICE_CUSTOMER_SUBTABLE_MARKER = config_settings.PATTERN_FOR_INVOICE_CUSTOMER_SUBTABLE_MARKER
-PATTERN_FOR_PARTNER_ID = config_settings.PATTERN_FOR_PARTNER_ID
-PATTERN_FOR_CUSTOMER_LEGAL_NAME = config_settings.PATTERN_FOR_CUSTOMER_LEGAL_NAME
-PATTERN_FOR_PARTNER_ADDRESS = config_settings.PATTERN_FOR_PARTNER_ADDRESS
-PATTERN_FOR_PARTNER_ADDRESS_COUNTRY = config_settings.PATTERN_FOR_PARTNER_ADDRESS_COUNTRY
-PATTERN_FOR_PARTNER_ADDRESS_CITY = config_settings.PATTERN_FOR_PARTNER_ADDRESS_CITY
-PATTERN_FOR_PARTNER_ADDRESS_STREET = config_settings.PATTERN_FOR_PARTNER_ADDRESS_STREET
-PATTERN_FOR_PARTNER_ADDRESS_ZIPCODE = config_settings.PATTERN_FOR_PARTNER_ADDRESS_ZIPCODE
-PATTERN_FOR_PARTNER_EMAIL = config_settings.PATTERN_FOR_PARTNER_EMAIL
-PATTERN_FOR_PARTNER_TEL = config_settings.PATTERN_FOR_PARTNER_TEL
-PATTERN_FOR_PARTNER_IBAN = config_settings.PATTERN_FOR_PARTNER_IBAN
-PATTERN_FOR_PARTNER_BANK = config_settings.PATTERN_FOR_PARTNER_BANK
-PATTERN_FOR_PARTNER_REGCOM = config_settings.PATTERN_FOR_PARTNER_REGCOM
-PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER = config_settings.PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER
-PATTERN_FOR_SUPPLIER_LEGAL_NAME = config_settings.PATTERN_FOR_SUPPLIER_LEGAL_NAME
-
-
-def rdinv(
-    file_to_process: str,
-    invoice_worksheet_name: str = None,
-    *,
-    debug_info: bool = False,
-    owner_datafile: Path = None
-) -> dict:
-    """read Excel file for invoice data.
-
+"""rdinv: modul de procesare a fisierului Excel ce contine factura si colectare a datelor aferente.
+
+Formatul acceptat fisier Excel este `XLSX`.
+
+Identification:
+
+* code-name: `rdinv`
+* copyright: (c) 2023 RENWare Software Systems
+* author: Petre Iordanescu (petre.iordanescu@gmail.com)
+
+Specifications:
+
+* document cerinte initiale: `110-SRE-api_to_roefact_requirements.md` section `Componenta xl2roefact`
+* INTRARI: fisier format XLSX ce contine factura emisa (cod: `f-XLSX`)
+* IESIRI: fisier format JSON imagine a datelor facturii (cod: `f-JSON`)
+"""
+
+import os, sys
+from datetime import datetime, timezone, tzinfo, timedelta
+from rich import print
+import copy
+from rich.pretty import pprint
+from string import ascii_lowercase
+import json
+import yaml
+from typing import Callable, Any
+from functools import partial
+from pathlib import Path
+import pylightxl as xl
+import openpyxl as opnxl
+
+# local modules (part of package), application misc/general utilities
+from .libutils import isnumber
+from .libutils import find_str_in_list
+from .libutils import dict_sum_by_key
+from .libutils import invoice_taxes_summary
+from .libutils import hier_get_data_file
+from . import config_settings  # application configuration parameters
+
+__all__ = ["rdinv"]  # limit what symbols to be available when import all/full module as `from xl2roefact.rdinv import *`
+
+# local constants. Change them with caution only for a functional objective
+SYS_FILLED_EMPTY_CELL = "_sys_keep_cell"
+
+# imported constants (NOTE: some are subject to change values as reading Excel file - these will be declared as `global` in function that will change them)
+DEFAULT_VAT_PERCENT = config_settings.DEFAULT_VAT_PERCENT
+DEFAULT_UNKNOWN_ITEM_NAME = config_settings.DEFAULT_UNKNOWN_ITEM_NAME
+DEFAULT_UNKNOWN_UOM = config_settings.DEFAULT_UNKNOWN_UOM
+DEFAULT_CURRENCY = config_settings.DEFAULT_CURRENCY
+DEFAULT_CUSTOMER_COUNTRY = config_settings.DEFAULT_CUSTOMER_COUNTRY
+DEFAULT_SUPPLIER_COUNTRY = config_settings.DEFAULT_SUPPLIER_COUNTRY
+DEFAULT_DUE_DATE_DAYS = config_settings.DEFAULT_DUE_DATE_DAYS
+PATTERN_FOR_INVOICE_ITEMS_SUBTABLE_MARKER = config_settings.PATTERN_FOR_INVOICE_ITEMS_SUBTABLE_MARKER
+PATTERN_FOR_INVOICE_NUMBER_LABEL = config_settings.PATTERN_FOR_INVOICE_NUMBER_LABEL
+PATTERN_FOR_INVOICE_CURRENCY_LABEL = config_settings.PATTERN_FOR_INVOICE_CURRENCY_LABEL
+PATTERN_FOR_INVOICE_ISSUE_DATE_LABEL = config_settings.PATTERN_FOR_INVOICE_ISSUE_DATE_LABEL
+PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER = config_settings.PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER
+PATTERN_FOR_INVOICE_CUSTOMER_SUBTABLE_MARKER = config_settings.PATTERN_FOR_INVOICE_CUSTOMER_SUBTABLE_MARKER
+PATTERN_FOR_PARTNER_ID = config_settings.PATTERN_FOR_PARTNER_ID
+PATTERN_FOR_CUSTOMER_LEGAL_NAME = config_settings.PATTERN_FOR_CUSTOMER_LEGAL_NAME
+PATTERN_FOR_PARTNER_ADDRESS = config_settings.PATTERN_FOR_PARTNER_ADDRESS
+PATTERN_FOR_PARTNER_ADDRESS_COUNTRY = config_settings.PATTERN_FOR_PARTNER_ADDRESS_COUNTRY
+PATTERN_FOR_PARTNER_ADDRESS_CITY = config_settings.PATTERN_FOR_PARTNER_ADDRESS_CITY
+PATTERN_FOR_PARTNER_ADDRESS_STREET = config_settings.PATTERN_FOR_PARTNER_ADDRESS_STREET
+PATTERN_FOR_PARTNER_ADDRESS_ZIPCODE = config_settings.PATTERN_FOR_PARTNER_ADDRESS_ZIPCODE
+PATTERN_FOR_PARTNER_EMAIL = config_settings.PATTERN_FOR_PARTNER_EMAIL
+PATTERN_FOR_PARTNER_TEL = config_settings.PATTERN_FOR_PARTNER_TEL
+PATTERN_FOR_PARTNER_IBAN = config_settings.PATTERN_FOR_PARTNER_IBAN
+PATTERN_FOR_PARTNER_BANK = config_settings.PATTERN_FOR_PARTNER_BANK
+PATTERN_FOR_PARTNER_REGCOM = config_settings.PATTERN_FOR_PARTNER_REGCOM
+PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER = config_settings.PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER
+PATTERN_FOR_SUPPLIER_LEGAL_NAME = config_settings.PATTERN_FOR_SUPPLIER_LEGAL_NAME
+PATTERN_FOR_DUE_DATE = config_settings.PATTERN_FOR_DUE_DATE
+
+
+def rdinv(
+    file_to_process: str,
+    invoice_worksheet_name: str = None,
+    *,
+    debug_info: bool = False,
+    owner_datafile: Path = None
+) -> dict:
+    """read Excel file for invoice data.
+
     Produce a dictionary structure + JSON file with all data regarding read invoice: canonical KV data, meta data, map to convert to XML and original Excel data.
 
     Args:
-
-        `file_to_process`: the invoice file (exact file with path).
-        `invoice_worksheet_name`: the worksheet containing invoice, optional, defaults to first found worksheet.
-        `debug_info`: key only, show debugging information, default `False`.
-        `owner_datafile`: specify a file to read supplier data from, default `None` meaning to read supplier data from Excel file
-
-    Return:
-    
+
+        `file_to_process`: the invoice file (exact file with path).
+        `invoice_worksheet_name`: the worksheet containing invoice, optional, defaults to first found worksheet.
+        `debug_info`: key only, show debugging information, default `False`.
+        `owner_datafile`: specify a file to read supplier data from, default `None` meaning to read supplier data from Excel file
+
+    Return:
+    
         `dict`: the invoice extracted information from Excel file as `dict(Invoice: dict, meta_info: dict, excel_original_data: dict)`
 
     Notes:
-
-    * `db: pylightxl object`: EXCEL object with invoice (as a whole)
-    * `ws: pylightxl object`: WORKSHEET object with invoice
-    """
-    # use as global only for those constants that could be changed by this function
-    global DEFAULT_VAT_PERCENT
-    global DEFAULT_UNKNOWN_ITEM_NAME
-    global DEFAULT_UNKNOWN_UOM
-    global DEFAULT_CURRENCY
-    global DEFAULT_SUPPLIER_COUNTRY
-    global DEFAULT_CUSTOMER_COUNTRY
-
-    print(f"*** Module [red]rdinv[/] started at {datetime.now()} to process file [green]{os.path.split(file_to_process)[1]}[/] (full path: {file_to_process})")
-
-    # read Excel file with Invoice data
-    try:
-        db = xl.readxl(fn=file_to_process)
-    except:
-        print(f"[red]---***FATAL ERROR - Cannot open Excel file {file_to_process} (possible problems: file corrupted, wrong type only XLSX accetpted, file does not exists or was deleted, operating system vilotation) in Module [red] RDINV (code-name: `rdinv`). File processing terminated[/]")
-        return False
-
-    # read the workshet with Invoice data
-    if invoice_worksheet_name is None:  # if parameter `invoice_worksheet_name` not specified try to open first worksheet from Excel worksheets - order is given by worksheets order in Excel file
-        list_of_excel_worksheets = db.ws_names
-        print(f"[yellow]INFO note:[/] `rdinv` module, no worksheet specified, will open first one: [cyan]'{list_of_excel_worksheets[0]}'[/]")
-        invoice_worksheet_name = list_of_excel_worksheets[0]
-
-    try:
-        ws = db.ws(invoice_worksheet_name)
-    except:
-        print(f"[red]***FATAL ERROR - Cannot open Excel specified Worksheet \"{invoice_worksheet_name}\" in Module [red] RDINV (code-name: `rdinv`). File processing terminated[/]")
-        return False
-
-    """#NOTE: section for search of `invoice_items_area: pylightxl.ssd`
-        - main result: `keyword_for_items_table_marker` = string marker to search for in oredr to isolate `invoice_items_area`
-        - other results: `_found_cell_for_invoice_items_area_marker = (row, col, val)`
-    """
-    _tmp_label_info = get_excel_data_at_label(
-        pattern_to_search_for=PATTERN_FOR_INVOICE_ITEMS_SUBTABLE_MARKER,
-        worksheet=ws,
-        targeted_type=str
-    )
-    if _tmp_label_info["label_value"]:  # only if found a potential cell usable as`invoice_items_area_marker`
-        _found_cell_for_invoice_items_area_marker = (
-            _tmp_label_info["label_location"][0],
-            _tmp_label_info["label_location"][1],
-            _tmp_label_info["label_value"]
-        )  # here you still need to construct `_found_cell_for_invoice_items_area_marker = (row, col, val)` as it is used in prev code (before `231220piu_a` change)
-    else:
-        print(f"[red]***FATAL ERROR - Cannot find a relevant cell where invoice items table start (basically containing string \" crt\"). File processing terminated[/]")
-        return False
-    keyword_for_items_table_marker = _found_cell_for_invoice_items_area_marker[2]
-
-    # detect all cells that should be filled with SYS_FILLED_EMPTY_CELL (these are cells id merged groups where first cell in merged group is relevant (diff from empty))
-    detected_cells_which_will_be_fake_filled = get_merged_cells_tobe_changed(
-        file_to_scan=file_to_process,
-        invoice_worksheet_name=invoice_worksheet_name,
-        keep_cells_of_items_ssd_marker=_found_cell_for_invoice_items_area_marker)  # this call specify to keep unchanged that cells with some description
-    for _cell_index in detected_cells_which_will_be_fake_filled:  # scan all detectected cell and change them
-        _cell_row = _cell_index[0]
-        _cell_col = _cell_index[1]
-        ws.update_index(row = _cell_row, col = _cell_col, val = SYS_FILLED_EMPTY_CELL)
-
-    """#NOTE: section to "solve" `invoice_items_area`. Steps:
-        - process it as Excel format (row & colymns tabular organization)
-        - transform it in "canonical JSON format" (as kv pairs) and update `cac_InvoiceLine` key
-    """
-    # process invoice to detect its items / lines ('invoice_items_area'), clean and extract data
-    invoice_items_area = get_invoice_items_area(
-        worksheet=ws,
-        invoice_items_area_marker=keyword_for_items_table_marker,
-        wks_name=invoice_worksheet_name
-    )
-
-    """#NOTE: section for localize areas: invoice header (`invoice_header_area`) & invoice footer (`invoice_footer_area`)
-        NOTE: its code suppose `invoice_items_area` is already defined (as location). It will be used as reference in "header" & "footer" localization logic
-    """
-    ulc_header = (1, 1)
-    lrc_header = (_found_cell_for_invoice_items_area_marker[0] - 1, ws.size[1],)  # info where header ends: row = from items data table start location `_found_cell_for_invoice_items_area_marker[0]-1` && col = las col of worksheet
-    invoice_header_area = dict(
-        start_cell = ulc_header,
-        end_cell = lrc_header
-    )
-    #
-    _ulc_footer_row = _found_cell_for_invoice_items_area_marker[0] + len(invoice_items_area["keyrows"]) + 1  # this is located at: row = items data table start row  (_found_cell_for_invoice_items_area_marker[0]) + # of items data table rows + 1 (invoice_items_area["data"]) && col = 1
-    _start_cell_val = ws.index(_ulc_footer_row, 1)
-    while (_start_cell_val != "") and (_ulc_footer_row <= ws.size[0]): # but if that cell is not blank repeatedly to go une more row down... (why could happen? because ietms data table header was composed of more rows by merging cells...)
-        _ulc_footer_row += 1
-        _start_cell_val = ws.index(_ulc_footer_row, 1)
-    ulc_footer = (_ulc_footer_row, 1)
-    lrc_footer =( ws.size[0], ws.size[1])  # end of worksheet
-    invoice_footer_area = dict(
-        start_cell = ulc_footer,
-        end_cell = lrc_footer
-    )
-
-    """#NOTE: section to "solve" `invoice_header_area`.
-            The kind of info expected in this area: invoice number,  currency, issued date, supplier data, customer data)
-    """
-    invoice_header_area = invoice_header_area | dict(  # build effective data area & merge localization info from initial dict creation
-        invoice_number = None,
-        issued_date = None,
-        currency = None,
-        customer_area = None,
-        supplier_area = None,
-    )
-    _area_to_search = (invoice_header_area["start_cell"], invoice_header_area["end_cell"])  # this is "global" for this section (corners of `invoice_header_area`)
-    #
-    # find invoice number ==> `cbc:ID`
-    invoice_number_info = get_excel_data_at_label(
-        pattern_to_search_for=PATTERN_FOR_INVOICE_NUMBER_LABEL,
-        worksheet=ws,
-        area_to_scan=_area_to_search,
-        targeted_type=str
-    )  # returned info: `{"value": ..., "location": (row..., col...)}`
-    invoice_header_area["invoice_number"] = copy.deepcopy(invoice_number_info)
-    #
-    # find invoice currency ==> `cbc:DocumentCurrencyCode`
-    invoice_currency_info = get_excel_data_at_label(
-        pattern_to_search_for=PATTERN_FOR_INVOICE_CURRENCY_LABEL,
-        worksheet=ws,
-        area_to_scan=_area_to_search,
-        targeted_type=str
-    )  # returned info: `{"value": ..., "location": (row..., col...)}`
-    if (invoice_currency_info["value"] is not None) and (invoice_currency_info["value"] != ""):  # if found a currency MUST CHANGE `DEFAULT_CURRENCY` to be properly used for `invoice_items_area`
-        DEFAULT_CURRENCY = invoice_currency_info["value"]
-    invoice_header_area["currency"] = copy.deepcopy(invoice_currency_info)
-    #
-    # find invoice issued date ==> `cbc:IssueDate`
-    issued_date_info = get_excel_data_at_label(
-        pattern_to_search_for=PATTERN_FOR_INVOICE_ISSUE_DATE_LABEL,
-        worksheet=ws,
-        area_to_scan=_area_to_search,
-        targeted_type=str
-    )  # returned info: `{"value": ..., "location": (row..., col...)}`
-    issued_date_info["value"] = issued_date_info["value"].replace("/", "-")  # convert from Excel format: YYYY/MM/DD (ex: 2023/08/28) to required format in XML file is: `YYYY-MM-DD` (ex: 2013-11-17)
-    invoice_header_area["issued_date"] = copy.deepcopy(issued_date_info)
-    #
-    # get and solve `invoice_header_area` for all CUSTOMER data
-    _ = get_partner_data(
-        partner_type="CUSTOMER",
-        wks=ws,
-        param_invoice_header_area=invoice_header_area
-    )
-    #
-    # get and solve `invoice_header_area` for all SUPPLIER data
-    if owner_datafile is None:  # get supplier data from Excel file
-        _ = get_partner_data(
-            partner_type="SUPPLIER",
-            wks=ws,
-            param_invoice_header_area=invoice_header_area
-        )
-    else:  # get supplier data from `owner-data-file`
-        _ = get_partner_data(
-            partner_type="OWNER",
-            wks=ws,
-            param_invoice_header_area=invoice_header_area,
-            supplier_datafile=owner_datafile
-        )
-    #
-    # TODO: ... mai sunt ai cele "pre-stabilite" in versiunea curenta, gen `cbc:InvoiceTypeCode = 380`. SEE ALSO line 331
-
-    """#NOTE: section to ( Excel data )--->( JSON ) format preparation and finishing
-        this is required to be after header determination (because CURRENCY could be known here and will impact config param `DEFAULT_CURRENCY`)
-    """
-    # transform `invoice_items_area` in "canonical JSON kv pairs format" (NOTE this step is done only for invoice_items_area and is required because this section is "table with more rows", ie, not a simple key-val)
-    invoice_items_as_kv_pairs = mk_kv_invoice_items_area(invoice_items_area_xl_format=invoice_items_area)
-
-    # preserve processed Excel file meta information: start address, size.
-    meta_info = build_meta_info_key(
-        excel_file_to_process=file_to_process,
-        invoice_worksheet_name=invoice_worksheet_name,
-        ws_size=tuple(ws.size),
-        keyword_for_items_table_marker=keyword_for_items_table_marker,
-        found_cell=tuple(_found_cell_for_invoice_items_area_marker))
-
-    # build final structure to be returned (`invoice`) - MAIN OBJECTIVE of this function
-    tmp_InvoiceLine_list = [_i for _i in invoice_items_as_kv_pairs],  # `invoice_items_as_kv_pairs` is list of dicts with keys as XML RO E-Fact standard
-    tmp_reusable_items = dict(
-        cbc_LineExtensionAmount = sum([dict_sum_by_key(i, "cbc_LineExtensionAmount") for i in tmp_InvoiceLine_list]),
-        LineVatAmount = sum([dict_sum_by_key(i, "LineVatAmount") for i in tmp_InvoiceLine_list]),
-    )  # reusable calculations to be used in next code. see details in issue `0.3.0b+240302piu01`
-    tmp_cac_TaxSummary = invoice_taxes_summary(tmp_InvoiceLine_list)  # invoke invoice tax summary calculation
-    invoice = {
-        "Invoice": {
-            "cbc_ID": copy.deepcopy(invoice_header_area["invoice_number"]["value"]),  # invoice number as `cbc_ID`
-            "cbc_DocumentCurrencyCode": copy.deepcopy(invoice_header_area["currency"]["value"]),  # invoice currency as `cbc_DocumentCurrencyCode`
-            "cbc_IssueDate": copy.deepcopy(invoice_header_area["issued_date"]["value"]),  # invoice issue date as `cbc_IssueDate`
-            "cac_AccountingCustomerParty": {
-                "cac_Party": {
-                    "cac_PartyLegalEntity": {
-                        "cbc_CompanyID": copy.deepcopy(invoice_header_area["customer_area"]["CUI"]["value"]),
-                        "cbc_RegistrationName": copy.deepcopy(invoice_header_area["customer_area"]["RegistrationName"]["value"]),
-                    },
-                    "cac_PostalAddress": copy.deepcopy(invoice_header_area["customer_area"]["PostalAddress"]),
-                    "cac_Contact": {
-                        "cbc_Telephone": copy.deepcopy(invoice_header_area["customer_area"]["phone"]["value"]),
-                        "cbc_ElectronicMail": copy.deepcopy(invoice_header_area["customer_area"]["email"]["value"]),
-                        "RegCom": copy.deepcopy(invoice_header_area["customer_area"]["reg_com"]["value"]),
-                        "Bank": copy.deepcopy(invoice_header_area["customer_area"]["bank"]["value"]),
-                        "IBAN": copy.deepcopy(invoice_header_area["customer_area"]["IBAN"]["value"]),
-                    },
-                },
-            },
-            "cac_AccountingSupplierParty": {
-                "cac_Party": {
-                    "cac_PartyLegalEntity": {
-                        "cbc_CompanyID": copy.deepcopy(invoice_header_area["supplier_area"]["CUI"]["value"]),
-                        "cbc_RegistrationName": copy.deepcopy(invoice_header_area["supplier_area"]["RegistrationName"]["value"]),
-                    },
-                    "cac_PostalAddress": copy.deepcopy(invoice_header_area["customer_area"]["PostalAddress"]),
-                    "cac_Contact": {
-                        "cbc_Telephone": copy.deepcopy(invoice_header_area["supplier_area"]["phone"]["value"]),
-                        "cbc_ElectronicMail": copy.deepcopy(invoice_header_area["supplier_area"]["email"]["value"]),
-                        "RegCom": copy.deepcopy(invoice_header_area["supplier_area"]["reg_com"]["value"]),
-                        "Bank": copy.deepcopy(invoice_header_area["supplier_area"]["bank"]["value"]),
-                        "IBAN": copy.deepcopy(invoice_header_area["supplier_area"]["IBAN"]["value"]),
-                    },
-                    "cac_PartyTaxScheme": {
-                        "cbc_CompanyID": copy.deepcopy(invoice_header_area["supplier_area"]["CUI"]["value"]),
-                        "cac_TaxScheme": {
-                            "cbc_ID": "VAT"
-                        },
-                    },
-                },
-            },
-            "cac_InvoiceLine": copy.deepcopy(tmp_InvoiceLine_list)[0],  # keep only 1st entry because from creating process resulted list(list)) first one being redundant
-            "cac_LegalMonetaryTotal": {
-                "cbc_LineExtensionAmount": round(tmp_reusable_items["cbc_LineExtensionAmount"], 2),
-                "cbc_TaxExclusiveAmount": round(tmp_reusable_items["cbc_LineExtensionAmount"], 2),
-                "cbc_TaxInclusiveAmount": round(tmp_reusable_items["cbc_LineExtensionAmount"] + tmp_reusable_items["LineVatAmount"], 2),
-                "cbc_PayableAmount": round(tmp_reusable_items["cbc_LineExtensionAmount"] + tmp_reusable_items["LineVatAmount"], 2),
-            },
-            "cac_TaxTotal": {
-                "cbc_TaxAmount": round(sum([i["cbc_TaxAmount"] if i["cbc_TaxAmount"] is not None else 0 for i in tmp_cac_TaxSummary]), 2),
-                "cac_TaxSubtotal": copy.deepcopy(tmp_cac_TaxSummary),
-            },
-            # TODO: ... chk for remained structure values and check XLM-JSON map. SEE ALSO line 254
-        },
-        "meta_info": copy.deepcopy(meta_info),
-        "excel_original_data": dict(
-            invoice_items_area = copy.deepcopy(invoice_items_area),  # NOTE ready, test PASS @ 231205 by [piu]
-            invoice_header_area = copy.deepcopy(invoice_header_area),  # NOTE ready, test PASS @ 2440326 by [piu]
-            invoice_footer_area = copy.deepcopy(invoice_footer_area)  #TODO wip... TBD-(cac_TaxTotal) / RDY-(cac_LegalMonetaryTotal
-        ),
-    }
-    #
-    # write `invoice` dict to file `f-JSON`
-    """ useful notes ref `f-JSON`:
-        - ref `f-JSON` file, see doc: `https://apitoroefact.renware.eu/commercial_agreement/110-SRE-api_to_roefact_requirements.html#vedere-de-ansamblu-a-solutiei`
-        - create `f-JSON` filename as Excel filename but with json extention
-        - helpers:
-                - os.path.split() gets @[0] directory & @[1] filename
-                - os.path.splitext() @[0] filename w/o ext, @[1] extention woth dot char included
-        - TODO: @231217 - writing a JSON file should be subject of option bool parameter in rdinv() with default value `True`
-    """
-    _fjson_filename = os.path.splitext(os.path.basename(file_to_process))[0] + ".json"
-    _fjson_fileobject = os.path.join(os.path.split(file_to_process)[0], _fjson_filename)
-    with open(_fjson_fileobject, 'w', encoding='utf-8') as _f:
-        json.dump(invoice, _f, ensure_ascii = False, indent = 4)
-    print(f"[yellow]INFO note:[/] `rdinv` module, written invoice JSON data to: [green]{_fjson_fileobject}[/]")
-
-    #TODO check for more TODOs, clean &&-->
-    #TODO wip...(@231125) TRANSFORM JSON FILE from Excel (row,col) format in a relational one (but respecting ROefact tags from used scheme)
-
-    return copy.deepcopy(invoice)
-
-
-
-
-
-
-# NOTE: ready, test PASS @ 231212 by [piu]
-def get_excel_data_at_label(
-    pattern_to_search_for: list[str],
-    worksheet: xl.Database.ws,
-    area_to_scan: list[list[int]] = None,
-    targeted_type: Callable = str,
-    down_search_try: bool = True
-) -> dict:
-    """get "one key Excel values", like invoice number or invoice issue date.
-
-    Args:
-    
-        `pattern_to_search_for`: for example for inv number, will pass the `PATTERN_FOR_INVOICE_NUMBER_LABEL`.
-        `worksheet`: the worksheet containing invoice (as object of `pyxllight` library).
-        `area_to_scan`: area of cells to be searched, default whole worksheet.
-        `targeted_type`: what type expect (will try to convert to, if cannot will return str), default `str`.
-        `down_search_try`: establish if DOWN search method is tried, default `True`.
-
-    Return:
-    
-        `None` if not found OR `dictionary` containing:
-            * `"value": int | float | str` - the value found covenrted to requested `targeted_type` if possible or `str` otherwise; if "out of space" then returns `None`
-            * `"location": (row, col)` - adrees of cell where found value
-
-    Notes:
-    
-    * normal scan order is 1.RIGHT, 2.DOWN (if allowed), 3.IN-LABEL only in given area and pattern.
-    """
-    def __check_value(val: Any) -> bool:
-        """ return `True` if a `val` is different of None or empty string or SYS_FILLED_EMPTY_CELL, otherwise return `False`
-        """
-        if val is None:
-            return False
-        if isinstance(val, str) and val.strip() == "":
-            return False
-        if val == SYS_FILLED_EMPTY_CELL:
-            return False
-        return True
-
-    if area_to_scan is None:  # if arg "passed" was default value then make it as the whole worksheet area
-        area_to_scan = ((1, 1), (worksheet.size[0], worksheet.size[1]))
-    ret_val = dict(  # initialize structure for what will return if information is found
-        value = None,
-        location = (None, None),
-        label_value = None,
-        label_location = None,
-    )
-    for i in range(area_to_scan[0][0], area_to_scan[1][0] + 1):
-        for j in range(area_to_scan[0][1], area_to_scan[1][1] + 1):
-            _crt_cell_val = [worksheet.index(i, j)]  # make it list to be iterable (of 1 element, but iterable)
-            # test if crt cell is in pattern_to_search_for
-            _found = find_str_in_list(list_of_str_to_find=pattern_to_search_for, list_to_search=_crt_cell_val)
-            if _found is not None:
-                if True:  # process label
-                    label_value = _crt_cell_val[0]  # preserve only first value (this will be next proccessed and if pass will remain)
-                    label_location = (i, j)
-                if True:  # process value
-                    value_found = None
-                    index_of_value_found = None
-                    # NOTE-LOGIC: test for RIGHT cell @(i,j+1) if cell exists in ws range AND if has a value then continue loop (to find other potential cell)
-                    if j < area_to_scan[1][1]:  # assure will remain in range of test area for next test (ie, exists cell @ (i, j+1))
-                        check_for_index = (i, j + 1)
-                        check_for = worksheet.index(check_for_index[0], check_for_index[1])
-                        if __check_value(check_for):
-                            value_found = check_for
-                            index_of_value_found = check_for_index
-                    # continue with DOWN test if NOT found somethinng at RIGHT and if this strategy is allowed to be used
-                    if down_search_try and not (value_found and index_of_value_found):  # try DOWN test only if method is allowed AND a relevant value not found or value is located in a wrong area
-                        # NOTE-LOGIC: test for DOWN cell @(i+1,j) if cell exists in ws range AND if has a value then continue loop (to find other potential cell)
-                        if i < area_to_scan[1][0] :  # if still in range if test (ie, exists cell @ (i+1, j))
-                            check_for_index = (i + 1, j)
-                            check_for = worksheet.index(check_for_index[0], check_for_index[1])
-                            if __check_value(check_for):
-                                value_found = check_for
-                                index_of_value_found = check_for_index
-                    # continue with IN-LABEL test if NOT found somethinng at DOWN
-                    if not (value_found and index_of_value_found):  # try IN-LABEL test only if a relevant value not found or value is located in a wrong area
-                        # NOTE-LOGIC: test for IN-LABEL cell (label is supposed only first word separated by space)
-                        check_for = label_value.strip()
-                        # keep all except first word (supposed to be label)
-                        if len(check_for) > 1:
-                            check_for = ' '.join(check_for.split()[1:])  # clean and keep all string except first word
-                        else:
-                            chech_for = ""
-                        if __check_value(check_for):
-                            value_found = check_for
-                            index_of_value_found = label_location
-                # create return dictionary for: label, value found, location of value foun
-                ret_val["label_value"] = label_value  # rule: if found a matching label, the label of info found will appear regardles of effective value found status
-                ret_val["label_location"] = label_location  # rule: same as for "label_value" key
-                if not (value_found and index_of_value_found):  # nothing found, nor @RIGHT, nor @DOWN, so break the loop and try for other poatential cell
-                    return ret_val  # will return the empty structure (as initialized)
-                if value_found and index_of_value_found:  # if found something will break all loops
-                    # all things are ok here (ref effective value), so return found data an, its location
-                    ret_val["location"] = index_of_value_found
-                    try:  # converting to requested `targeted_type` (will not test is isinstance(obj, Callable) because if not will raise `except` and convert to str)
-                        ret_val["value"] = targeted_type(value_found)
-                    except:  # noqa: E722
-                        ret_val["value"] = str(value_found)
-                    return ret_val
-    return ret_val  # if get here then will return the empty structure (as initialized)
-
-
-
-
-
-
-
-
-# NOTE: ready, test PASS @ 231126 by [piu]
-def mk_kv_invoice_items_area(invoice_items_area_xl_format) -> dict:
-    """transform `invoice_items_area` in "canonical JSON format" (as kv pairs).
-
-    Args:
-    
-        `invoice_items_area_xl_format`: invoice items area in Excel format (ie, DataFrame with row, col, data).
-
-    Return:
-    
-        `invoice_items_area_xl_format`: dictionary with invoice items in Excel format (ie, rows, columns).
-
-    Notes:
-    
-    * for ROefact XML model (& plan) see `invoice_files/__model_test_factura_generat_anaf.xml`.
-    """
-    _invoice_items_data_key = copy.deepcopy(invoice_items_area_xl_format["data"])
-    _invoice_items_cols_key = copy.deepcopy(invoice_items_area_xl_format["keycols"])
-    _invoice_items_rows_key = copy.deepcopy(invoice_items_area_xl_format["keyrows"])
-
-    _invoice_items_area_json_format = list()
-    for _i, _line in enumerate (_invoice_items_rows_key):
-        """ identify usual invoice columns: item desc, item UOM, item VAT_percent, item unit_price, item line_value, itemline_ VAT_value
-        """
-        if True:  # ---- find item quantity column ==> (`cbc_InvoicedQuantity`)
-            _col_index = find_str_in_list(["qty", "cant", "quantity"], _invoice_items_cols_key)
-            if _col_index is None:  # did not find a suitable column to represent number, so return None probably raising an error
-                print(f"[red]***FATAL ERROR - module 'RDINV', function `mk_kv_invoice_items_area(...)`. Cannot find a 'QUANTITY' column in items table. Processing terminated[/]")
-                return False
-            else:
-                _item_quantity = _invoice_items_data_key[_i][_col_index] if isnumber(str(_invoice_items_data_key[_i][_col_index])) else None
-
-        """ #NOTE-1: from here, the following columns are considered "valid" only if a quantity is specified (otherwise is considered an extended description)
-        """
-
-        if True:  # ---- find item VAT percent (if exists..., some invoices do noy specify percent itself but just value) ==> (`cbc_Percent`)
-            _col_index = find_str_in_list(["cota", "vat %", "% vat"], _invoice_items_cols_key)
-            if _col_index is None: # did not find a suitable column to represent number, so return None probably raising an error
-                _vat_percent = DEFAULT_VAT_PERCENT if _item_quantity else None  # see #NOTE-1
-            else:
-                #TODO check_what_is_here_and_if_actual [@231202]:  `_vat_percent` calculation should also consider a simplified invoice where only VAT value is specificed AND THEN SHOULD BE CALCULATED AS_IS in document (see "acciza line on REN... invoice")
-                _vat_percent = _invoice_items_data_key[_i][_col_index] if (_invoice_items_data_key[_i][_col_index] is not None) else (DEFAULT_VAT_PERCENT if _item_quantity else None)  # see #TODO-1 check it considering previous comment
-                _vat_percent = None if (str(_vat_percent).split() == "") else (float(_vat_percent) if isnumber(str(_vat_percent)) else None)  # finally make it None if remained empty string
-
-        if True:  # ---- find item description / name ==> (`cbc_Name`)
-            _col_index = find_str_in_list(["denumire", "name", "nume", "item", "desc"], _invoice_items_cols_key)
-            if _col_index is None: # did not find a suitable column to represent number, so return None probably raising an error
-                _name_description = DEFAULT_UNKNOWN_ITEM_NAME if _item_quantity else None  # see #NOTE-1
-            else:
-                _name_description = _invoice_items_data_key[_i][_col_index] if (_invoice_items_data_key[_i][_col_index] is not None) else (DEFAULT_UNKNOWN_ITEM_NAME if _item_quantity else None)  # see #NOTE-1
-
-        if True:  # --- find unit of measure ==> (`cbc_unitCode`)
-            _col_index = find_str_in_list(["uom", "um", "masura", "measure"], _invoice_items_cols_key)
-            if _col_index is None: # did not find a suitable column to represent number, so return None probably raising an error
-                _unif_of_measure = DEFAULT_UNKNOWN_UOM if _item_quantity else None  # see #NOTE-1
-            else:
-                _unif_of_measure = _invoice_items_data_key[_i][_col_index] if (_invoice_items_data_key[_i][_col_index] is not None) else (DEFAULT_UNKNOWN_UOM if _item_quantity else None)  # see #NOTE-1
-
-        if True:  # --- find unit price ==> (`cbc_PriceAmount`)
-            _col_index = find_str_in_list(["price", "pret"], _invoice_items_cols_key)
-            if _col_index is None:  # did not find a suitable column to represent number, so return None probably raising an error
-                _unit_price = 0 if _item_quantity else None  # see #NOTE-1
-            else:
-                _tmp = float(_invoice_items_data_key[_i][_col_index]) if isnumber(str(_invoice_items_data_key[_i][_col_index])) else None  # convert it to numer if possible
-                _unit_price = _tmp if (_tmp is not None) else (_tmp if _item_quantity else None)  # see #NOTE-1
-
-        if True:  # --- find CURRENCY ==> (`cbc_currencyID`)
-            pass # NOTE this will be identifyed in `invoice_header_area` ==> should be changed accordingly
-
-        if True:  # --- calculate line totals ==> (`cbc_LineExtensionAmount`)
-            _item_total = None
-            if (_item_quantity is not None) and (_unit_price is not None):
-                _item_total = round(_item_quantity * _unit_price, 2)
-                # line VAT calculation is subject of VAT existence and right calculation as number, otherwise it is set to NULL
-                if _item_total and _vat_percent:
-                    _item_VAT = round(float(_item_quantity * _unit_price * _vat_percent), 2)
-                else:
-                    _item_VAT = 0.0
-
-        # build dictionary with usual invoice columns (respecting as possible the XSD schemes listed in [`meta_info`][`invoice_XML_schemes`] key)
-        _line_info = {
-            "cac_InvoiceLine": {
-                "cbc_ID": str(_line),
-                "cbc_InvoicedQuantity": _item_quantity,
-                "cbc_unitCode": None if (_item_quantity is None or str(_item_quantity).split() == "") else _unif_of_measure,
-                "cac_Item": {  #-NOTE these are the item specifications (uom, vat)
-                    "cbc_Name": str(_name_description),
-                    "cac_ClassifiedTaxCategory": {
-                        "cbc_Percent": _vat_percent,
-                        "cac_TaxScheme": {
-                            "cbc_ID": None if (_vat_percent is None or str(_vat_percent).split() == "") else "VAT"
-                        }
-                    }
-                },
-                "cac_Price": {
-                    "cbc_PriceAmount" : _unit_price,
-                    "cbc_currencyID": None if (_item_quantity is None or str(_item_quantity).split() == "") else DEFAULT_CURRENCY
-                },
-                "cbc_LineExtensionAmount": _item_total,
-                "LineVatAmount": None if _item_total is None else _item_VAT,  # line VAT calculation is subject of some Amount existence
-            }
-        }
-        _invoice_items_area_json_format.append(_line_info["cac_InvoiceLine"])
-    return copy.deepcopy(_invoice_items_area_json_format)
-
-
-
-
-
-
-# NOTE: ready, test PASS @ 231121 by [piu]
-def get_invoice_items_area(
-    worksheet,
-    invoice_items_area_marker,
-    wks_name
-) -> dict:
-    """get invoice for `invoice_items_area`, process it and return its Excel format.
-
-    Process steps & notes:
-    
-    * find invoice items subtable.
-    * clean invoice items subtable.
-    * extract relevenat data.
-    * NOTE: all Excel cell addresses are in `(row, col)` format (ie, Not Excel format like "A:26, C:42, ...")
-
-    Args:
-    
-        `worksheet`: the worksheet containing invoice (as object of `pyxllight` library).
-        `invoice_items_area_marker`: string with exact marker of invoice items table.
-            NOTE: this is the UPPER-LEFT corner and is determined before calling this procedure.
-        `wks_name`: the wroksheet name (string) of the `worksheet` object.
-
-    Return:
-    
-        `invoice_items_area`: dictionary with invoice items in Excel format (ie, rows, columns).
-    """
-    # obtain table with invoice items ==> `invoice_items_area`
-    invoice_items_area = worksheet.ssd(keycols = invoice_items_area_marker, keyrows = invoice_items_area_marker)
-    if (invoice_items_area is None or ((isinstance(invoice_items_area, list)) and len(invoice_items_area) < 1)):  # there was not detected any area candidate to "invoice items / lines", so will exit rasing error
-        print(f"[red]***FATAL ERROR - Cannot find any candidate to for invoice ITEMS. Worksheet - \"{wks_name}\" in Module [red] RDINV (code-name: `rdinv`). File processing terminated[/]")
-        return False
-
-    #TODO test if list has more items (ie, that means more item tables that will need to be consolidated)
-    if isinstance(invoice_items_area, list) and len(invoice_items_area) > 0:
-        # NOTE `invoice_items_area` dictionary with keys: "keyrows", "keycols" and "data" (self explanatory)
-        invoice_items_area = invoice_items_area[0]  # will suppose found just one AND retain only first one (index [0]) - SEE AFTER TEST with RENware invoice...
-
-    """ CLEANING & CLEARING section
-    """
-    if True:  # preserve actual rows index in a separated structure (`invoice_items_area["keyrows_index"]`)
-        invoice_items_area["keyrows_index"] = list()
-        for _tmp_row_index, _tmp_row in enumerate(invoice_items_area["keyrows"]):  # scan all rows and those with empty name/title are first candidates
-            invoice_items_area["keyrows_index"].append(_tmp_row_index)
-            # clean full empty rows
-            if _tmp_row == SYS_FILLED_EMPTY_CELL:
-                # inspect all row cells to see if all are empty
-                _tmp_test_row_if_full_zero = sum([0 if _i == SYS_FILLED_EMPTY_CELL else 1 for _i in invoice_items_area["data"][_tmp_row_index]])
-                if _tmp_test_row_if_full_zero == 0:  # efectivelly delete in subject objects
-                    del invoice_items_area["keyrows"][_tmp_row_index]  # drop that row from "keyrows" keyword list
-                    # del invoice_items_area["keyrows_index"][_tmp_row_index]  # drop that row from "keyrows" keyword list #NOTE there is no need, you just enumerated this index and dropeed it in the same for-loop step
-                    del invoice_items_area["data"][_tmp_row_index]  # drop that row from "data" keyword list
-        del invoice_items_area["keyrows_index"]  # cleanup after do job ... :)
-
-    if True:  # clean empty columns: columns without a name will be completly dropped as they are unusable anyway (ie, do not know what to do with them...)
-        _tmp_cells_to_drop_in_data_key = list()
-        _tmp_items_to_drop_in_keycols_key = list()
-        for _tmp_col_index, _tmp_col in enumerate(invoice_items_area["keycols"]):  # scan all cols and those with empty name/title are first candidates
-            if _tmp_col == SYS_FILLED_EMPTY_CELL:
-                # inspect all col cells to see if all are empty & efectivelly delete in subject objects
-                _tmp_items_to_drop_in_keycols_key.append(_tmp_col_index)
-                for _data_row_index, _data_row in enumerate(invoice_items_area["data"]):  # scan all rows to find out cells that are part of in subject columns
-                    # find out DATA all cells that corresponding to columns to be dropped ==> `_tmp_cells_to_drop_in_data_key: list[(row, col)]`
-                    _tmp_tmp = (_data_row_index, _tmp_col_index)
-                    _tmp_cells_to_drop_in_data_key.append(_tmp_tmp)
-        # drop collected objects (column heads from KEYCOLS & correcsponding cell from DATA)
-        for _obj_to_delete in reversed(_tmp_items_to_drop_in_keycols_key):  # from KEYCOLS... (start with last item to not remain "in air" due to deletions :))
-            del invoice_items_area["keycols"][_obj_to_delete]
-        for _object_to_delete in reversed(_tmp_cells_to_drop_in_data_key):  # from DATA... (start with last item to not remain "in air" due to deletions :))
-            del invoice_items_area["data"][_object_to_delete[0]][_object_to_delete[1]]  # drop that col from "data" keyword list
-
-    if True:  # unknown header rows: set as a descriptive using format: `<current line number>.NOTE-<seq>`, where `seq` is an ordered sequence of letters (ie, resulting something like: `1.a, 1.b, ...`)
-        _prev_row_number = None
-        __letter_seq_idx = 0  # used for next letter sequence (will reset after "a normal one" row (ie, has a value))
-        for _crt_row_idx, _crt_row_val in enumerate(invoice_items_area["keyrows"]):
-            #
-            # if current row is "a normal one", then preserve index and reset letter sequencer
-            if _crt_row_val != SYS_FILLED_EMPTY_CELL:
-                _prev_row_number = _crt_row_val  # preserve row business index (ie, value shown invoice data not array index)
-                __letter_seq_idx = 0   # reset letter sequence generator
-            #
-            # if current row is "a unknown one" set its header as `<prev line number>.NOTE-<seq>`, where `seq` is an ordered sequence of letters (ie, resulting something like: `1.a, 1.b, ...`)
-            if _crt_row_val == SYS_FILLED_EMPTY_CELL:
-                _crt_row_seq = f"{_prev_row_number}.NOTE-{ascii_lowercase[__letter_seq_idx]}"  # build a sequence-text for current item (see #NOTE_format)
-                # update line header
-                invoice_items_area["keyrows"][_crt_row_idx] = str(_crt_row_seq)
-                __letter_seq_idx += 1
-
-    if True:  # set back to empty cells that remained to `SYS_FILLED_EMPTY_CELL` (only in `invoice_items_area`)
-        invoice_items_area["keycols"] = ["" if _i == SYS_FILLED_EMPTY_CELL else _i for _i in invoice_items_area["keycols"]]  # loop for 'keycols' keyword
-        invoice_items_area["keyrows"] = ["" if _i == SYS_FILLED_EMPTY_CELL else _i for _i in invoice_items_area["keyrows"]]  # loop for 'keyrows' keyword
-        for _tmp_row_index, _tmp_row in enumerate(invoice_items_area["data"]):  # # loop for 'data' keyword (first loop table rows, "data" key is matrix of lines & cells, ie as [][])
-            _tmp_row = ["" if _i == SYS_FILLED_EMPTY_CELL else _i for _i in _tmp_row]
-            invoice_items_area["data"][_tmp_row_index] = _tmp_row
-    return copy.deepcopy(invoice_items_area)
-
-
-
-
-
-
-# NOTE: ready, test PASS @ 231111 by [piu]
-def get_merged_cells_tobe_changed(
-    file_to_scan,
-    invoice_worksheet_name,
-    keep_cells_of_items_ssd_marker = None
-) -> list:
-    """scan Excel file to detect all merged ranges.
-
-    Args:
-    
-        `file_to_scan`: the excel file to be scanned.
-        `invoice_worksheet_name`: the worksheet to be scanned.
-        `keep_cells_of_items_ssd_marker`: tuple with cells that will be marked IN ANY CASE to be preserved:
-            * use case: to keep all potential invoice items ssd rows.
-            * format: `tuple(row, col, val)` where row & col are relevant here
-            * default: `None`
-
-    Return:
-    
-        `cells_to_be_changed`: list with cells that need to be chaged in format `(row,col)`.
-
-    Notes:
-    
-    * function is intended to be used ONLY internal in this module.
-    * use `openpyxl` library to do its job.
-    """
-    all_detected_ranges = []
-    # open Excel file & worksheet
-    workbook_opnxl= opnxl.load_workbook(file_to_scan)
-    worksheet_opnxl = workbook_opnxl[invoice_worksheet_name]
-    all_detected_ranges = worksheet_opnxl.merged_cells.ranges  # get all merged ranges
-    _cells_to_be_changed = list()  # will retaing cells that should be marked with SYS_FILLED_EMPTY_CELL
-    for _crt_range in all_detected_ranges:
-        # range coordinates
-        _crt_range_START_COL = _crt_range.bounds[0]
-        _crt_range_END_COL = _crt_range.bounds[2]
-        _crt_range_START_ROW = _crt_range.bounds[1]
-        _crt_range_END_ROW = _crt_range.bounds[3]
-        # traverse merged range for all cells in / set flags for first entry and when to completly break loop
-        _first_entry = True;
-        _full_break = False
-        for c in range(_crt_range_START_COL, _crt_range_END_COL + 1):  # traverse all COLS ...
-            for r in range(_crt_range_START_ROW, _crt_range_END_ROW + 1):  # traverse all ROWS ...
-                _crt_cell_value = worksheet_opnxl.cell(r, c).value
-                #print(f"\t/***** processing cell (row,col = {r},{c}) has value {_crt_cell_value}")  #NOTE for debug purposes
-                if _first_entry:  # at first pass, see if relevant (ie, not empty or empty string) AND if NOT then break all loops
-                    if _crt_cell_value is None:
-                        _full_break = True
-                        break
-                    if isinstance(_crt_cell_value, str) and _crt_cell_value.strip() == "":  # if is a string test if cell is a real empty string
-                        _full_break = True
-                        break
-                    #print(f"\t/***** RELEVANT cell (row,col = {r},{c}) has value {_crt_cell_value}")  #NOTE for debug purposes
-                    """ section applicable only when `keep_cells_of_items_ssd_marker` is note None
-                        * (r1) in this case, if found a relevant entry in a merged range and and first entry in merged range scan
-                        * (r2) to preserve cell @(`row=current_row`, `col=keep_cells_of_items_ssd_marker[1]`)
-                        * (r3) if that cell is empty, them add in `_cells_to_be_changed` list to be marked with SYS_FILLED_EMPTY_CELL
-                    """
-                    if keep_cells_of_items_ssd_marker:
-                        _potential_ROW_INDEX_address = (r, keep_cells_of_items_ssd_marker[1])
-                        __this_cell_value = worksheet_opnxl.cell(*_potential_ROW_INDEX_address).value
-                        if not (__this_cell_value) and (_potential_ROW_INDEX_address not in _cells_to_be_changed):  # apply (r3) rule - see long comment before this section
-                            _cells_to_be_changed.append(_potential_ROW_INDEX_address)
-                if not _first_entry:  # here the cell has a relevant value, store all next to be marked with SYS_FILLED_EMPTY_CELL
-                    _cells_to_be_changed.append((r, c))
-                    #print(f"\t/***** cell {(r, c)} marked for '___sys_filled_empty_cell' / [yellow]all list is {_cells_to_be_changed}[/]") #NOTE for debug purposes
-                _first_entry = False
-            if _full_break:
-                break
-    return tuple(copy.deepcopy(_cells_to_be_changed))  # always return a tuple as being immutable
-
-
-
-
-
-
-# NOTE: ready, test PASS @ 231127 by [piu]
-def build_meta_info_key(
-    excel_file_to_process: str,
-    invoice_worksheet_name: str,
-    ws_size: list,
-    keyword_for_items_table_marker: str,
-    found_cell: list
-) -> dict:
-    """build meta_info key to preserve processed Excel file meta information: start address, size.
-
-    Notes:
-    
-    * (1.) all cell addresses are in format (row, col) and are absolute (ie, valid for whole Excel file).
-    * (2.) this function is designed to be used internally by current module (using outside it is not guaranteed for information 'quality').
-
-    Args:
-    
-        `excel_file_to_process`: name of file to process as would appear in `meta_info` key.
-        `invoice_worksheet_name`: the worksheet name as would appear in `meta_info` key.
-        `ws_size`: worksheet size as would appear in `meta_info` key (index 0 max rows, index 1 max columns).
-        `keyword_for_items_table_marker`: the content of cell used as start of invoice items subtable as would appear in `meta_info`.
-        `found_cell`: position of cell used as start of invoice items subtable as would appear in `meta_info` key (index 0 row, index 1 column).
-
-    Returns:
-    
-        `meta_info`: dictionary built with meta information to be incorpoarted in final invoice dict
-    """
-    _tmp_meta_info = dict()
-
-    _tmp_meta_info["file"] = os.path.basename(excel_file_to_process)
-    _tmp_meta_info["file_CRC"] = "...file CRC (uniquely identify the invoice file used)"  #TODO to be done... #NOTE this calculation should be done as last step after final XLSX file writing
-    _tmp_meta_info["last_processing_time"] = datetime.now(timezone.utc).isoformat()  # set to ISO 8601 format
-    _tmp_meta_info["invoice_worksheet"] = invoice_worksheet_name
-    _tmp_meta_info["invoice_max_rows"] = ws_size[0]
-    _tmp_meta_info["invoice_max_cols"] = ws_size[1]
-    _tmp_meta_info["items_table_start_marker"] = keyword_for_items_table_marker
-    _tmp_meta_info["items_table_start_cell"] = (found_cell[0], found_cell[1])
-    _tmp_meta_info["invoice_XML_schemes"] = {
-        "xmlns": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2",
-        "xmlns:cbc": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2",
-        "xmlns:cac": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2",
-        "xmlns:ns4": "urn:oasis:names:specification:ubl:schema:xsd:CommonExtensionComponents-2",
-        "xmlns:xsi": "http://www.w3.org/2001/XMLSchema-instance",
-        "xsi:schemaLocation": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2 http://docs.oasis-open.org/ubl/os-UBL-2.1/xsd/maindoc/UBL-Invoice-2.1.xsd"
-    }
-    _tmp_meta_info["map_JSONkeys_XMLtags"] = [  # list of tuple(JSONkey: str, XMLtag: str) #TODO subject of documentation update
-        ("cac_InvoiceLine", "cac:InvoiceLine"),
-        ("cac_Item", "cac:Item"),
-        ("cac_ClassifiedTaxCategory", "cac:ClassifiedTaxCategory"),
-        ("cac_TaxScheme", "cac:TaxScheme"),
-        ("cac_Price", "cac:Price"),
-        ("cbc_ID", "cbc:ID"),
-        ("cbc_InvoicedQuantity", "cbc:InvoicedQuantity"),
-        ("cbc_unitCode", "cbc:unitCode"),  # this is attribute of tag InvoicedQuantity
-        ("cbc_Name", "cbc:Name"),
-        ("cbc_Percent", "cbc:Percent"),
-        ("cbc_PriceAmount", "cbc:PriceAmount"),
-        ("cbc_currencyID", "cbc:currencyID"),  # this is attribute of more tags (all monetary tags)
-        ("cbc_LineExtensionAmount", "cbc:LineExtensionAmount"),
-        ("cbc_DocumentCurrencyCode", "cbc:DocumentCurrencyCode"),  # invoice currency
-        ("cbc_IssueDate", "cbc:IssueDate"),  # invoice issue date
-        ("cac_AccountingCustomerParty", "cac:AccountingCustomerParty"),  # invoice customer information - MASTER RECORD
-        ("cac_Party", "cac:Party"),  # invoice customer details ref Parner info (legal, address, ...) - DETAIL L1 RECORD
-        ("cac_PartyLegalEntity", "cac:PartyLegalEntity"),  # invoice customer inforation - DETAIL L2 RECORD
-        ("cbc_CompanyID", "cbc:CompanyID"),  # invoice customer inforation - DETAIL L3 RECORD
-        ("cbc_RegistrationName", "cbc:RegistrationName"),  # invoice customer inforation - DETAIL L3 RECORD
-        ("cac_PostalAddress", "cac:PostalAddress"),  # invoice customer postal address info - DETAIL L2 RECORD
-        ("cbc_StreetName", "cbc:StreetName"),  # invoice customer inforation - DETAIL L3 RECORD
-        ("cbc_CityName", "cbc:CityName"),  # invoice customer inforation - DETAIL L3 RECORD
-        ("cbc_PostalZone", "cbc:PostalZone"),  # invoice customer inforation - DETAIL L3 RECORD
-        ("cac_Country", "cac:Country"),  # invoice customer inforation - DETAIL L3 RECORD
-        ("cbc_IdentificationCode", "cbc:IdentificationCode"),  # invoice customer inforation - DETAIL L3 RECORD
-        ("LineVatAmount", None),  # line / item total VAT. Has no correspondent in XML schema - DETAIL L3 RECORD
-        ("cac_Contact", "cac:Contact"),  #  customer contact information: email, phone - DETAIL L2 RECORD
-        ("cbc_Telephone", "cbc:Telephone"),  # customer phone -- DETAIL L3 RECORD
-        ("cbc_ElectronicMail", "cbc:ElectronicMail"),  # customer email - DETAIL L3 RECORD
-        ("RegCom", None),  # customer commerce register number (company legal registration number). Has no correspondent in XML schema - DETAIL L3 RECORD
-        ("Bank", None),  # customer bank. Has no correspondent in XML schema - DETAIL L3 RECORD
-        ("IBAN", None),  # customer bank account number (IBAN). Has no correspondent in XML schema - DETAIL L3 RECORD
-        ("cac_LegalMonetaryTotal", "cac:LegalMonetaryTotal"),  # summary item
-        ("cbc_LineExtensionAmount", "cbc:LineExtensionAmount"),  # summary item
-        ("cbc_TaxExclusiveAmount", "cbc:TaxExclusiveAmount"),  # summary item
-        ("cbc_TaxInclusiveAmount", "cbc:TaxInclusiveAmount",),  # summary item
-        ("cbc_PayableAmount", "cbc:PayableAmount"),  # summary item
-        ("cac_TaxTotal", "cac:TaxTotal"),  # specific for Tax Summary section
-        ("cbc_TaxAmount", "cbc:TaxAmount"),  # specific for Tax Summary section
-        ("cac_TaxSubtotal", "cac:TaxSubtotal"),  # specific for Tax Summary section
-        ("cbc_TaxableAmount", "cbc:TaxableAmount"),  # specific for Tax Summary section
-        ("cac_TaxCategory", "cac:TaxCategory"),  # specific for Tax Summary section
-        ("cac_AccountingSupplierParty", "cac:AccountingSupplierParty"),  # specific to supplier
-        ("cac_PartyTaxScheme", "cac:PartyTaxScheme"),  # specific to supplier
-    ]
-    return copy.deepcopy(_tmp_meta_info)
-
-
-
-
-
-
-# NOTE: ready, test PASS @ 240404 by [piu]
-def get_partner_data(
-    partner_type: str,
-    *,
-    wks,
-    param_invoice_header_area: dict,
-    supplier_datafile: Path = None
-) -> None:
-    """Get invoice partener data from Excel.
-
-    Notes:
-    
-    * *for developers*: function works by generating side effects and must be located in `rdinv.py`
-    * *side effects*: this function works by directly modifying `param_invoice_header_area` sent parameter
-    * *supplier_datafile exception*: if file is not found or cannot be read, this function will force complete application termination (`sys.exit`)
-
-    Args:
-    
-        `partner_type`: one of "CUSTOMER", "SUPPLIER" or "OWNER" to specify for what kind of parner get data. The value "OWNER" is designed to get data from an outside database / file (master data)
-        `wks`: current work-on `pylightxl Worksheet` object
-        `param_invoice_header_area`: _mode IN-OUT_, outside `param_invoice_header_area` as used and needed in `rdinv()`. This function will write back in this variable
-        `supplier_datafile`: for `partner_type = "CUSTOMER"` here is expected the file where to get supplier data
-
-    Return:
-    
-        `None`: all data is produced directly in parameters as side effect
-    """
-    # set variables constant-like suspected to be changed as global
-    global DEFAULT_CUSTOMER_COUNTRY
-    global DEFAULT_SUPPLIER_COUNTRY
-    # normalize partner_type for easier usage and more flexibility to developers misusing
-    partner_type = partner_type.upper().strip()
-    # unify search patterns and other constants function of partner_type
-    if partner_type == "CUSTOMER":
-        UNIF_PATTERN_FOR_INVOICE_PARTNER_SUBTABLE_MARKER = PATTERN_FOR_INVOICE_CUSTOMER_SUBTABLE_MARKER
-        UNIF_PATTERN_FOR_PARTNER_LEGAL_NAME = PATTERN_FOR_CUSTOMER_LEGAL_NAME
-        UNIF_DEFAULT_PARTNER_COUNTRY = DEFAULT_CUSTOMER_COUNTRY
-        unif_partner_area_key = "customer_area"
-    elif partner_type =="SUPPLIER":
-        # NOTE: pls be patient. Here will raise errs because used EXPECTED constant names. Check `config_settings.py` and adjust accordingly
-        UNIF_PATTERN_FOR_INVOICE_PARTNER_SUBTABLE_MARKER = PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER
-        UNIF_PATTERN_FOR_PARTNER_LEGAL_NAME = PATTERN_FOR_SUPPLIER_LEGAL_NAME
-        UNIF_DEFAULT_PARTNER_COUNTRY = DEFAULT_SUPPLIER_COUNTRY
-        unif_partner_area_key = "supplier_area"
-    elif partner_type == "OWNER":  # subject to load SUPPLIER data from external data source
-        unif_partner_area_key = "supplier_area"
-        # safe read data from `supplier_datafile` file only if it exists
-        file_ok = supplier_datafile.exists() and supplier_datafile.is_file()
-        if file_ok:
-            yaml_in = supplier_datafile.read_text()
-            suppl_data_read = yaml.safe_load(yaml_in)
-        else:
-            print(f"[red]ERROR: Owner / Supplier data file ([cyan]{supplier_datafile}[/]) cannot be read. Process terminated.[/].")
-            sys.exit()
-        supplier_datafile_name = str(supplier_datafile)
-        # save info about area to search as external file and its name
-        param_invoice_header_area[unif_partner_area_key] = {
-            "area_info": {
-               "value": supplier_datafile_name,
-                "location": "external file",
-            }
-        }
-        # CUI
-        param_invoice_header_area[unif_partner_area_key]["CUI"] = {
-            "value": suppl_data_read["PartyLegalEntity"]["CompanyID"],
-            "location": "external file (PartyLegalEntity -> CompanyID)",
-            "label_value": None,
-            "label_location": None
-        }
-        # RegName
-        param_invoice_header_area[unif_partner_area_key]["RegistrationName"] = {
-            "value": suppl_data_read["PartyLegalEntity"]["RegistrationName"],
-            "location": "external file (PartyLegalEntity -> CompanyID)",
-            "label_value": None,
-            "label_location": None
-        }
-        # PostalAddress
-        param_invoice_header_area[unif_partner_area_key]["PostalAddress"] = {
-            "cbc_StreetName": suppl_data_read["PostalAddress"]["StreetName"],
-            "cbc_CityName": suppl_data_read["PostalAddress"]["CityName"],
-            "cbc_PostalZone": suppl_data_read["PostalAddress"]["PostalZone"],
-            "cac_Country": { "cbc_IdentificationCode": suppl_data_read["PostalAddress"]["CountryCode"] },
-        }
-        # Bank, Tax & Contact
-        param_invoice_header_area[unif_partner_area_key]["reg_com"] = {
-            "value": suppl_data_read["PartyTaxScheme"]["CompanyID"],
-            "location": "external file (PartyLegalEntity -> CompanyID)"
-        }
-        param_invoice_header_area[unif_partner_area_key]["phone"] = {
-            "value": suppl_data_read["Contact"]["Telephone"],
-            "location": "external file (Contact -> Telephone)"
-        }
-        param_invoice_header_area[unif_partner_area_key]["email"] = {
-            "value": suppl_data_read["Contact"]["ElectronicMail"],
-            "location": "external file (Contact -> ElectronicMail)"
-        }
-        param_invoice_header_area[unif_partner_area_key]["bank"] = {
-            "value": suppl_data_read["Contact"]["Bank"],
-            "location": "external file (Contact -> Bank)"
-        }
-        param_invoice_header_area[unif_partner_area_key]["IBAN"] = {
-            "value": suppl_data_read["Contact"]["IBAN"],
-            "location": "external file (Contact -> IBAN)"
-        }
-        return
-    else:  # accept only known operations
-        raise Exception("partner_type parameter not recognized value")
-    #
-    # find invoice partner ==> one of (cac:AccountingCustomerParty , cac:AccountingSupplierParty)
-    invoice_partner_info = get_excel_data_at_label(
-        pattern_to_search_for=UNIF_PATTERN_FOR_INVOICE_PARTNER_SUBTABLE_MARKER,  # NOTE: constant adjusted in refactoring process
-        worksheet=wks,
-        area_to_scan=(param_invoice_header_area["start_cell"], param_invoice_header_area["end_cell"]),
-        targeted_type=str
-    )  # returned info: `{"value": ..., "location": (row..., col...)}`
-    # set a dedicated area to search for partner
-    _area_to_search_start_cell = [  # use `label_location` as being supposed "most far away" from effective-good info, so more chances to find info
-        0 if invoice_partner_info["label_location"][0] <= 0 else invoice_partner_info["label_location"][0] - 1,  # set one line up if this line exists
-        invoice_partner_info["label_location"][1],
-    ]
-    if wks.index(*_area_to_search_start_cell).strip() == "":  # prev set was for one line up but if that cell is blank remake it (ie, do a +1)
-        _area_to_search_start_cell[0] += 1
-    # from `_area_to_search_start_cell` go down up a blank (empty cell)
-    _last_ok_position = list([0, 0])
-    for __i in range(_area_to_search_start_cell[0], wks.size[0] + 1):  # scan rest of lines for a blank one
-        _crt_scanned_cell_idx = (__i, _area_to_search_start_cell[1])
-        _crt_scanned_cell_val = wks.index(*_crt_scanned_cell_idx)
-        if _crt_scanned_cell_val.strip() == "":
-            break  # case where stop
-        _last_ok_position = copy.deepcopy(_crt_scanned_cell_idx)  # save current position to be used after a break in other iteration
-    _area_to_search_end_cell = [
-        _last_ok_position[0],
-        wks.size[1] if _last_ok_position[1] > wks.size[1] else _last_ok_position[1] + 1,  # set one row right if this row exists
-    ]
-    # persist `_area_to_search` for next steps & save its key-info in associated invoice JSON (for further references)
-    _area_to_search = (tuple(_area_to_search_start_cell), tuple(_area_to_search_end_cell))
-    param_invoice_header_area[unif_partner_area_key] = {
-        "area_info": {
-            "value": wks.index(*_area_to_search[0]),  # ie, the value at area start position
-            "location": copy.deepcopy(_area_to_search),
-        }
-    }
-    #
-    # find partner key "CUI / Registration ID" ==> `param_invoice_header_area...[CUI]` && `Invoice...[cbc_CompanyID]`
-    _temp_found_data = get_excel_data_at_label(
-        pattern_to_search_for=PATTERN_FOR_PARTNER_ID,
-        worksheet=wks,
-        area_to_scan=_area_to_search,
-        targeted_type=str,
-        down_search_try=False  # partner area is supposed to be organized as "label & value @ RIGHT" or "label: value @ IN-LABEL" but never @ DOWN as being a "not-a-practiced-natural-way"
-    )  # returned info: `{"value": ..., "location": (row..., col...)}`
-    param_invoice_header_area[unif_partner_area_key]["CUI"] = {
-        "value": _temp_found_data["value"],
-        "location": _temp_found_data["location"],
-        "label_value": _temp_found_data["label_value"],
-        "label_location": _temp_found_data["label_location"]
-    }
-    #
-    # find partner key "RegistrationName" ==> `cbc_RegistrationName`
-    '''#NOTE: `ReNaSt`-RegNameStrategy (remark: step codes will referred as defined here)
-          ReNaSt.STEP-1. search for UNIF_PATTERN_FOR_PARTNER_LEGAL_NAME  # NOTE: constant adjusted in refactoring process
-          ReNaSt.STEP-2. if `label_location` of FOUND VALUE has the same location as `param_invoice_header_area[unif_partner_area_key]["area_info"]["location"][0]`:
-                             keep VALUE of FOUND info
-          ReNaSt.STEP-3. else:
-                             keep `param_invoice_header_area[unif_partner_area_key]["area_info"]["value"]`
-    '''
-    _temp_found_data = get_excel_data_at_label(  # NOTE: ReNaSt.STEP-1
-        pattern_to_search_for=UNIF_PATTERN_FOR_PARTNER_LEGAL_NAME,  # NOTE: constant adjusted in refactoring process
-        worksheet=wks,
-        area_to_scan=_area_to_search,
-        targeted_type=str,
-        down_search_try=True  # NOTE: set on True to obtain identical results as original search of `UNIF_PATTERN_FOR_INVOICE_PARTNER_SUBTABLE_MARKER` because name is supposed to be in a very "unstructured mode"
-    )  # returned info: `{"value": ..., "location": (row..., col...)}`
-    _location_of_header_partner_area = param_invoice_header_area[unif_partner_area_key]["area_info"]["location"][0]
-    _location_of_value_found = _temp_found_data["label_location"]
-    if _location_of_value_found == _location_of_header_partner_area:  # NOTE: ReNaSt.STEP-2
-        kept_RegistrationName = _temp_found_data["value"]
-        kept_RegistrationName_location = _temp_found_data["location"]
-    else:  # NOTE: ReNaSt.STEP-3
-        kept_RegistrationName = param_invoice_header_area[unif_partner_area_key]["area_info"]["value"]
-        kept_RegistrationName_location = param_invoice_header_area[unif_partner_area_key]["area_info"]["location"][0]
-    param_invoice_header_area[unif_partner_area_key]["RegistrationName"] = {
-        "value": kept_RegistrationName,
-        "location": kept_RegistrationName_location,
-        "label_value": "n/a",
-        "label_location": "n/a"
-    }
-    #
-    # find partner key `cac:PostalAddress` -> `param_invoice_header_area["cac_PostalAddress"]` && Invoice...["cac_PostalAddress"]
-    _temp_found_data = get_excel_data_at_label(
-        pattern_to_search_for=PATTERN_FOR_PARTNER_ADDRESS,
-        worksheet=wks,
-        area_to_scan=_area_to_search,
-        targeted_type=str,
-        down_search_try=False  # partner area is supposed to be organized as "label & value @ RIGHT" or "label: value @ IN-LABEL" but never @ DOWN as being a "not-a-practiced-natural-way"
-    )  # returned info: `{"value": ..., "location": (row..., col...)}`
-    _tmpstr = _temp_found_data["label_value"].lower()
-    _val_is_full_addr = ("adr" in _tmpstr) or ("addr" in _tmpstr)
-    if _val_is_full_addr:
-        area_to_scan_address_items = (_temp_found_data["location"], _temp_found_data["location"])
-    else:
-        area_to_scan_address_items = _area_to_search
-    search_address_parts = partial(  # define a partial function to be used for all address items search
-        get_excel_data_at_label,  # function to call
-        worksheet=wks,
-        area_to_scan=area_to_scan_address_items,
-        targeted_type=str,
-        down_search_try=False  # partner area is supposed to be organized as "label & value @ RIGHT" or "label: value @ IN-LABEL" but never @ DOWN as being a "not-a-practiced-natural-way"
-    )  # returned info: `{"value": ..., "location": (row..., col...)}`
-    _tmp_country = str(search_address_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_ADDRESS_COUNTRY)["value"]).replace("None", "").strip()
-    _tmp_city = str(search_address_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_ADDRESS_CITY)["value"]).replace("None", "").strip()
-    _tmp_street = str(search_address_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_ADDRESS_STREET)["value"]).replace("None", "").strip()
-    _tmp_zipcode = str(search_address_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_ADDRESS_ZIPCODE)["value"]).replace("None", "").strip()
-    if (_tmp_country is None) or (_tmp_country == ""):
-        _tmp_country = UNIF_DEFAULT_PARTNER_COUNTRY  # NOTE: constant adjusted in refactoring process
-    else:  # update default value to be re-used in other parts if neccesary. Update is made on original variables "global" defined
-        if partner_type == "CUSTOMER":
-            DEFAULT_CUSTOMER_COUNTRY = _tmp_country  # NOTE: constant adjusted in refactoring process
-        else:  # case of "SUPPLIER" and "OWNER"
-            DEFAULT_SUPPLIER_COUNTRY = _tmp_country  # NOTE: constant adjusted in refactoring process
-    param_invoice_header_area[unif_partner_area_key]["PostalAddress"] = {
-        "cbc_StreetName": _tmp_street,
-        "cbc_CityName": _tmp_city,
-        "cbc_PostalZone": _tmp_zipcode,
-        "cac_Country": {"cbc_IdentificationCode": _tmp_country},
-    }
-    #
-    # find / search_extended_parts: rest of keys, like: "reg com", "bank / IBAN / cont", "tel", "email" (in code will use names like this: "search_extended_parts")*
-    search_extended_parts = partial(  # define a partial function to be used for all "search_extended_parts"
-        get_excel_data_at_label,  # function to call
-        worksheet=wks,
-        area_to_scan=_area_to_search,  # supposed to still contain partner info found area
-        targeted_type=str,
-        down_search_try=False  # partner area is supposed to be organized as "label & value @ RIGHT" or "label: value @ IN-LABEL" but never @ DOWN as being a "not-a-practiced-natural-way"
-    )  # returned info: `{"value": ..., "location": (row..., col...)}`
-    _tmp_reg_com = search_extended_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_REGCOM)
-    _tmp_bank = search_extended_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_BANK)
-    _tmp_IBAN = search_extended_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_IBAN)
-    _tmp_phone = search_extended_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_TEL)
-    _tmp_email = search_extended_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_EMAIL)
-    # store "full" variables in `partner_area...` for excel original values
-    param_invoice_header_area[unif_partner_area_key]["reg_com"] = _tmp_reg_com
-    param_invoice_header_area[unif_partner_area_key]["bank"] = _tmp_bank
-    param_invoice_header_area[unif_partner_area_key]["IBAN"] = _tmp_IBAN
-    param_invoice_header_area[unif_partner_area_key]["phone"] = _tmp_phone
-    param_invoice_header_area[unif_partner_area_key]["email"] = _tmp_email
-    return
-
-
-
-
-
-
+
+    * `db: pylightxl object`: EXCEL object with invoice (as a whole)
+    * `ws: pylightxl object`: WORKSHEET object with invoice
+    """
+    # use as global only for those constants that could be changed by this function
+    global DEFAULT_VAT_PERCENT
+    global DEFAULT_UNKNOWN_ITEM_NAME
+    global DEFAULT_UNKNOWN_UOM
+    global DEFAULT_CURRENCY
+    global DEFAULT_SUPPLIER_COUNTRY
+    global DEFAULT_CUSTOMER_COUNTRY
+
+    print(f"*** Module [red]rdinv[/] started at {datetime.now()} to process file [green]{os.path.split(file_to_process)[1]}[/] (full path: {file_to_process})")
+
+    # read Excel file with Invoice data
+    try:
+        db = xl.readxl(fn=file_to_process)
+    except:
+        print(f"[red]---***FATAL ERROR - Cannot open Excel file {file_to_process} (possible problems: file corrupted, wrong type only XLSX accetpted, file does not exists or was deleted, operating system vilotation) in Module [red] RDINV (code-name: `rdinv`). File processing terminated[/]")
+        return False
+
+    # read the workshet with Invoice data
+    if invoice_worksheet_name is None:  # if parameter `invoice_worksheet_name` not specified try to open first worksheet from Excel worksheets - order is given by worksheets order in Excel file
+        list_of_excel_worksheets = db.ws_names
+        print(f"[yellow]INFO note:[/] `rdinv` module, no worksheet specified, will open first one: [cyan]'{list_of_excel_worksheets[0]}'[/]")
+        invoice_worksheet_name = list_of_excel_worksheets[0]
+
+    try:
+        ws = db.ws(invoice_worksheet_name)
+    except:
+        print(f"[red]***FATAL ERROR - Cannot open Excel specified Worksheet \"{invoice_worksheet_name}\" in Module [red] RDINV (code-name: `rdinv`). File processing terminated[/]")
+        return False
+
+    """#NOTE: section for search of `invoice_items_area: pylightxl.ssd`
+        - main result: `keyword_for_items_table_marker` = string marker to search for in oredr to isolate `invoice_items_area`
+        - other results: `_found_cell_for_invoice_items_area_marker = (row, col, val)`
+    """
+    _tmp_label_info = get_excel_data_at_label(
+        pattern_to_search_for=PATTERN_FOR_INVOICE_ITEMS_SUBTABLE_MARKER,
+        worksheet=ws,
+        targeted_type=str
+    )
+    if _tmp_label_info["label_value"]:  # only if found a potential cell usable as`invoice_items_area_marker`
+        _found_cell_for_invoice_items_area_marker = (
+            _tmp_label_info["label_location"][0],
+            _tmp_label_info["label_location"][1],
+            _tmp_label_info["label_value"]
+        )  # here you still need to construct `_found_cell_for_invoice_items_area_marker = (row, col, val)` as it is used in prev code (before `231220piu_a` change)
+    else:
+        print(f"[red]***FATAL ERROR - Cannot find a relevant cell where invoice items table start (basically containing string \" crt\"). File processing terminated[/]")
+        return False
+    keyword_for_items_table_marker = _found_cell_for_invoice_items_area_marker[2]
+
+    # detect all cells that should be filled with SYS_FILLED_EMPTY_CELL (these are cells id merged groups where first cell in merged group is relevant (diff from empty))
+    detected_cells_which_will_be_fake_filled = get_merged_cells_tobe_changed(
+        file_to_scan=file_to_process,
+        invoice_worksheet_name=invoice_worksheet_name,
+        keep_cells_of_items_ssd_marker=_found_cell_for_invoice_items_area_marker)  # this call specify to keep unchanged that cells with some description
+    for _cell_index in detected_cells_which_will_be_fake_filled:  # scan all detectected cell and change them
+        _cell_row = _cell_index[0]
+        _cell_col = _cell_index[1]
+        ws.update_index(row = _cell_row, col = _cell_col, val = SYS_FILLED_EMPTY_CELL)
+
+    """#NOTE: section to "solve" `invoice_items_area`. Steps:
+        - process it as Excel format (row & colymns tabular organization)
+        - transform it in "canonical JSON format" (as kv pairs) and update `cac_InvoiceLine` key
+    """
+    # process invoice to detect its items / lines ('invoice_items_area'), clean and extract data
+    invoice_items_area = get_invoice_items_area(
+        worksheet=ws,
+        invoice_items_area_marker=keyword_for_items_table_marker,
+        wks_name=invoice_worksheet_name
+    )
+
+    """#NOTE: section for localize areas: invoice header (`invoice_header_area`) & invoice footer (`invoice_footer_area`)
+        NOTE: its code suppose `invoice_items_area` is already defined (as location). It will be used as reference in "header" & "footer" localization logic
+    """
+    ulc_header = (1, 1)
+    lrc_header = (_found_cell_for_invoice_items_area_marker[0] - 1, ws.size[1],)  # info where header ends: row = from items data table start location `_found_cell_for_invoice_items_area_marker[0]-1` && col = las col of worksheet
+    invoice_header_area = dict(
+        start_cell = ulc_header,
+        end_cell = lrc_header
+    )
+    #
+    _ulc_footer_row = _found_cell_for_invoice_items_area_marker[0] + len(invoice_items_area["keyrows"]) + 1  # this is located at: row = items data table start row  (_found_cell_for_invoice_items_area_marker[0]) + # of items data table rows + 1 (invoice_items_area["data"]) && col = 1
+    _start_cell_val = ws.index(_ulc_footer_row, 1)
+    while (_start_cell_val != "") and (_ulc_footer_row <= ws.size[0]): # but if that cell is not blank repeatedly to go une more row down... (why could happen? because ietms data table header was composed of more rows by merging cells...)
+        _ulc_footer_row += 1
+        _start_cell_val = ws.index(_ulc_footer_row, 1)
+    ulc_footer = (_ulc_footer_row, 1)
+    lrc_footer =( ws.size[0], ws.size[1])  # end of worksheet
+    invoice_footer_area = dict(
+        start_cell = ulc_footer,
+        end_cell = lrc_footer
+    )
+
+    """#NOTE: section to "solve" `invoice_header_area`.
+            The kind of info expected in this area: invoice number,  currency, issued date, supplier data, customer data)
+    """
+    invoice_header_area = invoice_header_area | dict(  # build effective data area & merge localization info from initial dict creation
+        invoice_number = None,
+        issued_date = None,
+        currency = None,
+        due_date = None,
+        customer_area = None,
+        supplier_area = None,
+    )
+    _area_to_search = (invoice_header_area["start_cell"], invoice_header_area["end_cell"])  # this is "global" for this section (corners of `invoice_header_area`)
+    #
+    # find invoice number ==> `cbc:ID`
+    invoice_number_info = get_excel_data_at_label(
+        pattern_to_search_for=PATTERN_FOR_INVOICE_NUMBER_LABEL,
+        worksheet=ws,
+        area_to_scan=_area_to_search,
+        targeted_type=str
+    )  # returned info: `{"value": ..., "location": (row..., col...)}`
+    invoice_header_area["invoice_number"] = copy.deepcopy(invoice_number_info)
+    #
+    # find invoice currency ==> `cbc:DocumentCurrencyCode`
+    invoice_currency_info = get_excel_data_at_label(
+        pattern_to_search_for=PATTERN_FOR_INVOICE_CURRENCY_LABEL,
+        worksheet=ws,
+        area_to_scan=_area_to_search,
+        targeted_type=str
+    )  # returned info: `{"value": ..., "location": (row..., col...)}`
+    if (invoice_currency_info["value"] is not None) and (invoice_currency_info["value"] != ""):  # if found a currency MUST CHANGE `DEFAULT_CURRENCY` to be properly used for `invoice_items_area`
+        DEFAULT_CURRENCY = invoice_currency_info["value"]
+    invoice_header_area["currency"] = copy.deepcopy(invoice_currency_info)
+    #
+    # find invoice issued date ==> `cbc:IssueDate`
+    issued_date_info = get_excel_data_at_label(
+        pattern_to_search_for=PATTERN_FOR_INVOICE_ISSUE_DATE_LABEL,
+        worksheet=ws,
+        area_to_scan=_area_to_search,
+        targeted_type=str
+    )  # returned info: `{"value": ..., "location": (row..., col...)}`
+    issued_date_info["value"] = issued_date_info["value"].replace("/", "-")  # convert from Excel format: YYYY/MM/DD (ex: 2023/08/28) to required format in XML file is: `YYYY-MM-DD` (ex: 2013-11-17)
+    invoice_header_area["issued_date"] = copy.deepcopy(issued_date_info)
+    #
+    # find invoice due date ==> `cbc_DueDate`
+    due_date_info = get_excel_data_at_label(
+        pattern_to_search_for= PATTERN_FOR_DUE_DATE,
+        worksheet=ws,
+        area_to_scan=_area_to_search,
+        targeted_type=str
+    )  # returned info: `{"value": ..., "location": (row..., col...)}`
+    if due_date_info["value"] is not None:  # if found something then try to clean it in case is intended to be a date-time
+        due_date_info["value"] = due_date_info["value"].replace("/", "-")  # convert from Excel format: YYYY/MM/DD (ex: 2023/08/28) to required format in XML file is: `YYYY-MM-DD` (ex: 2013-11-17)
+    else:
+        # convert invoice issued daye to datetime format
+        invoice_issued_date_as_date = datetime.strptime(
+            invoice_header_area["issued_date"]["value"],
+            '%Y-%m-%d'
+        )
+        # apply `DEFAULT_DUE_DATE_DAYS` to invoice issue date and convert it to date isoformat
+        _tmp = invoice_issued_date_as_date + timedelta(days = DEFAULT_DUE_DATE_DAYS)
+        due_date_info["value"] = _tmp.date().isoformat()
+    invoice_header_area["due_date"] = copy.deepcopy(due_date_info)
+    #
+    # get and solve `invoice_header_area` for all CUSTOMER data
+    _ = get_partner_data(
+        partner_type="CUSTOMER",
+        wks=ws,
+        param_invoice_header_area=invoice_header_area
+    )
+    #
+    # get and solve `invoice_header_area` for all SUPPLIER data
+    if owner_datafile is None:  # get supplier data from Excel file
+        _ = get_partner_data(
+            partner_type="SUPPLIER",
+            wks=ws,
+            param_invoice_header_area=invoice_header_area
+        )
+    else:  # get supplier data from `owner-data-file`
+        _ = get_partner_data(
+            partner_type="OWNER",
+            wks=ws,
+            param_invoice_header_area=invoice_header_area,
+            supplier_datafile=owner_datafile
+        )
+    #
+    """#NOTE: section to ( Excel data )--->( JSON ) format preparation and finishing
+        this is required to be after header determination (because CURRENCY could be known here and will impact config param `DEFAULT_CURRENCY`)
+    """
+    # transform `invoice_items_area` in "canonical JSON kv pairs format" (NOTE this step is done only for invoice_items_area and is required because this section is "table with more rows", ie, not a simple key-val)
+    invoice_items_as_kv_pairs = mk_kv_invoice_items_area(invoice_items_area_xl_format=invoice_items_area)
+
+    # preserve processed Excel file meta information: start address, size.
+    meta_info = build_meta_info_key(
+        excel_file_to_process=file_to_process,
+        invoice_worksheet_name=invoice_worksheet_name,
+        ws_size=tuple(ws.size),
+        keyword_for_items_table_marker=keyword_for_items_table_marker,
+        found_cell=tuple(_found_cell_for_invoice_items_area_marker))
+
+    # build final structure to be returned (`invoice`) - MAIN OBJECTIVE of this function
+    tmp_InvoiceLine_list = [_i for _i in invoice_items_as_kv_pairs],  # `invoice_items_as_kv_pairs` is list of dicts with keys as XML RO E-Fact standard
+    tmp_reusable_items = dict(
+        cbc_LineExtensionAmount = sum([dict_sum_by_key(i, "cbc_LineExtensionAmount") for i in tmp_InvoiceLine_list]),
+        LineVatAmount = sum([dict_sum_by_key(i, "LineVatAmount") for i in tmp_InvoiceLine_list]),
+        invoice_issdate_asdate = datetime.strptime(
+            invoice_header_area["issued_date"]["value"],
+            '%Y-%m-%d'
+        ).date()
+    )  # reusable calculations to be used in next code. see details in issue `0.3.0b+240302piu01`
+    tmp_cac_TaxSummary = invoice_taxes_summary(tmp_InvoiceLine_list)  # invoke invoice tax summary calculation
+    # calculate date when VAT becomes eligible (@240417 is 25 of next month after issued month)
+    tmp_cbc_TaxPointDate = tmp_reusable_items["invoice_issdate_asdate"] + timedelta(days = 31)  # 31 days will move one month latter
+    tmp_cbc_TaxPointDate = datetime(
+        tmp_cbc_TaxPointDate.year,
+        tmp_cbc_TaxPointDate.month,
+        25
+    ).date()
+    tmp_cbc_TaxPointDate = tmp_cbc_TaxPointDate.isoformat()
+    invoice = {
+        "Invoice": {
+            "cbc_ID": copy.deepcopy(invoice_header_area["invoice_number"]["value"]),  # invoice number as `cbc_ID`
+            "cbc_DocumentCurrencyCode": copy.deepcopy(invoice_header_area["currency"]["value"]),  # invoice currency as `cbc_DocumentCurrencyCode`
+            "cbc_IssueDate": copy.deepcopy(invoice_header_area["issued_date"]["value"]),  # invoice issue date as `cbc_IssueDate`
+            "cbc_DueDate": copy.deepcopy(invoice_header_area["due_date"]["value"]),  # invoice due date as `cbc_DueDate`
+            "cac_AccountingCustomerParty": {
+                "cac_Party": {
+                    "cac_PartyLegalEntity": {
+                        "cbc_CompanyID": copy.deepcopy(invoice_header_area["customer_area"]["CUI"]["value"]),
+                        "cbc_RegistrationName": copy.deepcopy(invoice_header_area["customer_area"]["RegistrationName"]["value"]),
+                    },
+                    "cac_PostalAddress": copy.deepcopy(invoice_header_area["customer_area"]["PostalAddress"]),
+                    "cac_Contact": {
+                        "cbc_Telephone": copy.deepcopy(invoice_header_area["customer_area"]["phone"]["value"]),
+                        "cbc_ElectronicMail": copy.deepcopy(invoice_header_area["customer_area"]["email"]["value"]),
+                        "RegCom": copy.deepcopy(invoice_header_area["customer_area"]["reg_com"]["value"]),
+                        "Bank": copy.deepcopy(invoice_header_area["customer_area"]["bank"]["value"]),
+                        "IBAN": copy.deepcopy(invoice_header_area["customer_area"]["IBAN"]["value"]),
+                    },
+                },
+            },
+            "cac_AccountingSupplierParty": {
+                "cac_Party": {
+                    "cac_PartyLegalEntity": {
+                        "cbc_CompanyID": copy.deepcopy(invoice_header_area["supplier_area"]["CUI"]["value"]),
+                        "cbc_RegistrationName": copy.deepcopy(invoice_header_area["supplier_area"]["RegistrationName"]["value"]),
+                    },
+                    "cac_PostalAddress": copy.deepcopy(invoice_header_area["customer_area"]["PostalAddress"]),
+                    "cac_Contact": {
+                        "cbc_Telephone": copy.deepcopy(invoice_header_area["supplier_area"]["phone"]["value"]),
+                        "cbc_ElectronicMail": copy.deepcopy(invoice_header_area["supplier_area"]["email"]["value"]),
+                        "RegCom": copy.deepcopy(invoice_header_area["supplier_area"]["reg_com"]["value"]),
+                        "Bank": copy.deepcopy(invoice_header_area["supplier_area"]["bank"]["value"]),
+                        "IBAN": copy.deepcopy(invoice_header_area["supplier_area"]["IBAN"]["value"]),
+                    },
+                    "cac_PartyTaxScheme": {
+                        "cbc_CompanyID": copy.deepcopy(invoice_header_area["supplier_area"]["CUI"]["value"]),
+                        "cac_TaxScheme": {
+                            "cbc_ID": "VAT"
+                        },
+                    },
+                },
+            },
+            "cac_InvoiceLine": copy.deepcopy(tmp_InvoiceLine_list)[0],  # keep only 1st entry because from creating process resulted list(list)) first one being redundant
+            "cac_LegalMonetaryTotal": {
+                "cbc_LineExtensionAmount": round(tmp_reusable_items["cbc_LineExtensionAmount"], 2),
+                "cbc_TaxExclusiveAmount": round(tmp_reusable_items["cbc_LineExtensionAmount"], 2),
+                "cbc_TaxInclusiveAmount": round(tmp_reusable_items["cbc_LineExtensionAmount"] + tmp_reusable_items["LineVatAmount"], 2),
+                "cbc_PayableAmount": round(tmp_reusable_items["cbc_LineExtensionAmount"] + tmp_reusable_items["LineVatAmount"], 2),
+            },
+            "cac_TaxTotal": {
+                "cbc_TaxAmount": round(sum([i["cbc_TaxAmount"] if i["cbc_TaxAmount"] is not None else 0 for i in tmp_cac_TaxSummary]), 2),
+                "cac_TaxSubtotal": copy.deepcopy(tmp_cac_TaxSummary),
+            },
+            # remained mostly "administrative" structure values. For details see ISS `0.6rc1`+`code missing XML tags`
+            "cbc_Note": f"proccesed @{datetime.now(timezone.utc).isoformat()} with xl2roefact",
+            "cac_PaymentMeans": {
+                "cbc_PaymentMeansCode": 1  #NOTE ? do not know if simple Excel processing can give this info - NEEED ERP
+            },
+            "cac_Delivery": {
+                "cbc_ActualDeliveryDate": copy.deepcopy(invoice_header_area["issued_date"]["value"])  # suppose identical with invoice date. Format: `YYYY-MM-DD`
+            },
+            "cbc_TaxPointDate": str(tmp_cbc_TaxPointDate),
+            # TODO: ... ... ...
+            # can use `tmp_reusable_items["invoice_issdate_asdate"]` as datatime object
+
+
+            
+        },
+        "meta_info": copy.deepcopy(meta_info),
+        "excel_original_data": dict(
+            invoice_items_area = copy.deepcopy(invoice_items_area),  # NOTE ready, test PASS @ 231205 by [piu]
+            invoice_header_area = copy.deepcopy(invoice_header_area),  # NOTE ready, test PASS @ 2440326 by [piu]
+            invoice_footer_area = copy.deepcopy(invoice_footer_area)  #TODO wip... TBD-(cac_TaxTotal) / RDY-(cac_LegalMonetaryTotal
+        ),
+    }
+    #
+    # write `invoice` dict to file `f-JSON`
+    """ useful notes ref `f-JSON`:
+        - ref `f-JSON` file, see doc: `https://apitoroefact.renware.eu/commercial_agreement/110-SRE-api_to_roefact_requirements.html#vedere-de-ansamblu-a-solutiei`
+        - create `f-JSON` filename as Excel filename but with json extention
+        - helpers:
+                - os.path.split() gets @[0] directory & @[1] filename
+                - os.path.splitext() @[0] filename w/o ext, @[1] extention woth dot char included
+        - TODO: @231217 - writing a JSON file should be subject of option bool parameter in rdinv() with default value `True`
+    """
+    _fjson_filename = os.path.splitext(os.path.basename(file_to_process))[0] + ".json"
+    _fjson_fileobject = os.path.join(os.path.split(file_to_process)[0], _fjson_filename)
+    with open(_fjson_fileobject, 'w', encoding='utf-8') as _f:
+        json.dump(invoice, _f, ensure_ascii = False, indent = 4)
+    print(f"[yellow]INFO note:[/] `rdinv` module, written invoice JSON data to: [green]{_fjson_fileobject}[/]")
+
+    #TODO check for more TODOs, clean &&-->
+    #TODO wip...(@231125) TRANSFORM JSON FILE from Excel (row,col) format in a relational one (but respecting ROefact tags from used scheme)
+
+    return copy.deepcopy(invoice)
+
+
+
+
+
+
+# NOTE: ready, test PASS @ 231212 by [piu]
+def get_excel_data_at_label(
+    pattern_to_search_for: list[str],
+    worksheet: xl.Database.ws,
+    area_to_scan: list[list[int]] = None,
+    targeted_type: Callable = str,
+    down_search_try: bool = True
+) -> dict:
+    """get "one key Excel values", like invoice number or invoice issue date.
+
+    Args:
+    
+        `pattern_to_search_for`: for example for inv number, will pass the `PATTERN_FOR_INVOICE_NUMBER_LABEL`.
+        `worksheet`: the worksheet containing invoice (as object of `pyxllight` library).
+        `area_to_scan`: area of cells to be searched, default whole worksheet.
+        `targeted_type`: what type expect (will try to convert to, if cannot will return str), default `str`.
+        `down_search_try`: establish if DOWN search method is tried, default `True`.
+
+    Return:
+    
+        `None` if not found OR `dictionary` containing:
+            * `"value": int | float | str` - the value found covenrted to requested `targeted_type` if possible or `str` otherwise; if "out of space" then returns `None`
+            * `"location": (row, col)` - adrees of cell where found value
+
+    Notes:
+    
+    * normal scan order is 1.RIGHT, 2.DOWN (if allowed), 3.IN-LABEL only in given area and pattern.
+    """
+    def __check_value(val: Any) -> bool:
+        """ return `True` if a `val` is different of None or empty string or SYS_FILLED_EMPTY_CELL, otherwise return `False`
+        """
+        if val is None:
+            return False
+        if isinstance(val, str) and val.strip() == "":
+            return False
+        if val == SYS_FILLED_EMPTY_CELL:
+            return False
+        return True
+
+    if area_to_scan is None:  # if arg "passed" was default value then make it as the whole worksheet area
+        area_to_scan = ((1, 1), (worksheet.size[0], worksheet.size[1]))
+    ret_val = dict(  # initialize structure for what will return if information is found
+        value = None,
+        location = (None, None),
+        label_value = None,
+        label_location = None,
+    )
+    for i in range(area_to_scan[0][0], area_to_scan[1][0] + 1):
+        for j in range(area_to_scan[0][1], area_to_scan[1][1] + 1):
+            _crt_cell_val = [worksheet.index(i, j)]  # make it list to be iterable (of 1 element, but iterable)
+            # test if crt cell is in pattern_to_search_for
+            _found = find_str_in_list(list_of_str_to_find=pattern_to_search_for, list_to_search=_crt_cell_val)
+            if _found is not None:
+                if True:  # process label
+                    label_value = _crt_cell_val[0]  # preserve only first value (this will be next proccessed and if pass will remain)
+                    label_location = (i, j)
+                if True:  # process value
+                    value_found = None
+                    index_of_value_found = None
+                    # NOTE-LOGIC: test for RIGHT cell @(i,j+1) if cell exists in ws range AND if has a value then continue loop (to find other potential cell)
+                    if j < area_to_scan[1][1]:  # assure will remain in range of test area for next test (ie, exists cell @ (i, j+1))
+                        check_for_index = (i, j + 1)
+                        check_for = worksheet.index(check_for_index[0], check_for_index[1])
+                        if __check_value(check_for):
+                            value_found = check_for
+                            index_of_value_found = check_for_index
+                    # continue with DOWN test if NOT found somethinng at RIGHT and if this strategy is allowed to be used
+                    if down_search_try and not (value_found and index_of_value_found):  # try DOWN test only if method is allowed AND a relevant value not found or value is located in a wrong area
+                        # NOTE-LOGIC: test for DOWN cell @(i+1,j) if cell exists in ws range AND if has a value then continue loop (to find other potential cell)
+                        if i < area_to_scan[1][0] :  # if still in range if test (ie, exists cell @ (i+1, j))
+                            check_for_index = (i + 1, j)
+                            check_for = worksheet.index(check_for_index[0], check_for_index[1])
+                            if __check_value(check_for):
+                                value_found = check_for
+                                index_of_value_found = check_for_index
+                    # continue with IN-LABEL test if NOT found somethinng at DOWN
+                    if not (value_found and index_of_value_found):  # try IN-LABEL test only if a relevant value not found or value is located in a wrong area
+                        # NOTE-LOGIC: test for IN-LABEL cell (label is supposed only first word separated by space)
+                        check_for = label_value.strip()
+                        # keep all except first word (supposed to be label)
+                        if len(check_for) > 1:
+                            check_for = ' '.join(check_for.split()[1:])  # clean and keep all string except first word
+                        else:
+                            chech_for = ""
+                        if __check_value(check_for):
+                            value_found = check_for
+                            index_of_value_found = label_location
+                # create return dictionary for: label, value found, location of value foun
+                ret_val["label_value"] = label_value  # rule: if found a matching label, the label of info found will appear regardles of effective value found status
+                ret_val["label_location"] = label_location  # rule: same as for "label_value" key
+                if not (value_found and index_of_value_found):  # nothing found, nor @RIGHT, nor @DOWN, so break the loop and try for other poatential cell
+                    return ret_val  # will return the empty structure (as initialized)
+                if value_found and index_of_value_found:  # if found something will break all loops
+                    # all things are ok here (ref effective value), so return found data an, its location
+                    ret_val["location"] = index_of_value_found
+                    try:  # converting to requested `targeted_type` (will not test is isinstance(obj, Callable) because if not will raise `except` and convert to str)
+                        ret_val["value"] = targeted_type(value_found)
+                    except:  # noqa: E722
+                        ret_val["value"] = str(value_found)
+                    return ret_val
+    return ret_val  # if get here then will return the empty structure (as initialized)
+
+
+
+
+
+
+
+
+# NOTE: ready, test PASS @ 231126 by [piu]
+def mk_kv_invoice_items_area(invoice_items_area_xl_format) -> dict:
+    """transform `invoice_items_area` in "canonical JSON format" (as kv pairs).
+
+    Args:
+    
+        `invoice_items_area_xl_format`: invoice items area in Excel format (ie, DataFrame with row, col, data).
+
+    Return:
+    
+        `invoice_items_area_xl_format`: dictionary with invoice items in Excel format (ie, rows, columns).
+
+    Notes:
+    
+    * for ROefact XML model (& plan) see `invoice_files/__model_test_factura_generat_anaf.xml`.
+    """
+    _invoice_items_data_key = copy.deepcopy(invoice_items_area_xl_format["data"])
+    _invoice_items_cols_key = copy.deepcopy(invoice_items_area_xl_format["keycols"])
+    _invoice_items_rows_key = copy.deepcopy(invoice_items_area_xl_format["keyrows"])
+
+    _invoice_items_area_json_format = list()
+    for _i, _line in enumerate (_invoice_items_rows_key):
+        """ identify usual invoice columns: item desc, item UOM, item VAT_percent, item unit_price, item line_value, itemline_ VAT_value
+        """
+        if True:  # ---- find item quantity column ==> (`cbc_InvoicedQuantity`)
+            _col_index = find_str_in_list(["qty", "cant", "quantity"], _invoice_items_cols_key)
+            if _col_index is None:  # did not find a suitable column to represent number, so return None probably raising an error
+                print(f"[red]***FATAL ERROR - module 'RDINV', function `mk_kv_invoice_items_area(...)`. Cannot find a 'QUANTITY' column in items table. Processing terminated[/]")
+                return False
+            else:
+                _item_quantity = _invoice_items_data_key[_i][_col_index] if isnumber(str(_invoice_items_data_key[_i][_col_index])) else None
+
+        """ #NOTE-1: from here, the following columns are considered "valid" only if a quantity is specified (otherwise is considered an extended description)
+        """
+
+        if True:  # ---- find item VAT percent (if exists..., some invoices do noy specify percent itself but just value) ==> (`cbc_Percent`)
+            _col_index = find_str_in_list(["cota", "vat %", "% vat"], _invoice_items_cols_key)
+            if _col_index is None: # did not find a suitable column to represent number, so return None probably raising an error
+                _vat_percent = DEFAULT_VAT_PERCENT if _item_quantity else None  # see #NOTE-1
+            else:
+                #TODO check_what_is_here_and_if_actual [@231202]:  `_vat_percent` calculation should also consider a simplified invoice where only VAT value is specificed AND THEN SHOULD BE CALCULATED AS_IS in document (see "acciza line on REN... invoice")
+                _vat_percent = _invoice_items_data_key[_i][_col_index] if (_invoice_items_data_key[_i][_col_index] is not None) else (DEFAULT_VAT_PERCENT if _item_quantity else None)  # see #TODO-1 check it considering previous comment
+                _vat_percent = None if (str(_vat_percent).split() == "") else (float(_vat_percent) if isnumber(str(_vat_percent)) else None)  # finally make it None if remained empty string
+
+        if True:  # ---- find item description / name ==> (`cbc_Name`)
+            _col_index = find_str_in_list(["denumire", "name", "nume", "item", "desc"], _invoice_items_cols_key)
+            if _col_index is None: # did not find a suitable column to represent number, so return None probably raising an error
+                _name_description = DEFAULT_UNKNOWN_ITEM_NAME if _item_quantity else None  # see #NOTE-1
+            else:
+                _name_description = _invoice_items_data_key[_i][_col_index] if (_invoice_items_data_key[_i][_col_index] is not None) else (DEFAULT_UNKNOWN_ITEM_NAME if _item_quantity else None)  # see #NOTE-1
+
+        if True:  # --- find unit of measure ==> (`cbc_unitCode`)
+            _col_index = find_str_in_list(["uom", "um", "masura", "measure"], _invoice_items_cols_key)
+            if _col_index is None: # did not find a suitable column to represent number, so return None probably raising an error
+                _unif_of_measure = DEFAULT_UNKNOWN_UOM if _item_quantity else None  # see #NOTE-1
+            else:
+                _unif_of_measure = _invoice_items_data_key[_i][_col_index] if (_invoice_items_data_key[_i][_col_index] is not None) else (DEFAULT_UNKNOWN_UOM if _item_quantity else None)  # see #NOTE-1
+
+        if True:  # --- find unit price ==> (`cbc_PriceAmount`)
+            _col_index = find_str_in_list(["price", "pret"], _invoice_items_cols_key)
+            if _col_index is None:  # did not find a suitable column to represent number, so return None probably raising an error
+                _unit_price = 0 if _item_quantity else None  # see #NOTE-1
+            else:
+                _tmp = float(_invoice_items_data_key[_i][_col_index]) if isnumber(str(_invoice_items_data_key[_i][_col_index])) else None  # convert it to numer if possible
+                _unit_price = _tmp if (_tmp is not None) else (_tmp if _item_quantity else None)  # see #NOTE-1
+
+        if True:  # --- find CURRENCY ==> (`cbc_currencyID`)
+            pass # NOTE this will be identifyed in `invoice_header_area` ==> should be changed accordingly
+
+        if True:  # --- calculate line totals ==> (`cbc_LineExtensionAmount`)
+            _item_total = None
+            if (_item_quantity is not None) and (_unit_price is not None):
+                _item_total = round(_item_quantity * _unit_price, 2)
+                # line VAT calculation is subject of VAT existence and right calculation as number, otherwise it is set to NULL
+                if _item_total and _vat_percent:
+                    _item_VAT = round(float(_item_quantity * _unit_price * _vat_percent), 2)
+                else:
+                    _item_VAT = 0.0
+
+        # build dictionary with usual invoice columns (respecting as possible the XSD schemes listed in [`meta_info`][`invoice_XML_schemes`] key)
+        _line_info = {
+            "cac_InvoiceLine": {
+                "cbc_ID": str(_line),
+                "cbc_InvoicedQuantity": _item_quantity,
+                "cbc_unitCode": None if (_item_quantity is None or str(_item_quantity).split() == "") else _unif_of_measure,
+                "cac_Item": {  #-NOTE these are the item specifications (uom, vat)
+                    "cbc_Name": str(_name_description),
+                    "cac_ClassifiedTaxCategory": {
+                        "cbc_Percent": _vat_percent,
+                        "cac_TaxScheme": {
+                            "cbc_ID": None if (_vat_percent is None or str(_vat_percent).split() == "") else "VAT"
+                        }
+                    }
+                },
+                "cac_Price": {
+                    "cbc_PriceAmount" : _unit_price,
+                    "cbc_currencyID": None if (_item_quantity is None or str(_item_quantity).split() == "") else DEFAULT_CURRENCY
+                },
+                "cbc_LineExtensionAmount": _item_total,
+                "LineVatAmount": None if _item_total is None else _item_VAT,  # line VAT calculation is subject of some Amount existence
+            }
+        }
+        _invoice_items_area_json_format.append(_line_info["cac_InvoiceLine"])
+    return copy.deepcopy(_invoice_items_area_json_format)
+
+
+
+
+
+
+# NOTE: ready, test PASS @ 231121 by [piu]
+def get_invoice_items_area(
+    worksheet,
+    invoice_items_area_marker,
+    wks_name
+) -> dict:
+    """get invoice for `invoice_items_area`, process it and return its Excel format.
+
+    Process steps & notes:
+    
+    * find invoice items subtable.
+    * clean invoice items subtable.
+    * extract relevenat data.
+    * NOTE: all Excel cell addresses are in `(row, col)` format (ie, Not Excel format like "A:26, C:42, ...")
+
+    Args:
+    
+        `worksheet`: the worksheet containing invoice (as object of `pyxllight` library).
+        `invoice_items_area_marker`: string with exact marker of invoice items table.
+            NOTE: this is the UPPER-LEFT corner and is determined before calling this procedure.
+        `wks_name`: the wroksheet name (string) of the `worksheet` object.
+
+    Return:
+    
+        `invoice_items_area`: dictionary with invoice items in Excel format (ie, rows, columns).
+    """
+    # obtain table with invoice items ==> `invoice_items_area`
+    invoice_items_area = worksheet.ssd(keycols = invoice_items_area_marker, keyrows = invoice_items_area_marker)
+    if (invoice_items_area is None or ((isinstance(invoice_items_area, list)) and len(invoice_items_area) < 1)):  # there was not detected any area candidate to "invoice items / lines", so will exit rasing error
+        print(f"[red]***FATAL ERROR - Cannot find any candidate to for invoice ITEMS. Worksheet - \"{wks_name}\" in Module [red] RDINV (code-name: `rdinv`). File processing terminated[/]")
+        return False
+
+    #TODO test if list has more items (ie, that means more item tables that will need to be consolidated)
+    if isinstance(invoice_items_area, list) and len(invoice_items_area) > 0:
+        # NOTE `invoice_items_area` dictionary with keys: "keyrows", "keycols" and "data" (self explanatory)
+        invoice_items_area = invoice_items_area[0]  # will suppose found just one AND retain only first one (index [0]) - SEE AFTER TEST with RENware invoice...
+
+    """ CLEANING & CLEARING section
+    """
+    if True:  # preserve actual rows index in a separated structure (`invoice_items_area["keyrows_index"]`)
+        invoice_items_area["keyrows_index"] = list()
+        for _tmp_row_index, _tmp_row in enumerate(invoice_items_area["keyrows"]):  # scan all rows and those with empty name/title are first candidates
+            invoice_items_area["keyrows_index"].append(_tmp_row_index)
+            # clean full empty rows
+            if _tmp_row == SYS_FILLED_EMPTY_CELL:
+                # inspect all row cells to see if all are empty
+                _tmp_test_row_if_full_zero = sum([0 if _i == SYS_FILLED_EMPTY_CELL else 1 for _i in invoice_items_area["data"][_tmp_row_index]])
+                if _tmp_test_row_if_full_zero == 0:  # efectivelly delete in subject objects
+                    del invoice_items_area["keyrows"][_tmp_row_index]  # drop that row from "keyrows" keyword list
+                    # del invoice_items_area["keyrows_index"][_tmp_row_index]  # drop that row from "keyrows" keyword list #NOTE there is no need, you just enumerated this index and dropeed it in the same for-loop step
+                    del invoice_items_area["data"][_tmp_row_index]  # drop that row from "data" keyword list
+        del invoice_items_area["keyrows_index"]  # cleanup after do job ... :)
+
+    if True:  # clean empty columns: columns without a name will be completly dropped as they are unusable anyway (ie, do not know what to do with them...)
+        _tmp_cells_to_drop_in_data_key = list()
+        _tmp_items_to_drop_in_keycols_key = list()
+        for _tmp_col_index, _tmp_col in enumerate(invoice_items_area["keycols"]):  # scan all cols and those with empty name/title are first candidates
+            if _tmp_col == SYS_FILLED_EMPTY_CELL:
+                # inspect all col cells to see if all are empty & efectivelly delete in subject objects
+                _tmp_items_to_drop_in_keycols_key.append(_tmp_col_index)
+                for _data_row_index, _data_row in enumerate(invoice_items_area["data"]):  # scan all rows to find out cells that are part of in subject columns
+                    # find out DATA all cells that corresponding to columns to be dropped ==> `_tmp_cells_to_drop_in_data_key: list[(row, col)]`
+                    _tmp_tmp = (_data_row_index, _tmp_col_index)
+                    _tmp_cells_to_drop_in_data_key.append(_tmp_tmp)
+        # drop collected objects (column heads from KEYCOLS & correcsponding cell from DATA)
+        for _obj_to_delete in reversed(_tmp_items_to_drop_in_keycols_key):  # from KEYCOLS... (start with last item to not remain "in air" due to deletions :))
+            del invoice_items_area["keycols"][_obj_to_delete]
+        for _object_to_delete in reversed(_tmp_cells_to_drop_in_data_key):  # from DATA... (start with last item to not remain "in air" due to deletions :))
+            del invoice_items_area["data"][_object_to_delete[0]][_object_to_delete[1]]  # drop that col from "data" keyword list
+
+    if True:  # unknown header rows: set as a descriptive using format: `<current line number>.NOTE-<seq>`, where `seq` is an ordered sequence of letters (ie, resulting something like: `1.a, 1.b, ...`)
+        _prev_row_number = None
+        __letter_seq_idx = 0  # used for next letter sequence (will reset after "a normal one" row (ie, has a value))
+        for _crt_row_idx, _crt_row_val in enumerate(invoice_items_area["keyrows"]):
+            #
+            # if current row is "a normal one", then preserve index and reset letter sequencer
+            if _crt_row_val != SYS_FILLED_EMPTY_CELL:
+                _prev_row_number = _crt_row_val  # preserve row business index (ie, value shown invoice data not array index)
+                __letter_seq_idx = 0   # reset letter sequence generator
+            #
+            # if current row is "a unknown one" set its header as `<prev line number>.NOTE-<seq>`, where `seq` is an ordered sequence of letters (ie, resulting something like: `1.a, 1.b, ...`)
+            if _crt_row_val == SYS_FILLED_EMPTY_CELL:
+                _crt_row_seq = f"{_prev_row_number}.NOTE-{ascii_lowercase[__letter_seq_idx]}"  # build a sequence-text for current item (see #NOTE_format)
+                # update line header
+                invoice_items_area["keyrows"][_crt_row_idx] = str(_crt_row_seq)
+                __letter_seq_idx += 1
+
+    if True:  # set back to empty cells that remained to `SYS_FILLED_EMPTY_CELL` (only in `invoice_items_area`)
+        invoice_items_area["keycols"] = ["" if _i == SYS_FILLED_EMPTY_CELL else _i for _i in invoice_items_area["keycols"]]  # loop for 'keycols' keyword
+        invoice_items_area["keyrows"] = ["" if _i == SYS_FILLED_EMPTY_CELL else _i for _i in invoice_items_area["keyrows"]]  # loop for 'keyrows' keyword
+        for _tmp_row_index, _tmp_row in enumerate(invoice_items_area["data"]):  # # loop for 'data' keyword (first loop table rows, "data" key is matrix of lines & cells, ie as [][])
+            _tmp_row = ["" if _i == SYS_FILLED_EMPTY_CELL else _i for _i in _tmp_row]
+            invoice_items_area["data"][_tmp_row_index] = _tmp_row
+    return copy.deepcopy(invoice_items_area)
+
+
+
+
+
+
+# NOTE: ready, test PASS @ 231111 by [piu]
+def get_merged_cells_tobe_changed(
+    file_to_scan,
+    invoice_worksheet_name,
+    keep_cells_of_items_ssd_marker = None
+) -> list:
+    """scan Excel file to detect all merged ranges.
+
+    Args:
+    
+        `file_to_scan`: the excel file to be scanned.
+        `invoice_worksheet_name`: the worksheet to be scanned.
+        `keep_cells_of_items_ssd_marker`: tuple with cells that will be marked IN ANY CASE to be preserved:
+            * use case: to keep all potential invoice items ssd rows.
+            * format: `tuple(row, col, val)` where row & col are relevant here
+            * default: `None`
+
+    Return:
+    
+        `cells_to_be_changed`: list with cells that need to be chaged in format `(row,col)`.
+
+    Notes:
+    
+    * function is intended to be used ONLY internal in this module.
+    * use `openpyxl` library to do its job.
+    """
+    all_detected_ranges = []
+    # open Excel file & worksheet
+    workbook_opnxl= opnxl.load_workbook(file_to_scan)
+    worksheet_opnxl = workbook_opnxl[invoice_worksheet_name]
+    all_detected_ranges = worksheet_opnxl.merged_cells.ranges  # get all merged ranges
+    _cells_to_be_changed = list()  # will retaing cells that should be marked with SYS_FILLED_EMPTY_CELL
+    for _crt_range in all_detected_ranges:
+        # range coordinates
+        _crt_range_START_COL = _crt_range.bounds[0]
+        _crt_range_END_COL = _crt_range.bounds[2]
+        _crt_range_START_ROW = _crt_range.bounds[1]
+        _crt_range_END_ROW = _crt_range.bounds[3]
+        # traverse merged range for all cells in / set flags for first entry and when to completly break loop
+        _first_entry = True;
+        _full_break = False
+        for c in range(_crt_range_START_COL, _crt_range_END_COL + 1):  # traverse all COLS ...
+            for r in range(_crt_range_START_ROW, _crt_range_END_ROW + 1):  # traverse all ROWS ...
+                _crt_cell_value = worksheet_opnxl.cell(r, c).value
+                #print(f"\t/***** processing cell (row,col = {r},{c}) has value {_crt_cell_value}")  #NOTE for debug purposes
+                if _first_entry:  # at first pass, see if relevant (ie, not empty or empty string) AND if NOT then break all loops
+                    if _crt_cell_value is None:
+                        _full_break = True
+                        break
+                    if isinstance(_crt_cell_value, str) and _crt_cell_value.strip() == "":  # if is a string test if cell is a real empty string
+                        _full_break = True
+                        break
+                    #print(f"\t/***** RELEVANT cell (row,col = {r},{c}) has value {_crt_cell_value}")  #NOTE for debug purposes
+                    """ section applicable only when `keep_cells_of_items_ssd_marker` is note None
+                        * (r1) in this case, if found a relevant entry in a merged range and and first entry in merged range scan
+                        * (r2) to preserve cell @(`row=current_row`, `col=keep_cells_of_items_ssd_marker[1]`)
+                        * (r3) if that cell is empty, them add in `_cells_to_be_changed` list to be marked with SYS_FILLED_EMPTY_CELL
+                    """
+                    if keep_cells_of_items_ssd_marker:
+                        _potential_ROW_INDEX_address = (r, keep_cells_of_items_ssd_marker[1])
+                        __this_cell_value = worksheet_opnxl.cell(*_potential_ROW_INDEX_address).value
+                        if not (__this_cell_value) and (_potential_ROW_INDEX_address not in _cells_to_be_changed):  # apply (r3) rule - see long comment before this section
+                            _cells_to_be_changed.append(_potential_ROW_INDEX_address)
+                if not _first_entry:  # here the cell has a relevant value, store all next to be marked with SYS_FILLED_EMPTY_CELL
+                    _cells_to_be_changed.append((r, c))
+                    #print(f"\t/***** cell {(r, c)} marked for '___sys_filled_empty_cell' / [yellow]all list is {_cells_to_be_changed}[/]") #NOTE for debug purposes
+                _first_entry = False
+            if _full_break:
+                break
+    return tuple(copy.deepcopy(_cells_to_be_changed))  # always return a tuple as being immutable
+
+
+
+
+
+
+# NOTE: ready, test PASS @ 231127 by [piu]
+def build_meta_info_key(
+    excel_file_to_process: str,
+    invoice_worksheet_name: str,
+    ws_size: list,
+    keyword_for_items_table_marker: str,
+    found_cell: list
+) -> dict:
+    """build meta_info key to preserve processed Excel file meta information: start address, size.
+
+    Notes:
+    
+    * (1.) all cell addresses are in format (row, col) and are absolute (ie, valid for whole Excel file).
+    * (2.) this function is designed to be used internally by current module (using outside it is not guaranteed for information 'quality').
+
+    Args:
+    
+        `excel_file_to_process`: name of file to process as would appear in `meta_info` key.
+        `invoice_worksheet_name`: the worksheet name as would appear in `meta_info` key.
+        `ws_size`: worksheet size as would appear in `meta_info` key (index 0 max rows, index 1 max columns).
+        `keyword_for_items_table_marker`: the content of cell used as start of invoice items subtable as would appear in `meta_info`.
+        `found_cell`: position of cell used as start of invoice items subtable as would appear in `meta_info` key (index 0 row, index 1 column).
+
+    Returns:
+    
+        `meta_info`: dictionary built with meta information to be incorpoarted in final invoice dict
+    """
+    _tmp_meta_info = dict()
+
+    _tmp_meta_info["file"] = os.path.basename(excel_file_to_process)
+    _tmp_meta_info["file_CRC"] = "...file CRC (uniquely identify the invoice file used)"  #TODO to be done... #NOTE this calculation should be done as last step after final XLSX file writing
+    _tmp_meta_info["last_processing_time"] = datetime.now(timezone.utc).isoformat()  # set to ISO 8601 format
+    _tmp_meta_info["invoice_worksheet"] = invoice_worksheet_name
+    _tmp_meta_info["invoice_max_rows"] = ws_size[0]
+    _tmp_meta_info["invoice_max_cols"] = ws_size[1]
+    _tmp_meta_info["items_table_start_marker"] = keyword_for_items_table_marker
+    _tmp_meta_info["items_table_start_cell"] = (found_cell[0], found_cell[1])
+    _tmp_meta_info["invoice_XML_schemes"] = {
+        "xmlns": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2",
+        "xmlns:cbc": "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2",
+        "xmlns:cac": "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2",
+        "xmlns:ns4": "urn:oasis:names:specification:ubl:schema:xsd:CommonExtensionComponents-2",
+        "xmlns:xsi": "http://www.w3.org/2001/XMLSchema-instance",
+        "xsi:schemaLocation": "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2 http://docs.oasis-open.org/ubl/os-UBL-2.1/xsd/maindoc/UBL-Invoice-2.1.xsd"
+    }
+    _tmp_meta_info["map_JSONkeys_XMLtags"] = [  # list of tuple(JSONkey: str, XMLtag: str) #TODO subject of documentation update
+        ("cac_InvoiceLine", "cac:InvoiceLine"),
+        ("cac_Item", "cac:Item"),
+        ("cac_ClassifiedTaxCategory", "cac:ClassifiedTaxCategory"),
+        ("cac_TaxScheme", "cac:TaxScheme"),
+        ("cac_Price", "cac:Price"),
+        ("cbc_ID", "cbc:ID"),
+        ("cbc_InvoicedQuantity", "cbc:InvoicedQuantity"),
+        ("cbc_unitCode", "cbc:unitCode"),  # this is attribute of tag InvoicedQuantity
+        ("cbc_Name", "cbc:Name"),
+        ("cbc_Percent", "cbc:Percent"),
+        ("cbc_PriceAmount", "cbc:PriceAmount"),
+        ("cbc_currencyID", "cbc:currencyID"),  # this is attribute of more tags (all monetary tags)
+        ("cbc_LineExtensionAmount", "cbc:LineExtensionAmount"),
+        ("cbc_DocumentCurrencyCode", "cbc:DocumentCurrencyCode"),  # invoice currency
+        ("cbc_IssueDate", "cbc:IssueDate"),  # invoice issue date
+        ("cbc_DueDate", "cbc:DueDate"),  # invoice due date
+        ("cac_AccountingCustomerParty", "cac:AccountingCustomerParty"),  # invoice customer information - MASTER RECORD
+        ("cac_Party", "cac:Party"),  # invoice customer details ref Parner info (legal, address, ...) - DETAIL L1 RECORD
+        ("cac_PartyLegalEntity", "cac:PartyLegalEntity"),  # invoice customer inforation - DETAIL L2 RECORD
+        ("cbc_CompanyID", "cbc:CompanyID"),  # invoice customer inforation - DETAIL L3 RECORD
+        ("cbc_RegistrationName", "cbc:RegistrationName"),  # invoice customer inforation - DETAIL L3 RECORD
+        ("cac_PostalAddress", "cac:PostalAddress"),  # invoice customer postal address info - DETAIL L2 RECORD
+        ("cbc_StreetName", "cbc:StreetName"),  # invoice customer inforation - DETAIL L3 RECORD
+        ("cbc_CityName", "cbc:CityName"),  # invoice customer inforation - DETAIL L3 RECORD
+        ("cbc_PostalZone", "cbc:PostalZone"),  # invoice customer inforation - DETAIL L3 RECORD
+        ("cac_Country", "cac:Country"),  # invoice customer inforation - DETAIL L3 RECORD
+        ("cbc_IdentificationCode", "cbc:IdentificationCode"),  # invoice customer inforation - DETAIL L3 RECORD
+        ("LineVatAmount", None),  # line / item total VAT. Has no correspondent in XML schema - DETAIL L3 RECORD
+        ("cac_Contact", "cac:Contact"),  #  customer contact information: email, phone - DETAIL L2 RECORD
+        ("cbc_Telephone", "cbc:Telephone"),  # customer phone -- DETAIL L3 RECORD
+        ("cbc_ElectronicMail", "cbc:ElectronicMail"),  # customer email - DETAIL L3 RECORD
+        ("RegCom", None),  # customer commerce register number (company legal registration number). Has no correspondent in XML schema - DETAIL L3 RECORD
+        ("Bank", None),  # customer bank. Has no correspondent in XML schema - DETAIL L3 RECORD
+        ("IBAN", None),  # customer bank account number (IBAN). Has no correspondent in XML schema - DETAIL L3 RECORD
+        ("cac_LegalMonetaryTotal", "cac:LegalMonetaryTotal"),  # summary item
+        ("cbc_LineExtensionAmount", "cbc:LineExtensionAmount"),  # summary item
+        ("cbc_TaxExclusiveAmount", "cbc:TaxExclusiveAmount"),  # summary item
+        ("cbc_TaxInclusiveAmount", "cbc:TaxInclusiveAmount",),  # summary item
+        ("cbc_PayableAmount", "cbc:PayableAmount"),  # summary item
+        ("cac_TaxTotal", "cac:TaxTotal"),  # specific for Tax Summary section
+        ("cbc_TaxAmount", "cbc:TaxAmount"),  # specific for Tax Summary section
+        ("cac_TaxSubtotal", "cac:TaxSubtotal"),  # specific for Tax Summary section
+        ("cbc_TaxableAmount", "cbc:TaxableAmount"),  # specific for Tax Summary section
+        ("cac_TaxCategory", "cac:TaxCategory"),  # specific for Tax Summary section
+        ("cac_AccountingSupplierParty", "cac:AccountingSupplierParty"),  # specific to supplier
+        ("cac_PartyTaxScheme", "cac:PartyTaxScheme"),  # specific to supplier
+        # codes that are not from Excel file but that need to be present in XML file for RO eFact. Normally exceeds an Excel invoice, being at least for a "mini ERP" system
+        ("cbc_DueDate", "cbc:DueDate"),
+        ("cbc_InvoiceTypeCode", "cbc:InvoiceTypeCode"),
+        ("cbc_Note", "cbc:Note"),
+        ("cbc_TaxPointDate", "cbc:TaxPointDate"),
+        ("cac_Delivery", "cac:Delivery"),
+        ("cbc_ActualDeliveryDate", "cbc:ActualDeliveryDate"),
+        ("cac_PaymentMeans", "cac:PaymentMeans"),
+        ("cbc_PaymentMeansCode", "cbc:PaymentMeansCode"),
+        ("cbc_TaxPointDate", "cbc:TaxPointDate"),  # date when VAT becomes eligible for payment
+    ]
+    return copy.deepcopy(_tmp_meta_info)
+
+
+
+
+
+
+# NOTE: ready, test PASS @ 240404 by [piu]
+def get_partner_data(
+    partner_type: str,
+    *,
+    wks,
+    param_invoice_header_area: dict,
+    supplier_datafile: Path = None
+) -> None:
+    """Get invoice partener data from Excel.
+
+    Notes:
+    
+    * *for developers*: function works by generating side effects and must be located in `rdinv.py`
+    * *side effects*: this function works by directly modifying `param_invoice_header_area` sent parameter
+    * *supplier_datafile exception*: if file is not found or cannot be read, this function will force complete application termination (`sys.exit`)
+
+    Args:
+    
+        `partner_type`: one of "CUSTOMER", "SUPPLIER" or "OWNER" to specify for what kind of parner get data. The value "OWNER" is designed to get data from an outside database / file (master data)
+        `wks`: current work-on `pylightxl Worksheet` object
+        `param_invoice_header_area`: _mode IN-OUT_, outside `param_invoice_header_area` as used and needed in `rdinv()`. This function will write back in this variable
+        `supplier_datafile`: for `partner_type = "CUSTOMER"` here is expected the file where to get supplier data
+
+    Return:
+    
+        `None`: all data is produced directly in parameters as side effect
+    """
+    # set variables constant-like suspected to be changed as global
+    global DEFAULT_CUSTOMER_COUNTRY
+    global DEFAULT_SUPPLIER_COUNTRY
+    # normalize partner_type for easier usage and more flexibility to developers misusing
+    partner_type = partner_type.upper().strip()
+    # unify search patterns and other constants function of partner_type
+    if partner_type == "CUSTOMER":
+        UNIF_PATTERN_FOR_INVOICE_PARTNER_SUBTABLE_MARKER = PATTERN_FOR_INVOICE_CUSTOMER_SUBTABLE_MARKER
+        UNIF_PATTERN_FOR_PARTNER_LEGAL_NAME = PATTERN_FOR_CUSTOMER_LEGAL_NAME
+        UNIF_DEFAULT_PARTNER_COUNTRY = DEFAULT_CUSTOMER_COUNTRY
+        unif_partner_area_key = "customer_area"
+    elif partner_type =="SUPPLIER":
+        # NOTE: pls be patient. Here will raise errs because used EXPECTED constant names. Check `config_settings.py` and adjust accordingly
+        UNIF_PATTERN_FOR_INVOICE_PARTNER_SUBTABLE_MARKER = PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER
+        UNIF_PATTERN_FOR_PARTNER_LEGAL_NAME = PATTERN_FOR_SUPPLIER_LEGAL_NAME
+        UNIF_DEFAULT_PARTNER_COUNTRY = DEFAULT_SUPPLIER_COUNTRY
+        unif_partner_area_key = "supplier_area"
+    elif partner_type == "OWNER":  # subject to load SUPPLIER data from external data source
+        unif_partner_area_key = "supplier_area"
+        # safe read data from `supplier_datafile` file only if it exists
+        file_ok = supplier_datafile.exists() and supplier_datafile.is_file()
+        if file_ok:
+            yaml_in = supplier_datafile.read_text()
+            suppl_data_read = yaml.safe_load(yaml_in)
+        else:
+            print(f"[red]ERROR: Owner / Supplier data file ([cyan]{supplier_datafile}[/]) cannot be read. Process terminated.[/].")
+            sys.exit()
+        supplier_datafile_name = str(supplier_datafile)
+        # save info about area to search as external file and its name
+        param_invoice_header_area[unif_partner_area_key] = {
+            "area_info": {
+               "value": supplier_datafile_name,
+                "location": "external file",
+            }
+        }
+        # CUI
+        param_invoice_header_area[unif_partner_area_key]["CUI"] = {
+            "value": suppl_data_read["PartyLegalEntity"]["CompanyID"],
+            "location": "external file (PartyLegalEntity -> CompanyID)",
+            "label_value": None,
+            "label_location": None
+        }
+        # RegName
+        param_invoice_header_area[unif_partner_area_key]["RegistrationName"] = {
+            "value": suppl_data_read["PartyLegalEntity"]["RegistrationName"],
+            "location": "external file (PartyLegalEntity -> CompanyID)",
+            "label_value": None,
+            "label_location": None
+        }
+        # PostalAddress
+        param_invoice_header_area[unif_partner_area_key]["PostalAddress"] = {
+            "cbc_StreetName": suppl_data_read["PostalAddress"]["StreetName"],
+            "cbc_CityName": suppl_data_read["PostalAddress"]["CityName"],
+            "cbc_PostalZone": suppl_data_read["PostalAddress"]["PostalZone"],
+            "cac_Country": { "cbc_IdentificationCode": suppl_data_read["PostalAddress"]["CountryCode"] },
+        }
+        # Bank, Tax & Contact
+        param_invoice_header_area[unif_partner_area_key]["reg_com"] = {
+            "value": suppl_data_read["PartyTaxScheme"]["CompanyID"],
+            "location": "external file (PartyLegalEntity -> CompanyID)"
+        }
+        param_invoice_header_area[unif_partner_area_key]["phone"] = {
+            "value": suppl_data_read["Contact"]["Telephone"],
+            "location": "external file (Contact -> Telephone)"
+        }
+        param_invoice_header_area[unif_partner_area_key]["email"] = {
+            "value": suppl_data_read["Contact"]["ElectronicMail"],
+            "location": "external file (Contact -> ElectronicMail)"
+        }
+        param_invoice_header_area[unif_partner_area_key]["bank"] = {
+            "value": suppl_data_read["Contact"]["Bank"],
+            "location": "external file (Contact -> Bank)"
+        }
+        param_invoice_header_area[unif_partner_area_key]["IBAN"] = {
+            "value": suppl_data_read["Contact"]["IBAN"],
+            "location": "external file (Contact -> IBAN)"
+        }
+        return
+    else:  # accept only known operations
+        raise Exception("partner_type parameter not recognized value")
+    #
+    # find invoice partner ==> one of (cac:AccountingCustomerParty , cac:AccountingSupplierParty)
+    invoice_partner_info = get_excel_data_at_label(
+        pattern_to_search_for=UNIF_PATTERN_FOR_INVOICE_PARTNER_SUBTABLE_MARKER,  # NOTE: constant adjusted in refactoring process
+        worksheet=wks,
+        area_to_scan=(param_invoice_header_area["start_cell"], param_invoice_header_area["end_cell"]),
+        targeted_type=str
+    )  # returned info: `{"value": ..., "location": (row..., col...)}`
+    # set a dedicated area to search for partner
+    _area_to_search_start_cell = [  # use `label_location` as being supposed "most far away" from effective-good info, so more chances to find info
+        0 if invoice_partner_info["label_location"][0] <= 0 else invoice_partner_info["label_location"][0] - 1,  # set one line up if this line exists
+        invoice_partner_info["label_location"][1],
+    ]
+    if wks.index(*_area_to_search_start_cell).strip() == "":  # prev set was for one line up but if that cell is blank remake it (ie, do a +1)
+        _area_to_search_start_cell[0] += 1
+    # from `_area_to_search_start_cell` go down up a blank (empty cell)
+    _last_ok_position = list([0, 0])
+    for __i in range(_area_to_search_start_cell[0], wks.size[0] + 1):  # scan rest of lines for a blank one
+        _crt_scanned_cell_idx = (__i, _area_to_search_start_cell[1])
+        _crt_scanned_cell_val = wks.index(*_crt_scanned_cell_idx)
+        if _crt_scanned_cell_val.strip() == "":
+            break  # case where stop
+        _last_ok_position = copy.deepcopy(_crt_scanned_cell_idx)  # save current position to be used after a break in other iteration
+    _area_to_search_end_cell = [
+        _last_ok_position[0],
+        wks.size[1] if _last_ok_position[1] > wks.size[1] else _last_ok_position[1] + 1,  # set one row right if this row exists
+    ]
+    # persist `_area_to_search` for next steps & save its key-info in associated invoice JSON (for further references)
+    _area_to_search = (tuple(_area_to_search_start_cell), tuple(_area_to_search_end_cell))
+    param_invoice_header_area[unif_partner_area_key] = {
+        "area_info": {
+            "value": wks.index(*_area_to_search[0]),  # ie, the value at area start position
+            "location": copy.deepcopy(_area_to_search),
+        }
+    }
+    #
+    # find partner key "CUI / Registration ID" ==> `param_invoice_header_area...[CUI]` && `Invoice...[cbc_CompanyID]`
+    _temp_found_data = get_excel_data_at_label(
+        pattern_to_search_for=PATTERN_FOR_PARTNER_ID,
+        worksheet=wks,
+        area_to_scan=_area_to_search,
+        targeted_type=str,
+        down_search_try=False  # partner area is supposed to be organized as "label & value @ RIGHT" or "label: value @ IN-LABEL" but never @ DOWN as being a "not-a-practiced-natural-way"
+    )  # returned info: `{"value": ..., "location": (row..., col...)}`
+    param_invoice_header_area[unif_partner_area_key]["CUI"] = {
+        "value": _temp_found_data["value"],
+        "location": _temp_found_data["location"],
+        "label_value": _temp_found_data["label_value"],
+        "label_location": _temp_found_data["label_location"]
+    }
+    #
+    # find partner key "RegistrationName" ==> `cbc_RegistrationName`
+    '''#NOTE: `ReNaSt`-RegNameStrategy (remark: step codes will referred as defined here)
+          ReNaSt.STEP-1. search for UNIF_PATTERN_FOR_PARTNER_LEGAL_NAME  # NOTE: constant adjusted in refactoring process
+          ReNaSt.STEP-2. if `label_location` of FOUND VALUE has the same location as `param_invoice_header_area[unif_partner_area_key]["area_info"]["location"][0]`:
+                             keep VALUE of FOUND info
+          ReNaSt.STEP-3. else:
+                             keep `param_invoice_header_area[unif_partner_area_key]["area_info"]["value"]`
+    '''
+    _temp_found_data = get_excel_data_at_label(  # NOTE: ReNaSt.STEP-1
+        pattern_to_search_for=UNIF_PATTERN_FOR_PARTNER_LEGAL_NAME,  # NOTE: constant adjusted in refactoring process
+        worksheet=wks,
+        area_to_scan=_area_to_search,
+        targeted_type=str,
+        down_search_try=True  # NOTE: set on True to obtain identical results as original search of `UNIF_PATTERN_FOR_INVOICE_PARTNER_SUBTABLE_MARKER` because name is supposed to be in a very "unstructured mode"
+    )  # returned info: `{"value": ..., "location": (row..., col...)}`
+    _location_of_header_partner_area = param_invoice_header_area[unif_partner_area_key]["area_info"]["location"][0]
+    _location_of_value_found = _temp_found_data["label_location"]
+    if _location_of_value_found == _location_of_header_partner_area:  # NOTE: ReNaSt.STEP-2
+        kept_RegistrationName = _temp_found_data["value"]
+        kept_RegistrationName_location = _temp_found_data["location"]
+    else:  # NOTE: ReNaSt.STEP-3
+        kept_RegistrationName = param_invoice_header_area[unif_partner_area_key]["area_info"]["value"]
+        kept_RegistrationName_location = param_invoice_header_area[unif_partner_area_key]["area_info"]["location"][0]
+    param_invoice_header_area[unif_partner_area_key]["RegistrationName"] = {
+        "value": kept_RegistrationName,
+        "location": kept_RegistrationName_location,
+        "label_value": "n/a",
+        "label_location": "n/a"
+    }
+    #
+    # find partner key `cac:PostalAddress` -> `param_invoice_header_area["cac_PostalAddress"]` && Invoice...["cac_PostalAddress"]
+    _temp_found_data = get_excel_data_at_label(
+        pattern_to_search_for=PATTERN_FOR_PARTNER_ADDRESS,
+        worksheet=wks,
+        area_to_scan=_area_to_search,
+        targeted_type=str,
+        down_search_try=False  # partner area is supposed to be organized as "label & value @ RIGHT" or "label: value @ IN-LABEL" but never @ DOWN as being a "not-a-practiced-natural-way"
+    )  # returned info: `{"value": ..., "location": (row..., col...)}`
+    _tmpstr = _temp_found_data["label_value"].lower()
+    _val_is_full_addr = ("adr" in _tmpstr) or ("addr" in _tmpstr)
+    if _val_is_full_addr:
+        area_to_scan_address_items = (_temp_found_data["location"], _temp_found_data["location"])
+    else:
+        area_to_scan_address_items = _area_to_search
+    search_address_parts = partial(  # define a partial function to be used for all address items search
+        get_excel_data_at_label,  # function to call
+        worksheet=wks,
+        area_to_scan=area_to_scan_address_items,
+        targeted_type=str,
+        down_search_try=False  # partner area is supposed to be organized as "label & value @ RIGHT" or "label: value @ IN-LABEL" but never @ DOWN as being a "not-a-practiced-natural-way"
+    )  # returned info: `{"value": ..., "location": (row..., col...)}`
+    _tmp_country = str(search_address_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_ADDRESS_COUNTRY)["value"]).replace("None", "").strip()
+    _tmp_city = str(search_address_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_ADDRESS_CITY)["value"]).replace("None", "").strip()
+    _tmp_street = str(search_address_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_ADDRESS_STREET)["value"]).replace("None", "").strip()
+    _tmp_zipcode = str(search_address_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_ADDRESS_ZIPCODE)["value"]).replace("None", "").strip()
+    if (_tmp_country is None) or (_tmp_country == ""):
+        _tmp_country = UNIF_DEFAULT_PARTNER_COUNTRY  # NOTE: constant adjusted in refactoring process
+    else:  # update default value to be re-used in other parts if neccesary. Update is made on original variables "global" defined
+        if partner_type == "CUSTOMER":
+            DEFAULT_CUSTOMER_COUNTRY = _tmp_country  # NOTE: constant adjusted in refactoring process
+        else:  # case of "SUPPLIER" and "OWNER"
+            DEFAULT_SUPPLIER_COUNTRY = _tmp_country  # NOTE: constant adjusted in refactoring process
+    param_invoice_header_area[unif_partner_area_key]["PostalAddress"] = {
+        "cbc_StreetName": _tmp_street,
+        "cbc_CityName": _tmp_city,
+        "cbc_PostalZone": _tmp_zipcode,
+        "cac_Country": {"cbc_IdentificationCode": _tmp_country},
+    }
+    #
+    # find / search_extended_parts: rest of keys, like: "reg com", "bank / IBAN / cont", "tel", "email" (in code will use names like this: "search_extended_parts")*
+    search_extended_parts = partial(  # define a partial function to be used for all "search_extended_parts"
+        get_excel_data_at_label,  # function to call
+        worksheet=wks,
+        area_to_scan=_area_to_search,  # supposed to still contain partner info found area
+        targeted_type=str,
+        down_search_try=False  # partner area is supposed to be organized as "label & value @ RIGHT" or "label: value @ IN-LABEL" but never @ DOWN as being a "not-a-practiced-natural-way"
+    )  # returned info: `{"value": ..., "location": (row..., col...)}`
+    _tmp_reg_com = search_extended_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_REGCOM)
+    _tmp_bank = search_extended_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_BANK)
+    _tmp_IBAN = search_extended_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_IBAN)
+    _tmp_phone = search_extended_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_TEL)
+    _tmp_email = search_extended_parts(pattern_to_search_for=PATTERN_FOR_PARTNER_EMAIL)
+    # store "full" variables in `partner_area...` for excel original values
+    param_invoice_header_area[unif_partner_area_key]["reg_com"] = _tmp_reg_com
+    param_invoice_header_area[unif_partner_area_key]["bank"] = _tmp_bank
+    param_invoice_header_area[unif_partner_area_key]["IBAN"] = _tmp_IBAN
+    param_invoice_header_area[unif_partner_area_key]["phone"] = _tmp_phone
+    param_invoice_header_area[unif_partner_area_key]["email"] = _tmp_email
+    return
+
+
+
+
+
+
```

### Comparing `xl2roefact-0.5.4/xl2roefact/wrxml.py` & `xl2roefact-0.6rc0/xl2roefact/wrxml.py`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.5.4/PKG-INFO` & `xl2roefact-0.6rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xl2roefact
-Version: 0.5.4
+Version: 0.6rc0
 Summary: Excel invoices data retrieve, export & upload to RO E-Fact system
 Author-Email: Petre Iordanescu <petre.iordanescu@gmail.com>, RENware Software Systems <renware.systems@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,15 +684,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Office/Business :: Financial
 Project-URL: Homepage, https://invoicetoroefact.renware.eu
 Project-URL: Pdf-documentation, https://invoicetoroefact.renware.eu/pdfs/print_page.html/print_page.pdf
 Project-URL: Pypi-package, https://pypi.org/project/xl2roefact/
 Project-URL: Github, https://github.com/petre-renware/api_to_roefact
-Requires-Python: <3.11,>=3.10
+Requires-Python: <3.12,>=3.9
 Requires-Dist: altgraph~=0.17
 Requires-Dist: argcomplete~=3.2
 Requires-Dist: commonmark~=0.9
 Requires-Dist: et-xmlfile~=1.1
 Requires-Dist: Fraction~=2.2
 Requires-Dist: Jinja2~=3.1
 Requires-Dist: lief~=0.13
@@ -713,14 +713,16 @@
 Requires-Dist: pywin32-ctypes~=0.2
 Requires-Dist: rich~=13.7
 Requires-Dist: setuptools~=69.0
 Requires-Dist: shellingham~=1.5
 Requires-Dist: six~=1.16
 Requires-Dist: time-machine~=2.13
 Requires-Dist: tomli~=2.0
+Requires-Dist: click~=8.1
+Requires-Dist: typer~=0.9
 Requires-Dist: typing-extensions~=4.9
 Requires-Dist: tzdata~=2023.4
 Requires-Dist: userpath~=1.9
 Requires-Dist: wheel~=0.42
 Requires-Dist: msgpack>=1.0.8
 Requires-Dist: pyyaml>=6.0.1
 Description-Content-Type: text/markdown
@@ -733,16 +735,18 @@
 
 Legaturi externe utile:
 
 * [**Web Site**](https://invoicetoroefact.renware.eu/). (*Pentru acces corect la toate referintele din acest document vizitati site-ul dedicat acestui sistem.*)
 * [Pachet *PyPi*](https://pypi.org/project/xl2roefact/)
 * [Surse *GitHub*](https://github.com/petre-renware/api_to_roefact/)
 * [Vedere de ansamblu pachet biblioteca Python](./doc/README_xl2roefact_library.md)
-* [Referinta *API*](./doc/810.05a-xl2roefact_DLD_specs.md)
-
+* [Referinta *API*](https://invoicetoroefact.renware.eu/xl2roefact/doc/wrapper_810.05a-xl2roefact_DLD_specs.html)
+<!--Refrence to source doc. If used like that, then must be resolved with an external tool before generating a complete README.html doc. The `mkdoxs` is able to do that but in `PyPi` published version will be unusable
+(./doc/810.05a-xl2roefact_DLD_specs.md)
+-->
 
 
 ## Facilitati
 
 ![Static Badge](https://img.shields.io/badge/MSI_installer-YES-darkgreen)
 ![Static Badge](https://img.shields.io/badge/standlone_EXE-YES-darkgreen)
 ![Static Badge](https://img.shields.io/badge/script_Python3-YES-darkgreen)
```

